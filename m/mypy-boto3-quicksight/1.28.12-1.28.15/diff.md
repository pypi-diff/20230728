# Comparing `tmp/mypy-boto3-quicksight-1.28.12.tar.gz` & `tmp/mypy-boto3-quicksight-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-quicksight-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
+gzip compressed data, was "mypy-boto3-quicksight-1.28.15.tar", last modified: Fri Jul 28 20:43:30 2023, max compression
```

## Comparing `mypy-boto3-quicksight-1.28.12.tar` & `mypy-boto3-quicksight-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.561188 mypy-boto3-quicksight-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:43:30.000000 mypy-boto3-quicksight-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    89109 2023-07-27 11:49:27.557187 mypy-boto3-quicksight-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    87610 2023-07-27 11:43:30.000000 mypy-boto3-quicksight-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.549188 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-27 11:43:30.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-27 11:43:30.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 11:43:30.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   123489 2023-07-27 11:43:34.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   123296 2023-07-27 11:43:30.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    36327 2023-07-27 11:43:35.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    36325 2023-07-27 11:43:34.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29023 2023-07-27 11:43:34.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28996 2023-07-27 11:43:34.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:43:30.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   665127 2023-07-27 11:43:53.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   664279 2023-07-27 11:43:44.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:43:30.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.557187 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    89109 2023-07-27 11:49:27.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 11:49:27.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 11:49:27.000000 mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.561188 mypy-boto3-quicksight-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 11:43:29.000000 mypy-boto3-quicksight-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.937689 mypy-boto3-quicksight-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    75930 2023-07-28 20:43:30.933689 mypy-boto3-quicksight-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    74431 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.925689 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123489 2023-07-28 20:35:47.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123296 2023-07-28 20:35:47.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    36327 2023-07-28 20:35:48.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36325 2023-07-28 20:35:48.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29023 2023-07-28 20:35:47.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28996 2023-07-28 20:35:47.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   550945 2023-07-28 20:36:06.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   550229 2023-07-28 20:35:58.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.929689 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    75930 2023-07-28 20:43:30.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:43:30.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:30.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:43:30.000000 mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:30.937689 mypy-boto3-quicksight-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:35:46.000000 mypy-boto3-quicksight-1.28.15/setup.py
```

### Comparing `mypy-boto3-quicksight-1.28.12/LICENSE` & `mypy-boto3-quicksight-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/__init__.py` & `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/__init__.pyi` & `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/__main__.py` & `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QuickSight 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.QuickSight 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight\nOther"
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

### Comparing `mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/client.py` & `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/client.pyi` & `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/literals.py` & `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/literals.pyi` & `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/paginator.py` & `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/paginator.pyi` & `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/type_defs.py` & `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for quicksight service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_quicksight.type_defs import AccountCustomizationOutputTypeDef
+    from mypy_boto3_quicksight.type_defs import AccountCustomizationTypeDef
 
-    data: AccountCustomizationOutputTypeDef = {...}
+    data: AccountCustomizationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -198,163 +198,114 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AccountCustomizationOutputTypeDef",
     "AccountCustomizationTypeDef",
     "AccountInfoTypeDef",
     "AccountSettingsTypeDef",
     "ActiveIAMPolicyAssignmentTypeDef",
-    "AdHocFilteringOptionOutputTypeDef",
     "AdHocFilteringOptionTypeDef",
-    "AttributeAggregationFunctionOutputTypeDef",
     "AttributeAggregationFunctionTypeDef",
-    "ColumnIdentifierOutputTypeDef",
     "ColumnIdentifierTypeDef",
-    "AmazonElasticsearchParametersOutputTypeDef",
     "AmazonElasticsearchParametersTypeDef",
-    "AmazonOpenSearchParametersOutputTypeDef",
     "AmazonOpenSearchParametersTypeDef",
-    "CalculatedFieldOutputTypeDef",
-    "DataSetIdentifierDeclarationOutputTypeDef",
     "CalculatedFieldTypeDef",
     "DataSetIdentifierDeclarationTypeDef",
     "EntityTypeDef",
     "AnalysisSearchFilterTypeDef",
     "DataSetReferenceTypeDef",
     "AnalysisSummaryTypeDef",
     "SheetTypeDef",
-    "AnchorDateConfigurationOutputTypeDef",
     "AnchorDateConfigurationTypeDef",
     "AnonymousUserDashboardEmbeddingConfigurationTypeDef",
     "DashboardVisualIdTypeDef",
     "AnonymousUserQSearchBarEmbeddingConfigurationTypeDef",
-    "ArcAxisDisplayRangeOutputTypeDef",
     "ArcAxisDisplayRangeTypeDef",
-    "ArcConfigurationOutputTypeDef",
     "ArcConfigurationTypeDef",
-    "ArcOptionsOutputTypeDef",
     "ArcOptionsTypeDef",
     "AssetBundleExportJobAnalysisOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobDashboardOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobDataSetOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobDataSourceOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef",
-    "AssetBundleExportJobResourceIdOverrideConfigurationOutputTypeDef",
+    "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleExportJobThemeOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobVPCConnectionOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobAnalysisOverridePropertiesTypeDef",
     "AssetBundleExportJobDashboardOverridePropertiesTypeDef",
     "AssetBundleExportJobDataSetOverridePropertiesTypeDef",
     "AssetBundleExportJobDataSourceOverridePropertiesTypeDef",
     "AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef",
-    "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleExportJobThemeOverridePropertiesTypeDef",
     "AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef",
     "AssetBundleExportJobErrorTypeDef",
     "AssetBundleExportJobSummaryTypeDef",
-    "AssetBundleImportJobAnalysisOverrideParametersOutputTypeDef",
     "AssetBundleImportJobAnalysisOverrideParametersTypeDef",
-    "AssetBundleImportJobDashboardOverrideParametersOutputTypeDef",
     "AssetBundleImportJobDashboardOverrideParametersTypeDef",
-    "AssetBundleImportJobDataSetOverrideParametersOutputTypeDef",
     "AssetBundleImportJobDataSetOverrideParametersTypeDef",
-    "AssetBundleImportJobDataSourceCredentialPairOutputTypeDef",
     "AssetBundleImportJobDataSourceCredentialPairTypeDef",
-    "SslPropertiesOutputTypeDef",
-    "VpcConnectionPropertiesOutputTypeDef",
     "SslPropertiesTypeDef",
     "VpcConnectionPropertiesTypeDef",
     "AssetBundleImportJobErrorTypeDef",
     "AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef",
-    "AssetBundleImportJobResourceIdOverrideConfigurationOutputTypeDef",
-    "AssetBundleImportJobThemeOverrideParametersOutputTypeDef",
-    "AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef",
-    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
     "AssetBundleImportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleImportJobThemeOverrideParametersTypeDef",
+    "AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef",
+    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
     "AssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
     "AssetBundleImportJobSummaryTypeDef",
     "AssetBundleImportSourceDescriptionTypeDef",
     "AssetBundleImportSourceTypeDef",
-    "AthenaParametersOutputTypeDef",
     "AthenaParametersTypeDef",
-    "AuroraParametersOutputTypeDef",
     "AuroraParametersTypeDef",
-    "AuroraPostgreSqlParametersOutputTypeDef",
     "AuroraPostgreSqlParametersTypeDef",
-    "AwsIotAnalyticsParametersOutputTypeDef",
     "AwsIotAnalyticsParametersTypeDef",
-    "DateAxisOptionsOutputTypeDef",
     "DateAxisOptionsTypeDef",
-    "AxisDisplayMinMaxRangeOutputTypeDef",
     "AxisDisplayMinMaxRangeTypeDef",
-    "AxisLinearScaleOutputTypeDef",
     "AxisLinearScaleTypeDef",
-    "AxisLogarithmicScaleOutputTypeDef",
     "AxisLogarithmicScaleTypeDef",
-    "ItemsLimitConfigurationOutputTypeDef",
     "ItemsLimitConfigurationTypeDef",
-    "BinCountOptionsOutputTypeDef",
     "BinCountOptionsTypeDef",
-    "BinWidthOptionsOutputTypeDef",
     "BinWidthOptionsTypeDef",
     "BookmarksConfigurationsTypeDef",
-    "BorderStyleOutputTypeDef",
     "BorderStyleTypeDef",
-    "BoxPlotStyleOptionsOutputTypeDef",
     "BoxPlotStyleOptionsTypeDef",
-    "PaginationConfigurationOutputTypeDef",
     "PaginationConfigurationTypeDef",
-    "CalculatedColumnOutputTypeDef",
     "CalculatedColumnTypeDef",
-    "CalculatedMeasureFieldOutputTypeDef",
     "CalculatedMeasureFieldTypeDef",
     "CancelIngestionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "CastColumnTypeOperationOutputTypeDef",
     "CastColumnTypeOperationTypeDef",
-    "CustomFilterConfigurationOutputTypeDef",
+    "CustomFilterConfigurationTypeDef",
     "CustomFilterListConfigurationOutputTypeDef",
     "FilterListConfigurationOutputTypeDef",
-    "CustomFilterConfigurationTypeDef",
     "CustomFilterListConfigurationTypeDef",
     "FilterListConfigurationTypeDef",
     "CellValueSynonymOutputTypeDef",
     "CellValueSynonymTypeDef",
-    "SimpleClusterMarkerOutputTypeDef",
     "SimpleClusterMarkerTypeDef",
     "CollectiveConstantOutputTypeDef",
     "CollectiveConstantTypeDef",
-    "DataColorOutputTypeDef",
     "DataColorTypeDef",
-    "CustomColorOutputTypeDef",
     "CustomColorTypeDef",
-    "ColumnDescriptionOutputTypeDef",
     "ColumnDescriptionTypeDef",
-    "ColumnGroupColumnSchemaOutputTypeDef",
     "ColumnGroupColumnSchemaTypeDef",
     "GeoSpatialColumnGroupOutputTypeDef",
     "GeoSpatialColumnGroupTypeDef",
     "ColumnLevelPermissionRuleOutputTypeDef",
     "ColumnLevelPermissionRuleTypeDef",
-    "ColumnSchemaOutputTypeDef",
     "ColumnSchemaTypeDef",
     "ComparativeOrderOutputTypeDef",
     "ComparativeOrderTypeDef",
-    "ConditionalFormattingSolidColorOutputTypeDef",
     "ConditionalFormattingSolidColorTypeDef",
-    "ConditionalFormattingCustomIconOptionsOutputTypeDef",
-    "ConditionalFormattingIconDisplayConfigurationOutputTypeDef",
     "ConditionalFormattingCustomIconOptionsTypeDef",
     "ConditionalFormattingIconDisplayConfigurationTypeDef",
-    "ConditionalFormattingIconSetOutputTypeDef",
     "ConditionalFormattingIconSetTypeDef",
     "TagTypeDef",
     "CreateAccountSubscriptionRequestRequestTypeDef",
     "SignupResponseTypeDef",
     "ResourcePermissionTypeDef",
     "DataSetUsageConfigurationTypeDef",
     "FieldFolderTypeDef",
@@ -368,95 +319,51 @@
     "CreateIAMPolicyAssignmentRequestRequestTypeDef",
     "CreateIngestionRequestRequestTypeDef",
     "CreateTemplateAliasRequestRequestTypeDef",
     "TemplateAliasTypeDef",
     "CreateThemeAliasRequestRequestTypeDef",
     "ThemeAliasTypeDef",
     "TopicRefreshScheduleTypeDef",
-    "DecimalPlacesConfigurationOutputTypeDef",
-    "NegativeValueConfigurationOutputTypeDef",
-    "NullValueFormatConfigurationOutputTypeDef",
     "DecimalPlacesConfigurationTypeDef",
     "NegativeValueConfigurationTypeDef",
     "NullValueFormatConfigurationTypeDef",
-    "LocalNavigationConfigurationOutputTypeDef",
     "LocalNavigationConfigurationTypeDef",
-    "CustomActionURLOperationOutputTypeDef",
     "CustomActionURLOperationTypeDef",
-    "CustomContentConfigurationOutputTypeDef",
     "CustomContentConfigurationTypeDef",
-    "CustomNarrativeOptionsOutputTypeDef",
     "CustomNarrativeOptionsTypeDef",
     "CustomParameterValuesOutputTypeDef",
     "CustomParameterValuesTypeDef",
-    "InputColumnOutputTypeDef",
     "InputColumnTypeDef",
-    "DataPointDrillUpDownOptionOutputTypeDef",
-    "DataPointMenuLabelOptionOutputTypeDef",
-    "DataPointTooltipOptionOutputTypeDef",
-    "ExportToCSVOptionOutputTypeDef",
-    "ExportWithHiddenFieldsOptionOutputTypeDef",
-    "SheetControlsOptionOutputTypeDef",
-    "SheetLayoutElementMaximizationOptionOutputTypeDef",
-    "VisualAxisSortOptionOutputTypeDef",
-    "VisualMenuOptionOutputTypeDef",
     "DataPointDrillUpDownOptionTypeDef",
     "DataPointMenuLabelOptionTypeDef",
     "DataPointTooltipOptionTypeDef",
     "ExportToCSVOptionTypeDef",
     "ExportWithHiddenFieldsOptionTypeDef",
     "SheetControlsOptionTypeDef",
     "SheetLayoutElementMaximizationOptionTypeDef",
     "VisualAxisSortOptionTypeDef",
     "VisualMenuOptionTypeDef",
     "DashboardSearchFilterTypeDef",
     "DashboardSummaryTypeDef",
     "DashboardVersionSummaryTypeDef",
-    "ExportHiddenFieldsOptionOutputTypeDef",
     "ExportHiddenFieldsOptionTypeDef",
-    "DataAggregationOutputTypeDef",
     "DataAggregationTypeDef",
-    "DataBarsOptionsOutputTypeDef",
     "DataBarsOptionsTypeDef",
     "DataColorPaletteOutputTypeDef",
     "DataColorPaletteTypeDef",
-    "DataPathLabelTypeOutputTypeDef",
-    "FieldLabelTypeOutputTypeDef",
-    "MaximumLabelTypeOutputTypeDef",
-    "MinimumLabelTypeOutputTypeDef",
-    "RangeEndsLabelTypeOutputTypeDef",
     "DataPathLabelTypeTypeDef",
     "FieldLabelTypeTypeDef",
     "MaximumLabelTypeTypeDef",
     "MinimumLabelTypeTypeDef",
     "RangeEndsLabelTypeTypeDef",
-    "DataPathValueOutputTypeDef",
     "DataPathValueTypeDef",
     "DataSetSearchFilterTypeDef",
-    "RowLevelPermissionDataSetOutputTypeDef",
-    "DataSetUsageConfigurationOutputTypeDef",
     "FieldFolderOutputTypeDef",
     "OutputColumnTypeDef",
     "DataSourceErrorInfoTypeDef",
-    "DatabricksParametersOutputTypeDef",
-    "ExasolParametersOutputTypeDef",
-    "JiraParametersOutputTypeDef",
-    "MariaDbParametersOutputTypeDef",
-    "MySqlParametersOutputTypeDef",
-    "OracleParametersOutputTypeDef",
-    "PostgreSqlParametersOutputTypeDef",
-    "PrestoParametersOutputTypeDef",
-    "RdsParametersOutputTypeDef",
-    "RedshiftParametersOutputTypeDef",
-    "ServiceNowParametersOutputTypeDef",
-    "SnowflakeParametersOutputTypeDef",
-    "SparkParametersOutputTypeDef",
-    "SqlServerParametersOutputTypeDef",
-    "TeradataParametersOutputTypeDef",
-    "TwitterParametersOutputTypeDef",
     "DatabricksParametersTypeDef",
     "ExasolParametersTypeDef",
     "JiraParametersTypeDef",
     "MariaDbParametersTypeDef",
     "MySqlParametersTypeDef",
     "OracleParametersTypeDef",
     "PostgreSqlParametersTypeDef",
@@ -469,27 +376,23 @@
     "SqlServerParametersTypeDef",
     "TeradataParametersTypeDef",
     "TwitterParametersTypeDef",
     "DataSourceSearchFilterTypeDef",
     "DataSourceSummaryTypeDef",
     "DateTimeDatasetParameterDefaultValuesOutputTypeDef",
     "DateTimeDatasetParameterDefaultValuesTypeDef",
-    "RollingDateConfigurationOutputTypeDef",
     "RollingDateConfigurationTypeDef",
     "DateTimeValueWhenUnsetConfigurationOutputTypeDef",
-    "MappedDataSetParameterOutputTypeDef",
-    "DateTimeValueWhenUnsetConfigurationTypeDef",
     "MappedDataSetParameterTypeDef",
+    "DateTimeValueWhenUnsetConfigurationTypeDef",
     "DateTimeParameterOutputTypeDef",
     "DateTimeParameterTypeDef",
-    "SheetControlInfoIconLabelOptionsOutputTypeDef",
     "SheetControlInfoIconLabelOptionsTypeDef",
     "DecimalDatasetParameterDefaultValuesOutputTypeDef",
     "DecimalDatasetParameterDefaultValuesTypeDef",
-    "DecimalValueWhenUnsetConfigurationOutputTypeDef",
     "DecimalValueWhenUnsetConfigurationTypeDef",
     "DecimalParameterOutputTypeDef",
     "DecimalParameterTypeDef",
     "DeleteAccountCustomizationRequestRequestTypeDef",
     "DeleteAccountSubscriptionRequestRequestTypeDef",
     "DeleteAnalysisRequestRequestTypeDef",
     "DeleteDashboardRequestRequestTypeDef",
@@ -556,105 +459,72 @@
     "TopicRefreshDetailsTypeDef",
     "DescribeTopicRefreshScheduleRequestRequestTypeDef",
     "TopicRefreshScheduleOutputTypeDef",
     "DescribeTopicRequestRequestTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "UserTypeDef",
     "DescribeVPCConnectionRequestRequestTypeDef",
-    "NegativeFormatOutputTypeDef",
     "NegativeFormatTypeDef",
-    "DonutCenterOptionsOutputTypeDef",
     "DonutCenterOptionsTypeDef",
-    "ListControlSelectAllOptionsOutputTypeDef",
     "ListControlSelectAllOptionsTypeDef",
     "ErrorInfoTypeDef",
-    "ExcludePeriodConfigurationOutputTypeDef",
     "ExcludePeriodConfigurationTypeDef",
-    "FieldSortOutputTypeDef",
     "FieldSortTypeDef",
-    "FieldTooltipItemOutputTypeDef",
     "FieldTooltipItemTypeDef",
-    "GeospatialMapStyleOptionsOutputTypeDef",
     "GeospatialMapStyleOptionsTypeDef",
     "FilterSelectableValuesOutputTypeDef",
     "FilterSelectableValuesTypeDef",
-    "FilterOperationOutputTypeDef",
     "SameSheetTargetVisualConfigurationOutputTypeDef",
     "SameSheetTargetVisualConfigurationTypeDef",
     "FilterOperationTypeDef",
     "FolderSearchFilterTypeDef",
     "FolderSummaryTypeDef",
-    "FontSizeOutputTypeDef",
-    "FontWeightOutputTypeDef",
     "FontSizeTypeDef",
     "FontWeightTypeDef",
-    "FontOutputTypeDef",
     "FontTypeDef",
-    "TimeBasedForecastPropertiesOutputTypeDef",
     "TimeBasedForecastPropertiesTypeDef",
     "WhatIfPointScenarioOutputTypeDef",
     "WhatIfRangeScenarioOutputTypeDef",
     "WhatIfPointScenarioTypeDef",
     "WhatIfRangeScenarioTypeDef",
-    "FreeFormLayoutScreenCanvasSizeOptionsOutputTypeDef",
     "FreeFormLayoutScreenCanvasSizeOptionsTypeDef",
-    "FreeFormLayoutElementBackgroundStyleOutputTypeDef",
     "FreeFormLayoutElementBackgroundStyleTypeDef",
-    "FreeFormLayoutElementBorderStyleOutputTypeDef",
     "FreeFormLayoutElementBorderStyleTypeDef",
-    "LoadingAnimationOutputTypeDef",
     "LoadingAnimationTypeDef",
     "SessionTagTypeDef",
-    "GeospatialCoordinateBoundsOutputTypeDef",
     "GeospatialCoordinateBoundsTypeDef",
-    "GeospatialHeatmapDataColorOutputTypeDef",
     "GeospatialHeatmapDataColorTypeDef",
     "GetDashboardEmbedUrlRequestRequestTypeDef",
     "GetSessionEmbedUrlRequestRequestTypeDef",
-    "TableBorderOptionsOutputTypeDef",
     "TableBorderOptionsTypeDef",
-    "GradientStopOutputTypeDef",
     "GradientStopTypeDef",
-    "GridLayoutScreenCanvasSizeOptionsOutputTypeDef",
     "GridLayoutScreenCanvasSizeOptionsTypeDef",
-    "GridLayoutElementOutputTypeDef",
     "GridLayoutElementTypeDef",
     "GroupSearchFilterTypeDef",
-    "GutterStyleOutputTypeDef",
     "GutterStyleTypeDef",
     "IAMPolicyAssignmentSummaryTypeDef",
-    "LookbackWindowOutputTypeDef",
     "LookbackWindowTypeDef",
     "QueueInfoTypeDef",
     "RowInfoTypeDef",
     "IntegerDatasetParameterDefaultValuesOutputTypeDef",
     "IntegerDatasetParameterDefaultValuesTypeDef",
-    "IntegerValueWhenUnsetConfigurationOutputTypeDef",
     "IntegerValueWhenUnsetConfigurationTypeDef",
     "IntegerParameterOutputTypeDef",
     "IntegerParameterTypeDef",
-    "JoinKeyPropertiesOutputTypeDef",
     "JoinKeyPropertiesTypeDef",
-    "ProgressBarOptionsOutputTypeDef",
-    "SecondaryValueOptionsOutputTypeDef",
-    "TrendArrowOptionsOutputTypeDef",
     "ProgressBarOptionsTypeDef",
     "SecondaryValueOptionsTypeDef",
     "TrendArrowOptionsTypeDef",
-    "LineChartLineStyleSettingsOutputTypeDef",
-    "LineChartMarkerStyleSettingsOutputTypeDef",
     "LineChartLineStyleSettingsTypeDef",
     "LineChartMarkerStyleSettingsTypeDef",
-    "MissingDataConfigurationOutputTypeDef",
     "MissingDataConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "ListAnalysesRequestRequestTypeDef",
     "ListAssetBundleExportJobsRequestRequestTypeDef",
     "ListAssetBundleImportJobsRequestRequestTypeDef",
-    "ListControlSearchOptionsOutputTypeDef",
     "ListControlSearchOptionsTypeDef",
     "ListDashboardVersionsRequestRequestTypeDef",
     "ListDashboardsRequestRequestTypeDef",
     "ListDataSetsRequestRequestTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListFolderMembersRequestRequestTypeDef",
     "MemberIdArnPairTypeDef",
@@ -663,15 +533,14 @@
     "ListGroupsRequestRequestTypeDef",
     "ListIAMPolicyAssignmentsForUserRequestRequestTypeDef",
     "ListIAMPolicyAssignmentsRequestRequestTypeDef",
     "ListIngestionsRequestRequestTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListRefreshSchedulesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListTemplateAliasesRequestRequestTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "TemplateVersionSummaryTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "ListThemeAliasesRequestRequestTypeDef",
     "ListThemeVersionsRequestRequestTypeDef",
@@ -680,111 +549,77 @@
     "ThemeSummaryTypeDef",
     "ListTopicRefreshSchedulesRequestRequestTypeDef",
     "ListTopicsRequestRequestTypeDef",
     "TopicSummaryTypeDef",
     "ListUserGroupsRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVPCConnectionsRequestRequestTypeDef",
-    "LongFormatTextOutputTypeDef",
     "LongFormatTextTypeDef",
-    "ManifestFileLocationOutputTypeDef",
     "ManifestFileLocationTypeDef",
-    "MarginStyleOutputTypeDef",
     "MarginStyleTypeDef",
     "NamedEntityDefinitionMetricOutputTypeDef",
     "NamedEntityDefinitionMetricTypeDef",
     "NamespaceErrorTypeDef",
     "NetworkInterfaceTypeDef",
     "NewDefaultValuesOutputTypeDef",
     "NewDefaultValuesTypeDef",
-    "NumericRangeFilterValueOutputTypeDef",
     "NumericRangeFilterValueTypeDef",
-    "ThousandSeparatorOptionsOutputTypeDef",
     "ThousandSeparatorOptionsTypeDef",
-    "PercentileAggregationOutputTypeDef",
     "PercentileAggregationTypeDef",
     "StringParameterOutputTypeDef",
     "StringParameterTypeDef",
-    "PercentVisibleRangeOutputTypeDef",
     "PercentVisibleRangeTypeDef",
-    "PivotTableConditionalFormattingScopeOutputTypeDef",
     "PivotTableConditionalFormattingScopeTypeDef",
-    "PivotTablePaginatedReportOptionsOutputTypeDef",
     "PivotTablePaginatedReportOptionsTypeDef",
-    "PivotTableFieldOptionOutputTypeDef",
     "PivotTableFieldOptionTypeDef",
-    "PivotTableFieldSubtotalOptionsOutputTypeDef",
     "PivotTableFieldSubtotalOptionsTypeDef",
     "RowAlternateColorOptionsOutputTypeDef",
     "RowAlternateColorOptionsTypeDef",
     "ProjectOperationOutputTypeDef",
     "ProjectOperationTypeDef",
-    "RadarChartAreaStyleSettingsOutputTypeDef",
     "RadarChartAreaStyleSettingsTypeDef",
-    "RangeConstantOutputTypeDef",
     "RangeConstantTypeDef",
-    "ReferenceLineCustomLabelConfigurationOutputTypeDef",
     "ReferenceLineCustomLabelConfigurationTypeDef",
-    "ReferenceLineStaticDataConfigurationOutputTypeDef",
     "ReferenceLineStaticDataConfigurationTypeDef",
-    "ReferenceLineStyleConfigurationOutputTypeDef",
     "ReferenceLineStyleConfigurationTypeDef",
-    "ScheduleRefreshOnEntityOutputTypeDef",
     "ScheduleRefreshOnEntityTypeDef",
     "RegisterUserRequestRequestTypeDef",
     "StatePersistenceConfigurationsTypeDef",
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
-    "RenameColumnOperationOutputTypeDef",
     "RenameColumnOperationTypeDef",
     "RestoreAnalysisRequestRequestTypeDef",
-    "RowLevelPermissionTagRuleOutputTypeDef",
     "RowLevelPermissionTagRuleTypeDef",
-    "S3BucketConfigurationOutputTypeDef",
     "S3BucketConfigurationTypeDef",
-    "UploadSettingsOutputTypeDef",
     "UploadSettingsTypeDef",
-    "SectionAfterPageBreakOutputTypeDef",
     "SectionAfterPageBreakTypeDef",
-    "SpacingOutputTypeDef",
     "SpacingTypeDef",
     "SheetVisualScopingConfigurationOutputTypeDef",
     "SheetVisualScopingConfigurationTypeDef",
     "SemanticEntityTypeOutputTypeDef",
     "SemanticEntityTypeTypeDef",
     "SemanticTypeOutputTypeDef",
     "SemanticTypeTypeDef",
-    "SheetTextBoxOutputTypeDef",
     "SheetTextBoxTypeDef",
-    "SheetElementConfigurationOverridesOutputTypeDef",
     "SheetElementConfigurationOverridesTypeDef",
-    "ShortFormatTextOutputTypeDef",
     "ShortFormatTextTypeDef",
-    "SmallMultiplesAxisPropertiesOutputTypeDef",
     "SmallMultiplesAxisPropertiesTypeDef",
     "SnapshotAnonymousUserRedactedTypeDef",
     "SnapshotFileSheetSelectionOutputTypeDef",
     "SnapshotFileSheetSelectionTypeDef",
     "SnapshotJobResultErrorInfoTypeDef",
     "StringDatasetParameterDefaultValuesOutputTypeDef",
     "StringDatasetParameterDefaultValuesTypeDef",
-    "StringValueWhenUnsetConfigurationOutputTypeDef",
     "StringValueWhenUnsetConfigurationTypeDef",
-    "TableCellImageSizingConfigurationOutputTypeDef",
     "TableCellImageSizingConfigurationTypeDef",
-    "TablePaginatedReportOptionsOutputTypeDef",
     "TablePaginatedReportOptionsTypeDef",
-    "TableFieldCustomIconContentOutputTypeDef",
     "TableFieldCustomIconContentTypeDef",
     "TemplateSourceTemplateTypeDef",
-    "TextControlPlaceholderOptionsOutputTypeDef",
     "TextControlPlaceholderOptionsTypeDef",
-    "UIColorPaletteOutputTypeDef",
     "UIColorPaletteTypeDef",
     "ThemeErrorTypeDef",
-    "TopicSingularFilterConstantOutputTypeDef",
     "TopicSingularFilterConstantTypeDef",
     "UntagColumnOperationOutputTypeDef",
     "UntagColumnOperationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccountSettingsRequestRequestTypeDef",
     "UpdateDashboardPublishedVersionRequestRequestTypeDef",
     "UpdateFolderRequestRequestTypeDef",
@@ -792,63 +627,51 @@
     "UpdateIAMPolicyAssignmentRequestRequestTypeDef",
     "UpdateIpRestrictionRequestRequestTypeDef",
     "UpdatePublicSharingSettingsRequestRequestTypeDef",
     "UpdateTemplateAliasRequestRequestTypeDef",
     "UpdateThemeAliasRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateVPCConnectionRequestRequestTypeDef",
-    "WaterfallChartOptionsOutputTypeDef",
     "WaterfallChartOptionsTypeDef",
-    "WordCloudOptionsOutputTypeDef",
     "WordCloudOptionsTypeDef",
     "UpdateAccountCustomizationRequestRequestTypeDef",
-    "AxisLabelReferenceOptionsOutputTypeDef",
-    "CascadingControlSourceOutputTypeDef",
-    "CategoryDrillDownFilterOutputTypeDef",
-    "ContributionAnalysisDefaultOutputTypeDef",
-    "DynamicDefaultValueOutputTypeDef",
-    "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
-    "NumericEqualityDrillDownFilterOutputTypeDef",
-    "ParameterSelectableValuesOutputTypeDef",
-    "TimeEqualityFilterOutputTypeDef",
-    "TimeRangeDrillDownFilterOutputTypeDef",
     "AxisLabelReferenceOptionsTypeDef",
     "CascadingControlSourceTypeDef",
+    "CategoryDrillDownFilterOutputTypeDef",
     "CategoryDrillDownFilterTypeDef",
+    "ContributionAnalysisDefaultOutputTypeDef",
     "ContributionAnalysisDefaultTypeDef",
     "DynamicDefaultValueTypeDef",
+    "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
     "FilterOperationSelectedFieldsConfigurationTypeDef",
     "NumericEqualityDrillDownFilterTypeDef",
+    "ParameterSelectableValuesOutputTypeDef",
     "ParameterSelectableValuesTypeDef",
+    "TimeEqualityFilterOutputTypeDef",
     "TimeEqualityFilterTypeDef",
+    "TimeRangeDrillDownFilterOutputTypeDef",
     "TimeRangeDrillDownFilterTypeDef",
     "AnalysisErrorTypeDef",
     "DashboardErrorTypeDef",
     "TemplateErrorTypeDef",
     "SearchAnalysesRequestRequestTypeDef",
     "AnalysisSourceTemplateTypeDef",
     "DashboardSourceTemplateTypeDef",
     "TemplateSourceAnalysisTypeDef",
     "AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef",
     "RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef",
-    "ArcAxisConfigurationOutputTypeDef",
     "ArcAxisConfigurationTypeDef",
     "AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef",
     "AssetBundleCloudFormationOverridePropertyConfigurationTypeDef",
-    "AssetBundleImportJobDataSourceCredentialsOutputTypeDef",
     "AssetBundleImportJobDataSourceCredentialsTypeDef",
     "AxisDisplayRangeOutputTypeDef",
     "AxisDisplayRangeTypeDef",
-    "AxisScaleOutputTypeDef",
     "AxisScaleTypeDef",
-    "HistogramBinOptionsOutputTypeDef",
     "HistogramBinOptionsTypeDef",
-    "TileStyleOutputTypeDef",
     "TileStyleTypeDef",
-    "BoxPlotOptionsOutputTypeDef",
     "BoxPlotOptionsTypeDef",
     "CreateColumnsOperationOutputTypeDef",
     "CreateColumnsOperationTypeDef",
     "CancelIngestionResponseTypeDef",
     "CreateAccountCustomizationResponseTypeDef",
     "CreateAnalysisResponseTypeDef",
     "CreateDashboardResponseTypeDef",
@@ -924,46 +747,45 @@
     "UpdateTemplateResponseTypeDef",
     "UpdateThemeResponseTypeDef",
     "UpdateTopicRefreshScheduleResponseTypeDef",
     "UpdateTopicResponseTypeDef",
     "UpdateVPCConnectionResponseTypeDef",
     "CategoryFilterConfigurationOutputTypeDef",
     "CategoryFilterConfigurationTypeDef",
-    "ClusterMarkerOutputTypeDef",
     "ClusterMarkerTypeDef",
     "TopicCategoryFilterConstantOutputTypeDef",
     "TopicCategoryFilterConstantTypeDef",
     "ColorScaleOutputTypeDef",
     "ColorScaleTypeDef",
     "ColorsConfigurationOutputTypeDef",
     "ColorsConfigurationTypeDef",
-    "ColumnTagOutputTypeDef",
     "ColumnTagTypeDef",
     "ColumnGroupSchemaOutputTypeDef",
     "ColumnGroupSchemaTypeDef",
     "ColumnGroupOutputTypeDef",
     "ColumnGroupTypeDef",
     "DataSetSchemaOutputTypeDef",
     "DataSetSchemaTypeDef",
-    "ConditionalFormattingCustomIconConditionOutputTypeDef",
     "ConditionalFormattingCustomIconConditionTypeDef",
     "CreateAccountCustomizationRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateVPCConnectionRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateAccountSubscriptionResponseTypeDef",
     "CreateFolderRequestRequestTypeDef",
     "UpdateAnalysisPermissionsRequestRequestTypeDef",
     "UpdateDashboardPermissionsRequestRequestTypeDef",
     "UpdateDataSetPermissionsRequestRequestTypeDef",
     "UpdateDataSourcePermissionsRequestRequestTypeDef",
     "UpdateFolderPermissionsRequestRequestTypeDef",
     "UpdateTemplatePermissionsRequestRequestTypeDef",
     "UpdateThemePermissionsRequestRequestTypeDef",
     "UpdateTopicPermissionsRequestRequestTypeDef",
+    "DataSetSummaryTypeDef",
     "CreateFolderMembershipResponseTypeDef",
     "CreateGroupMembershipResponseTypeDef",
     "DescribeGroupMembershipResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "DescribeGroupResponseTypeDef",
     "ListGroupsResponseTypeDef",
@@ -976,42 +798,36 @@
     "UpdateTemplateAliasResponseTypeDef",
     "CreateThemeAliasResponseTypeDef",
     "DescribeThemeAliasResponseTypeDef",
     "ListThemeAliasesResponseTypeDef",
     "UpdateThemeAliasResponseTypeDef",
     "CreateTopicRefreshScheduleRequestRequestTypeDef",
     "UpdateTopicRefreshScheduleRequestRequestTypeDef",
-    "CustomActionNavigationOperationOutputTypeDef",
     "CustomActionNavigationOperationTypeDef",
     "CustomValuesConfigurationOutputTypeDef",
     "CustomValuesConfigurationTypeDef",
     "CustomSqlOutputTypeDef",
-    "RelationalTableOutputTypeDef",
     "CustomSqlTypeDef",
+    "RelationalTableOutputTypeDef",
     "RelationalTableTypeDef",
     "SearchDashboardsRequestRequestTypeDef",
     "ListDashboardsResponseTypeDef",
     "SearchDashboardsResponseTypeDef",
     "ListDashboardVersionsResponseTypeDef",
-    "DashboardVisualPublishOptionsOutputTypeDef",
     "DashboardVisualPublishOptionsTypeDef",
-    "TableInlineVisualizationOutputTypeDef",
     "TableInlineVisualizationTypeDef",
-    "DataLabelTypeOutputTypeDef",
     "DataLabelTypeTypeDef",
-    "DataPathColorOutputTypeDef",
-    "DataPathSortOutputTypeDef",
-    "PivotTableDataPathOptionOutputTypeDef",
-    "PivotTableFieldCollapseStateTargetOutputTypeDef",
     "DataPathColorTypeDef",
+    "DataPathSortOutputTypeDef",
     "DataPathSortTypeDef",
+    "PivotTableDataPathOptionOutputTypeDef",
     "PivotTableDataPathOptionTypeDef",
+    "PivotTableFieldCollapseStateTargetOutputTypeDef",
     "PivotTableFieldCollapseStateTargetTypeDef",
     "SearchDataSetsRequestRequestTypeDef",
-    "DataSetSummaryTypeDef",
     "SearchDataSourcesRequestRequestTypeDef",
     "SearchDataSourcesResponseTypeDef",
     "DateTimeDatasetParameterOutputTypeDef",
     "DateTimeDatasetParameterTypeDef",
     "TimeRangeFilterValueOutputTypeDef",
     "TimeRangeFilterValueTypeDef",
     "DecimalDatasetParameterOutputTypeDef",
@@ -1035,55 +851,43 @@
     "DescribeTopicRefreshResponseTypeDef",
     "DescribeTopicRefreshScheduleResponseTypeDef",
     "TopicRefreshScheduleSummaryTypeDef",
     "DescribeUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "RegisterUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
-    "DisplayFormatOptionsOutputTypeDef",
     "DisplayFormatOptionsTypeDef",
-    "DonutOptionsOutputTypeDef",
     "DonutOptionsTypeDef",
-    "RelativeDatesFilterOutputTypeDef",
     "RelativeDatesFilterTypeDef",
     "FilterOperationTargetVisualsConfigurationOutputTypeDef",
     "FilterOperationTargetVisualsConfigurationTypeDef",
     "SearchFoldersRequestRequestTypeDef",
     "ListFoldersResponseTypeDef",
     "SearchFoldersResponseTypeDef",
-    "FontConfigurationOutputTypeDef",
     "FontConfigurationTypeDef",
     "TypographyOutputTypeDef",
     "TypographyTypeDef",
     "ForecastScenarioOutputTypeDef",
     "ForecastScenarioTypeDef",
-    "FreeFormLayoutCanvasSizeOptionsOutputTypeDef",
     "FreeFormLayoutCanvasSizeOptionsTypeDef",
     "SnapshotAnonymousUserTypeDef",
-    "GeospatialWindowOptionsOutputTypeDef",
     "GeospatialWindowOptionsTypeDef",
     "GeospatialHeatmapColorScaleOutputTypeDef",
     "GeospatialHeatmapColorScaleTypeDef",
-    "TableSideBorderOptionsOutputTypeDef",
     "TableSideBorderOptionsTypeDef",
     "GradientColorOutputTypeDef",
     "GradientColorTypeDef",
-    "GridLayoutCanvasSizeOptionsOutputTypeDef",
     "GridLayoutCanvasSizeOptionsTypeDef",
     "SearchGroupsRequestRequestTypeDef",
     "ListIAMPolicyAssignmentsResponseTypeDef",
-    "IncrementalRefreshOutputTypeDef",
     "IncrementalRefreshTypeDef",
     "IngestionTypeDef",
     "IntegerDatasetParameterOutputTypeDef",
     "IntegerDatasetParameterTypeDef",
-    "JoinInstructionOutputTypeDef",
     "JoinInstructionTypeDef",
-    "LineChartDefaultSeriesSettingsOutputTypeDef",
-    "LineChartSeriesSettingsOutputTypeDef",
     "LineChartDefaultSeriesSettingsTypeDef",
     "LineChartSeriesSettingsTypeDef",
     "ListAnalysesRequestListAnalysesPaginateTypeDef",
     "ListAssetBundleExportJobsRequestListAssetBundleExportJobsPaginateTypeDef",
     "ListAssetBundleImportJobsRequestListAssetBundleImportJobsPaginateTypeDef",
     "ListDashboardVersionsRequestListDashboardVersionsPaginateTypeDef",
     "ListDashboardsRequestListDashboardsPaginateTypeDef",
@@ -1104,222 +908,177 @@
     "ListUsersRequestListUsersPaginateTypeDef",
     "SearchAnalysesRequestSearchAnalysesPaginateTypeDef",
     "SearchDashboardsRequestSearchDashboardsPaginateTypeDef",
     "SearchDataSetsRequestSearchDataSetsPaginateTypeDef",
     "SearchDataSourcesRequestSearchDataSourcesPaginateTypeDef",
     "SearchGroupsRequestSearchGroupsPaginateTypeDef",
     "ListFolderMembersResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTemplateVersionsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "ListThemeVersionsResponseTypeDef",
     "ListThemesResponseTypeDef",
     "ListTopicsResponseTypeDef",
-    "VisualSubtitleLabelOptionsOutputTypeDef",
     "VisualSubtitleLabelOptionsTypeDef",
-    "S3ParametersOutputTypeDef",
     "S3ParametersTypeDef",
-    "TileLayoutStyleOutputTypeDef",
     "TileLayoutStyleTypeDef",
     "NamedEntityDefinitionOutputTypeDef",
     "NamedEntityDefinitionTypeDef",
     "NamespaceInfoV2TypeDef",
     "VPCConnectionSummaryTypeDef",
     "VPCConnectionTypeDef",
     "OverrideDatasetParameterOperationOutputTypeDef",
     "OverrideDatasetParameterOperationTypeDef",
-    "NumericSeparatorConfigurationOutputTypeDef",
     "NumericSeparatorConfigurationTypeDef",
-    "NumericalAggregationFunctionOutputTypeDef",
     "NumericalAggregationFunctionTypeDef",
     "ParametersOutputTypeDef",
     "ParametersTypeDef",
-    "VisibleRangeOptionsOutputTypeDef",
     "VisibleRangeOptionsTypeDef",
-    "RadarChartSeriesSettingsOutputTypeDef",
     "RadarChartSeriesSettingsTypeDef",
-    "TopicRangeFilterConstantOutputTypeDef",
     "TopicRangeFilterConstantTypeDef",
-    "RefreshFrequencyOutputTypeDef",
     "RefreshFrequencyTypeDef",
     "RegisteredUserConsoleFeatureConfigurationsTypeDef",
     "RegisteredUserDashboardFeatureConfigurationsTypeDef",
     "RowLevelPermissionTagConfigurationOutputTypeDef",
     "RowLevelPermissionTagConfigurationTypeDef",
-    "SnapshotS3DestinationConfigurationOutputTypeDef",
     "SnapshotS3DestinationConfigurationTypeDef",
     "S3SourceOutputTypeDef",
     "S3SourceTypeDef",
-    "SectionPageBreakConfigurationOutputTypeDef",
     "SectionPageBreakConfigurationTypeDef",
-    "SectionBasedLayoutPaperCanvasSizeOptionsOutputTypeDef",
-    "SectionStyleOutputTypeDef",
     "SectionBasedLayoutPaperCanvasSizeOptionsTypeDef",
     "SectionStyleTypeDef",
     "SelectedSheetsFilterScopeConfigurationOutputTypeDef",
     "SelectedSheetsFilterScopeConfigurationTypeDef",
-    "SheetElementRenderingRuleOutputTypeDef",
     "SheetElementRenderingRuleTypeDef",
-    "VisualTitleLabelOptionsOutputTypeDef",
     "VisualTitleLabelOptionsTypeDef",
     "SnapshotUserConfigurationRedactedTypeDef",
     "SnapshotFileOutputTypeDef",
     "SnapshotFileTypeDef",
     "StringDatasetParameterOutputTypeDef",
     "StringDatasetParameterTypeDef",
-    "TableFieldImageConfigurationOutputTypeDef",
     "TableFieldImageConfigurationTypeDef",
-    "TopicNumericEqualityFilterOutputTypeDef",
-    "TopicRelativeDateFilterOutputTypeDef",
     "TopicNumericEqualityFilterTypeDef",
     "TopicRelativeDateFilterTypeDef",
     "CascadingControlConfigurationOutputTypeDef",
-    "DateTimeDefaultValuesOutputTypeDef",
-    "DecimalDefaultValuesOutputTypeDef",
-    "IntegerDefaultValuesOutputTypeDef",
-    "StringDefaultValuesOutputTypeDef",
-    "DrillDownFilterOutputTypeDef",
     "CascadingControlConfigurationTypeDef",
+    "DateTimeDefaultValuesOutputTypeDef",
     "DateTimeDefaultValuesTypeDef",
+    "DecimalDefaultValuesOutputTypeDef",
     "DecimalDefaultValuesTypeDef",
+    "IntegerDefaultValuesOutputTypeDef",
     "IntegerDefaultValuesTypeDef",
+    "StringDefaultValuesOutputTypeDef",
     "StringDefaultValuesTypeDef",
+    "DrillDownFilterOutputTypeDef",
     "DrillDownFilterTypeDef",
     "AnalysisTypeDef",
     "DashboardVersionTypeDef",
     "AnalysisSourceEntityTypeDef",
     "DashboardSourceEntityTypeDef",
     "TemplateSourceEntityTypeDef",
     "AnonymousUserEmbeddingExperienceConfigurationTypeDef",
     "DescribeAssetBundleExportJobResponseTypeDef",
     "StartAssetBundleExportJobRequestRequestTypeDef",
     "NumericAxisOptionsOutputTypeDef",
     "NumericAxisOptionsTypeDef",
     "CategoryFilterOutputTypeDef",
     "CategoryFilterTypeDef",
-    "ClusterMarkerConfigurationOutputTypeDef",
     "ClusterMarkerConfigurationTypeDef",
     "TopicCategoryFilterOutputTypeDef",
     "TopicCategoryFilterTypeDef",
     "TagColumnOperationOutputTypeDef",
     "TagColumnOperationTypeDef",
     "DataSetConfigurationOutputTypeDef",
     "DataSetConfigurationTypeDef",
-    "ConditionalFormattingIconOutputTypeDef",
     "ConditionalFormattingIconTypeDef",
+    "ListDataSetsResponseTypeDef",
+    "SearchDataSetsResponseTypeDef",
     "DestinationParameterValueConfigurationOutputTypeDef",
     "DestinationParameterValueConfigurationTypeDef",
-    "DashboardPublishOptionsOutputTypeDef",
     "DashboardPublishOptionsTypeDef",
     "VisualPaletteOutputTypeDef",
-    "PivotTableFieldCollapseStateOptionOutputTypeDef",
     "VisualPaletteTypeDef",
+    "PivotTableFieldCollapseStateOptionOutputTypeDef",
     "PivotTableFieldCollapseStateOptionTypeDef",
-    "ListDataSetsResponseTypeDef",
-    "SearchDataSetsResponseTypeDef",
     "TimeRangeFilterOutputTypeDef",
     "TimeRangeFilterTypeDef",
     "DescribeDashboardPermissionsResponseTypeDef",
     "UpdateDashboardPermissionsResponseTypeDef",
     "ListTopicRefreshSchedulesResponseTypeDef",
-    "DefaultFormattingOutputTypeDef",
     "DefaultFormattingTypeDef",
     "CustomActionFilterOperationOutputTypeDef",
     "CustomActionFilterOperationTypeDef",
-    "AxisLabelOptionsOutputTypeDef",
-    "DataLabelOptionsOutputTypeDef",
-    "FunnelChartDataLabelOptionsOutputTypeDef",
-    "LabelOptionsOutputTypeDef",
-    "PanelTitleOptionsOutputTypeDef",
-    "TableFieldCustomTextContentOutputTypeDef",
     "AxisLabelOptionsTypeDef",
+    "DataLabelOptionsOutputTypeDef",
     "DataLabelOptionsTypeDef",
     "FunnelChartDataLabelOptionsTypeDef",
     "LabelOptionsTypeDef",
     "PanelTitleOptionsTypeDef",
     "TableFieldCustomTextContentTypeDef",
     "ForecastConfigurationOutputTypeDef",
     "ForecastConfigurationTypeDef",
-    "DefaultFreeFormLayoutConfigurationOutputTypeDef",
     "DefaultFreeFormLayoutConfigurationTypeDef",
     "SnapshotUserConfigurationTypeDef",
     "GeospatialHeatmapConfigurationOutputTypeDef",
     "GeospatialHeatmapConfigurationTypeDef",
-    "GlobalTableBorderOptionsOutputTypeDef",
     "GlobalTableBorderOptionsTypeDef",
     "ConditionalFormattingGradientColorOutputTypeDef",
     "ConditionalFormattingGradientColorTypeDef",
-    "DefaultGridLayoutConfigurationOutputTypeDef",
-    "GridLayoutConfigurationOutputTypeDef",
     "DefaultGridLayoutConfigurationTypeDef",
+    "GridLayoutConfigurationOutputTypeDef",
     "GridLayoutConfigurationTypeDef",
-    "RefreshConfigurationOutputTypeDef",
     "RefreshConfigurationTypeDef",
     "DescribeIngestionResponseTypeDef",
     "ListIngestionsResponseTypeDef",
-    "LogicalTableSourceOutputTypeDef",
     "LogicalTableSourceTypeDef",
-    "DataFieldSeriesItemOutputTypeDef",
-    "FieldSeriesItemOutputTypeDef",
     "DataFieldSeriesItemTypeDef",
     "FieldSeriesItemTypeDef",
-    "DataSourceParametersOutputTypeDef",
     "DataSourceParametersTypeDef",
-    "SheetStyleOutputTypeDef",
     "SheetStyleTypeDef",
     "TopicNamedEntityOutputTypeDef",
     "TopicNamedEntityTypeDef",
     "DescribeNamespaceResponseTypeDef",
     "ListNamespacesResponseTypeDef",
     "ListVPCConnectionsResponseTypeDef",
     "DescribeVPCConnectionResponseTypeDef",
-    "CurrencyDisplayFormatConfigurationOutputTypeDef",
-    "NumberDisplayFormatConfigurationOutputTypeDef",
-    "PercentageDisplayFormatConfigurationOutputTypeDef",
     "CurrencyDisplayFormatConfigurationTypeDef",
     "NumberDisplayFormatConfigurationTypeDef",
     "PercentageDisplayFormatConfigurationTypeDef",
-    "AggregationFunctionOutputTypeDef",
     "AggregationFunctionTypeDef",
-    "ScrollBarOptionsOutputTypeDef",
     "ScrollBarOptionsTypeDef",
-    "TopicDateRangeFilterOutputTypeDef",
-    "TopicNumericRangeFilterOutputTypeDef",
     "TopicDateRangeFilterTypeDef",
     "TopicNumericRangeFilterTypeDef",
     "RefreshScheduleOutputTypeDef",
     "RefreshScheduleTypeDef",
     "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
     "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
     "SnapshotDestinationConfigurationOutputTypeDef",
-    "SnapshotJobS3ResultTypeDef",
     "SnapshotDestinationConfigurationTypeDef",
+    "SnapshotJobS3ResultTypeDef",
     "PhysicalTableOutputTypeDef",
     "PhysicalTableTypeDef",
-    "SectionBasedLayoutCanvasSizeOptionsOutputTypeDef",
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
     "FilterScopeConfigurationOutputTypeDef",
     "FilterScopeConfigurationTypeDef",
     "FreeFormLayoutElementOutputTypeDef",
     "FreeFormLayoutElementTypeDef",
     "SnapshotFileGroupOutputTypeDef",
     "SnapshotFileGroupTypeDef",
     "DatasetParameterOutputTypeDef",
     "DatasetParameterTypeDef",
     "DateTimeParameterDeclarationOutputTypeDef",
+    "DateTimeParameterDeclarationTypeDef",
     "DecimalParameterDeclarationOutputTypeDef",
+    "DecimalParameterDeclarationTypeDef",
     "IntegerParameterDeclarationOutputTypeDef",
+    "IntegerParameterDeclarationTypeDef",
     "StringParameterDeclarationOutputTypeDef",
+    "StringParameterDeclarationTypeDef",
     "DateTimeHierarchyOutputTypeDef",
     "ExplicitHierarchyOutputTypeDef",
     "PredefinedHierarchyOutputTypeDef",
-    "DateTimeParameterDeclarationTypeDef",
-    "DecimalParameterDeclarationTypeDef",
-    "IntegerParameterDeclarationTypeDef",
-    "StringParameterDeclarationTypeDef",
     "DateTimeHierarchyTypeDef",
     "ExplicitHierarchyTypeDef",
     "PredefinedHierarchyTypeDef",
     "DescribeAnalysisResponseTypeDef",
     "DashboardTypeDef",
     "GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
     "AxisDataOptionsOutputTypeDef",
@@ -1328,143 +1087,105 @@
     "TransformOperationTypeDef",
     "TemplateVersionTypeDef",
     "SetParameterValueConfigurationOutputTypeDef",
     "SetParameterValueConfigurationTypeDef",
     "PivotTableFieldOptionsOutputTypeDef",
     "PivotTableFieldOptionsTypeDef",
     "TopicCalculatedFieldOutputTypeDef",
-    "TopicColumnOutputTypeDef",
     "TopicCalculatedFieldTypeDef",
+    "TopicColumnOutputTypeDef",
     "TopicColumnTypeDef",
     "ChartAxisLabelOptionsOutputTypeDef",
-    "AxisTickLabelOptionsOutputTypeDef",
-    "DateTimePickerControlDisplayOptionsOutputTypeDef",
-    "DropDownControlDisplayOptionsOutputTypeDef",
-    "LegendOptionsOutputTypeDef",
-    "ListControlDisplayOptionsOutputTypeDef",
-    "RelativeDateTimeControlDisplayOptionsOutputTypeDef",
-    "SliderControlDisplayOptionsOutputTypeDef",
-    "TextAreaControlDisplayOptionsOutputTypeDef",
-    "TextFieldControlDisplayOptionsOutputTypeDef",
-    "PanelConfigurationOutputTypeDef",
-    "TableFieldLinkContentConfigurationOutputTypeDef",
     "ChartAxisLabelOptionsTypeDef",
     "AxisTickLabelOptionsTypeDef",
     "DateTimePickerControlDisplayOptionsTypeDef",
     "DropDownControlDisplayOptionsTypeDef",
     "LegendOptionsTypeDef",
     "ListControlDisplayOptionsTypeDef",
     "RelativeDateTimeControlDisplayOptionsTypeDef",
     "SliderControlDisplayOptionsTypeDef",
     "TextAreaControlDisplayOptionsTypeDef",
     "TextFieldControlDisplayOptionsTypeDef",
     "PanelConfigurationTypeDef",
     "TableFieldLinkContentConfigurationTypeDef",
     "GeospatialPointStyleOptionsOutputTypeDef",
     "GeospatialPointStyleOptionsTypeDef",
-    "TableCellStyleOutputTypeDef",
     "TableCellStyleTypeDef",
     "ConditionalFormattingColorOutputTypeDef",
     "ConditionalFormattingColorTypeDef",
-    "DefaultInteractiveLayoutConfigurationOutputTypeDef",
-    "SheetControlLayoutConfigurationOutputTypeDef",
     "DefaultInteractiveLayoutConfigurationTypeDef",
+    "SheetControlLayoutConfigurationOutputTypeDef",
     "SheetControlLayoutConfigurationTypeDef",
-    "DataSetRefreshPropertiesOutputTypeDef",
     "DataSetRefreshPropertiesTypeDef",
-    "SeriesItemOutputTypeDef",
     "SeriesItemTypeDef",
-    "AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef",
-    "DataSourceTypeDef",
     "AssetBundleImportJobDataSourceOverrideParametersTypeDef",
     "CredentialPairTypeDef",
+    "DataSourceTypeDef",
     "ThemeConfigurationOutputTypeDef",
     "ThemeConfigurationTypeDef",
-    "ComparisonFormatConfigurationOutputTypeDef",
-    "NumericFormatConfigurationOutputTypeDef",
     "ComparisonFormatConfigurationTypeDef",
     "NumericFormatConfigurationTypeDef",
-    "AggregationSortConfigurationOutputTypeDef",
-    "ColumnSortOutputTypeDef",
-    "ColumnTooltipItemOutputTypeDef",
-    "NumericEqualityFilterOutputTypeDef",
-    "NumericRangeFilterOutputTypeDef",
-    "ReferenceLineDynamicDataConfigurationOutputTypeDef",
     "AggregationSortConfigurationTypeDef",
     "ColumnSortTypeDef",
     "ColumnTooltipItemTypeDef",
     "NumericEqualityFilterTypeDef",
     "NumericRangeFilterTypeDef",
     "ReferenceLineDynamicDataConfigurationTypeDef",
     "TopicFilterOutputTypeDef",
     "TopicFilterTypeDef",
     "DescribeRefreshScheduleResponseTypeDef",
     "ListRefreshSchedulesResponseTypeDef",
     "CreateRefreshScheduleRequestRequestTypeDef",
     "UpdateRefreshScheduleRequestRequestTypeDef",
     "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
     "SnapshotJobResultFileGroupTypeDef",
-    "DefaultSectionBasedLayoutConfigurationOutputTypeDef",
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     "FreeFormLayoutConfigurationOutputTypeDef",
     "FreeFormSectionLayoutConfigurationOutputTypeDef",
     "FreeFormLayoutConfigurationTypeDef",
     "FreeFormSectionLayoutConfigurationTypeDef",
     "SnapshotConfigurationOutputTypeDef",
     "SnapshotConfigurationTypeDef",
     "ParameterDeclarationOutputTypeDef",
-    "ColumnHierarchyOutputTypeDef",
     "ParameterDeclarationTypeDef",
+    "ColumnHierarchyOutputTypeDef",
     "ColumnHierarchyTypeDef",
     "DescribeDashboardResponseTypeDef",
     "LogicalTableOutputTypeDef",
     "LogicalTableTypeDef",
     "TemplateTypeDef",
     "CustomActionSetParametersOperationOutputTypeDef",
     "CustomActionSetParametersOperationTypeDef",
     "AxisDisplayOptionsOutputTypeDef",
-    "FilterDateTimePickerControlOutputTypeDef",
-    "ParameterDateTimePickerControlOutputTypeDef",
-    "FilterDropDownControlOutputTypeDef",
-    "ParameterDropDownControlOutputTypeDef",
-    "FilterListControlOutputTypeDef",
-    "ParameterListControlOutputTypeDef",
-    "FilterRelativeDateTimeControlOutputTypeDef",
-    "FilterSliderControlOutputTypeDef",
-    "ParameterSliderControlOutputTypeDef",
-    "FilterTextAreaControlOutputTypeDef",
-    "ParameterTextAreaControlOutputTypeDef",
-    "FilterTextFieldControlOutputTypeDef",
-    "ParameterTextFieldControlOutputTypeDef",
-    "SmallMultiplesOptionsOutputTypeDef",
-    "TableFieldLinkConfigurationOutputTypeDef",
     "AxisDisplayOptionsTypeDef",
     "FilterDateTimePickerControlTypeDef",
     "ParameterDateTimePickerControlTypeDef",
+    "FilterDropDownControlOutputTypeDef",
     "FilterDropDownControlTypeDef",
+    "ParameterDropDownControlOutputTypeDef",
     "ParameterDropDownControlTypeDef",
+    "FilterListControlOutputTypeDef",
     "FilterListControlTypeDef",
+    "ParameterListControlOutputTypeDef",
     "ParameterListControlTypeDef",
     "FilterRelativeDateTimeControlTypeDef",
     "FilterSliderControlTypeDef",
     "ParameterSliderControlTypeDef",
     "FilterTextAreaControlTypeDef",
     "ParameterTextAreaControlTypeDef",
     "FilterTextFieldControlTypeDef",
     "ParameterTextFieldControlTypeDef",
     "SmallMultiplesOptionsTypeDef",
     "TableFieldLinkConfigurationTypeDef",
     "PivotTableOptionsOutputTypeDef",
-    "PivotTotalOptionsOutputTypeDef",
-    "SubtotalOptionsOutputTypeDef",
-    "TableOptionsOutputTypeDef",
-    "TotalOptionsOutputTypeDef",
     "PivotTableOptionsTypeDef",
     "PivotTotalOptionsTypeDef",
+    "SubtotalOptionsOutputTypeDef",
     "SubtotalOptionsTypeDef",
+    "TableOptionsOutputTypeDef",
     "TableOptionsTypeDef",
     "TotalOptionsTypeDef",
     "GaugeChartArcConditionalFormattingOutputTypeDef",
     "GaugeChartPrimaryValueConditionalFormattingOutputTypeDef",
     "KPIPrimaryValueConditionalFormattingOutputTypeDef",
     "KPIProgressBarConditionalFormattingOutputTypeDef",
     "ShapeConditionalFormatOutputTypeDef",
@@ -1478,63 +1199,53 @@
     "TableRowConditionalFormattingTypeDef",
     "TextConditionalFormatTypeDef",
     "SheetControlLayoutOutputTypeDef",
     "SheetControlLayoutTypeDef",
     "DescribeDataSetRefreshPropertiesResponseTypeDef",
     "PutDataSetRefreshPropertiesRequestRequestTypeDef",
     "AssetBundleImportJobOverrideParametersOutputTypeDef",
-    "DescribeDataSourceResponseTypeDef",
-    "ListDataSourcesResponseTypeDef",
     "AssetBundleImportJobOverrideParametersTypeDef",
     "DataSourceCredentialsTypeDef",
+    "DescribeDataSourceResponseTypeDef",
+    "ListDataSourcesResponseTypeDef",
     "ThemeVersionTypeDef",
     "CreateThemeRequestRequestTypeDef",
     "UpdateThemeRequestRequestTypeDef",
-    "ComparisonConfigurationOutputTypeDef",
-    "DateTimeFormatConfigurationOutputTypeDef",
-    "NumberFormatConfigurationOutputTypeDef",
-    "ReferenceLineValueLabelConfigurationOutputTypeDef",
-    "StringFormatConfigurationOutputTypeDef",
     "ComparisonConfigurationTypeDef",
     "DateTimeFormatConfigurationTypeDef",
     "NumberFormatConfigurationTypeDef",
     "ReferenceLineValueLabelConfigurationTypeDef",
     "StringFormatConfigurationTypeDef",
     "TopBottomFilterOutputTypeDef",
-    "FieldSortOptionsOutputTypeDef",
-    "PivotTableSortByOutputTypeDef",
-    "TooltipItemOutputTypeDef",
-    "ReferenceLineDataConfigurationOutputTypeDef",
     "TopBottomFilterTypeDef",
     "FieldSortOptionsTypeDef",
+    "PivotTableSortByOutputTypeDef",
     "PivotTableSortByTypeDef",
     "TooltipItemTypeDef",
     "ReferenceLineDataConfigurationTypeDef",
     "DatasetMetadataOutputTypeDef",
     "DatasetMetadataTypeDef",
     "GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
     "AnonymousUserSnapshotJobResultTypeDef",
-    "DefaultPaginatedLayoutConfigurationOutputTypeDef",
     "DefaultPaginatedLayoutConfigurationTypeDef",
     "SectionLayoutConfigurationOutputTypeDef",
     "SectionLayoutConfigurationTypeDef",
     "DescribeDashboardSnapshotJobResponseTypeDef",
     "StartDashboardSnapshotJobRequestRequestTypeDef",
     "DataSetTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "UpdateDataSetRequestRequestTypeDef",
     "DescribeTemplateResponseTypeDef",
     "VisualCustomActionOperationOutputTypeDef",
     "VisualCustomActionOperationTypeDef",
     "LineSeriesAxisDisplayOptionsOutputTypeDef",
-    "FilterControlOutputTypeDef",
-    "ParameterControlOutputTypeDef",
-    "TableFieldURLConfigurationOutputTypeDef",
     "LineSeriesAxisDisplayOptionsTypeDef",
+    "FilterControlOutputTypeDef",
     "FilterControlTypeDef",
+    "ParameterControlOutputTypeDef",
     "ParameterControlTypeDef",
     "TableFieldURLConfigurationTypeDef",
     "PivotTableTotalOptionsOutputTypeDef",
     "PivotTableTotalOptionsTypeDef",
     "GaugeChartConditionalFormattingOptionOutputTypeDef",
     "KPIConditionalFormattingOptionOutputTypeDef",
     "FilledMapShapeConditionalFormattingOutputTypeDef",
@@ -1546,116 +1257,99 @@
     "PivotTableCellConditionalFormattingTypeDef",
     "TableCellConditionalFormattingTypeDef",
     "DescribeAssetBundleImportJobResponseTypeDef",
     "StartAssetBundleImportJobRequestRequestTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "ThemeTypeDef",
-    "GaugeChartOptionsOutputTypeDef",
-    "KPIOptionsOutputTypeDef",
-    "DateDimensionFieldOutputTypeDef",
-    "DateMeasureFieldOutputTypeDef",
-    "NumericalDimensionFieldOutputTypeDef",
-    "NumericalMeasureFieldOutputTypeDef",
-    "ReferenceLineLabelConfigurationOutputTypeDef",
-    "CategoricalDimensionFieldOutputTypeDef",
-    "CategoricalMeasureFieldOutputTypeDef",
-    "FormatConfigurationOutputTypeDef",
     "GaugeChartOptionsTypeDef",
     "KPIOptionsTypeDef",
     "DateDimensionFieldTypeDef",
     "DateMeasureFieldTypeDef",
     "NumericalDimensionFieldTypeDef",
     "NumericalMeasureFieldTypeDef",
     "ReferenceLineLabelConfigurationTypeDef",
     "CategoricalDimensionFieldTypeDef",
     "CategoricalMeasureFieldTypeDef",
     "FormatConfigurationTypeDef",
     "FilterOutputTypeDef",
-    "BarChartSortConfigurationOutputTypeDef",
-    "BoxPlotSortConfigurationOutputTypeDef",
-    "ComboChartSortConfigurationOutputTypeDef",
-    "FilledMapSortConfigurationOutputTypeDef",
-    "FunnelChartSortConfigurationOutputTypeDef",
-    "HeatMapSortConfigurationOutputTypeDef",
-    "KPISortConfigurationOutputTypeDef",
-    "LineChartSortConfigurationOutputTypeDef",
-    "PieChartSortConfigurationOutputTypeDef",
-    "RadarChartSortConfigurationOutputTypeDef",
-    "SankeyDiagramSortConfigurationOutputTypeDef",
-    "TableSortConfigurationOutputTypeDef",
-    "TreeMapSortConfigurationOutputTypeDef",
-    "WaterfallChartSortConfigurationOutputTypeDef",
-    "WordCloudSortConfigurationOutputTypeDef",
-    "PivotFieldSortOptionsOutputTypeDef",
-    "FieldBasedTooltipOutputTypeDef",
     "FilterTypeDef",
+    "BarChartSortConfigurationOutputTypeDef",
     "BarChartSortConfigurationTypeDef",
+    "BoxPlotSortConfigurationOutputTypeDef",
     "BoxPlotSortConfigurationTypeDef",
+    "ComboChartSortConfigurationOutputTypeDef",
     "ComboChartSortConfigurationTypeDef",
+    "FilledMapSortConfigurationOutputTypeDef",
     "FilledMapSortConfigurationTypeDef",
+    "FunnelChartSortConfigurationOutputTypeDef",
     "FunnelChartSortConfigurationTypeDef",
+    "HeatMapSortConfigurationOutputTypeDef",
     "HeatMapSortConfigurationTypeDef",
+    "KPISortConfigurationOutputTypeDef",
     "KPISortConfigurationTypeDef",
+    "LineChartSortConfigurationOutputTypeDef",
     "LineChartSortConfigurationTypeDef",
+    "PieChartSortConfigurationOutputTypeDef",
     "PieChartSortConfigurationTypeDef",
+    "RadarChartSortConfigurationOutputTypeDef",
     "RadarChartSortConfigurationTypeDef",
+    "SankeyDiagramSortConfigurationOutputTypeDef",
     "SankeyDiagramSortConfigurationTypeDef",
+    "TableSortConfigurationOutputTypeDef",
     "TableSortConfigurationTypeDef",
+    "TreeMapSortConfigurationOutputTypeDef",
     "TreeMapSortConfigurationTypeDef",
+    "WaterfallChartSortConfigurationOutputTypeDef",
     "WaterfallChartSortConfigurationTypeDef",
+    "WordCloudSortConfigurationOutputTypeDef",
     "WordCloudSortConfigurationTypeDef",
+    "PivotFieldSortOptionsOutputTypeDef",
     "PivotFieldSortOptionsTypeDef",
+    "FieldBasedTooltipOutputTypeDef",
     "FieldBasedTooltipTypeDef",
     "TopicDetailsOutputTypeDef",
     "TopicDetailsTypeDef",
     "SnapshotJobResultTypeDef",
-    "DefaultNewSheetConfigurationOutputTypeDef",
     "DefaultNewSheetConfigurationTypeDef",
     "BodySectionContentOutputTypeDef",
     "HeaderFooterSectionConfigurationOutputTypeDef",
     "BodySectionContentTypeDef",
     "HeaderFooterSectionConfigurationTypeDef",
     "DescribeDataSetResponseTypeDef",
     "VisualCustomActionOutputTypeDef",
     "VisualCustomActionTypeDef",
-    "TableFieldOptionOutputTypeDef",
     "TableFieldOptionTypeDef",
     "GaugeChartConditionalFormattingOutputTypeDef",
     "KPIConditionalFormattingOutputTypeDef",
     "FilledMapConditionalFormattingOptionOutputTypeDef",
     "PivotTableConditionalFormattingOptionOutputTypeDef",
     "TableConditionalFormattingOptionOutputTypeDef",
     "GaugeChartConditionalFormattingTypeDef",
     "KPIConditionalFormattingTypeDef",
     "FilledMapConditionalFormattingOptionTypeDef",
     "PivotTableConditionalFormattingOptionTypeDef",
     "TableConditionalFormattingOptionTypeDef",
     "DescribeThemeResponseTypeDef",
-    "ReferenceLineOutputTypeDef",
-    "DimensionFieldOutputTypeDef",
-    "MeasureFieldOutputTypeDef",
-    "ColumnConfigurationOutputTypeDef",
-    "UnaggregatedFieldOutputTypeDef",
     "ReferenceLineTypeDef",
     "DimensionFieldTypeDef",
     "MeasureFieldTypeDef",
+    "ColumnConfigurationOutputTypeDef",
     "ColumnConfigurationTypeDef",
     "UnaggregatedFieldTypeDef",
     "FilterGroupOutputTypeDef",
-    "PivotTableSortConfigurationOutputTypeDef",
-    "TooltipOptionsOutputTypeDef",
     "FilterGroupTypeDef",
+    "PivotTableSortConfigurationOutputTypeDef",
     "PivotTableSortConfigurationTypeDef",
+    "TooltipOptionsOutputTypeDef",
     "TooltipOptionsTypeDef",
     "DescribeTopicResponseTypeDef",
     "CreateTopicRequestRequestTypeDef",
     "UpdateTopicRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobResultResponseTypeDef",
-    "AnalysisDefaultsOutputTypeDef",
     "AnalysisDefaultsTypeDef",
     "BodySectionConfigurationOutputTypeDef",
     "BodySectionConfigurationTypeDef",
     "CustomContentVisualOutputTypeDef",
     "EmptyVisualOutputTypeDef",
     "CustomContentVisualTypeDef",
     "EmptyVisualTypeDef",
@@ -1663,205 +1357,194 @@
     "TableFieldOptionsTypeDef",
     "FilledMapConditionalFormattingOutputTypeDef",
     "PivotTableConditionalFormattingOutputTypeDef",
     "TableConditionalFormattingOutputTypeDef",
     "FilledMapConditionalFormattingTypeDef",
     "PivotTableConditionalFormattingTypeDef",
     "TableConditionalFormattingTypeDef",
-    "UniqueValuesComputationOutputTypeDef",
-    "BarChartAggregatedFieldWellsOutputTypeDef",
-    "BoxPlotAggregatedFieldWellsOutputTypeDef",
-    "ComboChartAggregatedFieldWellsOutputTypeDef",
-    "FilledMapAggregatedFieldWellsOutputTypeDef",
-    "ForecastComputationOutputTypeDef",
-    "FunnelChartAggregatedFieldWellsOutputTypeDef",
-    "GaugeChartFieldWellsOutputTypeDef",
-    "GeospatialMapAggregatedFieldWellsOutputTypeDef",
-    "GrowthRateComputationOutputTypeDef",
-    "HeatMapAggregatedFieldWellsOutputTypeDef",
-    "HistogramAggregatedFieldWellsOutputTypeDef",
-    "KPIFieldWellsOutputTypeDef",
-    "LineChartAggregatedFieldWellsOutputTypeDef",
-    "MaximumMinimumComputationOutputTypeDef",
-    "MetricComparisonComputationOutputTypeDef",
-    "PeriodOverPeriodComputationOutputTypeDef",
-    "PeriodToDateComputationOutputTypeDef",
-    "PieChartAggregatedFieldWellsOutputTypeDef",
-    "PivotTableAggregatedFieldWellsOutputTypeDef",
-    "RadarChartAggregatedFieldWellsOutputTypeDef",
-    "SankeyDiagramAggregatedFieldWellsOutputTypeDef",
-    "ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef",
-    "ScatterPlotUnaggregatedFieldWellsOutputTypeDef",
-    "TableAggregatedFieldWellsOutputTypeDef",
-    "TopBottomMoversComputationOutputTypeDef",
-    "TopBottomRankedComputationOutputTypeDef",
-    "TotalAggregationComputationOutputTypeDef",
-    "TreeMapAggregatedFieldWellsOutputTypeDef",
-    "WaterfallChartAggregatedFieldWellsOutputTypeDef",
-    "WordCloudAggregatedFieldWellsOutputTypeDef",
-    "TableUnaggregatedFieldWellsOutputTypeDef",
     "UniqueValuesComputationTypeDef",
+    "BarChartAggregatedFieldWellsOutputTypeDef",
     "BarChartAggregatedFieldWellsTypeDef",
+    "BoxPlotAggregatedFieldWellsOutputTypeDef",
     "BoxPlotAggregatedFieldWellsTypeDef",
+    "ComboChartAggregatedFieldWellsOutputTypeDef",
     "ComboChartAggregatedFieldWellsTypeDef",
+    "FilledMapAggregatedFieldWellsOutputTypeDef",
     "FilledMapAggregatedFieldWellsTypeDef",
     "ForecastComputationTypeDef",
+    "FunnelChartAggregatedFieldWellsOutputTypeDef",
     "FunnelChartAggregatedFieldWellsTypeDef",
+    "GaugeChartFieldWellsOutputTypeDef",
     "GaugeChartFieldWellsTypeDef",
+    "GeospatialMapAggregatedFieldWellsOutputTypeDef",
     "GeospatialMapAggregatedFieldWellsTypeDef",
     "GrowthRateComputationTypeDef",
+    "HeatMapAggregatedFieldWellsOutputTypeDef",
     "HeatMapAggregatedFieldWellsTypeDef",
+    "HistogramAggregatedFieldWellsOutputTypeDef",
     "HistogramAggregatedFieldWellsTypeDef",
+    "KPIFieldWellsOutputTypeDef",
     "KPIFieldWellsTypeDef",
+    "LineChartAggregatedFieldWellsOutputTypeDef",
     "LineChartAggregatedFieldWellsTypeDef",
     "MaximumMinimumComputationTypeDef",
     "MetricComparisonComputationTypeDef",
     "PeriodOverPeriodComputationTypeDef",
     "PeriodToDateComputationTypeDef",
+    "PieChartAggregatedFieldWellsOutputTypeDef",
     "PieChartAggregatedFieldWellsTypeDef",
+    "PivotTableAggregatedFieldWellsOutputTypeDef",
     "PivotTableAggregatedFieldWellsTypeDef",
+    "RadarChartAggregatedFieldWellsOutputTypeDef",
     "RadarChartAggregatedFieldWellsTypeDef",
+    "SankeyDiagramAggregatedFieldWellsOutputTypeDef",
     "SankeyDiagramAggregatedFieldWellsTypeDef",
+    "ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef",
     "ScatterPlotCategoricallyAggregatedFieldWellsTypeDef",
+    "ScatterPlotUnaggregatedFieldWellsOutputTypeDef",
     "ScatterPlotUnaggregatedFieldWellsTypeDef",
+    "TableAggregatedFieldWellsOutputTypeDef",
     "TableAggregatedFieldWellsTypeDef",
     "TopBottomMoversComputationTypeDef",
     "TopBottomRankedComputationTypeDef",
     "TotalAggregationComputationTypeDef",
+    "TreeMapAggregatedFieldWellsOutputTypeDef",
     "TreeMapAggregatedFieldWellsTypeDef",
+    "WaterfallChartAggregatedFieldWellsOutputTypeDef",
     "WaterfallChartAggregatedFieldWellsTypeDef",
+    "WordCloudAggregatedFieldWellsOutputTypeDef",
     "WordCloudAggregatedFieldWellsTypeDef",
+    "TableUnaggregatedFieldWellsOutputTypeDef",
     "TableUnaggregatedFieldWellsTypeDef",
     "SectionBasedLayoutConfigurationOutputTypeDef",
     "SectionBasedLayoutConfigurationTypeDef",
     "BarChartFieldWellsOutputTypeDef",
-    "BoxPlotFieldWellsOutputTypeDef",
-    "ComboChartFieldWellsOutputTypeDef",
-    "FilledMapFieldWellsOutputTypeDef",
-    "FunnelChartFieldWellsOutputTypeDef",
-    "GaugeChartConfigurationOutputTypeDef",
-    "GeospatialMapFieldWellsOutputTypeDef",
-    "HeatMapFieldWellsOutputTypeDef",
-    "HistogramFieldWellsOutputTypeDef",
-    "KPIConfigurationOutputTypeDef",
-    "LineChartFieldWellsOutputTypeDef",
-    "PieChartFieldWellsOutputTypeDef",
-    "PivotTableFieldWellsOutputTypeDef",
-    "RadarChartFieldWellsOutputTypeDef",
-    "SankeyDiagramFieldWellsOutputTypeDef",
-    "ScatterPlotFieldWellsOutputTypeDef",
-    "ComputationOutputTypeDef",
-    "TreeMapFieldWellsOutputTypeDef",
-    "WaterfallChartFieldWellsOutputTypeDef",
-    "WordCloudFieldWellsOutputTypeDef",
-    "TableFieldWellsOutputTypeDef",
     "BarChartFieldWellsTypeDef",
+    "BoxPlotFieldWellsOutputTypeDef",
     "BoxPlotFieldWellsTypeDef",
+    "ComboChartFieldWellsOutputTypeDef",
     "ComboChartFieldWellsTypeDef",
+    "FilledMapFieldWellsOutputTypeDef",
     "FilledMapFieldWellsTypeDef",
+    "FunnelChartFieldWellsOutputTypeDef",
     "FunnelChartFieldWellsTypeDef",
+    "GaugeChartConfigurationOutputTypeDef",
     "GaugeChartConfigurationTypeDef",
+    "GeospatialMapFieldWellsOutputTypeDef",
     "GeospatialMapFieldWellsTypeDef",
+    "HeatMapFieldWellsOutputTypeDef",
     "HeatMapFieldWellsTypeDef",
+    "HistogramFieldWellsOutputTypeDef",
     "HistogramFieldWellsTypeDef",
+    "KPIConfigurationOutputTypeDef",
     "KPIConfigurationTypeDef",
+    "LineChartFieldWellsOutputTypeDef",
     "LineChartFieldWellsTypeDef",
+    "PieChartFieldWellsOutputTypeDef",
     "PieChartFieldWellsTypeDef",
+    "PivotTableFieldWellsOutputTypeDef",
     "PivotTableFieldWellsTypeDef",
+    "RadarChartFieldWellsOutputTypeDef",
     "RadarChartFieldWellsTypeDef",
+    "SankeyDiagramFieldWellsOutputTypeDef",
     "SankeyDiagramFieldWellsTypeDef",
+    "ScatterPlotFieldWellsOutputTypeDef",
     "ScatterPlotFieldWellsTypeDef",
     "ComputationTypeDef",
+    "TreeMapFieldWellsOutputTypeDef",
     "TreeMapFieldWellsTypeDef",
+    "WaterfallChartFieldWellsOutputTypeDef",
     "WaterfallChartFieldWellsTypeDef",
+    "WordCloudFieldWellsOutputTypeDef",
     "WordCloudFieldWellsTypeDef",
+    "TableFieldWellsOutputTypeDef",
     "TableFieldWellsTypeDef",
     "LayoutConfigurationOutputTypeDef",
     "LayoutConfigurationTypeDef",
     "BarChartConfigurationOutputTypeDef",
-    "BoxPlotChartConfigurationOutputTypeDef",
-    "ComboChartConfigurationOutputTypeDef",
-    "FilledMapConfigurationOutputTypeDef",
-    "FunnelChartConfigurationOutputTypeDef",
-    "GaugeChartVisualOutputTypeDef",
-    "GeospatialMapConfigurationOutputTypeDef",
-    "HeatMapConfigurationOutputTypeDef",
-    "HistogramConfigurationOutputTypeDef",
-    "KPIVisualOutputTypeDef",
-    "LineChartConfigurationOutputTypeDef",
-    "PieChartConfigurationOutputTypeDef",
-    "PivotTableConfigurationOutputTypeDef",
-    "RadarChartConfigurationOutputTypeDef",
-    "SankeyDiagramChartConfigurationOutputTypeDef",
-    "ScatterPlotConfigurationOutputTypeDef",
-    "InsightConfigurationOutputTypeDef",
-    "TreeMapConfigurationOutputTypeDef",
-    "WaterfallChartConfigurationOutputTypeDef",
-    "WordCloudChartConfigurationOutputTypeDef",
-    "TableConfigurationOutputTypeDef",
     "BarChartConfigurationTypeDef",
+    "BoxPlotChartConfigurationOutputTypeDef",
     "BoxPlotChartConfigurationTypeDef",
+    "ComboChartConfigurationOutputTypeDef",
     "ComboChartConfigurationTypeDef",
+    "FilledMapConfigurationOutputTypeDef",
     "FilledMapConfigurationTypeDef",
+    "FunnelChartConfigurationOutputTypeDef",
     "FunnelChartConfigurationTypeDef",
+    "GaugeChartVisualOutputTypeDef",
     "GaugeChartVisualTypeDef",
+    "GeospatialMapConfigurationOutputTypeDef",
     "GeospatialMapConfigurationTypeDef",
+    "HeatMapConfigurationOutputTypeDef",
     "HeatMapConfigurationTypeDef",
+    "HistogramConfigurationOutputTypeDef",
     "HistogramConfigurationTypeDef",
+    "KPIVisualOutputTypeDef",
     "KPIVisualTypeDef",
+    "LineChartConfigurationOutputTypeDef",
     "LineChartConfigurationTypeDef",
+    "PieChartConfigurationOutputTypeDef",
     "PieChartConfigurationTypeDef",
+    "PivotTableConfigurationOutputTypeDef",
     "PivotTableConfigurationTypeDef",
+    "RadarChartConfigurationOutputTypeDef",
     "RadarChartConfigurationTypeDef",
+    "SankeyDiagramChartConfigurationOutputTypeDef",
     "SankeyDiagramChartConfigurationTypeDef",
+    "ScatterPlotConfigurationOutputTypeDef",
     "ScatterPlotConfigurationTypeDef",
+    "InsightConfigurationOutputTypeDef",
     "InsightConfigurationTypeDef",
+    "TreeMapConfigurationOutputTypeDef",
     "TreeMapConfigurationTypeDef",
+    "WaterfallChartConfigurationOutputTypeDef",
     "WaterfallChartConfigurationTypeDef",
+    "WordCloudChartConfigurationOutputTypeDef",
     "WordCloudChartConfigurationTypeDef",
+    "TableConfigurationOutputTypeDef",
     "TableConfigurationTypeDef",
     "LayoutOutputTypeDef",
     "LayoutTypeDef",
     "BarChartVisualOutputTypeDef",
-    "BoxPlotVisualOutputTypeDef",
-    "ComboChartVisualOutputTypeDef",
-    "FilledMapVisualOutputTypeDef",
-    "FunnelChartVisualOutputTypeDef",
-    "GeospatialMapVisualOutputTypeDef",
-    "HeatMapVisualOutputTypeDef",
-    "HistogramVisualOutputTypeDef",
-    "LineChartVisualOutputTypeDef",
-    "PieChartVisualOutputTypeDef",
-    "PivotTableVisualOutputTypeDef",
-    "RadarChartVisualOutputTypeDef",
-    "SankeyDiagramVisualOutputTypeDef",
-    "ScatterPlotVisualOutputTypeDef",
-    "InsightVisualOutputTypeDef",
-    "TreeMapVisualOutputTypeDef",
-    "WaterfallVisualOutputTypeDef",
-    "WordCloudVisualOutputTypeDef",
-    "TableVisualOutputTypeDef",
     "BarChartVisualTypeDef",
+    "BoxPlotVisualOutputTypeDef",
     "BoxPlotVisualTypeDef",
+    "ComboChartVisualOutputTypeDef",
     "ComboChartVisualTypeDef",
+    "FilledMapVisualOutputTypeDef",
     "FilledMapVisualTypeDef",
+    "FunnelChartVisualOutputTypeDef",
     "FunnelChartVisualTypeDef",
+    "GeospatialMapVisualOutputTypeDef",
     "GeospatialMapVisualTypeDef",
+    "HeatMapVisualOutputTypeDef",
     "HeatMapVisualTypeDef",
+    "HistogramVisualOutputTypeDef",
     "HistogramVisualTypeDef",
+    "LineChartVisualOutputTypeDef",
     "LineChartVisualTypeDef",
+    "PieChartVisualOutputTypeDef",
     "PieChartVisualTypeDef",
+    "PivotTableVisualOutputTypeDef",
     "PivotTableVisualTypeDef",
+    "RadarChartVisualOutputTypeDef",
     "RadarChartVisualTypeDef",
+    "SankeyDiagramVisualOutputTypeDef",
     "SankeyDiagramVisualTypeDef",
+    "ScatterPlotVisualOutputTypeDef",
     "ScatterPlotVisualTypeDef",
+    "InsightVisualOutputTypeDef",
     "InsightVisualTypeDef",
+    "TreeMapVisualOutputTypeDef",
     "TreeMapVisualTypeDef",
+    "WaterfallVisualOutputTypeDef",
     "WaterfallVisualTypeDef",
+    "WordCloudVisualOutputTypeDef",
     "WordCloudVisualTypeDef",
+    "TableVisualOutputTypeDef",
     "TableVisualTypeDef",
     "VisualOutputTypeDef",
     "VisualTypeDef",
     "SheetDefinitionOutputTypeDef",
     "SheetDefinitionTypeDef",
     "AnalysisDefinitionOutputTypeDef",
     "DashboardVersionDefinitionOutputTypeDef",
@@ -1876,23 +1559,14 @@
     "UpdateAnalysisRequestRequestTypeDef",
     "CreateDashboardRequestRequestTypeDef",
     "UpdateDashboardRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
 )
 
-AccountCustomizationOutputTypeDef = TypedDict(
-    "AccountCustomizationOutputTypeDef",
-    {
-        "DefaultTheme": str,
-        "DefaultEmailCustomizationTemplate": str,
-    },
-    total=False,
-)
-
 AccountCustomizationTypeDef = TypedDict(
     "AccountCustomizationTypeDef",
     {
         "DefaultTheme": str,
         "DefaultEmailCustomizationTemplate": str,
     },
     total=False,
@@ -1928,109 +1602,53 @@
     {
         "AssignmentName": str,
         "PolicyArn": str,
     },
     total=False,
 )
 
-AdHocFilteringOptionOutputTypeDef = TypedDict(
-    "AdHocFilteringOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
 AdHocFilteringOptionTypeDef = TypedDict(
     "AdHocFilteringOptionTypeDef",
     {
         "AvailabilityStatus": DashboardBehaviorType,
     },
     total=False,
 )
 
-AttributeAggregationFunctionOutputTypeDef = TypedDict(
-    "AttributeAggregationFunctionOutputTypeDef",
-    {
-        "SimpleAttributeAggregation": Literal["UNIQUE_VALUE"],
-        "ValueForMultipleValues": str,
-    },
-    total=False,
-)
-
 AttributeAggregationFunctionTypeDef = TypedDict(
     "AttributeAggregationFunctionTypeDef",
     {
         "SimpleAttributeAggregation": Literal["UNIQUE_VALUE"],
         "ValueForMultipleValues": str,
     },
     total=False,
 )
 
-ColumnIdentifierOutputTypeDef = TypedDict(
-    "ColumnIdentifierOutputTypeDef",
-    {
-        "DataSetIdentifier": str,
-        "ColumnName": str,
-    },
-)
-
 ColumnIdentifierTypeDef = TypedDict(
     "ColumnIdentifierTypeDef",
     {
         "DataSetIdentifier": str,
         "ColumnName": str,
     },
 )
 
-AmazonElasticsearchParametersOutputTypeDef = TypedDict(
-    "AmazonElasticsearchParametersOutputTypeDef",
-    {
-        "Domain": str,
-    },
-)
-
 AmazonElasticsearchParametersTypeDef = TypedDict(
     "AmazonElasticsearchParametersTypeDef",
     {
         "Domain": str,
     },
 )
 
-AmazonOpenSearchParametersOutputTypeDef = TypedDict(
-    "AmazonOpenSearchParametersOutputTypeDef",
-    {
-        "Domain": str,
-    },
-)
-
 AmazonOpenSearchParametersTypeDef = TypedDict(
     "AmazonOpenSearchParametersTypeDef",
     {
         "Domain": str,
     },
 )
 
-CalculatedFieldOutputTypeDef = TypedDict(
-    "CalculatedFieldOutputTypeDef",
-    {
-        "DataSetIdentifier": str,
-        "Name": str,
-        "Expression": str,
-    },
-)
-
-DataSetIdentifierDeclarationOutputTypeDef = TypedDict(
-    "DataSetIdentifierDeclarationOutputTypeDef",
-    {
-        "Identifier": str,
-        "DataSetArn": str,
-    },
-)
-
 CalculatedFieldTypeDef = TypedDict(
     "CalculatedFieldTypeDef",
     {
         "DataSetIdentifier": str,
         "Name": str,
         "Expression": str,
     },
@@ -2088,23 +1706,14 @@
     {
         "SheetId": str,
         "Name": str,
     },
     total=False,
 )
 
-AnchorDateConfigurationOutputTypeDef = TypedDict(
-    "AnchorDateConfigurationOutputTypeDef",
-    {
-        "AnchorOption": Literal["NOW"],
-        "ParameterName": str,
-    },
-    total=False,
-)
-
 AnchorDateConfigurationTypeDef = TypedDict(
     "AnchorDateConfigurationTypeDef",
     {
         "AnchorOption": Literal["NOW"],
         "ParameterName": str,
     },
     total=False,
@@ -2129,58 +1738,32 @@
 AnonymousUserQSearchBarEmbeddingConfigurationTypeDef = TypedDict(
     "AnonymousUserQSearchBarEmbeddingConfigurationTypeDef",
     {
         "InitialTopicId": str,
     },
 )
 
-ArcAxisDisplayRangeOutputTypeDef = TypedDict(
-    "ArcAxisDisplayRangeOutputTypeDef",
-    {
-        "Min": float,
-        "Max": float,
-    },
-    total=False,
-)
-
 ArcAxisDisplayRangeTypeDef = TypedDict(
     "ArcAxisDisplayRangeTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-ArcConfigurationOutputTypeDef = TypedDict(
-    "ArcConfigurationOutputTypeDef",
-    {
-        "ArcAngle": float,
-        "ArcThickness": ArcThicknessOptionsType,
-    },
-    total=False,
-)
-
 ArcConfigurationTypeDef = TypedDict(
     "ArcConfigurationTypeDef",
     {
         "ArcAngle": float,
         "ArcThickness": ArcThicknessOptionsType,
     },
     total=False,
 )
 
-ArcOptionsOutputTypeDef = TypedDict(
-    "ArcOptionsOutputTypeDef",
-    {
-        "ArcThickness": ArcThicknessType,
-    },
-    total=False,
-)
-
 ArcOptionsTypeDef = TypedDict(
     "ArcOptionsTypeDef",
     {
         "ArcThickness": ArcThicknessType,
     },
     total=False,
 )
@@ -2291,16 +1874,16 @@
 class AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef(
     _RequiredAssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef,
     _OptionalAssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef,
 ):
     pass
 
 
-AssetBundleExportJobResourceIdOverrideConfigurationOutputTypeDef = TypedDict(
-    "AssetBundleExportJobResourceIdOverrideConfigurationOutputTypeDef",
+AssetBundleExportJobResourceIdOverrideConfigurationTypeDef = TypedDict(
+    "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
     {
         "PrefixForAllResources": bool,
     },
     total=False,
 )
 
 _RequiredAssetBundleExportJobThemeOverridePropertiesOutputTypeDef = TypedDict(
@@ -2453,22 +2036,14 @@
 class AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef(
     _RequiredAssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef,
     _OptionalAssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef,
 ):
     pass
 
 
-AssetBundleExportJobResourceIdOverrideConfigurationTypeDef = TypedDict(
-    "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
-    {
-        "PrefixForAllResources": bool,
-    },
-    total=False,
-)
-
 _RequiredAssetBundleExportJobThemeOverridePropertiesTypeDef = TypedDict(
     "_RequiredAssetBundleExportJobThemeOverridePropertiesTypeDef",
     {
         "Properties": Sequence[Literal["Name"]],
     },
 )
 _OptionalAssetBundleExportJobThemeOverridePropertiesTypeDef = TypedDict(
@@ -2528,36 +2103,14 @@
         "AssetBundleExportJobId": str,
         "IncludeAllDependencies": bool,
         "ExportFormat": AssetBundleExportFormatType,
     },
     total=False,
 )
 
-_RequiredAssetBundleImportJobAnalysisOverrideParametersOutputTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobAnalysisOverrideParametersOutputTypeDef",
-    {
-        "AnalysisId": str,
-    },
-)
-_OptionalAssetBundleImportJobAnalysisOverrideParametersOutputTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobAnalysisOverrideParametersOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-
-class AssetBundleImportJobAnalysisOverrideParametersOutputTypeDef(
-    _RequiredAssetBundleImportJobAnalysisOverrideParametersOutputTypeDef,
-    _OptionalAssetBundleImportJobAnalysisOverrideParametersOutputTypeDef,
-):
-    pass
-
-
 _RequiredAssetBundleImportJobAnalysisOverrideParametersTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobAnalysisOverrideParametersTypeDef",
     {
         "AnalysisId": str,
     },
 )
 _OptionalAssetBundleImportJobAnalysisOverrideParametersTypeDef = TypedDict(
@@ -2572,36 +2125,14 @@
 class AssetBundleImportJobAnalysisOverrideParametersTypeDef(
     _RequiredAssetBundleImportJobAnalysisOverrideParametersTypeDef,
     _OptionalAssetBundleImportJobAnalysisOverrideParametersTypeDef,
 ):
     pass
 
 
-_RequiredAssetBundleImportJobDashboardOverrideParametersOutputTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobDashboardOverrideParametersOutputTypeDef",
-    {
-        "DashboardId": str,
-    },
-)
-_OptionalAssetBundleImportJobDashboardOverrideParametersOutputTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobDashboardOverrideParametersOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-
-class AssetBundleImportJobDashboardOverrideParametersOutputTypeDef(
-    _RequiredAssetBundleImportJobDashboardOverrideParametersOutputTypeDef,
-    _OptionalAssetBundleImportJobDashboardOverrideParametersOutputTypeDef,
-):
-    pass
-
-
 _RequiredAssetBundleImportJobDashboardOverrideParametersTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobDashboardOverrideParametersTypeDef",
     {
         "DashboardId": str,
     },
 )
 _OptionalAssetBundleImportJobDashboardOverrideParametersTypeDef = TypedDict(
@@ -2616,36 +2147,14 @@
 class AssetBundleImportJobDashboardOverrideParametersTypeDef(
     _RequiredAssetBundleImportJobDashboardOverrideParametersTypeDef,
     _OptionalAssetBundleImportJobDashboardOverrideParametersTypeDef,
 ):
     pass
 
 
-_RequiredAssetBundleImportJobDataSetOverrideParametersOutputTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobDataSetOverrideParametersOutputTypeDef",
-    {
-        "DataSetId": str,
-    },
-)
-_OptionalAssetBundleImportJobDataSetOverrideParametersOutputTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobDataSetOverrideParametersOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-
-class AssetBundleImportJobDataSetOverrideParametersOutputTypeDef(
-    _RequiredAssetBundleImportJobDataSetOverrideParametersOutputTypeDef,
-    _OptionalAssetBundleImportJobDataSetOverrideParametersOutputTypeDef,
-):
-    pass
-
-
 _RequiredAssetBundleImportJobDataSetOverrideParametersTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobDataSetOverrideParametersTypeDef",
     {
         "DataSetId": str,
     },
 )
 _OptionalAssetBundleImportJobDataSetOverrideParametersTypeDef = TypedDict(
@@ -2660,45 +2169,22 @@
 class AssetBundleImportJobDataSetOverrideParametersTypeDef(
     _RequiredAssetBundleImportJobDataSetOverrideParametersTypeDef,
     _OptionalAssetBundleImportJobDataSetOverrideParametersTypeDef,
 ):
     pass
 
 
-AssetBundleImportJobDataSourceCredentialPairOutputTypeDef = TypedDict(
-    "AssetBundleImportJobDataSourceCredentialPairOutputTypeDef",
-    {
-        "Username": str,
-        "Password": str,
-    },
-)
-
 AssetBundleImportJobDataSourceCredentialPairTypeDef = TypedDict(
     "AssetBundleImportJobDataSourceCredentialPairTypeDef",
     {
         "Username": str,
         "Password": str,
     },
 )
 
-SslPropertiesOutputTypeDef = TypedDict(
-    "SslPropertiesOutputTypeDef",
-    {
-        "DisableSsl": bool,
-    },
-    total=False,
-)
-
-VpcConnectionPropertiesOutputTypeDef = TypedDict(
-    "VpcConnectionPropertiesOutputTypeDef",
-    {
-        "VpcConnectionArn": str,
-    },
-)
-
 SslPropertiesTypeDef = TypedDict(
     "SslPropertiesTypeDef",
     {
         "DisableSsl": bool,
     },
     total=False,
 )
@@ -2739,40 +2225,40 @@
 class AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef(
     _RequiredAssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef,
     _OptionalAssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef,
 ):
     pass
 
 
-AssetBundleImportJobResourceIdOverrideConfigurationOutputTypeDef = TypedDict(
-    "AssetBundleImportJobResourceIdOverrideConfigurationOutputTypeDef",
+AssetBundleImportJobResourceIdOverrideConfigurationTypeDef = TypedDict(
+    "AssetBundleImportJobResourceIdOverrideConfigurationTypeDef",
     {
         "PrefixForAllResources": str,
     },
     total=False,
 )
 
-_RequiredAssetBundleImportJobThemeOverrideParametersOutputTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobThemeOverrideParametersOutputTypeDef",
+_RequiredAssetBundleImportJobThemeOverrideParametersTypeDef = TypedDict(
+    "_RequiredAssetBundleImportJobThemeOverrideParametersTypeDef",
     {
         "ThemeId": str,
     },
 )
-_OptionalAssetBundleImportJobThemeOverrideParametersOutputTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobThemeOverrideParametersOutputTypeDef",
+_OptionalAssetBundleImportJobThemeOverrideParametersTypeDef = TypedDict(
+    "_OptionalAssetBundleImportJobThemeOverrideParametersTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
 
-class AssetBundleImportJobThemeOverrideParametersOutputTypeDef(
-    _RequiredAssetBundleImportJobThemeOverrideParametersOutputTypeDef,
-    _OptionalAssetBundleImportJobThemeOverrideParametersOutputTypeDef,
+class AssetBundleImportJobThemeOverrideParametersTypeDef(
+    _RequiredAssetBundleImportJobThemeOverrideParametersTypeDef,
+    _OptionalAssetBundleImportJobThemeOverrideParametersTypeDef,
 ):
     pass
 
 
 _RequiredAssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef",
     {
@@ -2818,44 +2304,14 @@
 class AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef(
     _RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
     _OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
 ):
     pass
 
 
-AssetBundleImportJobResourceIdOverrideConfigurationTypeDef = TypedDict(
-    "AssetBundleImportJobResourceIdOverrideConfigurationTypeDef",
-    {
-        "PrefixForAllResources": str,
-    },
-    total=False,
-)
-
-_RequiredAssetBundleImportJobThemeOverrideParametersTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobThemeOverrideParametersTypeDef",
-    {
-        "ThemeId": str,
-    },
-)
-_OptionalAssetBundleImportJobThemeOverrideParametersTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobThemeOverrideParametersTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-
-class AssetBundleImportJobThemeOverrideParametersTypeDef(
-    _RequiredAssetBundleImportJobThemeOverrideParametersTypeDef,
-    _OptionalAssetBundleImportJobThemeOverrideParametersTypeDef,
-):
-    pass
-
-
 _RequiredAssetBundleImportJobVPCConnectionOverrideParametersTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
     {
         "VPCConnectionId": str,
     },
 )
 _OptionalAssetBundleImportJobVPCConnectionOverrideParametersTypeDef = TypedDict(
@@ -2904,193 +2360,99 @@
     {
         "Body": Union[str, bytes, IO[Any], StreamingBody],
         "S3Uri": str,
     },
     total=False,
 )
 
-AthenaParametersOutputTypeDef = TypedDict(
-    "AthenaParametersOutputTypeDef",
-    {
-        "WorkGroup": str,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
 AthenaParametersTypeDef = TypedDict(
     "AthenaParametersTypeDef",
     {
         "WorkGroup": str,
         "RoleArn": str,
     },
     total=False,
 )
 
-AuroraParametersOutputTypeDef = TypedDict(
-    "AuroraParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
 AuroraParametersTypeDef = TypedDict(
     "AuroraParametersTypeDef",
     {
         "Host": str,
         "Port": int,
         "Database": str,
     },
 )
 
-AuroraPostgreSqlParametersOutputTypeDef = TypedDict(
-    "AuroraPostgreSqlParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
 AuroraPostgreSqlParametersTypeDef = TypedDict(
     "AuroraPostgreSqlParametersTypeDef",
     {
         "Host": str,
         "Port": int,
         "Database": str,
     },
 )
 
-AwsIotAnalyticsParametersOutputTypeDef = TypedDict(
-    "AwsIotAnalyticsParametersOutputTypeDef",
-    {
-        "DataSetName": str,
-    },
-)
-
 AwsIotAnalyticsParametersTypeDef = TypedDict(
     "AwsIotAnalyticsParametersTypeDef",
     {
         "DataSetName": str,
     },
 )
 
-DateAxisOptionsOutputTypeDef = TypedDict(
-    "DateAxisOptionsOutputTypeDef",
-    {
-        "MissingDateVisibility": VisibilityType,
-    },
-    total=False,
-)
-
 DateAxisOptionsTypeDef = TypedDict(
     "DateAxisOptionsTypeDef",
     {
         "MissingDateVisibility": VisibilityType,
     },
     total=False,
 )
 
-AxisDisplayMinMaxRangeOutputTypeDef = TypedDict(
-    "AxisDisplayMinMaxRangeOutputTypeDef",
-    {
-        "Minimum": float,
-        "Maximum": float,
-    },
-    total=False,
-)
-
 AxisDisplayMinMaxRangeTypeDef = TypedDict(
     "AxisDisplayMinMaxRangeTypeDef",
     {
         "Minimum": float,
         "Maximum": float,
     },
     total=False,
 )
 
-AxisLinearScaleOutputTypeDef = TypedDict(
-    "AxisLinearScaleOutputTypeDef",
-    {
-        "StepCount": int,
-        "StepSize": float,
-    },
-    total=False,
-)
-
 AxisLinearScaleTypeDef = TypedDict(
     "AxisLinearScaleTypeDef",
     {
         "StepCount": int,
         "StepSize": float,
     },
     total=False,
 )
 
-AxisLogarithmicScaleOutputTypeDef = TypedDict(
-    "AxisLogarithmicScaleOutputTypeDef",
-    {
-        "Base": float,
-    },
-    total=False,
-)
-
 AxisLogarithmicScaleTypeDef = TypedDict(
     "AxisLogarithmicScaleTypeDef",
     {
         "Base": float,
     },
     total=False,
 )
 
-ItemsLimitConfigurationOutputTypeDef = TypedDict(
-    "ItemsLimitConfigurationOutputTypeDef",
-    {
-        "ItemsLimit": int,
-        "OtherCategories": OtherCategoriesType,
-    },
-    total=False,
-)
-
 ItemsLimitConfigurationTypeDef = TypedDict(
     "ItemsLimitConfigurationTypeDef",
     {
         "ItemsLimit": int,
         "OtherCategories": OtherCategoriesType,
     },
     total=False,
 )
 
-BinCountOptionsOutputTypeDef = TypedDict(
-    "BinCountOptionsOutputTypeDef",
-    {
-        "Value": int,
-    },
-    total=False,
-)
-
 BinCountOptionsTypeDef = TypedDict(
     "BinCountOptionsTypeDef",
     {
         "Value": int,
     },
     total=False,
 )
 
-BinWidthOptionsOutputTypeDef = TypedDict(
-    "BinWidthOptionsOutputTypeDef",
-    {
-        "Value": float,
-        "BinCountLimit": int,
-    },
-    total=False,
-)
-
 BinWidthOptionsTypeDef = TypedDict(
     "BinWidthOptionsTypeDef",
     {
         "Value": float,
         "BinCountLimit": int,
     },
     total=False,
@@ -3099,88 +2461,47 @@
 BookmarksConfigurationsTypeDef = TypedDict(
     "BookmarksConfigurationsTypeDef",
     {
         "Enabled": bool,
     },
 )
 
-BorderStyleOutputTypeDef = TypedDict(
-    "BorderStyleOutputTypeDef",
-    {
-        "Show": bool,
-    },
-    total=False,
-)
-
 BorderStyleTypeDef = TypedDict(
     "BorderStyleTypeDef",
     {
         "Show": bool,
     },
     total=False,
 )
 
-BoxPlotStyleOptionsOutputTypeDef = TypedDict(
-    "BoxPlotStyleOptionsOutputTypeDef",
-    {
-        "FillStyle": BoxPlotFillStyleType,
-    },
-    total=False,
-)
-
 BoxPlotStyleOptionsTypeDef = TypedDict(
     "BoxPlotStyleOptionsTypeDef",
     {
         "FillStyle": BoxPlotFillStyleType,
     },
     total=False,
 )
 
-PaginationConfigurationOutputTypeDef = TypedDict(
-    "PaginationConfigurationOutputTypeDef",
-    {
-        "PageSize": int,
-        "PageNumber": int,
-    },
-)
-
 PaginationConfigurationTypeDef = TypedDict(
     "PaginationConfigurationTypeDef",
     {
         "PageSize": int,
         "PageNumber": int,
     },
 )
 
-CalculatedColumnOutputTypeDef = TypedDict(
-    "CalculatedColumnOutputTypeDef",
-    {
-        "ColumnName": str,
-        "ColumnId": str,
-        "Expression": str,
-    },
-)
-
 CalculatedColumnTypeDef = TypedDict(
     "CalculatedColumnTypeDef",
     {
         "ColumnName": str,
         "ColumnId": str,
         "Expression": str,
     },
 )
 
-CalculatedMeasureFieldOutputTypeDef = TypedDict(
-    "CalculatedMeasureFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Expression": str,
-    },
-)
-
 CalculatedMeasureFieldTypeDef = TypedDict(
     "CalculatedMeasureFieldTypeDef",
     {
         "FieldId": str,
         "Expression": str,
     },
 )
@@ -3201,36 +2522,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredCastColumnTypeOperationOutputTypeDef = TypedDict(
-    "_RequiredCastColumnTypeOperationOutputTypeDef",
-    {
-        "ColumnName": str,
-        "NewColumnType": ColumnDataTypeType,
-    },
-)
-_OptionalCastColumnTypeOperationOutputTypeDef = TypedDict(
-    "_OptionalCastColumnTypeOperationOutputTypeDef",
-    {
-        "Format": str,
-    },
-    total=False,
-)
-
-
-class CastColumnTypeOperationOutputTypeDef(
-    _RequiredCastColumnTypeOperationOutputTypeDef, _OptionalCastColumnTypeOperationOutputTypeDef
-):
-    pass
-
-
 _RequiredCastColumnTypeOperationTypeDef = TypedDict(
     "_RequiredCastColumnTypeOperationTypeDef",
     {
         "ColumnName": str,
         "NewColumnType": ColumnDataTypeType,
     },
 )
@@ -3245,34 +2544,34 @@
 
 class CastColumnTypeOperationTypeDef(
     _RequiredCastColumnTypeOperationTypeDef, _OptionalCastColumnTypeOperationTypeDef
 ):
     pass
 
 
-_RequiredCustomFilterConfigurationOutputTypeDef = TypedDict(
-    "_RequiredCustomFilterConfigurationOutputTypeDef",
+_RequiredCustomFilterConfigurationTypeDef = TypedDict(
+    "_RequiredCustomFilterConfigurationTypeDef",
     {
         "MatchOperator": CategoryFilterMatchOperatorType,
         "NullOption": FilterNullOptionType,
     },
 )
-_OptionalCustomFilterConfigurationOutputTypeDef = TypedDict(
-    "_OptionalCustomFilterConfigurationOutputTypeDef",
+_OptionalCustomFilterConfigurationTypeDef = TypedDict(
+    "_OptionalCustomFilterConfigurationTypeDef",
     {
         "CategoryValue": str,
         "SelectAllOptions": Literal["FILTER_ALL_VALUES"],
         "ParameterName": str,
     },
     total=False,
 )
 
 
-class CustomFilterConfigurationOutputTypeDef(
-    _RequiredCustomFilterConfigurationOutputTypeDef, _OptionalCustomFilterConfigurationOutputTypeDef
+class CustomFilterConfigurationTypeDef(
+    _RequiredCustomFilterConfigurationTypeDef, _OptionalCustomFilterConfigurationTypeDef
 ):
     pass
 
 
 _RequiredCustomFilterListConfigurationOutputTypeDef = TypedDict(
     "_RequiredCustomFilterListConfigurationOutputTypeDef",
     {
@@ -3315,38 +2614,14 @@
 
 class FilterListConfigurationOutputTypeDef(
     _RequiredFilterListConfigurationOutputTypeDef, _OptionalFilterListConfigurationOutputTypeDef
 ):
     pass
 
 
-_RequiredCustomFilterConfigurationTypeDef = TypedDict(
-    "_RequiredCustomFilterConfigurationTypeDef",
-    {
-        "MatchOperator": CategoryFilterMatchOperatorType,
-        "NullOption": FilterNullOptionType,
-    },
-)
-_OptionalCustomFilterConfigurationTypeDef = TypedDict(
-    "_OptionalCustomFilterConfigurationTypeDef",
-    {
-        "CategoryValue": str,
-        "SelectAllOptions": Literal["FILTER_ALL_VALUES"],
-        "ParameterName": str,
-    },
-    total=False,
-)
-
-
-class CustomFilterConfigurationTypeDef(
-    _RequiredCustomFilterConfigurationTypeDef, _OptionalCustomFilterConfigurationTypeDef
-):
-    pass
-
-
 _RequiredCustomFilterListConfigurationTypeDef = TypedDict(
     "_RequiredCustomFilterListConfigurationTypeDef",
     {
         "MatchOperator": CategoryFilterMatchOperatorType,
         "NullOption": FilterNullOptionType,
     },
 )
@@ -3402,22 +2677,14 @@
     {
         "CellValue": str,
         "Synonyms": Sequence[str],
     },
     total=False,
 )
 
-SimpleClusterMarkerOutputTypeDef = TypedDict(
-    "SimpleClusterMarkerOutputTypeDef",
-    {
-        "Color": str,
-    },
-    total=False,
-)
-
 SimpleClusterMarkerTypeDef = TypedDict(
     "SimpleClusterMarkerTypeDef",
     {
         "Color": str,
     },
     total=False,
 )
@@ -3434,54 +2701,23 @@
     "CollectiveConstantTypeDef",
     {
         "ValueList": Sequence[str],
     },
     total=False,
 )
 
-DataColorOutputTypeDef = TypedDict(
-    "DataColorOutputTypeDef",
-    {
-        "Color": str,
-        "DataValue": float,
-    },
-    total=False,
-)
-
 DataColorTypeDef = TypedDict(
     "DataColorTypeDef",
     {
         "Color": str,
         "DataValue": float,
     },
     total=False,
 )
 
-_RequiredCustomColorOutputTypeDef = TypedDict(
-    "_RequiredCustomColorOutputTypeDef",
-    {
-        "Color": str,
-    },
-)
-_OptionalCustomColorOutputTypeDef = TypedDict(
-    "_OptionalCustomColorOutputTypeDef",
-    {
-        "FieldValue": str,
-        "SpecialValue": SpecialValueType,
-    },
-    total=False,
-)
-
-
-class CustomColorOutputTypeDef(
-    _RequiredCustomColorOutputTypeDef, _OptionalCustomColorOutputTypeDef
-):
-    pass
-
-
 _RequiredCustomColorTypeDef = TypedDict(
     "_RequiredCustomColorTypeDef",
     {
         "Color": str,
     },
 )
 _OptionalCustomColorTypeDef = TypedDict(
@@ -3494,38 +2730,22 @@
 )
 
 
 class CustomColorTypeDef(_RequiredCustomColorTypeDef, _OptionalCustomColorTypeDef):
     pass
 
 
-ColumnDescriptionOutputTypeDef = TypedDict(
-    "ColumnDescriptionOutputTypeDef",
-    {
-        "Text": str,
-    },
-    total=False,
-)
-
 ColumnDescriptionTypeDef = TypedDict(
     "ColumnDescriptionTypeDef",
     {
         "Text": str,
     },
     total=False,
 )
 
-ColumnGroupColumnSchemaOutputTypeDef = TypedDict(
-    "ColumnGroupColumnSchemaOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
 ColumnGroupColumnSchemaTypeDef = TypedDict(
     "ColumnGroupColumnSchemaTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -3588,24 +2808,14 @@
     {
         "Principals": Sequence[str],
         "ColumnNames": Sequence[str],
     },
     total=False,
 )
 
-ColumnSchemaOutputTypeDef = TypedDict(
-    "ColumnSchemaOutputTypeDef",
-    {
-        "Name": str,
-        "DataType": str,
-        "GeographicRole": str,
-    },
-    total=False,
-)
-
 ColumnSchemaTypeDef = TypedDict(
     "ColumnSchemaTypeDef",
     {
         "Name": str,
         "DataType": str,
         "GeographicRole": str,
     },
@@ -3628,36 +2838,14 @@
         "UseOrdering": ColumnOrderingTypeType,
         "SpecifedOrder": Sequence[str],
         "TreatUndefinedSpecifiedValues": UndefinedSpecifiedValueTypeType,
     },
     total=False,
 )
 
-_RequiredConditionalFormattingSolidColorOutputTypeDef = TypedDict(
-    "_RequiredConditionalFormattingSolidColorOutputTypeDef",
-    {
-        "Expression": str,
-    },
-)
-_OptionalConditionalFormattingSolidColorOutputTypeDef = TypedDict(
-    "_OptionalConditionalFormattingSolidColorOutputTypeDef",
-    {
-        "Color": str,
-    },
-    total=False,
-)
-
-
-class ConditionalFormattingSolidColorOutputTypeDef(
-    _RequiredConditionalFormattingSolidColorOutputTypeDef,
-    _OptionalConditionalFormattingSolidColorOutputTypeDef,
-):
-    pass
-
-
 _RequiredConditionalFormattingSolidColorTypeDef = TypedDict(
     "_RequiredConditionalFormattingSolidColorTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalConditionalFormattingSolidColorTypeDef = TypedDict(
@@ -3671,31 +2859,14 @@
 
 class ConditionalFormattingSolidColorTypeDef(
     _RequiredConditionalFormattingSolidColorTypeDef, _OptionalConditionalFormattingSolidColorTypeDef
 ):
     pass
 
 
-ConditionalFormattingCustomIconOptionsOutputTypeDef = TypedDict(
-    "ConditionalFormattingCustomIconOptionsOutputTypeDef",
-    {
-        "Icon": IconType,
-        "UnicodeIcon": str,
-    },
-    total=False,
-)
-
-ConditionalFormattingIconDisplayConfigurationOutputTypeDef = TypedDict(
-    "ConditionalFormattingIconDisplayConfigurationOutputTypeDef",
-    {
-        "IconDisplayOption": Literal["ICON_ONLY"],
-    },
-    total=False,
-)
-
 ConditionalFormattingCustomIconOptionsTypeDef = TypedDict(
     "ConditionalFormattingCustomIconOptionsTypeDef",
     {
         "Icon": IconType,
         "UnicodeIcon": str,
     },
     total=False,
@@ -3705,36 +2876,14 @@
     "ConditionalFormattingIconDisplayConfigurationTypeDef",
     {
         "IconDisplayOption": Literal["ICON_ONLY"],
     },
     total=False,
 )
 
-_RequiredConditionalFormattingIconSetOutputTypeDef = TypedDict(
-    "_RequiredConditionalFormattingIconSetOutputTypeDef",
-    {
-        "Expression": str,
-    },
-)
-_OptionalConditionalFormattingIconSetOutputTypeDef = TypedDict(
-    "_OptionalConditionalFormattingIconSetOutputTypeDef",
-    {
-        "IconSetType": ConditionalFormattingIconSetTypeType,
-    },
-    total=False,
-)
-
-
-class ConditionalFormattingIconSetOutputTypeDef(
-    _RequiredConditionalFormattingIconSetOutputTypeDef,
-    _OptionalConditionalFormattingIconSetOutputTypeDef,
-):
-    pass
-
-
 _RequiredConditionalFormattingIconSetTypeDef = TypedDict(
     "_RequiredConditionalFormattingIconSetTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalConditionalFormattingIconSetTypeDef = TypedDict(
@@ -4038,35 +3187,14 @@
 
 class TopicRefreshScheduleTypeDef(
     _RequiredTopicRefreshScheduleTypeDef, _OptionalTopicRefreshScheduleTypeDef
 ):
     pass
 
 
-DecimalPlacesConfigurationOutputTypeDef = TypedDict(
-    "DecimalPlacesConfigurationOutputTypeDef",
-    {
-        "DecimalPlaces": int,
-    },
-)
-
-NegativeValueConfigurationOutputTypeDef = TypedDict(
-    "NegativeValueConfigurationOutputTypeDef",
-    {
-        "DisplayMode": NegativeValueDisplayModeType,
-    },
-)
-
-NullValueFormatConfigurationOutputTypeDef = TypedDict(
-    "NullValueFormatConfigurationOutputTypeDef",
-    {
-        "NullString": str,
-    },
-)
-
 DecimalPlacesConfigurationTypeDef = TypedDict(
     "DecimalPlacesConfigurationTypeDef",
     {
         "DecimalPlaces": int,
     },
 )
 
@@ -4080,71 +3208,39 @@
 NullValueFormatConfigurationTypeDef = TypedDict(
     "NullValueFormatConfigurationTypeDef",
     {
         "NullString": str,
     },
 )
 
-LocalNavigationConfigurationOutputTypeDef = TypedDict(
-    "LocalNavigationConfigurationOutputTypeDef",
-    {
-        "TargetSheetId": str,
-    },
-)
-
 LocalNavigationConfigurationTypeDef = TypedDict(
     "LocalNavigationConfigurationTypeDef",
     {
         "TargetSheetId": str,
     },
 )
 
-CustomActionURLOperationOutputTypeDef = TypedDict(
-    "CustomActionURLOperationOutputTypeDef",
-    {
-        "URLTemplate": str,
-        "URLTarget": URLTargetConfigurationType,
-    },
-)
-
 CustomActionURLOperationTypeDef = TypedDict(
     "CustomActionURLOperationTypeDef",
     {
         "URLTemplate": str,
         "URLTarget": URLTargetConfigurationType,
     },
 )
 
-CustomContentConfigurationOutputTypeDef = TypedDict(
-    "CustomContentConfigurationOutputTypeDef",
-    {
-        "ContentUrl": str,
-        "ContentType": CustomContentTypeType,
-        "ImageScaling": CustomContentImageScalingConfigurationType,
-    },
-    total=False,
-)
-
 CustomContentConfigurationTypeDef = TypedDict(
     "CustomContentConfigurationTypeDef",
     {
         "ContentUrl": str,
         "ContentType": CustomContentTypeType,
         "ImageScaling": CustomContentImageScalingConfigurationType,
     },
     total=False,
 )
 
-CustomNarrativeOptionsOutputTypeDef = TypedDict(
-    "CustomNarrativeOptionsOutputTypeDef",
-    {
-        "Narrative": str,
-    },
-)
-
 CustomNarrativeOptionsTypeDef = TypedDict(
     "CustomNarrativeOptionsTypeDef",
     {
         "Narrative": str,
     },
 )
 
@@ -4166,102 +3262,22 @@
         "IntegerValues": Sequence[int],
         "DecimalValues": Sequence[float],
         "DateTimeValues": Sequence[Union[datetime, str]],
     },
     total=False,
 )
 
-InputColumnOutputTypeDef = TypedDict(
-    "InputColumnOutputTypeDef",
-    {
-        "Name": str,
-        "Type": InputColumnDataTypeType,
-    },
-)
-
 InputColumnTypeDef = TypedDict(
     "InputColumnTypeDef",
     {
         "Name": str,
         "Type": InputColumnDataTypeType,
     },
 )
 
-DataPointDrillUpDownOptionOutputTypeDef = TypedDict(
-    "DataPointDrillUpDownOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-DataPointMenuLabelOptionOutputTypeDef = TypedDict(
-    "DataPointMenuLabelOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-DataPointTooltipOptionOutputTypeDef = TypedDict(
-    "DataPointTooltipOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-ExportToCSVOptionOutputTypeDef = TypedDict(
-    "ExportToCSVOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-ExportWithHiddenFieldsOptionOutputTypeDef = TypedDict(
-    "ExportWithHiddenFieldsOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-SheetControlsOptionOutputTypeDef = TypedDict(
-    "SheetControlsOptionOutputTypeDef",
-    {
-        "VisibilityState": DashboardUIStateType,
-    },
-    total=False,
-)
-
-SheetLayoutElementMaximizationOptionOutputTypeDef = TypedDict(
-    "SheetLayoutElementMaximizationOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-VisualAxisSortOptionOutputTypeDef = TypedDict(
-    "VisualAxisSortOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-VisualMenuOptionOutputTypeDef = TypedDict(
-    "VisualMenuOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
 DataPointDrillUpDownOptionTypeDef = TypedDict(
     "DataPointDrillUpDownOptionTypeDef",
     {
         "AvailabilityStatus": DashboardBehaviorType,
     },
     total=False,
 )
@@ -4375,70 +3391,31 @@
         "Status": ResourceStatusType,
         "SourceEntityArn": str,
         "Description": str,
     },
     total=False,
 )
 
-ExportHiddenFieldsOptionOutputTypeDef = TypedDict(
-    "ExportHiddenFieldsOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
 ExportHiddenFieldsOptionTypeDef = TypedDict(
     "ExportHiddenFieldsOptionTypeDef",
     {
         "AvailabilityStatus": DashboardBehaviorType,
     },
     total=False,
 )
 
-DataAggregationOutputTypeDef = TypedDict(
-    "DataAggregationOutputTypeDef",
-    {
-        "DatasetRowDateGranularity": TopicTimeGranularityType,
-        "DefaultDateColumnName": str,
-    },
-    total=False,
-)
-
 DataAggregationTypeDef = TypedDict(
     "DataAggregationTypeDef",
     {
         "DatasetRowDateGranularity": TopicTimeGranularityType,
         "DefaultDateColumnName": str,
     },
     total=False,
 )
 
-_RequiredDataBarsOptionsOutputTypeDef = TypedDict(
-    "_RequiredDataBarsOptionsOutputTypeDef",
-    {
-        "FieldId": str,
-    },
-)
-_OptionalDataBarsOptionsOutputTypeDef = TypedDict(
-    "_OptionalDataBarsOptionsOutputTypeDef",
-    {
-        "PositiveColor": str,
-        "NegativeColor": str,
-    },
-    total=False,
-)
-
-
-class DataBarsOptionsOutputTypeDef(
-    _RequiredDataBarsOptionsOutputTypeDef, _OptionalDataBarsOptionsOutputTypeDef
-):
-    pass
-
-
 _RequiredDataBarsOptionsTypeDef = TypedDict(
     "_RequiredDataBarsOptionsTypeDef",
     {
         "FieldId": str,
     },
 )
 _OptionalDataBarsOptionsTypeDef = TypedDict(
@@ -4471,57 +3448,14 @@
         "Colors": Sequence[str],
         "MinMaxGradient": Sequence[str],
         "EmptyFillColor": str,
     },
     total=False,
 )
 
-DataPathLabelTypeOutputTypeDef = TypedDict(
-    "DataPathLabelTypeOutputTypeDef",
-    {
-        "FieldId": str,
-        "FieldValue": str,
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-FieldLabelTypeOutputTypeDef = TypedDict(
-    "FieldLabelTypeOutputTypeDef",
-    {
-        "FieldId": str,
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-MaximumLabelTypeOutputTypeDef = TypedDict(
-    "MaximumLabelTypeOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-MinimumLabelTypeOutputTypeDef = TypedDict(
-    "MinimumLabelTypeOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-RangeEndsLabelTypeOutputTypeDef = TypedDict(
-    "RangeEndsLabelTypeOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 DataPathLabelTypeTypeDef = TypedDict(
     "DataPathLabelTypeTypeDef",
     {
         "FieldId": str,
         "FieldValue": str,
         "Visibility": VisibilityType,
     },
@@ -4557,22 +3491,14 @@
     "RangeEndsLabelTypeTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
 
-DataPathValueOutputTypeDef = TypedDict(
-    "DataPathValueOutputTypeDef",
-    {
-        "FieldId": str,
-        "FieldValue": str,
-    },
-)
-
 DataPathValueTypeDef = TypedDict(
     "DataPathValueTypeDef",
     {
         "FieldId": str,
         "FieldValue": str,
     },
 )
@@ -4582,47 +3508,14 @@
     {
         "Operator": FilterOperatorType,
         "Name": DataSetFilterAttributeType,
         "Value": str,
     },
 )
 
-_RequiredRowLevelPermissionDataSetOutputTypeDef = TypedDict(
-    "_RequiredRowLevelPermissionDataSetOutputTypeDef",
-    {
-        "Arn": str,
-        "PermissionPolicy": RowLevelPermissionPolicyType,
-    },
-)
-_OptionalRowLevelPermissionDataSetOutputTypeDef = TypedDict(
-    "_OptionalRowLevelPermissionDataSetOutputTypeDef",
-    {
-        "Namespace": str,
-        "FormatVersion": RowLevelPermissionFormatVersionType,
-        "Status": StatusType,
-    },
-    total=False,
-)
-
-
-class RowLevelPermissionDataSetOutputTypeDef(
-    _RequiredRowLevelPermissionDataSetOutputTypeDef, _OptionalRowLevelPermissionDataSetOutputTypeDef
-):
-    pass
-
-
-DataSetUsageConfigurationOutputTypeDef = TypedDict(
-    "DataSetUsageConfigurationOutputTypeDef",
-    {
-        "DisableUseAsDirectQuerySource": bool,
-        "DisableUseAsImportedSource": bool,
-    },
-    total=False,
-)
-
 FieldFolderOutputTypeDef = TypedDict(
     "FieldFolderOutputTypeDef",
     {
         "description": str,
         "columns": List[str],
     },
     total=False,
@@ -4643,164 +3536,14 @@
     {
         "Type": DataSourceErrorInfoTypeType,
         "Message": str,
     },
     total=False,
 )
 
-DatabricksParametersOutputTypeDef = TypedDict(
-    "DatabricksParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "SqlEndpointPath": str,
-    },
-)
-
-ExasolParametersOutputTypeDef = TypedDict(
-    "ExasolParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-    },
-)
-
-JiraParametersOutputTypeDef = TypedDict(
-    "JiraParametersOutputTypeDef",
-    {
-        "SiteBaseUrl": str,
-    },
-)
-
-MariaDbParametersOutputTypeDef = TypedDict(
-    "MariaDbParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
-MySqlParametersOutputTypeDef = TypedDict(
-    "MySqlParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
-OracleParametersOutputTypeDef = TypedDict(
-    "OracleParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
-PostgreSqlParametersOutputTypeDef = TypedDict(
-    "PostgreSqlParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
-PrestoParametersOutputTypeDef = TypedDict(
-    "PrestoParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Catalog": str,
-    },
-)
-
-RdsParametersOutputTypeDef = TypedDict(
-    "RdsParametersOutputTypeDef",
-    {
-        "InstanceId": str,
-        "Database": str,
-    },
-)
-
-_RequiredRedshiftParametersOutputTypeDef = TypedDict(
-    "_RequiredRedshiftParametersOutputTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalRedshiftParametersOutputTypeDef = TypedDict(
-    "_OptionalRedshiftParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "ClusterId": str,
-    },
-    total=False,
-)
-
-
-class RedshiftParametersOutputTypeDef(
-    _RequiredRedshiftParametersOutputTypeDef, _OptionalRedshiftParametersOutputTypeDef
-):
-    pass
-
-
-ServiceNowParametersOutputTypeDef = TypedDict(
-    "ServiceNowParametersOutputTypeDef",
-    {
-        "SiteBaseUrl": str,
-    },
-)
-
-SnowflakeParametersOutputTypeDef = TypedDict(
-    "SnowflakeParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Database": str,
-        "Warehouse": str,
-    },
-)
-
-SparkParametersOutputTypeDef = TypedDict(
-    "SparkParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-    },
-)
-
-SqlServerParametersOutputTypeDef = TypedDict(
-    "SqlServerParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
-TeradataParametersOutputTypeDef = TypedDict(
-    "TeradataParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
-TwitterParametersOutputTypeDef = TypedDict(
-    "TwitterParametersOutputTypeDef",
-    {
-        "Query": str,
-        "MaxRows": int,
-    },
-)
-
 DatabricksParametersTypeDef = TypedDict(
     "DatabricksParametersTypeDef",
     {
         "Host": str,
         "Port": int,
         "SqlEndpointPath": str,
     },
@@ -4981,35 +3724,14 @@
     "DateTimeDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": Sequence[Union[datetime, str]],
     },
     total=False,
 )
 
-_RequiredRollingDateConfigurationOutputTypeDef = TypedDict(
-    "_RequiredRollingDateConfigurationOutputTypeDef",
-    {
-        "Expression": str,
-    },
-)
-_OptionalRollingDateConfigurationOutputTypeDef = TypedDict(
-    "_OptionalRollingDateConfigurationOutputTypeDef",
-    {
-        "DataSetIdentifier": str,
-    },
-    total=False,
-)
-
-
-class RollingDateConfigurationOutputTypeDef(
-    _RequiredRollingDateConfigurationOutputTypeDef, _OptionalRollingDateConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredRollingDateConfigurationTypeDef = TypedDict(
     "_RequiredRollingDateConfigurationTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalRollingDateConfigurationTypeDef = TypedDict(
@@ -5032,16 +3754,16 @@
     {
         "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
         "CustomValue": datetime,
     },
     total=False,
 )
 
-MappedDataSetParameterOutputTypeDef = TypedDict(
-    "MappedDataSetParameterOutputTypeDef",
+MappedDataSetParameterTypeDef = TypedDict(
+    "MappedDataSetParameterTypeDef",
     {
         "DataSetIdentifier": str,
         "DataSetParameterName": str,
     },
 )
 
 DateTimeValueWhenUnsetConfigurationTypeDef = TypedDict(
@@ -5049,22 +3771,14 @@
     {
         "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
         "CustomValue": Union[datetime, str],
     },
     total=False,
 )
 
-MappedDataSetParameterTypeDef = TypedDict(
-    "MappedDataSetParameterTypeDef",
-    {
-        "DataSetIdentifier": str,
-        "DataSetParameterName": str,
-    },
-)
-
 DateTimeParameterOutputTypeDef = TypedDict(
     "DateTimeParameterOutputTypeDef",
     {
         "Name": str,
         "Values": List[datetime],
     },
 )
@@ -5073,23 +3787,14 @@
     "DateTimeParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[Union[datetime, str]],
     },
 )
 
-SheetControlInfoIconLabelOptionsOutputTypeDef = TypedDict(
-    "SheetControlInfoIconLabelOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "InfoIconText": str,
-    },
-    total=False,
-)
-
 SheetControlInfoIconLabelOptionsTypeDef = TypedDict(
     "SheetControlInfoIconLabelOptionsTypeDef",
     {
         "Visibility": VisibilityType,
         "InfoIconText": str,
     },
     total=False,
@@ -5107,23 +3812,14 @@
     "DecimalDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": Sequence[float],
     },
     total=False,
 )
 
-DecimalValueWhenUnsetConfigurationOutputTypeDef = TypedDict(
-    "DecimalValueWhenUnsetConfigurationOutputTypeDef",
-    {
-        "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
-        "CustomValue": float,
-    },
-    total=False,
-)
-
 DecimalValueWhenUnsetConfigurationTypeDef = TypedDict(
     "DecimalValueWhenUnsetConfigurationTypeDef",
     {
         "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
         "CustomValue": float,
     },
     total=False,
@@ -5934,56 +4630,31 @@
     "DescribeVPCConnectionRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "VPCConnectionId": str,
     },
 )
 
-NegativeFormatOutputTypeDef = TypedDict(
-    "NegativeFormatOutputTypeDef",
-    {
-        "Prefix": str,
-        "Suffix": str,
-    },
-    total=False,
-)
-
 NegativeFormatTypeDef = TypedDict(
     "NegativeFormatTypeDef",
     {
         "Prefix": str,
         "Suffix": str,
     },
     total=False,
 )
 
-DonutCenterOptionsOutputTypeDef = TypedDict(
-    "DonutCenterOptionsOutputTypeDef",
-    {
-        "LabelVisibility": VisibilityType,
-    },
-    total=False,
-)
-
 DonutCenterOptionsTypeDef = TypedDict(
     "DonutCenterOptionsTypeDef",
     {
         "LabelVisibility": VisibilityType,
     },
     total=False,
 )
 
-ListControlSelectAllOptionsOutputTypeDef = TypedDict(
-    "ListControlSelectAllOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 ListControlSelectAllOptionsTypeDef = TypedDict(
     "ListControlSelectAllOptionsTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
@@ -5993,37 +4664,14 @@
     {
         "Type": IngestionErrorTypeType,
         "Message": str,
     },
     total=False,
 )
 
-_RequiredExcludePeriodConfigurationOutputTypeDef = TypedDict(
-    "_RequiredExcludePeriodConfigurationOutputTypeDef",
-    {
-        "Amount": int,
-        "Granularity": TimeGranularityType,
-    },
-)
-_OptionalExcludePeriodConfigurationOutputTypeDef = TypedDict(
-    "_OptionalExcludePeriodConfigurationOutputTypeDef",
-    {
-        "Status": WidgetStatusType,
-    },
-    total=False,
-)
-
-
-class ExcludePeriodConfigurationOutputTypeDef(
-    _RequiredExcludePeriodConfigurationOutputTypeDef,
-    _OptionalExcludePeriodConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredExcludePeriodConfigurationTypeDef = TypedDict(
     "_RequiredExcludePeriodConfigurationTypeDef",
     {
         "Amount": int,
         "Granularity": TimeGranularityType,
     },
 )
@@ -6038,52 +4686,22 @@
 
 class ExcludePeriodConfigurationTypeDef(
     _RequiredExcludePeriodConfigurationTypeDef, _OptionalExcludePeriodConfigurationTypeDef
 ):
     pass
 
 
-FieldSortOutputTypeDef = TypedDict(
-    "FieldSortOutputTypeDef",
-    {
-        "FieldId": str,
-        "Direction": SortDirectionType,
-    },
-)
-
 FieldSortTypeDef = TypedDict(
     "FieldSortTypeDef",
     {
         "FieldId": str,
         "Direction": SortDirectionType,
     },
 )
 
-_RequiredFieldTooltipItemOutputTypeDef = TypedDict(
-    "_RequiredFieldTooltipItemOutputTypeDef",
-    {
-        "FieldId": str,
-    },
-)
-_OptionalFieldTooltipItemOutputTypeDef = TypedDict(
-    "_OptionalFieldTooltipItemOutputTypeDef",
-    {
-        "Label": str,
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-
-class FieldTooltipItemOutputTypeDef(
-    _RequiredFieldTooltipItemOutputTypeDef, _OptionalFieldTooltipItemOutputTypeDef
-):
-    pass
-
-
 _RequiredFieldTooltipItemTypeDef = TypedDict(
     "_RequiredFieldTooltipItemTypeDef",
     {
         "FieldId": str,
     },
 )
 _OptionalFieldTooltipItemTypeDef = TypedDict(
@@ -6096,22 +4714,14 @@
 )
 
 
 class FieldTooltipItemTypeDef(_RequiredFieldTooltipItemTypeDef, _OptionalFieldTooltipItemTypeDef):
     pass
 
 
-GeospatialMapStyleOptionsOutputTypeDef = TypedDict(
-    "GeospatialMapStyleOptionsOutputTypeDef",
-    {
-        "BaseMapStyle": BaseMapStyleTypeType,
-    },
-    total=False,
-)
-
 GeospatialMapStyleOptionsTypeDef = TypedDict(
     "GeospatialMapStyleOptionsTypeDef",
     {
         "BaseMapStyle": BaseMapStyleTypeType,
     },
     total=False,
 )
@@ -6128,21 +4738,14 @@
     "FilterSelectableValuesTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
-FilterOperationOutputTypeDef = TypedDict(
-    "FilterOperationOutputTypeDef",
-    {
-        "ConditionExpression": str,
-    },
-)
-
 SameSheetTargetVisualConfigurationOutputTypeDef = TypedDict(
     "SameSheetTargetVisualConfigurationOutputTypeDef",
     {
         "TargetVisuals": List[str],
         "TargetVisualOptions": Literal["ALL_VISUALS"],
     },
     total=False,
@@ -6183,30 +4786,14 @@
         "FolderType": Literal["SHARED"],
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
-FontSizeOutputTypeDef = TypedDict(
-    "FontSizeOutputTypeDef",
-    {
-        "Relative": RelativeFontSizeType,
-    },
-    total=False,
-)
-
-FontWeightOutputTypeDef = TypedDict(
-    "FontWeightOutputTypeDef",
-    {
-        "Name": FontWeightNameType,
-    },
-    total=False,
-)
-
 FontSizeTypeDef = TypedDict(
     "FontSizeTypeDef",
     {
         "Relative": RelativeFontSizeType,
     },
     total=False,
 )
@@ -6215,43 +4802,22 @@
     "FontWeightTypeDef",
     {
         "Name": FontWeightNameType,
     },
     total=False,
 )
 
-FontOutputTypeDef = TypedDict(
-    "FontOutputTypeDef",
-    {
-        "FontFamily": str,
-    },
-    total=False,
-)
-
 FontTypeDef = TypedDict(
     "FontTypeDef",
     {
         "FontFamily": str,
     },
     total=False,
 )
 
-TimeBasedForecastPropertiesOutputTypeDef = TypedDict(
-    "TimeBasedForecastPropertiesOutputTypeDef",
-    {
-        "PeriodsForward": int,
-        "PeriodsBackward": int,
-        "UpperBoundary": float,
-        "LowerBoundary": float,
-        "PredictionInterval": int,
-        "Seasonality": int,
-    },
-    total=False,
-)
-
 TimeBasedForecastPropertiesTypeDef = TypedDict(
     "TimeBasedForecastPropertiesTypeDef",
     {
         "PeriodsForward": int,
         "PeriodsBackward": int,
         "UpperBoundary": float,
         "LowerBoundary": float,
@@ -6291,72 +4857,39 @@
     {
         "StartDate": Union[datetime, str],
         "EndDate": Union[datetime, str],
         "Value": float,
     },
 )
 
-FreeFormLayoutScreenCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "FreeFormLayoutScreenCanvasSizeOptionsOutputTypeDef",
-    {
-        "OptimizedViewPortWidth": str,
-    },
-)
-
 FreeFormLayoutScreenCanvasSizeOptionsTypeDef = TypedDict(
     "FreeFormLayoutScreenCanvasSizeOptionsTypeDef",
     {
         "OptimizedViewPortWidth": str,
     },
 )
 
-FreeFormLayoutElementBackgroundStyleOutputTypeDef = TypedDict(
-    "FreeFormLayoutElementBackgroundStyleOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "Color": str,
-    },
-    total=False,
-)
-
 FreeFormLayoutElementBackgroundStyleTypeDef = TypedDict(
     "FreeFormLayoutElementBackgroundStyleTypeDef",
     {
         "Visibility": VisibilityType,
         "Color": str,
     },
     total=False,
 )
 
-FreeFormLayoutElementBorderStyleOutputTypeDef = TypedDict(
-    "FreeFormLayoutElementBorderStyleOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "Color": str,
-    },
-    total=False,
-)
-
 FreeFormLayoutElementBorderStyleTypeDef = TypedDict(
     "FreeFormLayoutElementBorderStyleTypeDef",
     {
         "Visibility": VisibilityType,
         "Color": str,
     },
     total=False,
 )
 
-LoadingAnimationOutputTypeDef = TypedDict(
-    "LoadingAnimationOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 LoadingAnimationTypeDef = TypedDict(
     "LoadingAnimationTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
@@ -6365,41 +4898,24 @@
     "SessionTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-GeospatialCoordinateBoundsOutputTypeDef = TypedDict(
-    "GeospatialCoordinateBoundsOutputTypeDef",
-    {
-        "North": float,
-        "South": float,
-        "West": float,
-        "East": float,
-    },
-)
-
 GeospatialCoordinateBoundsTypeDef = TypedDict(
     "GeospatialCoordinateBoundsTypeDef",
     {
         "North": float,
         "South": float,
         "West": float,
         "East": float,
     },
 )
 
-GeospatialHeatmapDataColorOutputTypeDef = TypedDict(
-    "GeospatialHeatmapDataColorOutputTypeDef",
-    {
-        "Color": str,
-    },
-)
-
 GeospatialHeatmapDataColorTypeDef = TypedDict(
     "GeospatialHeatmapDataColorTypeDef",
     {
         "Color": str,
     },
 )
 
@@ -6453,56 +4969,24 @@
 class GetSessionEmbedUrlRequestRequestTypeDef(
     _RequiredGetSessionEmbedUrlRequestRequestTypeDef,
     _OptionalGetSessionEmbedUrlRequestRequestTypeDef,
 ):
     pass
 
 
-TableBorderOptionsOutputTypeDef = TypedDict(
-    "TableBorderOptionsOutputTypeDef",
-    {
-        "Color": str,
-        "Thickness": int,
-        "Style": TableBorderStyleType,
-    },
-    total=False,
-)
-
 TableBorderOptionsTypeDef = TypedDict(
     "TableBorderOptionsTypeDef",
     {
         "Color": str,
         "Thickness": int,
         "Style": TableBorderStyleType,
     },
     total=False,
 )
 
-_RequiredGradientStopOutputTypeDef = TypedDict(
-    "_RequiredGradientStopOutputTypeDef",
-    {
-        "GradientOffset": float,
-    },
-)
-_OptionalGradientStopOutputTypeDef = TypedDict(
-    "_OptionalGradientStopOutputTypeDef",
-    {
-        "DataValue": float,
-        "Color": str,
-    },
-    total=False,
-)
-
-
-class GradientStopOutputTypeDef(
-    _RequiredGradientStopOutputTypeDef, _OptionalGradientStopOutputTypeDef
-):
-    pass
-
-
 _RequiredGradientStopTypeDef = TypedDict(
     "_RequiredGradientStopTypeDef",
     {
         "GradientOffset": float,
     },
 )
 _OptionalGradientStopTypeDef = TypedDict(
@@ -6515,36 +4999,14 @@
 )
 
 
 class GradientStopTypeDef(_RequiredGradientStopTypeDef, _OptionalGradientStopTypeDef):
     pass
 
 
-_RequiredGridLayoutScreenCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "_RequiredGridLayoutScreenCanvasSizeOptionsOutputTypeDef",
-    {
-        "ResizeOption": ResizeOptionType,
-    },
-)
-_OptionalGridLayoutScreenCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "_OptionalGridLayoutScreenCanvasSizeOptionsOutputTypeDef",
-    {
-        "OptimizedViewPortWidth": str,
-    },
-    total=False,
-)
-
-
-class GridLayoutScreenCanvasSizeOptionsOutputTypeDef(
-    _RequiredGridLayoutScreenCanvasSizeOptionsOutputTypeDef,
-    _OptionalGridLayoutScreenCanvasSizeOptionsOutputTypeDef,
-):
-    pass
-
-
 _RequiredGridLayoutScreenCanvasSizeOptionsTypeDef = TypedDict(
     "_RequiredGridLayoutScreenCanvasSizeOptionsTypeDef",
     {
         "ResizeOption": ResizeOptionType,
     },
 )
 _OptionalGridLayoutScreenCanvasSizeOptionsTypeDef = TypedDict(
@@ -6559,39 +5021,14 @@
 class GridLayoutScreenCanvasSizeOptionsTypeDef(
     _RequiredGridLayoutScreenCanvasSizeOptionsTypeDef,
     _OptionalGridLayoutScreenCanvasSizeOptionsTypeDef,
 ):
     pass
 
 
-_RequiredGridLayoutElementOutputTypeDef = TypedDict(
-    "_RequiredGridLayoutElementOutputTypeDef",
-    {
-        "ElementId": str,
-        "ElementType": LayoutElementTypeType,
-        "ColumnSpan": int,
-        "RowSpan": int,
-    },
-)
-_OptionalGridLayoutElementOutputTypeDef = TypedDict(
-    "_OptionalGridLayoutElementOutputTypeDef",
-    {
-        "ColumnIndex": int,
-        "RowIndex": int,
-    },
-    total=False,
-)
-
-
-class GridLayoutElementOutputTypeDef(
-    _RequiredGridLayoutElementOutputTypeDef, _OptionalGridLayoutElementOutputTypeDef
-):
-    pass
-
-
 _RequiredGridLayoutElementTypeDef = TypedDict(
     "_RequiredGridLayoutElementTypeDef",
     {
         "ElementId": str,
         "ElementType": LayoutElementTypeType,
         "ColumnSpan": int,
         "RowSpan": int,
@@ -6618,22 +5055,14 @@
     {
         "Operator": Literal["StartsWith"],
         "Name": Literal["GROUP_NAME"],
         "Value": str,
     },
 )
 
-GutterStyleOutputTypeDef = TypedDict(
-    "GutterStyleOutputTypeDef",
-    {
-        "Show": bool,
-    },
-    total=False,
-)
-
 GutterStyleTypeDef = TypedDict(
     "GutterStyleTypeDef",
     {
         "Show": bool,
     },
     total=False,
 )
@@ -6643,23 +5072,14 @@
     {
         "AssignmentName": str,
         "AssignmentStatus": AssignmentStatusType,
     },
     total=False,
 )
 
-LookbackWindowOutputTypeDef = TypedDict(
-    "LookbackWindowOutputTypeDef",
-    {
-        "ColumnName": str,
-        "Size": int,
-        "SizeUnit": LookbackWindowSizeUnitType,
-    },
-)
-
 LookbackWindowTypeDef = TypedDict(
     "LookbackWindowTypeDef",
     {
         "ColumnName": str,
         "Size": int,
         "SizeUnit": LookbackWindowSizeUnitType,
     },
@@ -6695,23 +5115,14 @@
     "IntegerDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": Sequence[int],
     },
     total=False,
 )
 
-IntegerValueWhenUnsetConfigurationOutputTypeDef = TypedDict(
-    "IntegerValueWhenUnsetConfigurationOutputTypeDef",
-    {
-        "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
-        "CustomValue": int,
-    },
-    total=False,
-)
-
 IntegerValueWhenUnsetConfigurationTypeDef = TypedDict(
     "IntegerValueWhenUnsetConfigurationTypeDef",
     {
         "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
         "CustomValue": int,
     },
     total=False,
@@ -6729,54 +5140,22 @@
     "IntegerParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[int],
     },
 )
 
-JoinKeyPropertiesOutputTypeDef = TypedDict(
-    "JoinKeyPropertiesOutputTypeDef",
-    {
-        "UniqueKey": bool,
-    },
-    total=False,
-)
-
 JoinKeyPropertiesTypeDef = TypedDict(
     "JoinKeyPropertiesTypeDef",
     {
         "UniqueKey": bool,
     },
     total=False,
 )
 
-ProgressBarOptionsOutputTypeDef = TypedDict(
-    "ProgressBarOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-SecondaryValueOptionsOutputTypeDef = TypedDict(
-    "SecondaryValueOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-TrendArrowOptionsOutputTypeDef = TypedDict(
-    "TrendArrowOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 ProgressBarOptionsTypeDef = TypedDict(
     "ProgressBarOptionsTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
@@ -6793,36 +5172,14 @@
     "TrendArrowOptionsTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
 
-LineChartLineStyleSettingsOutputTypeDef = TypedDict(
-    "LineChartLineStyleSettingsOutputTypeDef",
-    {
-        "LineVisibility": VisibilityType,
-        "LineInterpolation": LineInterpolationType,
-        "LineStyle": LineChartLineStyleType,
-        "LineWidth": str,
-    },
-    total=False,
-)
-
-LineChartMarkerStyleSettingsOutputTypeDef = TypedDict(
-    "LineChartMarkerStyleSettingsOutputTypeDef",
-    {
-        "MarkerVisibility": VisibilityType,
-        "MarkerShape": LineChartMarkerShapeType,
-        "MarkerSize": str,
-        "MarkerColor": str,
-    },
-    total=False,
-)
-
 LineChartLineStyleSettingsTypeDef = TypedDict(
     "LineChartLineStyleSettingsTypeDef",
     {
         "LineVisibility": VisibilityType,
         "LineInterpolation": LineInterpolationType,
         "LineStyle": LineChartLineStyleType,
         "LineWidth": str,
@@ -6837,22 +5194,14 @@
         "MarkerShape": LineChartMarkerShapeType,
         "MarkerSize": str,
         "MarkerColor": str,
     },
     total=False,
 )
 
-MissingDataConfigurationOutputTypeDef = TypedDict(
-    "MissingDataConfigurationOutputTypeDef",
-    {
-        "TreatmentOption": MissingDataTreatmentOptionType,
-    },
-    total=False,
-)
-
 MissingDataConfigurationTypeDef = TypedDict(
     "MissingDataConfigurationTypeDef",
     {
         "TreatmentOption": MissingDataTreatmentOptionType,
     },
     total=False,
 )
@@ -6931,22 +5280,14 @@
 class ListAssetBundleImportJobsRequestRequestTypeDef(
     _RequiredListAssetBundleImportJobsRequestRequestTypeDef,
     _OptionalListAssetBundleImportJobsRequestRequestTypeDef,
 ):
     pass
 
 
-ListControlSearchOptionsOutputTypeDef = TypedDict(
-    "ListControlSearchOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 ListControlSearchOptionsTypeDef = TypedDict(
     "ListControlSearchOptionsTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
@@ -7249,22 +5590,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredListTemplateAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateAliasesRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TemplateId": str,
     },
 )
@@ -7556,56 +5889,31 @@
 class ListVPCConnectionsRequestRequestTypeDef(
     _RequiredListVPCConnectionsRequestRequestTypeDef,
     _OptionalListVPCConnectionsRequestRequestTypeDef,
 ):
     pass
 
 
-LongFormatTextOutputTypeDef = TypedDict(
-    "LongFormatTextOutputTypeDef",
-    {
-        "PlainText": str,
-        "RichText": str,
-    },
-    total=False,
-)
-
 LongFormatTextTypeDef = TypedDict(
     "LongFormatTextTypeDef",
     {
         "PlainText": str,
         "RichText": str,
     },
     total=False,
 )
 
-ManifestFileLocationOutputTypeDef = TypedDict(
-    "ManifestFileLocationOutputTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-)
-
 ManifestFileLocationTypeDef = TypedDict(
     "ManifestFileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
-MarginStyleOutputTypeDef = TypedDict(
-    "MarginStyleOutputTypeDef",
-    {
-        "Show": bool,
-    },
-    total=False,
-)
-
 MarginStyleTypeDef = TypedDict(
     "MarginStyleTypeDef",
     {
         "Show": bool,
     },
     total=False,
 )
@@ -7667,58 +5975,32 @@
         "DecimalStaticValues": Sequence[float],
         "DateTimeStaticValues": Sequence[Union[datetime, str]],
         "IntegerStaticValues": Sequence[int],
     },
     total=False,
 )
 
-NumericRangeFilterValueOutputTypeDef = TypedDict(
-    "NumericRangeFilterValueOutputTypeDef",
-    {
-        "StaticValue": float,
-        "Parameter": str,
-    },
-    total=False,
-)
-
 NumericRangeFilterValueTypeDef = TypedDict(
     "NumericRangeFilterValueTypeDef",
     {
         "StaticValue": float,
         "Parameter": str,
     },
     total=False,
 )
 
-ThousandSeparatorOptionsOutputTypeDef = TypedDict(
-    "ThousandSeparatorOptionsOutputTypeDef",
-    {
-        "Symbol": NumericSeparatorSymbolType,
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 ThousandSeparatorOptionsTypeDef = TypedDict(
     "ThousandSeparatorOptionsTypeDef",
     {
         "Symbol": NumericSeparatorSymbolType,
         "Visibility": VisibilityType,
     },
     total=False,
 )
 
-PercentileAggregationOutputTypeDef = TypedDict(
-    "PercentileAggregationOutputTypeDef",
-    {
-        "PercentileValue": float,
-    },
-    total=False,
-)
-
 PercentileAggregationTypeDef = TypedDict(
     "PercentileAggregationTypeDef",
     {
         "PercentileValue": float,
     },
     total=False,
 )
@@ -7735,88 +6017,40 @@
     "StringParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
-PercentVisibleRangeOutputTypeDef = TypedDict(
-    "PercentVisibleRangeOutputTypeDef",
-    {
-        "From": float,
-        "To": float,
-    },
-    total=False,
-)
-
 PercentVisibleRangeTypeDef = TypedDict(
     "PercentVisibleRangeTypeDef",
     {
         "From": float,
         "To": float,
     },
     total=False,
 )
 
-PivotTableConditionalFormattingScopeOutputTypeDef = TypedDict(
-    "PivotTableConditionalFormattingScopeOutputTypeDef",
-    {
-        "Role": PivotTableConditionalFormattingScopeRoleType,
-    },
-    total=False,
-)
-
 PivotTableConditionalFormattingScopeTypeDef = TypedDict(
     "PivotTableConditionalFormattingScopeTypeDef",
     {
         "Role": PivotTableConditionalFormattingScopeRoleType,
     },
     total=False,
 )
 
-PivotTablePaginatedReportOptionsOutputTypeDef = TypedDict(
-    "PivotTablePaginatedReportOptionsOutputTypeDef",
-    {
-        "VerticalOverflowVisibility": VisibilityType,
-        "OverflowColumnHeaderVisibility": VisibilityType,
-    },
-    total=False,
-)
-
 PivotTablePaginatedReportOptionsTypeDef = TypedDict(
     "PivotTablePaginatedReportOptionsTypeDef",
     {
         "VerticalOverflowVisibility": VisibilityType,
         "OverflowColumnHeaderVisibility": VisibilityType,
     },
     total=False,
 )
 
-_RequiredPivotTableFieldOptionOutputTypeDef = TypedDict(
-    "_RequiredPivotTableFieldOptionOutputTypeDef",
-    {
-        "FieldId": str,
-    },
-)
-_OptionalPivotTableFieldOptionOutputTypeDef = TypedDict(
-    "_OptionalPivotTableFieldOptionOutputTypeDef",
-    {
-        "CustomLabel": str,
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-
-class PivotTableFieldOptionOutputTypeDef(
-    _RequiredPivotTableFieldOptionOutputTypeDef, _OptionalPivotTableFieldOptionOutputTypeDef
-):
-    pass
-
-
 _RequiredPivotTableFieldOptionTypeDef = TypedDict(
     "_RequiredPivotTableFieldOptionTypeDef",
     {
         "FieldId": str,
     },
 )
 _OptionalPivotTableFieldOptionTypeDef = TypedDict(
@@ -7831,22 +6065,14 @@
 
 class PivotTableFieldOptionTypeDef(
     _RequiredPivotTableFieldOptionTypeDef, _OptionalPivotTableFieldOptionTypeDef
 ):
     pass
 
 
-PivotTableFieldSubtotalOptionsOutputTypeDef = TypedDict(
-    "PivotTableFieldSubtotalOptionsOutputTypeDef",
-    {
-        "FieldId": str,
-    },
-    total=False,
-)
-
 PivotTableFieldSubtotalOptionsTypeDef = TypedDict(
     "PivotTableFieldSubtotalOptionsTypeDef",
     {
         "FieldId": str,
     },
     total=False,
 )
@@ -7879,103 +6105,54 @@
 ProjectOperationTypeDef = TypedDict(
     "ProjectOperationTypeDef",
     {
         "ProjectedColumns": Sequence[str],
     },
 )
 
-RadarChartAreaStyleSettingsOutputTypeDef = TypedDict(
-    "RadarChartAreaStyleSettingsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 RadarChartAreaStyleSettingsTypeDef = TypedDict(
     "RadarChartAreaStyleSettingsTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
 
-RangeConstantOutputTypeDef = TypedDict(
-    "RangeConstantOutputTypeDef",
-    {
-        "Minimum": str,
-        "Maximum": str,
-    },
-    total=False,
-)
-
 RangeConstantTypeDef = TypedDict(
     "RangeConstantTypeDef",
     {
         "Minimum": str,
         "Maximum": str,
     },
     total=False,
 )
 
-ReferenceLineCustomLabelConfigurationOutputTypeDef = TypedDict(
-    "ReferenceLineCustomLabelConfigurationOutputTypeDef",
-    {
-        "CustomLabel": str,
-    },
-)
-
 ReferenceLineCustomLabelConfigurationTypeDef = TypedDict(
     "ReferenceLineCustomLabelConfigurationTypeDef",
     {
         "CustomLabel": str,
     },
 )
 
-ReferenceLineStaticDataConfigurationOutputTypeDef = TypedDict(
-    "ReferenceLineStaticDataConfigurationOutputTypeDef",
-    {
-        "Value": float,
-    },
-)
-
 ReferenceLineStaticDataConfigurationTypeDef = TypedDict(
     "ReferenceLineStaticDataConfigurationTypeDef",
     {
         "Value": float,
     },
 )
 
-ReferenceLineStyleConfigurationOutputTypeDef = TypedDict(
-    "ReferenceLineStyleConfigurationOutputTypeDef",
-    {
-        "Pattern": ReferenceLinePatternTypeType,
-        "Color": str,
-    },
-    total=False,
-)
-
 ReferenceLineStyleConfigurationTypeDef = TypedDict(
     "ReferenceLineStyleConfigurationTypeDef",
     {
         "Pattern": ReferenceLinePatternTypeType,
         "Color": str,
     },
     total=False,
 )
 
-ScheduleRefreshOnEntityOutputTypeDef = TypedDict(
-    "ScheduleRefreshOnEntityOutputTypeDef",
-    {
-        "DayOfWeek": DayOfWeekType,
-        "DayOfMonth": str,
-    },
-    total=False,
-)
-
 ScheduleRefreshOnEntityTypeDef = TypedDict(
     "ScheduleRefreshOnEntityTypeDef",
     {
         "DayOfWeek": DayOfWeekType,
         "DayOfMonth": str,
     },
     total=False,
@@ -8023,22 +6200,14 @@
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
     {
         "InitialTopicId": str,
     },
     total=False,
 )
 
-RenameColumnOperationOutputTypeDef = TypedDict(
-    "RenameColumnOperationOutputTypeDef",
-    {
-        "ColumnName": str,
-        "NewColumnName": str,
-    },
-)
-
 RenameColumnOperationTypeDef = TypedDict(
     "RenameColumnOperationTypeDef",
     {
         "ColumnName": str,
         "NewColumnName": str,
     },
 )
@@ -8047,37 +6216,14 @@
     "RestoreAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
 
-_RequiredRowLevelPermissionTagRuleOutputTypeDef = TypedDict(
-    "_RequiredRowLevelPermissionTagRuleOutputTypeDef",
-    {
-        "TagKey": str,
-        "ColumnName": str,
-    },
-)
-_OptionalRowLevelPermissionTagRuleOutputTypeDef = TypedDict(
-    "_OptionalRowLevelPermissionTagRuleOutputTypeDef",
-    {
-        "TagMultiValueDelimiter": str,
-        "MatchAllValue": str,
-    },
-    total=False,
-)
-
-
-class RowLevelPermissionTagRuleOutputTypeDef(
-    _RequiredRowLevelPermissionTagRuleOutputTypeDef, _OptionalRowLevelPermissionTagRuleOutputTypeDef
-):
-    pass
-
-
 _RequiredRowLevelPermissionTagRuleTypeDef = TypedDict(
     "_RequiredRowLevelPermissionTagRuleTypeDef",
     {
         "TagKey": str,
         "ColumnName": str,
     },
 )
@@ -8093,83 +6239,43 @@
 
 class RowLevelPermissionTagRuleTypeDef(
     _RequiredRowLevelPermissionTagRuleTypeDef, _OptionalRowLevelPermissionTagRuleTypeDef
 ):
     pass
 
 
-S3BucketConfigurationOutputTypeDef = TypedDict(
-    "S3BucketConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-        "BucketPrefix": str,
-        "BucketRegion": str,
-    },
-)
-
 S3BucketConfigurationTypeDef = TypedDict(
     "S3BucketConfigurationTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
         "BucketRegion": str,
     },
 )
 
-UploadSettingsOutputTypeDef = TypedDict(
-    "UploadSettingsOutputTypeDef",
-    {
-        "Format": FileFormatType,
-        "StartFromRow": int,
-        "ContainsHeader": bool,
-        "TextQualifier": TextQualifierType,
-        "Delimiter": str,
-    },
-    total=False,
-)
-
 UploadSettingsTypeDef = TypedDict(
     "UploadSettingsTypeDef",
     {
         "Format": FileFormatType,
         "StartFromRow": int,
         "ContainsHeader": bool,
         "TextQualifier": TextQualifierType,
         "Delimiter": str,
     },
     total=False,
 )
 
-SectionAfterPageBreakOutputTypeDef = TypedDict(
-    "SectionAfterPageBreakOutputTypeDef",
-    {
-        "Status": SectionPageBreakStatusType,
-    },
-    total=False,
-)
-
 SectionAfterPageBreakTypeDef = TypedDict(
     "SectionAfterPageBreakTypeDef",
     {
         "Status": SectionPageBreakStatusType,
     },
     total=False,
 )
 
-SpacingOutputTypeDef = TypedDict(
-    "SpacingOutputTypeDef",
-    {
-        "Top": str,
-        "Bottom": str,
-        "Left": str,
-        "Right": str,
-    },
-    total=False,
-)
-
 SpacingTypeDef = TypedDict(
     "SpacingTypeDef",
     {
         "Top": str,
         "Bottom": str,
         "Left": str,
         "Right": str,
@@ -8266,35 +6372,14 @@
         "TruthyCellValueSynonyms": Sequence[str],
         "FalseyCellValue": str,
         "FalseyCellValueSynonyms": Sequence[str],
     },
     total=False,
 )
 
-_RequiredSheetTextBoxOutputTypeDef = TypedDict(
-    "_RequiredSheetTextBoxOutputTypeDef",
-    {
-        "SheetTextBoxId": str,
-    },
-)
-_OptionalSheetTextBoxOutputTypeDef = TypedDict(
-    "_OptionalSheetTextBoxOutputTypeDef",
-    {
-        "Content": str,
-    },
-    total=False,
-)
-
-
-class SheetTextBoxOutputTypeDef(
-    _RequiredSheetTextBoxOutputTypeDef, _OptionalSheetTextBoxOutputTypeDef
-):
-    pass
-
-
 _RequiredSheetTextBoxTypeDef = TypedDict(
     "_RequiredSheetTextBoxTypeDef",
     {
         "SheetTextBoxId": str,
     },
 )
 _OptionalSheetTextBoxTypeDef = TypedDict(
@@ -8306,57 +6391,31 @@
 )
 
 
 class SheetTextBoxTypeDef(_RequiredSheetTextBoxTypeDef, _OptionalSheetTextBoxTypeDef):
     pass
 
 
-SheetElementConfigurationOverridesOutputTypeDef = TypedDict(
-    "SheetElementConfigurationOverridesOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 SheetElementConfigurationOverridesTypeDef = TypedDict(
     "SheetElementConfigurationOverridesTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
 
-ShortFormatTextOutputTypeDef = TypedDict(
-    "ShortFormatTextOutputTypeDef",
-    {
-        "PlainText": str,
-        "RichText": str,
-    },
-    total=False,
-)
-
 ShortFormatTextTypeDef = TypedDict(
     "ShortFormatTextTypeDef",
     {
         "PlainText": str,
         "RichText": str,
     },
     total=False,
 )
 
-SmallMultiplesAxisPropertiesOutputTypeDef = TypedDict(
-    "SmallMultiplesAxisPropertiesOutputTypeDef",
-    {
-        "Scale": SmallMultiplesAxisScaleType,
-        "Placement": SmallMultiplesAxisPlacementType,
-    },
-    total=False,
-)
-
 SmallMultiplesAxisPropertiesTypeDef = TypedDict(
     "SmallMultiplesAxisPropertiesTypeDef",
     {
         "Scale": SmallMultiplesAxisScaleType,
         "Placement": SmallMultiplesAxisPlacementType,
     },
     total=False,
@@ -8436,74 +6495,40 @@
     "StringDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": Sequence[str],
     },
     total=False,
 )
 
-StringValueWhenUnsetConfigurationOutputTypeDef = TypedDict(
-    "StringValueWhenUnsetConfigurationOutputTypeDef",
-    {
-        "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
-        "CustomValue": str,
-    },
-    total=False,
-)
-
 StringValueWhenUnsetConfigurationTypeDef = TypedDict(
     "StringValueWhenUnsetConfigurationTypeDef",
     {
         "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
         "CustomValue": str,
     },
     total=False,
 )
 
-TableCellImageSizingConfigurationOutputTypeDef = TypedDict(
-    "TableCellImageSizingConfigurationOutputTypeDef",
-    {
-        "TableCellImageScalingConfiguration": TableCellImageScalingConfigurationType,
-    },
-    total=False,
-)
-
 TableCellImageSizingConfigurationTypeDef = TypedDict(
     "TableCellImageSizingConfigurationTypeDef",
     {
         "TableCellImageScalingConfiguration": TableCellImageScalingConfigurationType,
     },
     total=False,
 )
 
-TablePaginatedReportOptionsOutputTypeDef = TypedDict(
-    "TablePaginatedReportOptionsOutputTypeDef",
-    {
-        "VerticalOverflowVisibility": VisibilityType,
-        "OverflowColumnHeaderVisibility": VisibilityType,
-    },
-    total=False,
-)
-
 TablePaginatedReportOptionsTypeDef = TypedDict(
     "TablePaginatedReportOptionsTypeDef",
     {
         "VerticalOverflowVisibility": VisibilityType,
         "OverflowColumnHeaderVisibility": VisibilityType,
     },
     total=False,
 )
 
-TableFieldCustomIconContentOutputTypeDef = TypedDict(
-    "TableFieldCustomIconContentOutputTypeDef",
-    {
-        "Icon": Literal["LINK"],
-    },
-    total=False,
-)
-
 TableFieldCustomIconContentTypeDef = TypedDict(
     "TableFieldCustomIconContentTypeDef",
     {
         "Icon": Literal["LINK"],
     },
     total=False,
 )
@@ -8511,53 +6536,22 @@
 TemplateSourceTemplateTypeDef = TypedDict(
     "TemplateSourceTemplateTypeDef",
     {
         "Arn": str,
     },
 )
 
-TextControlPlaceholderOptionsOutputTypeDef = TypedDict(
-    "TextControlPlaceholderOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 TextControlPlaceholderOptionsTypeDef = TypedDict(
     "TextControlPlaceholderOptionsTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
 
-UIColorPaletteOutputTypeDef = TypedDict(
-    "UIColorPaletteOutputTypeDef",
-    {
-        "PrimaryForeground": str,
-        "PrimaryBackground": str,
-        "SecondaryForeground": str,
-        "SecondaryBackground": str,
-        "Accent": str,
-        "AccentForeground": str,
-        "Danger": str,
-        "DangerForeground": str,
-        "Warning": str,
-        "WarningForeground": str,
-        "Success": str,
-        "SuccessForeground": str,
-        "Dimension": str,
-        "DimensionForeground": str,
-        "Measure": str,
-        "MeasureForeground": str,
-    },
-    total=False,
-)
-
 UIColorPaletteTypeDef = TypedDict(
     "UIColorPaletteTypeDef",
     {
         "PrimaryForeground": str,
         "PrimaryBackground": str,
         "SecondaryForeground": str,
         "SecondaryBackground": str,
@@ -8582,23 +6576,14 @@
     {
         "Type": Literal["INTERNAL_FAILURE"],
         "Message": str,
     },
     total=False,
 )
 
-TopicSingularFilterConstantOutputTypeDef = TypedDict(
-    "TopicSingularFilterConstantOutputTypeDef",
-    {
-        "ConstantType": ConstantTypeType,
-        "SingularConstant": str,
-    },
-    total=False,
-)
-
 TopicSingularFilterConstantTypeDef = TypedDict(
     "TopicSingularFilterConstantTypeDef",
     {
         "ConstantType": ConstantTypeType,
         "SingularConstant": str,
     },
     total=False,
@@ -8836,43 +6821,22 @@
 class UpdateVPCConnectionRequestRequestTypeDef(
     _RequiredUpdateVPCConnectionRequestRequestTypeDef,
     _OptionalUpdateVPCConnectionRequestRequestTypeDef,
 ):
     pass
 
 
-WaterfallChartOptionsOutputTypeDef = TypedDict(
-    "WaterfallChartOptionsOutputTypeDef",
-    {
-        "TotalBarLabel": str,
-    },
-    total=False,
-)
-
 WaterfallChartOptionsTypeDef = TypedDict(
     "WaterfallChartOptionsTypeDef",
     {
         "TotalBarLabel": str,
     },
     total=False,
 )
 
-WordCloudOptionsOutputTypeDef = TypedDict(
-    "WordCloudOptionsOutputTypeDef",
-    {
-        "WordOrientation": WordCloudWordOrientationType,
-        "WordScaling": WordCloudWordScalingType,
-        "CloudLayout": WordCloudCloudLayoutType,
-        "WordCasing": WordCloudWordCasingType,
-        "WordPadding": WordCloudWordPaddingType,
-        "MaximumStringLength": int,
-    },
-    total=False,
-)
-
 WordCloudOptionsTypeDef = TypedDict(
     "WordCloudOptionsTypeDef",
     {
         "WordOrientation": WordCloudWordOrientationType,
         "WordScaling": WordCloudWordScalingType,
         "CloudLayout": WordCloudCloudLayoutType,
         "WordCasing": WordCloudWordCasingType,
@@ -8901,152 +6865,52 @@
 class UpdateAccountCustomizationRequestRequestTypeDef(
     _RequiredUpdateAccountCustomizationRequestRequestTypeDef,
     _OptionalUpdateAccountCustomizationRequestRequestTypeDef,
 ):
     pass
 
 
-AxisLabelReferenceOptionsOutputTypeDef = TypedDict(
-    "AxisLabelReferenceOptionsOutputTypeDef",
+AxisLabelReferenceOptionsTypeDef = TypedDict(
+    "AxisLabelReferenceOptionsTypeDef",
     {
         "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
+        "Column": ColumnIdentifierTypeDef,
     },
 )
 
-CascadingControlSourceOutputTypeDef = TypedDict(
-    "CascadingControlSourceOutputTypeDef",
+CascadingControlSourceTypeDef = TypedDict(
+    "CascadingControlSourceTypeDef",
     {
         "SourceSheetControlId": str,
-        "ColumnToMatch": ColumnIdentifierOutputTypeDef,
+        "ColumnToMatch": ColumnIdentifierTypeDef,
     },
     total=False,
 )
 
 CategoryDrillDownFilterOutputTypeDef = TypedDict(
     "CategoryDrillDownFilterOutputTypeDef",
     {
-        "Column": ColumnIdentifierOutputTypeDef,
+        "Column": ColumnIdentifierTypeDef,
         "CategoryValues": List[str],
     },
 )
 
-ContributionAnalysisDefaultOutputTypeDef = TypedDict(
-    "ContributionAnalysisDefaultOutputTypeDef",
-    {
-        "MeasureFieldId": str,
-        "ContributorDimensions": List[ColumnIdentifierOutputTypeDef],
-    },
-)
-
-_RequiredDynamicDefaultValueOutputTypeDef = TypedDict(
-    "_RequiredDynamicDefaultValueOutputTypeDef",
-    {
-        "DefaultValueColumn": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalDynamicDefaultValueOutputTypeDef = TypedDict(
-    "_OptionalDynamicDefaultValueOutputTypeDef",
-    {
-        "UserNameColumn": ColumnIdentifierOutputTypeDef,
-        "GroupNameColumn": ColumnIdentifierOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class DynamicDefaultValueOutputTypeDef(
-    _RequiredDynamicDefaultValueOutputTypeDef, _OptionalDynamicDefaultValueOutputTypeDef
-):
-    pass
-
-
-FilterOperationSelectedFieldsConfigurationOutputTypeDef = TypedDict(
-    "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
-    {
-        "SelectedFields": List[str],
-        "SelectedFieldOptions": Literal["ALL_FIELDS"],
-        "SelectedColumns": List[ColumnIdentifierOutputTypeDef],
-    },
-    total=False,
-)
-
-NumericEqualityDrillDownFilterOutputTypeDef = TypedDict(
-    "NumericEqualityDrillDownFilterOutputTypeDef",
-    {
-        "Column": ColumnIdentifierOutputTypeDef,
-        "Value": float,
-    },
-)
-
-ParameterSelectableValuesOutputTypeDef = TypedDict(
-    "ParameterSelectableValuesOutputTypeDef",
-    {
-        "Values": List[str],
-        "LinkToDataSetColumn": ColumnIdentifierOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredTimeEqualityFilterOutputTypeDef = TypedDict(
-    "_RequiredTimeEqualityFilterOutputTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalTimeEqualityFilterOutputTypeDef = TypedDict(
-    "_OptionalTimeEqualityFilterOutputTypeDef",
-    {
-        "Value": datetime,
-        "ParameterName": str,
-        "TimeGranularity": TimeGranularityType,
-    },
-    total=False,
-)
-
-
-class TimeEqualityFilterOutputTypeDef(
-    _RequiredTimeEqualityFilterOutputTypeDef, _OptionalTimeEqualityFilterOutputTypeDef
-):
-    pass
-
-
-TimeRangeDrillDownFilterOutputTypeDef = TypedDict(
-    "TimeRangeDrillDownFilterOutputTypeDef",
-    {
-        "Column": ColumnIdentifierOutputTypeDef,
-        "RangeMinimum": datetime,
-        "RangeMaximum": datetime,
-        "TimeGranularity": TimeGranularityType,
-    },
-)
-
-AxisLabelReferenceOptionsTypeDef = TypedDict(
-    "AxisLabelReferenceOptionsTypeDef",
+CategoryDrillDownFilterTypeDef = TypedDict(
+    "CategoryDrillDownFilterTypeDef",
     {
-        "FieldId": str,
         "Column": ColumnIdentifierTypeDef,
+        "CategoryValues": Sequence[str],
     },
 )
 
-CascadingControlSourceTypeDef = TypedDict(
-    "CascadingControlSourceTypeDef",
-    {
-        "SourceSheetControlId": str,
-        "ColumnToMatch": ColumnIdentifierTypeDef,
-    },
-    total=False,
-)
-
-CategoryDrillDownFilterTypeDef = TypedDict(
-    "CategoryDrillDownFilterTypeDef",
+ContributionAnalysisDefaultOutputTypeDef = TypedDict(
+    "ContributionAnalysisDefaultOutputTypeDef",
     {
-        "Column": ColumnIdentifierTypeDef,
-        "CategoryValues": Sequence[str],
+        "MeasureFieldId": str,
+        "ContributorDimensions": List[ColumnIdentifierTypeDef],
     },
 )
 
 ContributionAnalysisDefaultTypeDef = TypedDict(
     "ContributionAnalysisDefaultTypeDef",
     {
         "MeasureFieldId": str,
@@ -9072,14 +6936,24 @@
 
 class DynamicDefaultValueTypeDef(
     _RequiredDynamicDefaultValueTypeDef, _OptionalDynamicDefaultValueTypeDef
 ):
     pass
 
 
+FilterOperationSelectedFieldsConfigurationOutputTypeDef = TypedDict(
+    "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
+    {
+        "SelectedFields": List[str],
+        "SelectedFieldOptions": Literal["ALL_FIELDS"],
+        "SelectedColumns": List[ColumnIdentifierTypeDef],
+    },
+    total=False,
+)
+
 FilterOperationSelectedFieldsConfigurationTypeDef = TypedDict(
     "FilterOperationSelectedFieldsConfigurationTypeDef",
     {
         "SelectedFields": Sequence[str],
         "SelectedFieldOptions": Literal["ALL_FIELDS"],
         "SelectedColumns": Sequence[ColumnIdentifierTypeDef],
     },
@@ -9090,23 +6964,56 @@
     "NumericEqualityDrillDownFilterTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "Value": float,
     },
 )
 
+ParameterSelectableValuesOutputTypeDef = TypedDict(
+    "ParameterSelectableValuesOutputTypeDef",
+    {
+        "Values": List[str],
+        "LinkToDataSetColumn": ColumnIdentifierTypeDef,
+    },
+    total=False,
+)
+
 ParameterSelectableValuesTypeDef = TypedDict(
     "ParameterSelectableValuesTypeDef",
     {
         "Values": Sequence[str],
         "LinkToDataSetColumn": ColumnIdentifierTypeDef,
     },
     total=False,
 )
 
+_RequiredTimeEqualityFilterOutputTypeDef = TypedDict(
+    "_RequiredTimeEqualityFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+    },
+)
+_OptionalTimeEqualityFilterOutputTypeDef = TypedDict(
+    "_OptionalTimeEqualityFilterOutputTypeDef",
+    {
+        "Value": datetime,
+        "ParameterName": str,
+        "TimeGranularity": TimeGranularityType,
+    },
+    total=False,
+)
+
+
+class TimeEqualityFilterOutputTypeDef(
+    _RequiredTimeEqualityFilterOutputTypeDef, _OptionalTimeEqualityFilterOutputTypeDef
+):
+    pass
+
+
 _RequiredTimeEqualityFilterTypeDef = TypedDict(
     "_RequiredTimeEqualityFilterTypeDef",
     {
         "FilterId": str,
         "Column": ColumnIdentifierTypeDef,
     },
 )
@@ -9123,14 +7030,24 @@
 
 class TimeEqualityFilterTypeDef(
     _RequiredTimeEqualityFilterTypeDef, _OptionalTimeEqualityFilterTypeDef
 ):
     pass
 
 
+TimeRangeDrillDownFilterOutputTypeDef = TypedDict(
+    "TimeRangeDrillDownFilterOutputTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+        "RangeMinimum": datetime,
+        "RangeMaximum": datetime,
+        "TimeGranularity": TimeGranularityType,
+    },
+)
+
 TimeRangeDrillDownFilterTypeDef = TypedDict(
     "TimeRangeDrillDownFilterTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "RangeMinimum": Union[datetime, str],
         "RangeMaximum": Union[datetime, str],
         "TimeGranularity": TimeGranularityType,
@@ -9224,37 +7141,28 @@
 RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef = TypedDict(
     "RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef",
     {
         "InitialDashboardVisualId": DashboardVisualIdTypeDef,
     },
 )
 
-ArcAxisConfigurationOutputTypeDef = TypedDict(
-    "ArcAxisConfigurationOutputTypeDef",
-    {
-        "Range": ArcAxisDisplayRangeOutputTypeDef,
-        "ReserveRange": int,
-    },
-    total=False,
-)
-
 ArcAxisConfigurationTypeDef = TypedDict(
     "ArcAxisConfigurationTypeDef",
     {
         "Range": ArcAxisDisplayRangeTypeDef,
         "ReserveRange": int,
     },
     total=False,
 )
 
 AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef = TypedDict(
     "AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef",
     {
         "ResourceIdOverrideConfiguration": (
-            AssetBundleExportJobResourceIdOverrideConfigurationOutputTypeDef
+            AssetBundleExportJobResourceIdOverrideConfigurationTypeDef
         ),
         "VPCConnections": List[AssetBundleExportJobVPCConnectionOverridePropertiesOutputTypeDef],
         "RefreshSchedules": List[
             AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef
         ],
         "DataSources": List[AssetBundleExportJobDataSourceOverridePropertiesOutputTypeDef],
         "DataSets": List[AssetBundleExportJobDataSetOverridePropertiesOutputTypeDef],
@@ -9278,130 +7186,83 @@
         "Themes": Sequence[AssetBundleExportJobThemeOverridePropertiesTypeDef],
         "Analyses": Sequence[AssetBundleExportJobAnalysisOverridePropertiesTypeDef],
         "Dashboards": Sequence[AssetBundleExportJobDashboardOverridePropertiesTypeDef],
     },
     total=False,
 )
 
-AssetBundleImportJobDataSourceCredentialsOutputTypeDef = TypedDict(
-    "AssetBundleImportJobDataSourceCredentialsOutputTypeDef",
-    {
-        "CredentialPair": AssetBundleImportJobDataSourceCredentialPairOutputTypeDef,
-        "SecretArn": str,
-    },
-    total=False,
-)
-
 AssetBundleImportJobDataSourceCredentialsTypeDef = TypedDict(
     "AssetBundleImportJobDataSourceCredentialsTypeDef",
     {
         "CredentialPair": AssetBundleImportJobDataSourceCredentialPairTypeDef,
         "SecretArn": str,
     },
     total=False,
 )
 
 AxisDisplayRangeOutputTypeDef = TypedDict(
     "AxisDisplayRangeOutputTypeDef",
     {
-        "MinMax": AxisDisplayMinMaxRangeOutputTypeDef,
+        "MinMax": AxisDisplayMinMaxRangeTypeDef,
         "DataDriven": Dict[str, Any],
     },
     total=False,
 )
 
 AxisDisplayRangeTypeDef = TypedDict(
     "AxisDisplayRangeTypeDef",
     {
         "MinMax": AxisDisplayMinMaxRangeTypeDef,
         "DataDriven": Mapping[str, Any],
     },
     total=False,
 )
 
-AxisScaleOutputTypeDef = TypedDict(
-    "AxisScaleOutputTypeDef",
-    {
-        "Linear": AxisLinearScaleOutputTypeDef,
-        "Logarithmic": AxisLogarithmicScaleOutputTypeDef,
-    },
-    total=False,
-)
-
 AxisScaleTypeDef = TypedDict(
     "AxisScaleTypeDef",
     {
         "Linear": AxisLinearScaleTypeDef,
         "Logarithmic": AxisLogarithmicScaleTypeDef,
     },
     total=False,
 )
 
-HistogramBinOptionsOutputTypeDef = TypedDict(
-    "HistogramBinOptionsOutputTypeDef",
-    {
-        "SelectedBinType": HistogramBinTypeType,
-        "BinCount": BinCountOptionsOutputTypeDef,
-        "BinWidth": BinWidthOptionsOutputTypeDef,
-        "StartValue": float,
-    },
-    total=False,
-)
-
 HistogramBinOptionsTypeDef = TypedDict(
     "HistogramBinOptionsTypeDef",
     {
         "SelectedBinType": HistogramBinTypeType,
         "BinCount": BinCountOptionsTypeDef,
         "BinWidth": BinWidthOptionsTypeDef,
         "StartValue": float,
     },
     total=False,
 )
 
-TileStyleOutputTypeDef = TypedDict(
-    "TileStyleOutputTypeDef",
-    {
-        "Border": BorderStyleOutputTypeDef,
-    },
-    total=False,
-)
-
 TileStyleTypeDef = TypedDict(
     "TileStyleTypeDef",
     {
         "Border": BorderStyleTypeDef,
     },
     total=False,
 )
 
-BoxPlotOptionsOutputTypeDef = TypedDict(
-    "BoxPlotOptionsOutputTypeDef",
-    {
-        "StyleOptions": BoxPlotStyleOptionsOutputTypeDef,
-        "OutlierVisibility": VisibilityType,
-        "AllDataPointsVisibility": VisibilityType,
-    },
-    total=False,
-)
-
 BoxPlotOptionsTypeDef = TypedDict(
     "BoxPlotOptionsTypeDef",
     {
         "StyleOptions": BoxPlotStyleOptionsTypeDef,
         "OutlierVisibility": VisibilityType,
         "AllDataPointsVisibility": VisibilityType,
     },
     total=False,
 )
 
 CreateColumnsOperationOutputTypeDef = TypedDict(
     "CreateColumnsOperationOutputTypeDef",
     {
-        "Columns": List[CalculatedColumnOutputTypeDef],
+        "Columns": List[CalculatedColumnTypeDef],
     },
 )
 
 CreateColumnsOperationTypeDef = TypedDict(
     "CreateColumnsOperationTypeDef",
     {
         "Columns": Sequence[CalculatedColumnTypeDef],
@@ -9421,15 +7282,15 @@
 
 CreateAccountCustomizationResponseTypeDef = TypedDict(
     "CreateAccountCustomizationResponseTypeDef",
     {
         "Arn": str,
         "AwsAccountId": str,
         "Namespace": str,
-        "AccountCustomization": AccountCustomizationOutputTypeDef,
+        "AccountCustomization": AccountCustomizationTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAnalysisResponseTypeDef = TypedDict(
@@ -9849,15 +7710,15 @@
 
 DescribeAccountCustomizationResponseTypeDef = TypedDict(
     "DescribeAccountCustomizationResponseTypeDef",
     {
         "Arn": str,
         "AwsAccountId": str,
         "Namespace": str,
-        "AccountCustomization": AccountCustomizationOutputTypeDef,
+        "AccountCustomization": AccountCustomizationTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountSettingsResponseTypeDef = TypedDict(
@@ -10061,15 +7922,15 @@
 
 UpdateAccountCustomizationResponseTypeDef = TypedDict(
     "UpdateAccountCustomizationResponseTypeDef",
     {
         "Arn": str,
         "AwsAccountId": str,
         "Namespace": str,
-        "AccountCustomization": AccountCustomizationOutputTypeDef,
+        "AccountCustomization": AccountCustomizationTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountSettingsResponseTypeDef = TypedDict(
@@ -10283,37 +8144,29 @@
 )
 
 CategoryFilterConfigurationOutputTypeDef = TypedDict(
     "CategoryFilterConfigurationOutputTypeDef",
     {
         "FilterListConfiguration": FilterListConfigurationOutputTypeDef,
         "CustomFilterListConfiguration": CustomFilterListConfigurationOutputTypeDef,
-        "CustomFilterConfiguration": CustomFilterConfigurationOutputTypeDef,
+        "CustomFilterConfiguration": CustomFilterConfigurationTypeDef,
     },
     total=False,
 )
 
 CategoryFilterConfigurationTypeDef = TypedDict(
     "CategoryFilterConfigurationTypeDef",
     {
         "FilterListConfiguration": FilterListConfigurationTypeDef,
         "CustomFilterListConfiguration": CustomFilterListConfigurationTypeDef,
         "CustomFilterConfiguration": CustomFilterConfigurationTypeDef,
     },
     total=False,
 )
 
-ClusterMarkerOutputTypeDef = TypedDict(
-    "ClusterMarkerOutputTypeDef",
-    {
-        "SimpleClusterMarker": SimpleClusterMarkerOutputTypeDef,
-    },
-    total=False,
-)
-
 ClusterMarkerTypeDef = TypedDict(
     "ClusterMarkerTypeDef",
     {
         "SimpleClusterMarker": SimpleClusterMarkerTypeDef,
     },
     total=False,
 )
@@ -10337,22 +8190,22 @@
     },
     total=False,
 )
 
 _RequiredColorScaleOutputTypeDef = TypedDict(
     "_RequiredColorScaleOutputTypeDef",
     {
-        "Colors": List[DataColorOutputTypeDef],
+        "Colors": List[DataColorTypeDef],
         "ColorFillType": ColorFillTypeType,
     },
 )
 _OptionalColorScaleOutputTypeDef = TypedDict(
     "_OptionalColorScaleOutputTypeDef",
     {
-        "NullValueColor": DataColorOutputTypeDef,
+        "NullValueColor": DataColorTypeDef,
     },
     total=False,
 )
 
 
 class ColorScaleOutputTypeDef(_RequiredColorScaleOutputTypeDef, _OptionalColorScaleOutputTypeDef):
     pass
@@ -10377,50 +8230,41 @@
 class ColorScaleTypeDef(_RequiredColorScaleTypeDef, _OptionalColorScaleTypeDef):
     pass
 
 
 ColorsConfigurationOutputTypeDef = TypedDict(
     "ColorsConfigurationOutputTypeDef",
     {
-        "CustomColors": List[CustomColorOutputTypeDef],
+        "CustomColors": List[CustomColorTypeDef],
     },
     total=False,
 )
 
 ColorsConfigurationTypeDef = TypedDict(
     "ColorsConfigurationTypeDef",
     {
         "CustomColors": Sequence[CustomColorTypeDef],
     },
     total=False,
 )
 
-ColumnTagOutputTypeDef = TypedDict(
-    "ColumnTagOutputTypeDef",
-    {
-        "ColumnGeographicRole": GeoSpatialDataRoleType,
-        "ColumnDescription": ColumnDescriptionOutputTypeDef,
-    },
-    total=False,
-)
-
 ColumnTagTypeDef = TypedDict(
     "ColumnTagTypeDef",
     {
         "ColumnGeographicRole": GeoSpatialDataRoleType,
         "ColumnDescription": ColumnDescriptionTypeDef,
     },
     total=False,
 )
 
 ColumnGroupSchemaOutputTypeDef = TypedDict(
     "ColumnGroupSchemaOutputTypeDef",
     {
         "Name": str,
-        "ColumnGroupColumnSchemaList": List[ColumnGroupColumnSchemaOutputTypeDef],
+        "ColumnGroupColumnSchemaList": List[ColumnGroupColumnSchemaTypeDef],
     },
     total=False,
 )
 
 ColumnGroupSchemaTypeDef = TypedDict(
     "ColumnGroupSchemaTypeDef",
     {
@@ -10445,51 +8289,27 @@
     },
     total=False,
 )
 
 DataSetSchemaOutputTypeDef = TypedDict(
     "DataSetSchemaOutputTypeDef",
     {
-        "ColumnSchemaList": List[ColumnSchemaOutputTypeDef],
+        "ColumnSchemaList": List[ColumnSchemaTypeDef],
     },
     total=False,
 )
 
 DataSetSchemaTypeDef = TypedDict(
     "DataSetSchemaTypeDef",
     {
         "ColumnSchemaList": Sequence[ColumnSchemaTypeDef],
     },
     total=False,
 )
 
-_RequiredConditionalFormattingCustomIconConditionOutputTypeDef = TypedDict(
-    "_RequiredConditionalFormattingCustomIconConditionOutputTypeDef",
-    {
-        "Expression": str,
-        "IconOptions": ConditionalFormattingCustomIconOptionsOutputTypeDef,
-    },
-)
-_OptionalConditionalFormattingCustomIconConditionOutputTypeDef = TypedDict(
-    "_OptionalConditionalFormattingCustomIconConditionOutputTypeDef",
-    {
-        "Color": str,
-        "DisplayConfiguration": ConditionalFormattingIconDisplayConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ConditionalFormattingCustomIconConditionOutputTypeDef(
-    _RequiredConditionalFormattingCustomIconConditionOutputTypeDef,
-    _OptionalConditionalFormattingCustomIconConditionOutputTypeDef,
-):
-    pass
-
-
 _RequiredConditionalFormattingCustomIconConditionTypeDef = TypedDict(
     "_RequiredConditionalFormattingCustomIconConditionTypeDef",
     {
         "Expression": str,
         "IconOptions": ConditionalFormattingCustomIconOptionsTypeDef,
     },
 )
@@ -10581,14 +8401,24 @@
 class CreateVPCConnectionRequestRequestTypeDef(
     _RequiredCreateVPCConnectionRequestRequestTypeDef,
     _OptionalCreateVPCConnectionRequestRequestTypeDef,
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "RequestId": str,
+        "Status": int,
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
@@ -10819,14 +8649,30 @@
 class UpdateTopicPermissionsRequestRequestTypeDef(
     _RequiredUpdateTopicPermissionsRequestRequestTypeDef,
     _OptionalUpdateTopicPermissionsRequestRequestTypeDef,
 ):
     pass
 
 
+DataSetSummaryTypeDef = TypedDict(
+    "DataSetSummaryTypeDef",
+    {
+        "Arn": str,
+        "DataSetId": str,
+        "Name": str,
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "ImportMode": DataSetImportModeType,
+        "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
+        "RowLevelPermissionTagConfigurationApplied": bool,
+        "ColumnLevelPermissionRulesApplied": bool,
+    },
+    total=False,
+)
+
 CreateFolderMembershipResponseTypeDef = TypedDict(
     "CreateFolderMembershipResponseTypeDef",
     {
         "Status": int,
         "FolderMember": FolderMemberTypeDef,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -11040,22 +8886,14 @@
         "AwsAccountId": str,
         "TopicId": str,
         "DatasetId": str,
         "RefreshSchedule": TopicRefreshScheduleTypeDef,
     },
 )
 
-CustomActionNavigationOperationOutputTypeDef = TypedDict(
-    "CustomActionNavigationOperationOutputTypeDef",
-    {
-        "LocalNavigationConfiguration": LocalNavigationConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 CustomActionNavigationOperationTypeDef = TypedDict(
     "CustomActionNavigationOperationTypeDef",
     {
         "LocalNavigationConfiguration": LocalNavigationConfigurationTypeDef,
     },
     total=False,
 )
@@ -11109,66 +8947,66 @@
         "Name": str,
         "SqlQuery": str,
     },
 )
 _OptionalCustomSqlOutputTypeDef = TypedDict(
     "_OptionalCustomSqlOutputTypeDef",
     {
-        "Columns": List[InputColumnOutputTypeDef],
+        "Columns": List[InputColumnTypeDef],
     },
     total=False,
 )
 
 
 class CustomSqlOutputTypeDef(_RequiredCustomSqlOutputTypeDef, _OptionalCustomSqlOutputTypeDef):
     pass
 
 
-_RequiredRelationalTableOutputTypeDef = TypedDict(
-    "_RequiredRelationalTableOutputTypeDef",
+_RequiredCustomSqlTypeDef = TypedDict(
+    "_RequiredCustomSqlTypeDef",
     {
         "DataSourceArn": str,
         "Name": str,
-        "InputColumns": List[InputColumnOutputTypeDef],
+        "SqlQuery": str,
     },
 )
-_OptionalRelationalTableOutputTypeDef = TypedDict(
-    "_OptionalRelationalTableOutputTypeDef",
+_OptionalCustomSqlTypeDef = TypedDict(
+    "_OptionalCustomSqlTypeDef",
     {
-        "Catalog": str,
-        "Schema": str,
+        "Columns": Sequence[InputColumnTypeDef],
     },
     total=False,
 )
 
 
-class RelationalTableOutputTypeDef(
-    _RequiredRelationalTableOutputTypeDef, _OptionalRelationalTableOutputTypeDef
-):
+class CustomSqlTypeDef(_RequiredCustomSqlTypeDef, _OptionalCustomSqlTypeDef):
     pass
 
 
-_RequiredCustomSqlTypeDef = TypedDict(
-    "_RequiredCustomSqlTypeDef",
+_RequiredRelationalTableOutputTypeDef = TypedDict(
+    "_RequiredRelationalTableOutputTypeDef",
     {
         "DataSourceArn": str,
         "Name": str,
-        "SqlQuery": str,
+        "InputColumns": List[InputColumnTypeDef],
     },
 )
-_OptionalCustomSqlTypeDef = TypedDict(
-    "_OptionalCustomSqlTypeDef",
+_OptionalRelationalTableOutputTypeDef = TypedDict(
+    "_OptionalRelationalTableOutputTypeDef",
     {
-        "Columns": Sequence[InputColumnTypeDef],
+        "Catalog": str,
+        "Schema": str,
     },
     total=False,
 )
 
 
-class CustomSqlTypeDef(_RequiredCustomSqlTypeDef, _OptionalCustomSqlTypeDef):
+class RelationalTableOutputTypeDef(
+    _RequiredRelationalTableOutputTypeDef, _OptionalRelationalTableOutputTypeDef
+):
     pass
 
 
 _RequiredRelationalTableTypeDef = TypedDict(
     "_RequiredRelationalTableTypeDef",
     {
         "DataSourceArn": str,
@@ -11242,104 +9080,82 @@
         "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DashboardVisualPublishOptionsOutputTypeDef = TypedDict(
-    "DashboardVisualPublishOptionsOutputTypeDef",
-    {
-        "ExportHiddenFieldsOption": ExportHiddenFieldsOptionOutputTypeDef,
-    },
-    total=False,
-)
-
 DashboardVisualPublishOptionsTypeDef = TypedDict(
     "DashboardVisualPublishOptionsTypeDef",
     {
         "ExportHiddenFieldsOption": ExportHiddenFieldsOptionTypeDef,
     },
     total=False,
 )
 
-TableInlineVisualizationOutputTypeDef = TypedDict(
-    "TableInlineVisualizationOutputTypeDef",
-    {
-        "DataBars": DataBarsOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 TableInlineVisualizationTypeDef = TypedDict(
     "TableInlineVisualizationTypeDef",
     {
         "DataBars": DataBarsOptionsTypeDef,
     },
     total=False,
 )
 
-DataLabelTypeOutputTypeDef = TypedDict(
-    "DataLabelTypeOutputTypeDef",
-    {
-        "FieldLabelType": FieldLabelTypeOutputTypeDef,
-        "DataPathLabelType": DataPathLabelTypeOutputTypeDef,
-        "RangeEndsLabelType": RangeEndsLabelTypeOutputTypeDef,
-        "MinimumLabelType": MinimumLabelTypeOutputTypeDef,
-        "MaximumLabelType": MaximumLabelTypeOutputTypeDef,
-    },
-    total=False,
-)
-
 DataLabelTypeTypeDef = TypedDict(
     "DataLabelTypeTypeDef",
     {
         "FieldLabelType": FieldLabelTypeTypeDef,
         "DataPathLabelType": DataPathLabelTypeTypeDef,
         "RangeEndsLabelType": RangeEndsLabelTypeTypeDef,
         "MinimumLabelType": MinimumLabelTypeTypeDef,
         "MaximumLabelType": MaximumLabelTypeTypeDef,
     },
     total=False,
 )
 
-_RequiredDataPathColorOutputTypeDef = TypedDict(
-    "_RequiredDataPathColorOutputTypeDef",
+_RequiredDataPathColorTypeDef = TypedDict(
+    "_RequiredDataPathColorTypeDef",
     {
-        "Element": DataPathValueOutputTypeDef,
+        "Element": DataPathValueTypeDef,
         "Color": str,
     },
 )
-_OptionalDataPathColorOutputTypeDef = TypedDict(
-    "_OptionalDataPathColorOutputTypeDef",
+_OptionalDataPathColorTypeDef = TypedDict(
+    "_OptionalDataPathColorTypeDef",
     {
         "TimeGranularity": TimeGranularityType,
     },
     total=False,
 )
 
 
-class DataPathColorOutputTypeDef(
-    _RequiredDataPathColorOutputTypeDef, _OptionalDataPathColorOutputTypeDef
-):
+class DataPathColorTypeDef(_RequiredDataPathColorTypeDef, _OptionalDataPathColorTypeDef):
     pass
 
 
 DataPathSortOutputTypeDef = TypedDict(
     "DataPathSortOutputTypeDef",
     {
         "Direction": SortDirectionType,
-        "SortPaths": List[DataPathValueOutputTypeDef],
+        "SortPaths": List[DataPathValueTypeDef],
+    },
+)
+
+DataPathSortTypeDef = TypedDict(
+    "DataPathSortTypeDef",
+    {
+        "Direction": SortDirectionType,
+        "SortPaths": Sequence[DataPathValueTypeDef],
     },
 )
 
 _RequiredPivotTableDataPathOptionOutputTypeDef = TypedDict(
     "_RequiredPivotTableDataPathOptionOutputTypeDef",
     {
-        "DataPathList": List[DataPathValueOutputTypeDef],
+        "DataPathList": List[DataPathValueTypeDef],
     },
 )
 _OptionalPivotTableDataPathOptionOutputTypeDef = TypedDict(
     "_OptionalPivotTableDataPathOptionOutputTypeDef",
     {
         "Width": str,
     },
@@ -11349,51 +9165,14 @@
 
 class PivotTableDataPathOptionOutputTypeDef(
     _RequiredPivotTableDataPathOptionOutputTypeDef, _OptionalPivotTableDataPathOptionOutputTypeDef
 ):
     pass
 
 
-PivotTableFieldCollapseStateTargetOutputTypeDef = TypedDict(
-    "PivotTableFieldCollapseStateTargetOutputTypeDef",
-    {
-        "FieldId": str,
-        "FieldDataPathValues": List[DataPathValueOutputTypeDef],
-    },
-    total=False,
-)
-
-_RequiredDataPathColorTypeDef = TypedDict(
-    "_RequiredDataPathColorTypeDef",
-    {
-        "Element": DataPathValueTypeDef,
-        "Color": str,
-    },
-)
-_OptionalDataPathColorTypeDef = TypedDict(
-    "_OptionalDataPathColorTypeDef",
-    {
-        "TimeGranularity": TimeGranularityType,
-    },
-    total=False,
-)
-
-
-class DataPathColorTypeDef(_RequiredDataPathColorTypeDef, _OptionalDataPathColorTypeDef):
-    pass
-
-
-DataPathSortTypeDef = TypedDict(
-    "DataPathSortTypeDef",
-    {
-        "Direction": SortDirectionType,
-        "SortPaths": Sequence[DataPathValueTypeDef],
-    },
-)
-
 _RequiredPivotTableDataPathOptionTypeDef = TypedDict(
     "_RequiredPivotTableDataPathOptionTypeDef",
     {
         "DataPathList": Sequence[DataPathValueTypeDef],
     },
 )
 _OptionalPivotTableDataPathOptionTypeDef = TypedDict(
@@ -11407,14 +9186,23 @@
 
 class PivotTableDataPathOptionTypeDef(
     _RequiredPivotTableDataPathOptionTypeDef, _OptionalPivotTableDataPathOptionTypeDef
 ):
     pass
 
 
+PivotTableFieldCollapseStateTargetOutputTypeDef = TypedDict(
+    "PivotTableFieldCollapseStateTargetOutputTypeDef",
+    {
+        "FieldId": str,
+        "FieldDataPathValues": List[DataPathValueTypeDef],
+    },
+    total=False,
+)
+
 PivotTableFieldCollapseStateTargetTypeDef = TypedDict(
     "PivotTableFieldCollapseStateTargetTypeDef",
     {
         "FieldId": str,
         "FieldDataPathValues": Sequence[DataPathValueTypeDef],
     },
     total=False,
@@ -11439,30 +9227,14 @@
 
 class SearchDataSetsRequestRequestTypeDef(
     _RequiredSearchDataSetsRequestRequestTypeDef, _OptionalSearchDataSetsRequestRequestTypeDef
 ):
     pass
 
 
-DataSetSummaryTypeDef = TypedDict(
-    "DataSetSummaryTypeDef",
-    {
-        "Arn": str,
-        "DataSetId": str,
-        "Name": str,
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "ImportMode": DataSetImportModeType,
-        "RowLevelPermissionDataSet": RowLevelPermissionDataSetOutputTypeDef,
-        "RowLevelPermissionTagConfigurationApplied": bool,
-        "ColumnLevelPermissionRulesApplied": bool,
-    },
-    total=False,
-)
-
 _RequiredSearchDataSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchDataSourcesRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "Filters": Sequence[DataSourceSearchFilterTypeDef],
     },
 )
@@ -11541,15 +9313,15 @@
     pass
 
 
 TimeRangeFilterValueOutputTypeDef = TypedDict(
     "TimeRangeFilterValueOutputTypeDef",
     {
         "StaticValue": datetime,
-        "RollingDate": RollingDateConfigurationOutputTypeDef,
+        "RollingDate": RollingDateConfigurationTypeDef,
         "Parameter": str,
     },
     total=False,
 )
 
 TimeRangeFilterValueTypeDef = TypedDict(
     "TimeRangeFilterValueTypeDef",
@@ -11863,33 +9635,14 @@
         "User": UserTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisplayFormatOptionsOutputTypeDef = TypedDict(
-    "DisplayFormatOptionsOutputTypeDef",
-    {
-        "UseBlankCellFormat": bool,
-        "BlankCellFormat": str,
-        "DateFormat": str,
-        "DecimalSeparator": TopicNumericSeparatorSymbolType,
-        "GroupingSeparator": str,
-        "UseGrouping": bool,
-        "FractionDigits": int,
-        "Prefix": str,
-        "Suffix": str,
-        "UnitScaler": NumberScaleType,
-        "NegativeFormat": NegativeFormatOutputTypeDef,
-        "CurrencySymbol": str,
-    },
-    total=False,
-)
-
 DisplayFormatOptionsTypeDef = TypedDict(
     "DisplayFormatOptionsTypeDef",
     {
         "UseBlankCellFormat": bool,
         "BlankCellFormat": str,
         "DateFormat": str,
         "DecimalSeparator": TopicNumericSeparatorSymbolType,
@@ -11901,61 +9654,23 @@
         "UnitScaler": NumberScaleType,
         "NegativeFormat": NegativeFormatTypeDef,
         "CurrencySymbol": str,
     },
     total=False,
 )
 
-DonutOptionsOutputTypeDef = TypedDict(
-    "DonutOptionsOutputTypeDef",
-    {
-        "ArcOptions": ArcOptionsOutputTypeDef,
-        "DonutCenterOptions": DonutCenterOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 DonutOptionsTypeDef = TypedDict(
     "DonutOptionsTypeDef",
     {
         "ArcOptions": ArcOptionsTypeDef,
         "DonutCenterOptions": DonutCenterOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredRelativeDatesFilterOutputTypeDef = TypedDict(
-    "_RequiredRelativeDatesFilterOutputTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-        "AnchorDateConfiguration": AnchorDateConfigurationOutputTypeDef,
-        "TimeGranularity": TimeGranularityType,
-        "RelativeDateType": RelativeDateTypeType,
-        "NullOption": FilterNullOptionType,
-    },
-)
-_OptionalRelativeDatesFilterOutputTypeDef = TypedDict(
-    "_OptionalRelativeDatesFilterOutputTypeDef",
-    {
-        "MinimumGranularity": TimeGranularityType,
-        "RelativeDateValue": int,
-        "ParameterName": str,
-        "ExcludePeriodConfiguration": ExcludePeriodConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class RelativeDatesFilterOutputTypeDef(
-    _RequiredRelativeDatesFilterOutputTypeDef, _OptionalRelativeDatesFilterOutputTypeDef
-):
-    pass
-
-
 _RequiredRelativeDatesFilterTypeDef = TypedDict(
     "_RequiredRelativeDatesFilterTypeDef",
     {
         "FilterId": str,
         "Column": ColumnIdentifierTypeDef,
         "AnchorDateConfiguration": AnchorDateConfigurationTypeDef,
         "TimeGranularity": TimeGranularityType,
@@ -12038,26 +9753,14 @@
         "FolderSummaryList": List[FolderSummaryTypeDef],
         "NextToken": str,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FontConfigurationOutputTypeDef = TypedDict(
-    "FontConfigurationOutputTypeDef",
-    {
-        "FontSize": FontSizeOutputTypeDef,
-        "FontDecoration": FontDecorationType,
-        "FontColor": str,
-        "FontWeight": FontWeightOutputTypeDef,
-        "FontStyle": FontStyleType,
-    },
-    total=False,
-)
-
 FontConfigurationTypeDef = TypedDict(
     "FontConfigurationTypeDef",
     {
         "FontSize": FontSizeTypeDef,
         "FontDecoration": FontDecorationType,
         "FontColor": str,
         "FontWeight": FontWeightTypeDef,
@@ -12065,15 +9768,15 @@
     },
     total=False,
 )
 
 TypographyOutputTypeDef = TypedDict(
     "TypographyOutputTypeDef",
     {
-        "FontFamilies": List[FontOutputTypeDef],
+        "FontFamilies": List[FontTypeDef],
     },
     total=False,
 )
 
 TypographyTypeDef = TypedDict(
     "TypographyTypeDef",
     {
@@ -12096,22 +9799,14 @@
     {
         "WhatIfPointScenario": WhatIfPointScenarioTypeDef,
         "WhatIfRangeScenario": WhatIfRangeScenarioTypeDef,
     },
     total=False,
 )
 
-FreeFormLayoutCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "FreeFormLayoutCanvasSizeOptionsOutputTypeDef",
-    {
-        "ScreenCanvasSizeOptions": FreeFormLayoutScreenCanvasSizeOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 FreeFormLayoutCanvasSizeOptionsTypeDef = TypedDict(
     "FreeFormLayoutCanvasSizeOptionsTypeDef",
     {
         "ScreenCanvasSizeOptions": FreeFormLayoutScreenCanvasSizeOptionsTypeDef,
     },
     total=False,
 )
@@ -12120,61 +9815,39 @@
     "SnapshotAnonymousUserTypeDef",
     {
         "RowLevelPermissionTags": Sequence[SessionTagTypeDef],
     },
     total=False,
 )
 
-GeospatialWindowOptionsOutputTypeDef = TypedDict(
-    "GeospatialWindowOptionsOutputTypeDef",
-    {
-        "Bounds": GeospatialCoordinateBoundsOutputTypeDef,
-        "MapZoomMode": MapZoomModeType,
-    },
-    total=False,
-)
-
 GeospatialWindowOptionsTypeDef = TypedDict(
     "GeospatialWindowOptionsTypeDef",
     {
         "Bounds": GeospatialCoordinateBoundsTypeDef,
         "MapZoomMode": MapZoomModeType,
     },
     total=False,
 )
 
 GeospatialHeatmapColorScaleOutputTypeDef = TypedDict(
     "GeospatialHeatmapColorScaleOutputTypeDef",
     {
-        "Colors": List[GeospatialHeatmapDataColorOutputTypeDef],
+        "Colors": List[GeospatialHeatmapDataColorTypeDef],
     },
     total=False,
 )
 
 GeospatialHeatmapColorScaleTypeDef = TypedDict(
     "GeospatialHeatmapColorScaleTypeDef",
     {
         "Colors": Sequence[GeospatialHeatmapDataColorTypeDef],
     },
     total=False,
 )
 
-TableSideBorderOptionsOutputTypeDef = TypedDict(
-    "TableSideBorderOptionsOutputTypeDef",
-    {
-        "InnerVertical": TableBorderOptionsOutputTypeDef,
-        "InnerHorizontal": TableBorderOptionsOutputTypeDef,
-        "Left": TableBorderOptionsOutputTypeDef,
-        "Right": TableBorderOptionsOutputTypeDef,
-        "Top": TableBorderOptionsOutputTypeDef,
-        "Bottom": TableBorderOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 TableSideBorderOptionsTypeDef = TypedDict(
     "TableSideBorderOptionsTypeDef",
     {
         "InnerVertical": TableBorderOptionsTypeDef,
         "InnerHorizontal": TableBorderOptionsTypeDef,
         "Left": TableBorderOptionsTypeDef,
         "Right": TableBorderOptionsTypeDef,
@@ -12183,35 +9856,27 @@
     },
     total=False,
 )
 
 GradientColorOutputTypeDef = TypedDict(
     "GradientColorOutputTypeDef",
     {
-        "Stops": List[GradientStopOutputTypeDef],
+        "Stops": List[GradientStopTypeDef],
     },
     total=False,
 )
 
 GradientColorTypeDef = TypedDict(
     "GradientColorTypeDef",
     {
         "Stops": Sequence[GradientStopTypeDef],
     },
     total=False,
 )
 
-GridLayoutCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "GridLayoutCanvasSizeOptionsOutputTypeDef",
-    {
-        "ScreenCanvasSizeOptions": GridLayoutScreenCanvasSizeOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 GridLayoutCanvasSizeOptionsTypeDef = TypedDict(
     "GridLayoutCanvasSizeOptionsTypeDef",
     {
         "ScreenCanvasSizeOptions": GridLayoutScreenCanvasSizeOptionsTypeDef,
     },
     total=False,
 )
@@ -12247,21 +9912,14 @@
         "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IncrementalRefreshOutputTypeDef = TypedDict(
-    "IncrementalRefreshOutputTypeDef",
-    {
-        "LookbackWindow": LookbackWindowOutputTypeDef,
-    },
-)
-
 IncrementalRefreshTypeDef = TypedDict(
     "IncrementalRefreshTypeDef",
     {
         "LookbackWindow": LookbackWindowTypeDef,
     },
 )
 
@@ -12335,39 +9993,14 @@
 
 class IntegerDatasetParameterTypeDef(
     _RequiredIntegerDatasetParameterTypeDef, _OptionalIntegerDatasetParameterTypeDef
 ):
     pass
 
 
-_RequiredJoinInstructionOutputTypeDef = TypedDict(
-    "_RequiredJoinInstructionOutputTypeDef",
-    {
-        "LeftOperand": str,
-        "RightOperand": str,
-        "Type": JoinTypeType,
-        "OnClause": str,
-    },
-)
-_OptionalJoinInstructionOutputTypeDef = TypedDict(
-    "_OptionalJoinInstructionOutputTypeDef",
-    {
-        "LeftJoinKeyProperties": JoinKeyPropertiesOutputTypeDef,
-        "RightJoinKeyProperties": JoinKeyPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class JoinInstructionOutputTypeDef(
-    _RequiredJoinInstructionOutputTypeDef, _OptionalJoinInstructionOutputTypeDef
-):
-    pass
-
-
 _RequiredJoinInstructionTypeDef = TypedDict(
     "_RequiredJoinInstructionTypeDef",
     {
         "LeftOperand": str,
         "RightOperand": str,
         "Type": JoinTypeType,
         "OnClause": str,
@@ -12383,33 +10016,14 @@
 )
 
 
 class JoinInstructionTypeDef(_RequiredJoinInstructionTypeDef, _OptionalJoinInstructionTypeDef):
     pass
 
 
-LineChartDefaultSeriesSettingsOutputTypeDef = TypedDict(
-    "LineChartDefaultSeriesSettingsOutputTypeDef",
-    {
-        "AxisBinding": AxisBindingType,
-        "LineStyleSettings": LineChartLineStyleSettingsOutputTypeDef,
-        "MarkerStyleSettings": LineChartMarkerStyleSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-LineChartSeriesSettingsOutputTypeDef = TypedDict(
-    "LineChartSeriesSettingsOutputTypeDef",
-    {
-        "LineStyleSettings": LineChartLineStyleSettingsOutputTypeDef,
-        "MarkerStyleSettings": LineChartMarkerStyleSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 LineChartDefaultSeriesSettingsTypeDef = TypedDict(
     "LineChartDefaultSeriesSettingsTypeDef",
     {
         "AxisBinding": AxisBindingType,
         "LineStyleSettings": LineChartLineStyleSettingsTypeDef,
         "MarkerStyleSettings": LineChartMarkerStyleSettingsTypeDef,
     },
@@ -13004,24 +10618,14 @@
         "FolderMemberList": List[MemberIdArnPairTypeDef],
         "NextToken": str,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTemplateVersionsResponseTypeDef = TypedDict(
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionSummaryList": List[TemplateVersionSummaryTypeDef],
         "NextToken": str,
         "Status": int,
         "RequestId": str,
@@ -13069,53 +10673,23 @@
         "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VisualSubtitleLabelOptionsOutputTypeDef = TypedDict(
-    "VisualSubtitleLabelOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "FormatText": LongFormatTextOutputTypeDef,
-    },
-    total=False,
-)
-
 VisualSubtitleLabelOptionsTypeDef = TypedDict(
     "VisualSubtitleLabelOptionsTypeDef",
     {
         "Visibility": VisibilityType,
         "FormatText": LongFormatTextTypeDef,
     },
     total=False,
 )
 
-_RequiredS3ParametersOutputTypeDef = TypedDict(
-    "_RequiredS3ParametersOutputTypeDef",
-    {
-        "ManifestFileLocation": ManifestFileLocationOutputTypeDef,
-    },
-)
-_OptionalS3ParametersOutputTypeDef = TypedDict(
-    "_OptionalS3ParametersOutputTypeDef",
-    {
-        "RoleArn": str,
-    },
-    total=False,
-)
-
-
-class S3ParametersOutputTypeDef(
-    _RequiredS3ParametersOutputTypeDef, _OptionalS3ParametersOutputTypeDef
-):
-    pass
-
-
 _RequiredS3ParametersTypeDef = TypedDict(
     "_RequiredS3ParametersTypeDef",
     {
         "ManifestFileLocation": ManifestFileLocationTypeDef,
     },
 )
 _OptionalS3ParametersTypeDef = TypedDict(
@@ -13127,23 +10701,14 @@
 )
 
 
 class S3ParametersTypeDef(_RequiredS3ParametersTypeDef, _OptionalS3ParametersTypeDef):
     pass
 
 
-TileLayoutStyleOutputTypeDef = TypedDict(
-    "TileLayoutStyleOutputTypeDef",
-    {
-        "Gutter": GutterStyleOutputTypeDef,
-        "Margin": MarginStyleOutputTypeDef,
-    },
-    total=False,
-)
-
 TileLayoutStyleTypeDef = TypedDict(
     "TileLayoutStyleTypeDef",
     {
         "Gutter": GutterStyleTypeDef,
         "Margin": MarginStyleTypeDef,
     },
     total=False,
@@ -13266,41 +10831,23 @@
 class OverrideDatasetParameterOperationTypeDef(
     _RequiredOverrideDatasetParameterOperationTypeDef,
     _OptionalOverrideDatasetParameterOperationTypeDef,
 ):
     pass
 
 
-NumericSeparatorConfigurationOutputTypeDef = TypedDict(
-    "NumericSeparatorConfigurationOutputTypeDef",
-    {
-        "DecimalSeparator": NumericSeparatorSymbolType,
-        "ThousandsSeparator": ThousandSeparatorOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 NumericSeparatorConfigurationTypeDef = TypedDict(
     "NumericSeparatorConfigurationTypeDef",
     {
         "DecimalSeparator": NumericSeparatorSymbolType,
         "ThousandsSeparator": ThousandSeparatorOptionsTypeDef,
     },
     total=False,
 )
 
-NumericalAggregationFunctionOutputTypeDef = TypedDict(
-    "NumericalAggregationFunctionOutputTypeDef",
-    {
-        "SimpleNumericalAggregation": SimpleNumericalAggregationFunctionType,
-        "PercentileAggregation": PercentileAggregationOutputTypeDef,
-    },
-    total=False,
-)
-
 NumericalAggregationFunctionTypeDef = TypedDict(
     "NumericalAggregationFunctionTypeDef",
     {
         "SimpleNumericalAggregation": SimpleNumericalAggregationFunctionType,
         "PercentileAggregation": PercentileAggregationTypeDef,
     },
     total=False,
@@ -13324,87 +10871,39 @@
         "IntegerParameters": Sequence[IntegerParameterTypeDef],
         "DecimalParameters": Sequence[DecimalParameterTypeDef],
         "DateTimeParameters": Sequence[DateTimeParameterTypeDef],
     },
     total=False,
 )
 
-VisibleRangeOptionsOutputTypeDef = TypedDict(
-    "VisibleRangeOptionsOutputTypeDef",
-    {
-        "PercentRange": PercentVisibleRangeOutputTypeDef,
-    },
-    total=False,
-)
-
 VisibleRangeOptionsTypeDef = TypedDict(
     "VisibleRangeOptionsTypeDef",
     {
         "PercentRange": PercentVisibleRangeTypeDef,
     },
     total=False,
 )
 
-RadarChartSeriesSettingsOutputTypeDef = TypedDict(
-    "RadarChartSeriesSettingsOutputTypeDef",
-    {
-        "AreaStyleSettings": RadarChartAreaStyleSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 RadarChartSeriesSettingsTypeDef = TypedDict(
     "RadarChartSeriesSettingsTypeDef",
     {
         "AreaStyleSettings": RadarChartAreaStyleSettingsTypeDef,
     },
     total=False,
 )
 
-TopicRangeFilterConstantOutputTypeDef = TypedDict(
-    "TopicRangeFilterConstantOutputTypeDef",
-    {
-        "ConstantType": ConstantTypeType,
-        "RangeConstant": RangeConstantOutputTypeDef,
-    },
-    total=False,
-)
-
 TopicRangeFilterConstantTypeDef = TypedDict(
     "TopicRangeFilterConstantTypeDef",
     {
         "ConstantType": ConstantTypeType,
         "RangeConstant": RangeConstantTypeDef,
     },
     total=False,
 )
 
-_RequiredRefreshFrequencyOutputTypeDef = TypedDict(
-    "_RequiredRefreshFrequencyOutputTypeDef",
-    {
-        "Interval": RefreshIntervalType,
-    },
-)
-_OptionalRefreshFrequencyOutputTypeDef = TypedDict(
-    "_OptionalRefreshFrequencyOutputTypeDef",
-    {
-        "RefreshOnDay": ScheduleRefreshOnEntityOutputTypeDef,
-        "Timezone": str,
-        "TimeOfTheDay": str,
-    },
-    total=False,
-)
-
-
-class RefreshFrequencyOutputTypeDef(
-    _RequiredRefreshFrequencyOutputTypeDef, _OptionalRefreshFrequencyOutputTypeDef
-):
-    pass
-
-
 _RequiredRefreshFrequencyTypeDef = TypedDict(
     "_RequiredRefreshFrequencyTypeDef",
     {
         "Interval": RefreshIntervalType,
     },
 )
 _OptionalRefreshFrequencyTypeDef = TypedDict(
@@ -13438,15 +10937,15 @@
     },
     total=False,
 )
 
 _RequiredRowLevelPermissionTagConfigurationOutputTypeDef = TypedDict(
     "_RequiredRowLevelPermissionTagConfigurationOutputTypeDef",
     {
-        "TagRules": List[RowLevelPermissionTagRuleOutputTypeDef],
+        "TagRules": List[RowLevelPermissionTagRuleTypeDef],
     },
 )
 _OptionalRowLevelPermissionTagConfigurationOutputTypeDef = TypedDict(
     "_OptionalRowLevelPermissionTagConfigurationOutputTypeDef",
     {
         "Status": StatusType,
         "TagRuleConfigurations": List[List[str]],
@@ -13481,41 +10980,33 @@
 class RowLevelPermissionTagConfigurationTypeDef(
     _RequiredRowLevelPermissionTagConfigurationTypeDef,
     _OptionalRowLevelPermissionTagConfigurationTypeDef,
 ):
     pass
 
 
-SnapshotS3DestinationConfigurationOutputTypeDef = TypedDict(
-    "SnapshotS3DestinationConfigurationOutputTypeDef",
-    {
-        "BucketConfiguration": S3BucketConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 SnapshotS3DestinationConfigurationTypeDef = TypedDict(
     "SnapshotS3DestinationConfigurationTypeDef",
     {
         "BucketConfiguration": S3BucketConfigurationTypeDef,
     },
     total=False,
 )
 
 _RequiredS3SourceOutputTypeDef = TypedDict(
     "_RequiredS3SourceOutputTypeDef",
     {
         "DataSourceArn": str,
-        "InputColumns": List[InputColumnOutputTypeDef],
+        "InputColumns": List[InputColumnTypeDef],
     },
 )
 _OptionalS3SourceOutputTypeDef = TypedDict(
     "_OptionalS3SourceOutputTypeDef",
     {
-        "UploadSettings": UploadSettingsOutputTypeDef,
+        "UploadSettings": UploadSettingsTypeDef,
     },
     total=False,
 )
 
 
 class S3SourceOutputTypeDef(_RequiredS3SourceOutputTypeDef, _OptionalS3SourceOutputTypeDef):
     pass
@@ -13537,49 +11028,22 @@
 )
 
 
 class S3SourceTypeDef(_RequiredS3SourceTypeDef, _OptionalS3SourceTypeDef):
     pass
 
 
-SectionPageBreakConfigurationOutputTypeDef = TypedDict(
-    "SectionPageBreakConfigurationOutputTypeDef",
-    {
-        "After": SectionAfterPageBreakOutputTypeDef,
-    },
-    total=False,
-)
-
 SectionPageBreakConfigurationTypeDef = TypedDict(
     "SectionPageBreakConfigurationTypeDef",
     {
         "After": SectionAfterPageBreakTypeDef,
     },
     total=False,
 )
 
-SectionBasedLayoutPaperCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "SectionBasedLayoutPaperCanvasSizeOptionsOutputTypeDef",
-    {
-        "PaperSize": PaperSizeType,
-        "PaperOrientation": PaperOrientationType,
-        "PaperMargin": SpacingOutputTypeDef,
-    },
-    total=False,
-)
-
-SectionStyleOutputTypeDef = TypedDict(
-    "SectionStyleOutputTypeDef",
-    {
-        "Height": str,
-        "Padding": SpacingOutputTypeDef,
-    },
-    total=False,
-)
-
 SectionBasedLayoutPaperCanvasSizeOptionsTypeDef = TypedDict(
     "SectionBasedLayoutPaperCanvasSizeOptionsTypeDef",
     {
         "PaperSize": PaperSizeType,
         "PaperOrientation": PaperOrientationType,
         "PaperMargin": SpacingTypeDef,
     },
@@ -13607,39 +11071,22 @@
     "SelectedSheetsFilterScopeConfigurationTypeDef",
     {
         "SheetVisualScopingConfigurations": Sequence[SheetVisualScopingConfigurationTypeDef],
     },
     total=False,
 )
 
-SheetElementRenderingRuleOutputTypeDef = TypedDict(
-    "SheetElementRenderingRuleOutputTypeDef",
-    {
-        "Expression": str,
-        "ConfigurationOverrides": SheetElementConfigurationOverridesOutputTypeDef,
-    },
-)
-
 SheetElementRenderingRuleTypeDef = TypedDict(
     "SheetElementRenderingRuleTypeDef",
     {
         "Expression": str,
         "ConfigurationOverrides": SheetElementConfigurationOverridesTypeDef,
     },
 )
 
-VisualTitleLabelOptionsOutputTypeDef = TypedDict(
-    "VisualTitleLabelOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "FormatText": ShortFormatTextOutputTypeDef,
-    },
-    total=False,
-)
-
 VisualTitleLabelOptionsTypeDef = TypedDict(
     "VisualTitleLabelOptionsTypeDef",
     {
         "Visibility": VisibilityType,
         "FormatText": ShortFormatTextTypeDef,
     },
     total=False,
@@ -13711,49 +11158,22 @@
 
 class StringDatasetParameterTypeDef(
     _RequiredStringDatasetParameterTypeDef, _OptionalStringDatasetParameterTypeDef
 ):
     pass
 
 
-TableFieldImageConfigurationOutputTypeDef = TypedDict(
-    "TableFieldImageConfigurationOutputTypeDef",
-    {
-        "SizingOptions": TableCellImageSizingConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 TableFieldImageConfigurationTypeDef = TypedDict(
     "TableFieldImageConfigurationTypeDef",
     {
         "SizingOptions": TableCellImageSizingConfigurationTypeDef,
     },
     total=False,
 )
 
-TopicNumericEqualityFilterOutputTypeDef = TypedDict(
-    "TopicNumericEqualityFilterOutputTypeDef",
-    {
-        "Constant": TopicSingularFilterConstantOutputTypeDef,
-        "Aggregation": NamedFilterAggTypeType,
-    },
-    total=False,
-)
-
-TopicRelativeDateFilterOutputTypeDef = TypedDict(
-    "TopicRelativeDateFilterOutputTypeDef",
-    {
-        "TimeGranularity": TopicTimeGranularityType,
-        "RelativeDateFilterFunction": TopicRelativeDateFilterFunctionType,
-        "Constant": TopicSingularFilterConstantOutputTypeDef,
-    },
-    total=False,
-)
-
 TopicNumericEqualityFilterTypeDef = TypedDict(
     "TopicNumericEqualityFilterTypeDef",
     {
         "Constant": TopicSingularFilterConstantTypeDef,
         "Aggregation": NamedFilterAggTypeType,
     },
     total=False,
@@ -13768,107 +11188,107 @@
     },
     total=False,
 )
 
 CascadingControlConfigurationOutputTypeDef = TypedDict(
     "CascadingControlConfigurationOutputTypeDef",
     {
-        "SourceControls": List[CascadingControlSourceOutputTypeDef],
+        "SourceControls": List[CascadingControlSourceTypeDef],
     },
     total=False,
 )
 
-DateTimeDefaultValuesOutputTypeDef = TypedDict(
-    "DateTimeDefaultValuesOutputTypeDef",
+CascadingControlConfigurationTypeDef = TypedDict(
+    "CascadingControlConfigurationTypeDef",
     {
-        "DynamicValue": DynamicDefaultValueOutputTypeDef,
-        "StaticValues": List[datetime],
-        "RollingDate": RollingDateConfigurationOutputTypeDef,
+        "SourceControls": Sequence[CascadingControlSourceTypeDef],
     },
     total=False,
 )
 
-DecimalDefaultValuesOutputTypeDef = TypedDict(
-    "DecimalDefaultValuesOutputTypeDef",
+DateTimeDefaultValuesOutputTypeDef = TypedDict(
+    "DateTimeDefaultValuesOutputTypeDef",
     {
-        "DynamicValue": DynamicDefaultValueOutputTypeDef,
-        "StaticValues": List[float],
+        "DynamicValue": DynamicDefaultValueTypeDef,
+        "StaticValues": List[datetime],
+        "RollingDate": RollingDateConfigurationTypeDef,
     },
     total=False,
 )
 
-IntegerDefaultValuesOutputTypeDef = TypedDict(
-    "IntegerDefaultValuesOutputTypeDef",
+DateTimeDefaultValuesTypeDef = TypedDict(
+    "DateTimeDefaultValuesTypeDef",
     {
-        "DynamicValue": DynamicDefaultValueOutputTypeDef,
-        "StaticValues": List[int],
+        "DynamicValue": DynamicDefaultValueTypeDef,
+        "StaticValues": Sequence[Union[datetime, str]],
+        "RollingDate": RollingDateConfigurationTypeDef,
     },
     total=False,
 )
 
-StringDefaultValuesOutputTypeDef = TypedDict(
-    "StringDefaultValuesOutputTypeDef",
+DecimalDefaultValuesOutputTypeDef = TypedDict(
+    "DecimalDefaultValuesOutputTypeDef",
     {
-        "DynamicValue": DynamicDefaultValueOutputTypeDef,
-        "StaticValues": List[str],
+        "DynamicValue": DynamicDefaultValueTypeDef,
+        "StaticValues": List[float],
     },
     total=False,
 )
 
-DrillDownFilterOutputTypeDef = TypedDict(
-    "DrillDownFilterOutputTypeDef",
+DecimalDefaultValuesTypeDef = TypedDict(
+    "DecimalDefaultValuesTypeDef",
     {
-        "NumericEqualityFilter": NumericEqualityDrillDownFilterOutputTypeDef,
-        "CategoryFilter": CategoryDrillDownFilterOutputTypeDef,
-        "TimeRangeFilter": TimeRangeDrillDownFilterOutputTypeDef,
+        "DynamicValue": DynamicDefaultValueTypeDef,
+        "StaticValues": Sequence[float],
     },
     total=False,
 )
 
-CascadingControlConfigurationTypeDef = TypedDict(
-    "CascadingControlConfigurationTypeDef",
+IntegerDefaultValuesOutputTypeDef = TypedDict(
+    "IntegerDefaultValuesOutputTypeDef",
     {
-        "SourceControls": Sequence[CascadingControlSourceTypeDef],
+        "DynamicValue": DynamicDefaultValueTypeDef,
+        "StaticValues": List[int],
     },
     total=False,
 )
 
-DateTimeDefaultValuesTypeDef = TypedDict(
-    "DateTimeDefaultValuesTypeDef",
+IntegerDefaultValuesTypeDef = TypedDict(
+    "IntegerDefaultValuesTypeDef",
     {
         "DynamicValue": DynamicDefaultValueTypeDef,
-        "StaticValues": Sequence[Union[datetime, str]],
-        "RollingDate": RollingDateConfigurationTypeDef,
+        "StaticValues": Sequence[int],
     },
     total=False,
 )
 
-DecimalDefaultValuesTypeDef = TypedDict(
-    "DecimalDefaultValuesTypeDef",
+StringDefaultValuesOutputTypeDef = TypedDict(
+    "StringDefaultValuesOutputTypeDef",
     {
         "DynamicValue": DynamicDefaultValueTypeDef,
-        "StaticValues": Sequence[float],
+        "StaticValues": List[str],
     },
     total=False,
 )
 
-IntegerDefaultValuesTypeDef = TypedDict(
-    "IntegerDefaultValuesTypeDef",
+StringDefaultValuesTypeDef = TypedDict(
+    "StringDefaultValuesTypeDef",
     {
         "DynamicValue": DynamicDefaultValueTypeDef,
-        "StaticValues": Sequence[int],
+        "StaticValues": Sequence[str],
     },
     total=False,
 )
 
-StringDefaultValuesTypeDef = TypedDict(
-    "StringDefaultValuesTypeDef",
+DrillDownFilterOutputTypeDef = TypedDict(
+    "DrillDownFilterOutputTypeDef",
     {
-        "DynamicValue": DynamicDefaultValueTypeDef,
-        "StaticValues": Sequence[str],
+        "NumericEqualityFilter": NumericEqualityDrillDownFilterTypeDef,
+        "CategoryFilter": CategoryDrillDownFilterOutputTypeDef,
+        "TimeRangeFilter": TimeRangeDrillDownFilterOutputTypeDef,
     },
     total=False,
 )
 
 DrillDownFilterTypeDef = TypedDict(
     "DrillDownFilterTypeDef",
     {
@@ -13997,15 +11417,15 @@
 ):
     pass
 
 
 NumericAxisOptionsOutputTypeDef = TypedDict(
     "NumericAxisOptionsOutputTypeDef",
     {
-        "Scale": AxisScaleOutputTypeDef,
+        "Scale": AxisScaleTypeDef,
         "Range": AxisDisplayRangeOutputTypeDef,
     },
     total=False,
 )
 
 NumericAxisOptionsTypeDef = TypedDict(
     "NumericAxisOptionsTypeDef",
@@ -14016,36 +11436,28 @@
     total=False,
 )
 
 CategoryFilterOutputTypeDef = TypedDict(
     "CategoryFilterOutputTypeDef",
     {
         "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
+        "Column": ColumnIdentifierTypeDef,
         "Configuration": CategoryFilterConfigurationOutputTypeDef,
     },
 )
 
 CategoryFilterTypeDef = TypedDict(
     "CategoryFilterTypeDef",
     {
         "FilterId": str,
         "Column": ColumnIdentifierTypeDef,
         "Configuration": CategoryFilterConfigurationTypeDef,
     },
 )
 
-ClusterMarkerConfigurationOutputTypeDef = TypedDict(
-    "ClusterMarkerConfigurationOutputTypeDef",
-    {
-        "ClusterMarker": ClusterMarkerOutputTypeDef,
-    },
-    total=False,
-)
-
 ClusterMarkerConfigurationTypeDef = TypedDict(
     "ClusterMarkerConfigurationTypeDef",
     {
         "ClusterMarker": ClusterMarkerTypeDef,
     },
     total=False,
 )
@@ -14072,15 +11484,15 @@
     total=False,
 )
 
 TagColumnOperationOutputTypeDef = TypedDict(
     "TagColumnOperationOutputTypeDef",
     {
         "ColumnName": str,
-        "Tags": List[ColumnTagOutputTypeDef],
+        "Tags": List[ColumnTagTypeDef],
     },
 )
 
 TagColumnOperationTypeDef = TypedDict(
     "TagColumnOperationTypeDef",
     {
         "ColumnName": str,
@@ -14104,40 +11516,53 @@
         "Placeholder": str,
         "DataSetSchema": DataSetSchemaTypeDef,
         "ColumnGroupSchemaList": Sequence[ColumnGroupSchemaTypeDef],
     },
     total=False,
 )
 
-ConditionalFormattingIconOutputTypeDef = TypedDict(
-    "ConditionalFormattingIconOutputTypeDef",
-    {
-        "IconSet": ConditionalFormattingIconSetOutputTypeDef,
-        "CustomCondition": ConditionalFormattingCustomIconConditionOutputTypeDef,
-    },
-    total=False,
-)
-
 ConditionalFormattingIconTypeDef = TypedDict(
     "ConditionalFormattingIconTypeDef",
     {
         "IconSet": ConditionalFormattingIconSetTypeDef,
         "CustomCondition": ConditionalFormattingCustomIconConditionTypeDef,
     },
     total=False,
 )
 
+ListDataSetsResponseTypeDef = TypedDict(
+    "ListDataSetsResponseTypeDef",
+    {
+        "DataSetSummaries": List[DataSetSummaryTypeDef],
+        "NextToken": str,
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchDataSetsResponseTypeDef = TypedDict(
+    "SearchDataSetsResponseTypeDef",
+    {
+        "DataSetSummaries": List[DataSetSummaryTypeDef],
+        "NextToken": str,
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DestinationParameterValueConfigurationOutputTypeDef = TypedDict(
     "DestinationParameterValueConfigurationOutputTypeDef",
     {
         "CustomValuesConfiguration": CustomValuesConfigurationOutputTypeDef,
         "SelectAllValueOptions": Literal["ALL_VALUES"],
         "SourceParameterName": str,
         "SourceField": str,
-        "SourceColumn": ColumnIdentifierOutputTypeDef,
+        "SourceColumn": ColumnIdentifierTypeDef,
     },
     total=False,
 )
 
 DestinationParameterValueConfigurationTypeDef = TypedDict(
     "DestinationParameterValueConfigurationTypeDef",
     {
@@ -14146,32 +11571,14 @@
         "SourceParameterName": str,
         "SourceField": str,
         "SourceColumn": ColumnIdentifierTypeDef,
     },
     total=False,
 )
 
-DashboardPublishOptionsOutputTypeDef = TypedDict(
-    "DashboardPublishOptionsOutputTypeDef",
-    {
-        "AdHocFilteringOption": AdHocFilteringOptionOutputTypeDef,
-        "ExportToCSVOption": ExportToCSVOptionOutputTypeDef,
-        "SheetControlsOption": SheetControlsOptionOutputTypeDef,
-        "VisualPublishOptions": DashboardVisualPublishOptionsOutputTypeDef,
-        "SheetLayoutElementMaximizationOption": SheetLayoutElementMaximizationOptionOutputTypeDef,
-        "VisualMenuOption": VisualMenuOptionOutputTypeDef,
-        "VisualAxisSortOption": VisualAxisSortOptionOutputTypeDef,
-        "ExportWithHiddenFieldsOption": ExportWithHiddenFieldsOptionOutputTypeDef,
-        "DataPointDrillUpDownOption": DataPointDrillUpDownOptionOutputTypeDef,
-        "DataPointMenuLabelOption": DataPointMenuLabelOptionOutputTypeDef,
-        "DataPointTooltipOption": DataPointTooltipOptionOutputTypeDef,
-    },
-    total=False,
-)
-
 DashboardPublishOptionsTypeDef = TypedDict(
     "DashboardPublishOptionsTypeDef",
     {
         "AdHocFilteringOption": AdHocFilteringOptionTypeDef,
         "ExportToCSVOption": ExportToCSVOptionTypeDef,
         "SheetControlsOption": SheetControlsOptionTypeDef,
         "VisualPublishOptions": DashboardVisualPublishOptionsTypeDef,
@@ -14186,15 +11593,24 @@
     total=False,
 )
 
 VisualPaletteOutputTypeDef = TypedDict(
     "VisualPaletteOutputTypeDef",
     {
         "ChartColor": str,
-        "ColorMap": List[DataPathColorOutputTypeDef],
+        "ColorMap": List[DataPathColorTypeDef],
+    },
+    total=False,
+)
+
+VisualPaletteTypeDef = TypedDict(
+    "VisualPaletteTypeDef",
+    {
+        "ChartColor": str,
+        "ColorMap": Sequence[DataPathColorTypeDef],
     },
     total=False,
 )
 
 _RequiredPivotTableFieldCollapseStateOptionOutputTypeDef = TypedDict(
     "_RequiredPivotTableFieldCollapseStateOptionOutputTypeDef",
     {
@@ -14213,23 +11629,14 @@
 class PivotTableFieldCollapseStateOptionOutputTypeDef(
     _RequiredPivotTableFieldCollapseStateOptionOutputTypeDef,
     _OptionalPivotTableFieldCollapseStateOptionOutputTypeDef,
 ):
     pass
 
 
-VisualPaletteTypeDef = TypedDict(
-    "VisualPaletteTypeDef",
-    {
-        "ChartColor": str,
-        "ColorMap": Sequence[DataPathColorTypeDef],
-    },
-    total=False,
-)
-
 _RequiredPivotTableFieldCollapseStateOptionTypeDef = TypedDict(
     "_RequiredPivotTableFieldCollapseStateOptionTypeDef",
     {
         "Target": PivotTableFieldCollapseStateTargetTypeDef,
     },
 )
 _OptionalPivotTableFieldCollapseStateOptionTypeDef = TypedDict(
@@ -14244,52 +11651,30 @@
 class PivotTableFieldCollapseStateOptionTypeDef(
     _RequiredPivotTableFieldCollapseStateOptionTypeDef,
     _OptionalPivotTableFieldCollapseStateOptionTypeDef,
 ):
     pass
 
 
-ListDataSetsResponseTypeDef = TypedDict(
-    "ListDataSetsResponseTypeDef",
-    {
-        "DataSetSummaries": List[DataSetSummaryTypeDef],
-        "NextToken": str,
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SearchDataSetsResponseTypeDef = TypedDict(
-    "SearchDataSetsResponseTypeDef",
-    {
-        "DataSetSummaries": List[DataSetSummaryTypeDef],
-        "NextToken": str,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredTimeRangeFilterOutputTypeDef = TypedDict(
     "_RequiredTimeRangeFilterOutputTypeDef",
     {
         "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
+        "Column": ColumnIdentifierTypeDef,
         "NullOption": FilterNullOptionType,
     },
 )
 _OptionalTimeRangeFilterOutputTypeDef = TypedDict(
     "_OptionalTimeRangeFilterOutputTypeDef",
     {
         "IncludeMinimum": bool,
         "IncludeMaximum": bool,
         "RangeMinimumValue": TimeRangeFilterValueOutputTypeDef,
         "RangeMaximumValue": TimeRangeFilterValueOutputTypeDef,
-        "ExcludePeriodConfiguration": ExcludePeriodConfigurationOutputTypeDef,
+        "ExcludePeriodConfiguration": ExcludePeriodConfigurationTypeDef,
         "TimeGranularity": TimeGranularityType,
     },
     total=False,
 )
 
 
 class TimeRangeFilterOutputTypeDef(
@@ -14358,23 +11743,14 @@
         "RefreshSchedules": List[TopicRefreshScheduleSummaryTypeDef],
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DefaultFormattingOutputTypeDef = TypedDict(
-    "DefaultFormattingOutputTypeDef",
-    {
-        "DisplayFormat": DisplayFormatType,
-        "DisplayFormatOptions": DisplayFormatOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 DefaultFormattingTypeDef = TypedDict(
     "DefaultFormattingTypeDef",
     {
         "DisplayFormat": DisplayFormatType,
         "DisplayFormatOptions": DisplayFormatOptionsTypeDef,
     },
     total=False,
@@ -14392,107 +11768,41 @@
     "CustomActionFilterOperationTypeDef",
     {
         "SelectedFieldsConfiguration": FilterOperationSelectedFieldsConfigurationTypeDef,
         "TargetVisualsConfiguration": FilterOperationTargetVisualsConfigurationTypeDef,
     },
 )
 
-AxisLabelOptionsOutputTypeDef = TypedDict(
-    "AxisLabelOptionsOutputTypeDef",
+AxisLabelOptionsTypeDef = TypedDict(
+    "AxisLabelOptionsTypeDef",
     {
-        "FontConfiguration": FontConfigurationOutputTypeDef,
+        "FontConfiguration": FontConfigurationTypeDef,
         "CustomLabel": str,
-        "ApplyTo": AxisLabelReferenceOptionsOutputTypeDef,
+        "ApplyTo": AxisLabelReferenceOptionsTypeDef,
     },
     total=False,
 )
 
 DataLabelOptionsOutputTypeDef = TypedDict(
     "DataLabelOptionsOutputTypeDef",
     {
         "Visibility": VisibilityType,
         "CategoryLabelVisibility": VisibilityType,
         "MeasureLabelVisibility": VisibilityType,
-        "DataLabelTypes": List[DataLabelTypeOutputTypeDef],
+        "DataLabelTypes": List[DataLabelTypeTypeDef],
         "Position": DataLabelPositionType,
         "LabelContent": DataLabelContentType,
-        "LabelFontConfiguration": FontConfigurationOutputTypeDef,
+        "LabelFontConfiguration": FontConfigurationTypeDef,
         "LabelColor": str,
         "Overlap": DataLabelOverlapType,
         "TotalsVisibility": VisibilityType,
     },
     total=False,
 )
 
-FunnelChartDataLabelOptionsOutputTypeDef = TypedDict(
-    "FunnelChartDataLabelOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "CategoryLabelVisibility": VisibilityType,
-        "MeasureLabelVisibility": VisibilityType,
-        "Position": DataLabelPositionType,
-        "LabelFontConfiguration": FontConfigurationOutputTypeDef,
-        "LabelColor": str,
-        "MeasureDataLabelStyle": FunnelChartMeasureDataLabelStyleType,
-    },
-    total=False,
-)
-
-LabelOptionsOutputTypeDef = TypedDict(
-    "LabelOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "FontConfiguration": FontConfigurationOutputTypeDef,
-        "CustomLabel": str,
-    },
-    total=False,
-)
-
-PanelTitleOptionsOutputTypeDef = TypedDict(
-    "PanelTitleOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "FontConfiguration": FontConfigurationOutputTypeDef,
-        "HorizontalTextAlignment": HorizontalTextAlignmentType,
-    },
-    total=False,
-)
-
-_RequiredTableFieldCustomTextContentOutputTypeDef = TypedDict(
-    "_RequiredTableFieldCustomTextContentOutputTypeDef",
-    {
-        "FontConfiguration": FontConfigurationOutputTypeDef,
-    },
-)
-_OptionalTableFieldCustomTextContentOutputTypeDef = TypedDict(
-    "_OptionalTableFieldCustomTextContentOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-
-class TableFieldCustomTextContentOutputTypeDef(
-    _RequiredTableFieldCustomTextContentOutputTypeDef,
-    _OptionalTableFieldCustomTextContentOutputTypeDef,
-):
-    pass
-
-
-AxisLabelOptionsTypeDef = TypedDict(
-    "AxisLabelOptionsTypeDef",
-    {
-        "FontConfiguration": FontConfigurationTypeDef,
-        "CustomLabel": str,
-        "ApplyTo": AxisLabelReferenceOptionsTypeDef,
-    },
-    total=False,
-)
-
 DataLabelOptionsTypeDef = TypedDict(
     "DataLabelOptionsTypeDef",
     {
         "Visibility": VisibilityType,
         "CategoryLabelVisibility": VisibilityType,
         "MeasureLabelVisibility": VisibilityType,
         "DataLabelTypes": Sequence[DataLabelTypeTypeDef],
@@ -14560,36 +11870,29 @@
 ):
     pass
 
 
 ForecastConfigurationOutputTypeDef = TypedDict(
     "ForecastConfigurationOutputTypeDef",
     {
-        "ForecastProperties": TimeBasedForecastPropertiesOutputTypeDef,
+        "ForecastProperties": TimeBasedForecastPropertiesTypeDef,
         "Scenario": ForecastScenarioOutputTypeDef,
     },
     total=False,
 )
 
 ForecastConfigurationTypeDef = TypedDict(
     "ForecastConfigurationTypeDef",
     {
         "ForecastProperties": TimeBasedForecastPropertiesTypeDef,
         "Scenario": ForecastScenarioTypeDef,
     },
     total=False,
 )
 
-DefaultFreeFormLayoutConfigurationOutputTypeDef = TypedDict(
-    "DefaultFreeFormLayoutConfigurationOutputTypeDef",
-    {
-        "CanvasSizeOptions": FreeFormLayoutCanvasSizeOptionsOutputTypeDef,
-    },
-)
-
 DefaultFreeFormLayoutConfigurationTypeDef = TypedDict(
     "DefaultFreeFormLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": FreeFormLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
@@ -14613,23 +11916,14 @@
     "GeospatialHeatmapConfigurationTypeDef",
     {
         "HeatmapColor": GeospatialHeatmapColorScaleTypeDef,
     },
     total=False,
 )
 
-GlobalTableBorderOptionsOutputTypeDef = TypedDict(
-    "GlobalTableBorderOptionsOutputTypeDef",
-    {
-        "UniformBorder": TableBorderOptionsOutputTypeDef,
-        "SideSpecificBorder": TableSideBorderOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 GlobalTableBorderOptionsTypeDef = TypedDict(
     "GlobalTableBorderOptionsTypeDef",
     {
         "UniformBorder": TableBorderOptionsTypeDef,
         "SideSpecificBorder": TableSideBorderOptionsTypeDef,
     },
     total=False,
@@ -14647,49 +11941,42 @@
     "ConditionalFormattingGradientColorTypeDef",
     {
         "Expression": str,
         "Color": GradientColorTypeDef,
     },
 )
 
-DefaultGridLayoutConfigurationOutputTypeDef = TypedDict(
-    "DefaultGridLayoutConfigurationOutputTypeDef",
+DefaultGridLayoutConfigurationTypeDef = TypedDict(
+    "DefaultGridLayoutConfigurationTypeDef",
     {
-        "CanvasSizeOptions": GridLayoutCanvasSizeOptionsOutputTypeDef,
+        "CanvasSizeOptions": GridLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
 _RequiredGridLayoutConfigurationOutputTypeDef = TypedDict(
     "_RequiredGridLayoutConfigurationOutputTypeDef",
     {
-        "Elements": List[GridLayoutElementOutputTypeDef],
+        "Elements": List[GridLayoutElementTypeDef],
     },
 )
 _OptionalGridLayoutConfigurationOutputTypeDef = TypedDict(
     "_OptionalGridLayoutConfigurationOutputTypeDef",
     {
-        "CanvasSizeOptions": GridLayoutCanvasSizeOptionsOutputTypeDef,
+        "CanvasSizeOptions": GridLayoutCanvasSizeOptionsTypeDef,
     },
     total=False,
 )
 
 
 class GridLayoutConfigurationOutputTypeDef(
     _RequiredGridLayoutConfigurationOutputTypeDef, _OptionalGridLayoutConfigurationOutputTypeDef
 ):
     pass
 
 
-DefaultGridLayoutConfigurationTypeDef = TypedDict(
-    "DefaultGridLayoutConfigurationTypeDef",
-    {
-        "CanvasSizeOptions": GridLayoutCanvasSizeOptionsTypeDef,
-    },
-)
-
 _RequiredGridLayoutConfigurationTypeDef = TypedDict(
     "_RequiredGridLayoutConfigurationTypeDef",
     {
         "Elements": Sequence[GridLayoutElementTypeDef],
     },
 )
 _OptionalGridLayoutConfigurationTypeDef = TypedDict(
@@ -14703,21 +11990,14 @@
 
 class GridLayoutConfigurationTypeDef(
     _RequiredGridLayoutConfigurationTypeDef, _OptionalGridLayoutConfigurationTypeDef
 ):
     pass
 
 
-RefreshConfigurationOutputTypeDef = TypedDict(
-    "RefreshConfigurationOutputTypeDef",
-    {
-        "IncrementalRefresh": IncrementalRefreshOutputTypeDef,
-    },
-)
-
 RefreshConfigurationTypeDef = TypedDict(
     "RefreshConfigurationTypeDef",
     {
         "IncrementalRefresh": IncrementalRefreshTypeDef,
     },
 )
 
@@ -14738,79 +12018,24 @@
         "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LogicalTableSourceOutputTypeDef = TypedDict(
-    "LogicalTableSourceOutputTypeDef",
-    {
-        "JoinInstruction": JoinInstructionOutputTypeDef,
-        "PhysicalTableId": str,
-        "DataSetArn": str,
-    },
-    total=False,
-)
-
 LogicalTableSourceTypeDef = TypedDict(
     "LogicalTableSourceTypeDef",
     {
         "JoinInstruction": JoinInstructionTypeDef,
         "PhysicalTableId": str,
         "DataSetArn": str,
     },
     total=False,
 )
 
-_RequiredDataFieldSeriesItemOutputTypeDef = TypedDict(
-    "_RequiredDataFieldSeriesItemOutputTypeDef",
-    {
-        "FieldId": str,
-        "AxisBinding": AxisBindingType,
-    },
-)
-_OptionalDataFieldSeriesItemOutputTypeDef = TypedDict(
-    "_OptionalDataFieldSeriesItemOutputTypeDef",
-    {
-        "FieldValue": str,
-        "Settings": LineChartSeriesSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class DataFieldSeriesItemOutputTypeDef(
-    _RequiredDataFieldSeriesItemOutputTypeDef, _OptionalDataFieldSeriesItemOutputTypeDef
-):
-    pass
-
-
-_RequiredFieldSeriesItemOutputTypeDef = TypedDict(
-    "_RequiredFieldSeriesItemOutputTypeDef",
-    {
-        "FieldId": str,
-        "AxisBinding": AxisBindingType,
-    },
-)
-_OptionalFieldSeriesItemOutputTypeDef = TypedDict(
-    "_OptionalFieldSeriesItemOutputTypeDef",
-    {
-        "Settings": LineChartSeriesSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class FieldSeriesItemOutputTypeDef(
-    _RequiredFieldSeriesItemOutputTypeDef, _OptionalFieldSeriesItemOutputTypeDef
-):
-    pass
-
-
 _RequiredDataFieldSeriesItemTypeDef = TypedDict(
     "_RequiredDataFieldSeriesItemTypeDef",
     {
         "FieldId": str,
         "AxisBinding": AxisBindingType,
     },
 )
@@ -14846,44 +12071,14 @@
 )
 
 
 class FieldSeriesItemTypeDef(_RequiredFieldSeriesItemTypeDef, _OptionalFieldSeriesItemTypeDef):
     pass
 
 
-DataSourceParametersOutputTypeDef = TypedDict(
-    "DataSourceParametersOutputTypeDef",
-    {
-        "AmazonElasticsearchParameters": AmazonElasticsearchParametersOutputTypeDef,
-        "AthenaParameters": AthenaParametersOutputTypeDef,
-        "AuroraParameters": AuroraParametersOutputTypeDef,
-        "AuroraPostgreSqlParameters": AuroraPostgreSqlParametersOutputTypeDef,
-        "AwsIotAnalyticsParameters": AwsIotAnalyticsParametersOutputTypeDef,
-        "JiraParameters": JiraParametersOutputTypeDef,
-        "MariaDbParameters": MariaDbParametersOutputTypeDef,
-        "MySqlParameters": MySqlParametersOutputTypeDef,
-        "OracleParameters": OracleParametersOutputTypeDef,
-        "PostgreSqlParameters": PostgreSqlParametersOutputTypeDef,
-        "PrestoParameters": PrestoParametersOutputTypeDef,
-        "RdsParameters": RdsParametersOutputTypeDef,
-        "RedshiftParameters": RedshiftParametersOutputTypeDef,
-        "S3Parameters": S3ParametersOutputTypeDef,
-        "ServiceNowParameters": ServiceNowParametersOutputTypeDef,
-        "SnowflakeParameters": SnowflakeParametersOutputTypeDef,
-        "SparkParameters": SparkParametersOutputTypeDef,
-        "SqlServerParameters": SqlServerParametersOutputTypeDef,
-        "TeradataParameters": TeradataParametersOutputTypeDef,
-        "TwitterParameters": TwitterParametersOutputTypeDef,
-        "AmazonOpenSearchParameters": AmazonOpenSearchParametersOutputTypeDef,
-        "ExasolParameters": ExasolParametersOutputTypeDef,
-        "DatabricksParameters": DatabricksParametersOutputTypeDef,
-    },
-    total=False,
-)
-
 DataSourceParametersTypeDef = TypedDict(
     "DataSourceParametersTypeDef",
     {
         "AmazonElasticsearchParameters": AmazonElasticsearchParametersTypeDef,
         "AthenaParameters": AthenaParametersTypeDef,
         "AuroraParameters": AuroraParametersTypeDef,
         "AuroraPostgreSqlParameters": AuroraPostgreSqlParametersTypeDef,
@@ -14906,23 +12101,14 @@
         "AmazonOpenSearchParameters": AmazonOpenSearchParametersTypeDef,
         "ExasolParameters": ExasolParametersTypeDef,
         "DatabricksParameters": DatabricksParametersTypeDef,
     },
     total=False,
 )
 
-SheetStyleOutputTypeDef = TypedDict(
-    "SheetStyleOutputTypeDef",
-    {
-        "Tile": TileStyleOutputTypeDef,
-        "TileLayout": TileLayoutStyleOutputTypeDef,
-    },
-    total=False,
-)
-
 SheetStyleTypeDef = TypedDict(
     "SheetStyleTypeDef",
     {
         "Tile": TileStyleTypeDef,
         "TileLayout": TileLayoutStyleTypeDef,
     },
     total=False,
@@ -15012,56 +12198,14 @@
         "VPCConnection": VPCConnectionTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CurrencyDisplayFormatConfigurationOutputTypeDef = TypedDict(
-    "CurrencyDisplayFormatConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-        "Suffix": str,
-        "SeparatorConfiguration": NumericSeparatorConfigurationOutputTypeDef,
-        "Symbol": str,
-        "DecimalPlacesConfiguration": DecimalPlacesConfigurationOutputTypeDef,
-        "NumberScale": NumberScaleType,
-        "NegativeValueConfiguration": NegativeValueConfigurationOutputTypeDef,
-        "NullValueFormatConfiguration": NullValueFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-NumberDisplayFormatConfigurationOutputTypeDef = TypedDict(
-    "NumberDisplayFormatConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-        "Suffix": str,
-        "SeparatorConfiguration": NumericSeparatorConfigurationOutputTypeDef,
-        "DecimalPlacesConfiguration": DecimalPlacesConfigurationOutputTypeDef,
-        "NumberScale": NumberScaleType,
-        "NegativeValueConfiguration": NegativeValueConfigurationOutputTypeDef,
-        "NullValueFormatConfiguration": NullValueFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-PercentageDisplayFormatConfigurationOutputTypeDef = TypedDict(
-    "PercentageDisplayFormatConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-        "Suffix": str,
-        "SeparatorConfiguration": NumericSeparatorConfigurationOutputTypeDef,
-        "DecimalPlacesConfiguration": DecimalPlacesConfigurationOutputTypeDef,
-        "NegativeValueConfiguration": NegativeValueConfigurationOutputTypeDef,
-        "NullValueFormatConfiguration": NullValueFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 CurrencyDisplayFormatConfigurationTypeDef = TypedDict(
     "CurrencyDisplayFormatConfigurationTypeDef",
     {
         "Prefix": str,
         "Suffix": str,
         "SeparatorConfiguration": NumericSeparatorConfigurationTypeDef,
         "Symbol": str,
@@ -15096,73 +12240,34 @@
         "DecimalPlacesConfiguration": DecimalPlacesConfigurationTypeDef,
         "NegativeValueConfiguration": NegativeValueConfigurationTypeDef,
         "NullValueFormatConfiguration": NullValueFormatConfigurationTypeDef,
     },
     total=False,
 )
 
-AggregationFunctionOutputTypeDef = TypedDict(
-    "AggregationFunctionOutputTypeDef",
-    {
-        "NumericalAggregationFunction": NumericalAggregationFunctionOutputTypeDef,
-        "CategoricalAggregationFunction": CategoricalAggregationFunctionType,
-        "DateAggregationFunction": DateAggregationFunctionType,
-        "AttributeAggregationFunction": AttributeAggregationFunctionOutputTypeDef,
-    },
-    total=False,
-)
-
 AggregationFunctionTypeDef = TypedDict(
     "AggregationFunctionTypeDef",
     {
         "NumericalAggregationFunction": NumericalAggregationFunctionTypeDef,
         "CategoricalAggregationFunction": CategoricalAggregationFunctionType,
         "DateAggregationFunction": DateAggregationFunctionType,
         "AttributeAggregationFunction": AttributeAggregationFunctionTypeDef,
     },
     total=False,
 )
 
-ScrollBarOptionsOutputTypeDef = TypedDict(
-    "ScrollBarOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "VisibleRange": VisibleRangeOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 ScrollBarOptionsTypeDef = TypedDict(
     "ScrollBarOptionsTypeDef",
     {
         "Visibility": VisibilityType,
         "VisibleRange": VisibleRangeOptionsTypeDef,
     },
     total=False,
 )
 
-TopicDateRangeFilterOutputTypeDef = TypedDict(
-    "TopicDateRangeFilterOutputTypeDef",
-    {
-        "Inclusive": bool,
-        "Constant": TopicRangeFilterConstantOutputTypeDef,
-    },
-    total=False,
-)
-
-TopicNumericRangeFilterOutputTypeDef = TypedDict(
-    "TopicNumericRangeFilterOutputTypeDef",
-    {
-        "Inclusive": bool,
-        "Constant": TopicRangeFilterConstantOutputTypeDef,
-        "Aggregation": NamedFilterAggTypeType,
-    },
-    total=False,
-)
-
 TopicDateRangeFilterTypeDef = TypedDict(
     "TopicDateRangeFilterTypeDef",
     {
         "Inclusive": bool,
         "Constant": TopicRangeFilterConstantTypeDef,
     },
     total=False,
@@ -15178,15 +12283,15 @@
     total=False,
 )
 
 _RequiredRefreshScheduleOutputTypeDef = TypedDict(
     "_RequiredRefreshScheduleOutputTypeDef",
     {
         "ScheduleId": str,
-        "ScheduleFrequency": RefreshFrequencyOutputTypeDef,
+        "ScheduleFrequency": RefreshFrequencyTypeDef,
         "RefreshType": IngestionTypeType,
     },
 )
 _OptionalRefreshScheduleOutputTypeDef = TypedDict(
     "_OptionalRefreshScheduleOutputTypeDef",
     {
         "StartAfterDateTime": datetime,
@@ -15254,33 +12359,33 @@
 ):
     pass
 
 
 SnapshotDestinationConfigurationOutputTypeDef = TypedDict(
     "SnapshotDestinationConfigurationOutputTypeDef",
     {
-        "S3Destinations": List[SnapshotS3DestinationConfigurationOutputTypeDef],
+        "S3Destinations": List[SnapshotS3DestinationConfigurationTypeDef],
     },
     total=False,
 )
 
-SnapshotJobS3ResultTypeDef = TypedDict(
-    "SnapshotJobS3ResultTypeDef",
+SnapshotDestinationConfigurationTypeDef = TypedDict(
+    "SnapshotDestinationConfigurationTypeDef",
     {
-        "S3DestinationConfiguration": SnapshotS3DestinationConfigurationOutputTypeDef,
-        "S3Uri": str,
-        "ErrorInfo": List[SnapshotJobResultErrorInfoTypeDef],
+        "S3Destinations": Sequence[SnapshotS3DestinationConfigurationTypeDef],
     },
     total=False,
 )
 
-SnapshotDestinationConfigurationTypeDef = TypedDict(
-    "SnapshotDestinationConfigurationTypeDef",
+SnapshotJobS3ResultTypeDef = TypedDict(
+    "SnapshotJobS3ResultTypeDef",
     {
-        "S3Destinations": Sequence[SnapshotS3DestinationConfigurationTypeDef],
+        "S3DestinationConfiguration": SnapshotS3DestinationConfigurationTypeDef,
+        "S3Uri": str,
+        "ErrorInfo": List[SnapshotJobResultErrorInfoTypeDef],
     },
     total=False,
 )
 
 PhysicalTableOutputTypeDef = TypedDict(
     "PhysicalTableOutputTypeDef",
     {
@@ -15297,22 +12402,14 @@
         "RelationalTable": RelationalTableTypeDef,
         "CustomSql": CustomSqlTypeDef,
         "S3Source": S3SourceTypeDef,
     },
     total=False,
 )
 
-SectionBasedLayoutCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "SectionBasedLayoutCanvasSizeOptionsOutputTypeDef",
-    {
-        "PaperCanvasSizeOptions": SectionBasedLayoutPaperCanvasSizeOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 SectionBasedLayoutCanvasSizeOptionsTypeDef = TypedDict(
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
     {
         "PaperCanvasSizeOptions": SectionBasedLayoutPaperCanvasSizeOptionsTypeDef,
     },
     total=False,
 )
@@ -15344,19 +12441,19 @@
         "Height": str,
     },
 )
 _OptionalFreeFormLayoutElementOutputTypeDef = TypedDict(
     "_OptionalFreeFormLayoutElementOutputTypeDef",
     {
         "Visibility": VisibilityType,
-        "RenderingRules": List[SheetElementRenderingRuleOutputTypeDef],
-        "BorderStyle": FreeFormLayoutElementBorderStyleOutputTypeDef,
-        "SelectedBorderStyle": FreeFormLayoutElementBorderStyleOutputTypeDef,
-        "BackgroundStyle": FreeFormLayoutElementBackgroundStyleOutputTypeDef,
-        "LoadingAnimation": LoadingAnimationOutputTypeDef,
+        "RenderingRules": List[SheetElementRenderingRuleTypeDef],
+        "BorderStyle": FreeFormLayoutElementBorderStyleTypeDef,
+        "SelectedBorderStyle": FreeFormLayoutElementBorderStyleTypeDef,
+        "BackgroundStyle": FreeFormLayoutElementBackgroundStyleTypeDef,
+        "LoadingAnimation": LoadingAnimationTypeDef,
     },
     total=False,
 )
 
 
 class FreeFormLayoutElementOutputTypeDef(
     _RequiredFreeFormLayoutElementOutputTypeDef, _OptionalFreeFormLayoutElementOutputTypeDef
@@ -15441,259 +12538,259 @@
 )
 _OptionalDateTimeParameterDeclarationOutputTypeDef = TypedDict(
     "_OptionalDateTimeParameterDeclarationOutputTypeDef",
     {
         "DefaultValues": DateTimeDefaultValuesOutputTypeDef,
         "TimeGranularity": TimeGranularityType,
         "ValueWhenUnset": DateTimeValueWhenUnsetConfigurationOutputTypeDef,
-        "MappedDataSetParameters": List[MappedDataSetParameterOutputTypeDef],
+        "MappedDataSetParameters": List[MappedDataSetParameterTypeDef],
     },
     total=False,
 )
 
 
 class DateTimeParameterDeclarationOutputTypeDef(
     _RequiredDateTimeParameterDeclarationOutputTypeDef,
     _OptionalDateTimeParameterDeclarationOutputTypeDef,
 ):
     pass
 
 
-_RequiredDecimalParameterDeclarationOutputTypeDef = TypedDict(
-    "_RequiredDecimalParameterDeclarationOutputTypeDef",
+_RequiredDateTimeParameterDeclarationTypeDef = TypedDict(
+    "_RequiredDateTimeParameterDeclarationTypeDef",
     {
-        "ParameterValueType": ParameterValueTypeType,
         "Name": str,
     },
 )
-_OptionalDecimalParameterDeclarationOutputTypeDef = TypedDict(
-    "_OptionalDecimalParameterDeclarationOutputTypeDef",
+_OptionalDateTimeParameterDeclarationTypeDef = TypedDict(
+    "_OptionalDateTimeParameterDeclarationTypeDef",
     {
-        "DefaultValues": DecimalDefaultValuesOutputTypeDef,
-        "ValueWhenUnset": DecimalValueWhenUnsetConfigurationOutputTypeDef,
-        "MappedDataSetParameters": List[MappedDataSetParameterOutputTypeDef],
+        "DefaultValues": DateTimeDefaultValuesTypeDef,
+        "TimeGranularity": TimeGranularityType,
+        "ValueWhenUnset": DateTimeValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
     },
     total=False,
 )
 
 
-class DecimalParameterDeclarationOutputTypeDef(
-    _RequiredDecimalParameterDeclarationOutputTypeDef,
-    _OptionalDecimalParameterDeclarationOutputTypeDef,
+class DateTimeParameterDeclarationTypeDef(
+    _RequiredDateTimeParameterDeclarationTypeDef, _OptionalDateTimeParameterDeclarationTypeDef
 ):
     pass
 
 
-_RequiredIntegerParameterDeclarationOutputTypeDef = TypedDict(
-    "_RequiredIntegerParameterDeclarationOutputTypeDef",
+_RequiredDecimalParameterDeclarationOutputTypeDef = TypedDict(
+    "_RequiredDecimalParameterDeclarationOutputTypeDef",
     {
         "ParameterValueType": ParameterValueTypeType,
         "Name": str,
     },
 )
-_OptionalIntegerParameterDeclarationOutputTypeDef = TypedDict(
-    "_OptionalIntegerParameterDeclarationOutputTypeDef",
+_OptionalDecimalParameterDeclarationOutputTypeDef = TypedDict(
+    "_OptionalDecimalParameterDeclarationOutputTypeDef",
     {
-        "DefaultValues": IntegerDefaultValuesOutputTypeDef,
-        "ValueWhenUnset": IntegerValueWhenUnsetConfigurationOutputTypeDef,
-        "MappedDataSetParameters": List[MappedDataSetParameterOutputTypeDef],
+        "DefaultValues": DecimalDefaultValuesOutputTypeDef,
+        "ValueWhenUnset": DecimalValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": List[MappedDataSetParameterTypeDef],
     },
     total=False,
 )
 
 
-class IntegerParameterDeclarationOutputTypeDef(
-    _RequiredIntegerParameterDeclarationOutputTypeDef,
-    _OptionalIntegerParameterDeclarationOutputTypeDef,
+class DecimalParameterDeclarationOutputTypeDef(
+    _RequiredDecimalParameterDeclarationOutputTypeDef,
+    _OptionalDecimalParameterDeclarationOutputTypeDef,
 ):
     pass
 
 
-_RequiredStringParameterDeclarationOutputTypeDef = TypedDict(
-    "_RequiredStringParameterDeclarationOutputTypeDef",
+_RequiredDecimalParameterDeclarationTypeDef = TypedDict(
+    "_RequiredDecimalParameterDeclarationTypeDef",
     {
         "ParameterValueType": ParameterValueTypeType,
         "Name": str,
     },
 )
-_OptionalStringParameterDeclarationOutputTypeDef = TypedDict(
-    "_OptionalStringParameterDeclarationOutputTypeDef",
+_OptionalDecimalParameterDeclarationTypeDef = TypedDict(
+    "_OptionalDecimalParameterDeclarationTypeDef",
     {
-        "DefaultValues": StringDefaultValuesOutputTypeDef,
-        "ValueWhenUnset": StringValueWhenUnsetConfigurationOutputTypeDef,
-        "MappedDataSetParameters": List[MappedDataSetParameterOutputTypeDef],
+        "DefaultValues": DecimalDefaultValuesTypeDef,
+        "ValueWhenUnset": DecimalValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
     },
     total=False,
 )
 
 
-class StringParameterDeclarationOutputTypeDef(
-    _RequiredStringParameterDeclarationOutputTypeDef,
-    _OptionalStringParameterDeclarationOutputTypeDef,
+class DecimalParameterDeclarationTypeDef(
+    _RequiredDecimalParameterDeclarationTypeDef, _OptionalDecimalParameterDeclarationTypeDef
 ):
     pass
 
 
-_RequiredDateTimeHierarchyOutputTypeDef = TypedDict(
-    "_RequiredDateTimeHierarchyOutputTypeDef",
+_RequiredIntegerParameterDeclarationOutputTypeDef = TypedDict(
+    "_RequiredIntegerParameterDeclarationOutputTypeDef",
     {
-        "HierarchyId": str,
+        "ParameterValueType": ParameterValueTypeType,
+        "Name": str,
     },
 )
-_OptionalDateTimeHierarchyOutputTypeDef = TypedDict(
-    "_OptionalDateTimeHierarchyOutputTypeDef",
+_OptionalIntegerParameterDeclarationOutputTypeDef = TypedDict(
+    "_OptionalIntegerParameterDeclarationOutputTypeDef",
     {
-        "DrillDownFilters": List[DrillDownFilterOutputTypeDef],
+        "DefaultValues": IntegerDefaultValuesOutputTypeDef,
+        "ValueWhenUnset": IntegerValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": List[MappedDataSetParameterTypeDef],
     },
     total=False,
 )
 
 
-class DateTimeHierarchyOutputTypeDef(
-    _RequiredDateTimeHierarchyOutputTypeDef, _OptionalDateTimeHierarchyOutputTypeDef
+class IntegerParameterDeclarationOutputTypeDef(
+    _RequiredIntegerParameterDeclarationOutputTypeDef,
+    _OptionalIntegerParameterDeclarationOutputTypeDef,
 ):
     pass
 
 
-_RequiredExplicitHierarchyOutputTypeDef = TypedDict(
-    "_RequiredExplicitHierarchyOutputTypeDef",
+_RequiredIntegerParameterDeclarationTypeDef = TypedDict(
+    "_RequiredIntegerParameterDeclarationTypeDef",
     {
-        "HierarchyId": str,
-        "Columns": List[ColumnIdentifierOutputTypeDef],
+        "ParameterValueType": ParameterValueTypeType,
+        "Name": str,
     },
 )
-_OptionalExplicitHierarchyOutputTypeDef = TypedDict(
-    "_OptionalExplicitHierarchyOutputTypeDef",
+_OptionalIntegerParameterDeclarationTypeDef = TypedDict(
+    "_OptionalIntegerParameterDeclarationTypeDef",
     {
-        "DrillDownFilters": List[DrillDownFilterOutputTypeDef],
+        "DefaultValues": IntegerDefaultValuesTypeDef,
+        "ValueWhenUnset": IntegerValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
     },
     total=False,
 )
 
 
-class ExplicitHierarchyOutputTypeDef(
-    _RequiredExplicitHierarchyOutputTypeDef, _OptionalExplicitHierarchyOutputTypeDef
+class IntegerParameterDeclarationTypeDef(
+    _RequiredIntegerParameterDeclarationTypeDef, _OptionalIntegerParameterDeclarationTypeDef
 ):
     pass
 
 
-_RequiredPredefinedHierarchyOutputTypeDef = TypedDict(
-    "_RequiredPredefinedHierarchyOutputTypeDef",
+_RequiredStringParameterDeclarationOutputTypeDef = TypedDict(
+    "_RequiredStringParameterDeclarationOutputTypeDef",
     {
-        "HierarchyId": str,
-        "Columns": List[ColumnIdentifierOutputTypeDef],
+        "ParameterValueType": ParameterValueTypeType,
+        "Name": str,
     },
 )
-_OptionalPredefinedHierarchyOutputTypeDef = TypedDict(
-    "_OptionalPredefinedHierarchyOutputTypeDef",
+_OptionalStringParameterDeclarationOutputTypeDef = TypedDict(
+    "_OptionalStringParameterDeclarationOutputTypeDef",
     {
-        "DrillDownFilters": List[DrillDownFilterOutputTypeDef],
+        "DefaultValues": StringDefaultValuesOutputTypeDef,
+        "ValueWhenUnset": StringValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": List[MappedDataSetParameterTypeDef],
     },
     total=False,
 )
 
 
-class PredefinedHierarchyOutputTypeDef(
-    _RequiredPredefinedHierarchyOutputTypeDef, _OptionalPredefinedHierarchyOutputTypeDef
+class StringParameterDeclarationOutputTypeDef(
+    _RequiredStringParameterDeclarationOutputTypeDef,
+    _OptionalStringParameterDeclarationOutputTypeDef,
 ):
     pass
 
 
-_RequiredDateTimeParameterDeclarationTypeDef = TypedDict(
-    "_RequiredDateTimeParameterDeclarationTypeDef",
+_RequiredStringParameterDeclarationTypeDef = TypedDict(
+    "_RequiredStringParameterDeclarationTypeDef",
     {
+        "ParameterValueType": ParameterValueTypeType,
         "Name": str,
     },
 )
-_OptionalDateTimeParameterDeclarationTypeDef = TypedDict(
-    "_OptionalDateTimeParameterDeclarationTypeDef",
+_OptionalStringParameterDeclarationTypeDef = TypedDict(
+    "_OptionalStringParameterDeclarationTypeDef",
     {
-        "DefaultValues": DateTimeDefaultValuesTypeDef,
-        "TimeGranularity": TimeGranularityType,
-        "ValueWhenUnset": DateTimeValueWhenUnsetConfigurationTypeDef,
+        "DefaultValues": StringDefaultValuesTypeDef,
+        "ValueWhenUnset": StringValueWhenUnsetConfigurationTypeDef,
         "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
     },
     total=False,
 )
 
 
-class DateTimeParameterDeclarationTypeDef(
-    _RequiredDateTimeParameterDeclarationTypeDef, _OptionalDateTimeParameterDeclarationTypeDef
+class StringParameterDeclarationTypeDef(
+    _RequiredStringParameterDeclarationTypeDef, _OptionalStringParameterDeclarationTypeDef
 ):
     pass
 
 
-_RequiredDecimalParameterDeclarationTypeDef = TypedDict(
-    "_RequiredDecimalParameterDeclarationTypeDef",
+_RequiredDateTimeHierarchyOutputTypeDef = TypedDict(
+    "_RequiredDateTimeHierarchyOutputTypeDef",
     {
-        "ParameterValueType": ParameterValueTypeType,
-        "Name": str,
+        "HierarchyId": str,
     },
 )
-_OptionalDecimalParameterDeclarationTypeDef = TypedDict(
-    "_OptionalDecimalParameterDeclarationTypeDef",
+_OptionalDateTimeHierarchyOutputTypeDef = TypedDict(
+    "_OptionalDateTimeHierarchyOutputTypeDef",
     {
-        "DefaultValues": DecimalDefaultValuesTypeDef,
-        "ValueWhenUnset": DecimalValueWhenUnsetConfigurationTypeDef,
-        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
+        "DrillDownFilters": List[DrillDownFilterOutputTypeDef],
     },
     total=False,
 )
 
 
-class DecimalParameterDeclarationTypeDef(
-    _RequiredDecimalParameterDeclarationTypeDef, _OptionalDecimalParameterDeclarationTypeDef
+class DateTimeHierarchyOutputTypeDef(
+    _RequiredDateTimeHierarchyOutputTypeDef, _OptionalDateTimeHierarchyOutputTypeDef
 ):
     pass
 
 
-_RequiredIntegerParameterDeclarationTypeDef = TypedDict(
-    "_RequiredIntegerParameterDeclarationTypeDef",
+_RequiredExplicitHierarchyOutputTypeDef = TypedDict(
+    "_RequiredExplicitHierarchyOutputTypeDef",
     {
-        "ParameterValueType": ParameterValueTypeType,
-        "Name": str,
+        "HierarchyId": str,
+        "Columns": List[ColumnIdentifierTypeDef],
     },
 )
-_OptionalIntegerParameterDeclarationTypeDef = TypedDict(
-    "_OptionalIntegerParameterDeclarationTypeDef",
+_OptionalExplicitHierarchyOutputTypeDef = TypedDict(
+    "_OptionalExplicitHierarchyOutputTypeDef",
     {
-        "DefaultValues": IntegerDefaultValuesTypeDef,
-        "ValueWhenUnset": IntegerValueWhenUnsetConfigurationTypeDef,
-        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
+        "DrillDownFilters": List[DrillDownFilterOutputTypeDef],
     },
     total=False,
 )
 
 
-class IntegerParameterDeclarationTypeDef(
-    _RequiredIntegerParameterDeclarationTypeDef, _OptionalIntegerParameterDeclarationTypeDef
+class ExplicitHierarchyOutputTypeDef(
+    _RequiredExplicitHierarchyOutputTypeDef, _OptionalExplicitHierarchyOutputTypeDef
 ):
     pass
 
 
-_RequiredStringParameterDeclarationTypeDef = TypedDict(
-    "_RequiredStringParameterDeclarationTypeDef",
+_RequiredPredefinedHierarchyOutputTypeDef = TypedDict(
+    "_RequiredPredefinedHierarchyOutputTypeDef",
     {
-        "ParameterValueType": ParameterValueTypeType,
-        "Name": str,
+        "HierarchyId": str,
+        "Columns": List[ColumnIdentifierTypeDef],
     },
 )
-_OptionalStringParameterDeclarationTypeDef = TypedDict(
-    "_OptionalStringParameterDeclarationTypeDef",
+_OptionalPredefinedHierarchyOutputTypeDef = TypedDict(
+    "_OptionalPredefinedHierarchyOutputTypeDef",
     {
-        "DefaultValues": StringDefaultValuesTypeDef,
-        "ValueWhenUnset": StringValueWhenUnsetConfigurationTypeDef,
-        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
+        "DrillDownFilters": List[DrillDownFilterOutputTypeDef],
     },
     total=False,
 )
 
 
-class StringParameterDeclarationTypeDef(
-    _RequiredStringParameterDeclarationTypeDef, _OptionalStringParameterDeclarationTypeDef
+class PredefinedHierarchyOutputTypeDef(
+    _RequiredPredefinedHierarchyOutputTypeDef, _OptionalPredefinedHierarchyOutputTypeDef
 ):
     pass
 
 
 _RequiredDateTimeHierarchyTypeDef = TypedDict(
     "_RequiredDateTimeHierarchyTypeDef",
     {
@@ -15810,15 +12907,15 @@
     pass
 
 
 AxisDataOptionsOutputTypeDef = TypedDict(
     "AxisDataOptionsOutputTypeDef",
     {
         "NumericAxisOptions": NumericAxisOptionsOutputTypeDef,
-        "DateAxisOptions": DateAxisOptionsOutputTypeDef,
+        "DateAxisOptions": DateAxisOptionsTypeDef,
     },
     total=False,
 )
 
 AxisDataOptionsTypeDef = TypedDict(
     "AxisDataOptionsTypeDef",
     {
@@ -15828,18 +12925,18 @@
     total=False,
 )
 
 TransformOperationOutputTypeDef = TypedDict(
     "TransformOperationOutputTypeDef",
     {
         "ProjectOperation": ProjectOperationOutputTypeDef,
-        "FilterOperation": FilterOperationOutputTypeDef,
+        "FilterOperation": FilterOperationTypeDef,
         "CreateColumnsOperation": CreateColumnsOperationOutputTypeDef,
-        "RenameColumnOperation": RenameColumnOperationOutputTypeDef,
-        "CastColumnTypeOperation": CastColumnTypeOperationOutputTypeDef,
+        "RenameColumnOperation": RenameColumnOperationTypeDef,
+        "CastColumnTypeOperation": CastColumnTypeOperationTypeDef,
         "TagColumnOperation": TagColumnOperationOutputTypeDef,
         "UntagColumnOperation": UntagColumnOperationOutputTypeDef,
         "OverrideDatasetParameterOperation": OverrideDatasetParameterOperationOutputTypeDef,
     },
     total=False,
 )
 
@@ -15889,15 +12986,15 @@
         "Value": DestinationParameterValueConfigurationTypeDef,
     },
 )
 
 PivotTableFieldOptionsOutputTypeDef = TypedDict(
     "PivotTableFieldOptionsOutputTypeDef",
     {
-        "SelectedFieldOptions": List[PivotTableFieldOptionOutputTypeDef],
+        "SelectedFieldOptions": List[PivotTableFieldOptionTypeDef],
         "DataPathOptions": List[PivotTableDataPathOptionOutputTypeDef],
         "CollapseStateOptions": List[PivotTableFieldCollapseStateOptionOutputTypeDef],
     },
     total=False,
 )
 
 PivotTableFieldOptionsTypeDef = TypedDict(
@@ -15922,15 +13019,15 @@
     {
         "CalculatedFieldDescription": str,
         "CalculatedFieldSynonyms": List[str],
         "IsIncludedInTopic": bool,
         "DisableIndexing": bool,
         "ColumnDataRole": ColumnDataRoleType,
         "TimeGranularity": TopicTimeGranularityType,
-        "DefaultFormatting": DefaultFormattingOutputTypeDef,
+        "DefaultFormatting": DefaultFormattingTypeDef,
         "Aggregation": DefaultAggregationType,
         "ComparativeOrder": ComparativeOrderOutputTypeDef,
         "SemanticType": SemanticTypeOutputTypeDef,
         "AllowedAggregations": List[AuthorSpecifiedAggregationType],
         "NotAllowedAggregations": List[AuthorSpecifiedAggregationType],
         "NeverAggregateInFilter": bool,
         "CellValueSynonyms": List[CellValueSynonymOutputTypeDef],
@@ -15941,49 +13038,14 @@
 
 class TopicCalculatedFieldOutputTypeDef(
     _RequiredTopicCalculatedFieldOutputTypeDef, _OptionalTopicCalculatedFieldOutputTypeDef
 ):
     pass
 
 
-_RequiredTopicColumnOutputTypeDef = TypedDict(
-    "_RequiredTopicColumnOutputTypeDef",
-    {
-        "ColumnName": str,
-    },
-)
-_OptionalTopicColumnOutputTypeDef = TypedDict(
-    "_OptionalTopicColumnOutputTypeDef",
-    {
-        "ColumnFriendlyName": str,
-        "ColumnDescription": str,
-        "ColumnSynonyms": List[str],
-        "ColumnDataRole": ColumnDataRoleType,
-        "Aggregation": DefaultAggregationType,
-        "IsIncludedInTopic": bool,
-        "DisableIndexing": bool,
-        "ComparativeOrder": ComparativeOrderOutputTypeDef,
-        "SemanticType": SemanticTypeOutputTypeDef,
-        "TimeGranularity": TopicTimeGranularityType,
-        "AllowedAggregations": List[AuthorSpecifiedAggregationType],
-        "NotAllowedAggregations": List[AuthorSpecifiedAggregationType],
-        "DefaultFormatting": DefaultFormattingOutputTypeDef,
-        "NeverAggregateInFilter": bool,
-        "CellValueSynonyms": List[CellValueSynonymOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class TopicColumnOutputTypeDef(
-    _RequiredTopicColumnOutputTypeDef, _OptionalTopicColumnOutputTypeDef
-):
-    pass
-
-
 _RequiredTopicCalculatedFieldTypeDef = TypedDict(
     "_RequiredTopicCalculatedFieldTypeDef",
     {
         "CalculatedFieldName": str,
         "Expression": str,
     },
 )
@@ -16011,14 +13073,49 @@
 
 class TopicCalculatedFieldTypeDef(
     _RequiredTopicCalculatedFieldTypeDef, _OptionalTopicCalculatedFieldTypeDef
 ):
     pass
 
 
+_RequiredTopicColumnOutputTypeDef = TypedDict(
+    "_RequiredTopicColumnOutputTypeDef",
+    {
+        "ColumnName": str,
+    },
+)
+_OptionalTopicColumnOutputTypeDef = TypedDict(
+    "_OptionalTopicColumnOutputTypeDef",
+    {
+        "ColumnFriendlyName": str,
+        "ColumnDescription": str,
+        "ColumnSynonyms": List[str],
+        "ColumnDataRole": ColumnDataRoleType,
+        "Aggregation": DefaultAggregationType,
+        "IsIncludedInTopic": bool,
+        "DisableIndexing": bool,
+        "ComparativeOrder": ComparativeOrderOutputTypeDef,
+        "SemanticType": SemanticTypeOutputTypeDef,
+        "TimeGranularity": TopicTimeGranularityType,
+        "AllowedAggregations": List[AuthorSpecifiedAggregationType],
+        "NotAllowedAggregations": List[AuthorSpecifiedAggregationType],
+        "DefaultFormatting": DefaultFormattingTypeDef,
+        "NeverAggregateInFilter": bool,
+        "CellValueSynonyms": List[CellValueSynonymOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class TopicColumnOutputTypeDef(
+    _RequiredTopicColumnOutputTypeDef, _OptionalTopicColumnOutputTypeDef
+):
+    pass
+
+
 _RequiredTopicColumnTypeDef = TypedDict(
     "_RequiredTopicColumnTypeDef",
     {
         "ColumnName": str,
     },
 )
 _OptionalTopicColumnTypeDef = TypedDict(
@@ -16049,131 +13146,15 @@
 
 
 ChartAxisLabelOptionsOutputTypeDef = TypedDict(
     "ChartAxisLabelOptionsOutputTypeDef",
     {
         "Visibility": VisibilityType,
         "SortIconVisibility": VisibilityType,
-        "AxisLabelOptions": List[AxisLabelOptionsOutputTypeDef],
-    },
-    total=False,
-)
-
-AxisTickLabelOptionsOutputTypeDef = TypedDict(
-    "AxisTickLabelOptionsOutputTypeDef",
-    {
-        "LabelOptions": LabelOptionsOutputTypeDef,
-        "RotationAngle": float,
-    },
-    total=False,
-)
-
-DateTimePickerControlDisplayOptionsOutputTypeDef = TypedDict(
-    "DateTimePickerControlDisplayOptionsOutputTypeDef",
-    {
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "DateTimeFormat": str,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-DropDownControlDisplayOptionsOutputTypeDef = TypedDict(
-    "DropDownControlDisplayOptionsOutputTypeDef",
-    {
-        "SelectAllOptions": ListControlSelectAllOptionsOutputTypeDef,
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-LegendOptionsOutputTypeDef = TypedDict(
-    "LegendOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "Title": LabelOptionsOutputTypeDef,
-        "Position": LegendPositionType,
-        "Width": str,
-        "Height": str,
-    },
-    total=False,
-)
-
-ListControlDisplayOptionsOutputTypeDef = TypedDict(
-    "ListControlDisplayOptionsOutputTypeDef",
-    {
-        "SearchOptions": ListControlSearchOptionsOutputTypeDef,
-        "SelectAllOptions": ListControlSelectAllOptionsOutputTypeDef,
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-RelativeDateTimeControlDisplayOptionsOutputTypeDef = TypedDict(
-    "RelativeDateTimeControlDisplayOptionsOutputTypeDef",
-    {
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "DateTimeFormat": str,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-SliderControlDisplayOptionsOutputTypeDef = TypedDict(
-    "SliderControlDisplayOptionsOutputTypeDef",
-    {
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-TextAreaControlDisplayOptionsOutputTypeDef = TypedDict(
-    "TextAreaControlDisplayOptionsOutputTypeDef",
-    {
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "PlaceholderOptions": TextControlPlaceholderOptionsOutputTypeDef,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-TextFieldControlDisplayOptionsOutputTypeDef = TypedDict(
-    "TextFieldControlDisplayOptionsOutputTypeDef",
-    {
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "PlaceholderOptions": TextControlPlaceholderOptionsOutputTypeDef,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-PanelConfigurationOutputTypeDef = TypedDict(
-    "PanelConfigurationOutputTypeDef",
-    {
-        "Title": PanelTitleOptionsOutputTypeDef,
-        "BorderVisibility": VisibilityType,
-        "BorderThickness": str,
-        "BorderStyle": PanelBorderStyleType,
-        "BorderColor": str,
-        "GutterVisibility": VisibilityType,
-        "GutterSpacing": str,
-        "BackgroundVisibility": VisibilityType,
-        "BackgroundColor": str,
-    },
-    total=False,
-)
-
-TableFieldLinkContentConfigurationOutputTypeDef = TypedDict(
-    "TableFieldLinkContentConfigurationOutputTypeDef",
-    {
-        "CustomTextContent": TableFieldCustomTextContentOutputTypeDef,
-        "CustomIconContent": TableFieldCustomIconContentOutputTypeDef,
+        "AxisLabelOptions": List[AxisLabelOptionsTypeDef],
     },
     total=False,
 )
 
 ChartAxisLabelOptionsTypeDef = TypedDict(
     "ChartAxisLabelOptionsTypeDef",
     {
@@ -16300,15 +13281,15 @@
     total=False,
 )
 
 GeospatialPointStyleOptionsOutputTypeDef = TypedDict(
     "GeospatialPointStyleOptionsOutputTypeDef",
     {
         "SelectedPointStyle": GeospatialSelectedPointStyleType,
-        "ClusterMarkerConfiguration": ClusterMarkerConfigurationOutputTypeDef,
+        "ClusterMarkerConfiguration": ClusterMarkerConfigurationTypeDef,
         "HeatmapConfiguration": GeospatialHeatmapConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 GeospatialPointStyleOptionsTypeDef = TypedDict(
     "GeospatialPointStyleOptionsTypeDef",
@@ -16316,29 +13297,14 @@
         "SelectedPointStyle": GeospatialSelectedPointStyleType,
         "ClusterMarkerConfiguration": ClusterMarkerConfigurationTypeDef,
         "HeatmapConfiguration": GeospatialHeatmapConfigurationTypeDef,
     },
     total=False,
 )
 
-TableCellStyleOutputTypeDef = TypedDict(
-    "TableCellStyleOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "FontConfiguration": FontConfigurationOutputTypeDef,
-        "TextWrap": TextWrapType,
-        "HorizontalTextAlignment": HorizontalTextAlignmentType,
-        "VerticalTextAlignment": VerticalTextAlignmentType,
-        "BackgroundColor": str,
-        "Height": int,
-        "Border": GlobalTableBorderOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 TableCellStyleTypeDef = TypedDict(
     "TableCellStyleTypeDef",
     {
         "Visibility": VisibilityType,
         "FontConfiguration": FontConfigurationTypeDef,
         "TextWrap": TextWrapType,
         "HorizontalTextAlignment": HorizontalTextAlignmentType,
@@ -16349,141 +13315,70 @@
     },
     total=False,
 )
 
 ConditionalFormattingColorOutputTypeDef = TypedDict(
     "ConditionalFormattingColorOutputTypeDef",
     {
-        "Solid": ConditionalFormattingSolidColorOutputTypeDef,
+        "Solid": ConditionalFormattingSolidColorTypeDef,
         "Gradient": ConditionalFormattingGradientColorOutputTypeDef,
     },
     total=False,
 )
 
 ConditionalFormattingColorTypeDef = TypedDict(
     "ConditionalFormattingColorTypeDef",
     {
         "Solid": ConditionalFormattingSolidColorTypeDef,
         "Gradient": ConditionalFormattingGradientColorTypeDef,
     },
     total=False,
 )
 
-DefaultInteractiveLayoutConfigurationOutputTypeDef = TypedDict(
-    "DefaultInteractiveLayoutConfigurationOutputTypeDef",
+DefaultInteractiveLayoutConfigurationTypeDef = TypedDict(
+    "DefaultInteractiveLayoutConfigurationTypeDef",
     {
-        "Grid": DefaultGridLayoutConfigurationOutputTypeDef,
-        "FreeForm": DefaultFreeFormLayoutConfigurationOutputTypeDef,
+        "Grid": DefaultGridLayoutConfigurationTypeDef,
+        "FreeForm": DefaultFreeFormLayoutConfigurationTypeDef,
     },
     total=False,
 )
 
 SheetControlLayoutConfigurationOutputTypeDef = TypedDict(
     "SheetControlLayoutConfigurationOutputTypeDef",
     {
         "GridLayout": GridLayoutConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-DefaultInteractiveLayoutConfigurationTypeDef = TypedDict(
-    "DefaultInteractiveLayoutConfigurationTypeDef",
-    {
-        "Grid": DefaultGridLayoutConfigurationTypeDef,
-        "FreeForm": DefaultFreeFormLayoutConfigurationTypeDef,
-    },
-    total=False,
-)
-
 SheetControlLayoutConfigurationTypeDef = TypedDict(
     "SheetControlLayoutConfigurationTypeDef",
     {
         "GridLayout": GridLayoutConfigurationTypeDef,
     },
     total=False,
 )
 
-DataSetRefreshPropertiesOutputTypeDef = TypedDict(
-    "DataSetRefreshPropertiesOutputTypeDef",
-    {
-        "RefreshConfiguration": RefreshConfigurationOutputTypeDef,
-    },
-)
-
 DataSetRefreshPropertiesTypeDef = TypedDict(
     "DataSetRefreshPropertiesTypeDef",
     {
         "RefreshConfiguration": RefreshConfigurationTypeDef,
     },
 )
 
-SeriesItemOutputTypeDef = TypedDict(
-    "SeriesItemOutputTypeDef",
-    {
-        "FieldSeriesItem": FieldSeriesItemOutputTypeDef,
-        "DataFieldSeriesItem": DataFieldSeriesItemOutputTypeDef,
-    },
-    total=False,
-)
-
 SeriesItemTypeDef = TypedDict(
     "SeriesItemTypeDef",
     {
         "FieldSeriesItem": FieldSeriesItemTypeDef,
         "DataFieldSeriesItem": DataFieldSeriesItemTypeDef,
     },
     total=False,
 )
 
-_RequiredAssetBundleImportJobDataSourceOverrideParametersOutputTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobDataSourceOverrideParametersOutputTypeDef",
-    {
-        "DataSourceId": str,
-    },
-)
-_OptionalAssetBundleImportJobDataSourceOverrideParametersOutputTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobDataSourceOverrideParametersOutputTypeDef",
-    {
-        "Name": str,
-        "DataSourceParameters": DataSourceParametersOutputTypeDef,
-        "VpcConnectionProperties": VpcConnectionPropertiesOutputTypeDef,
-        "SslProperties": SslPropertiesOutputTypeDef,
-        "Credentials": AssetBundleImportJobDataSourceCredentialsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef(
-    _RequiredAssetBundleImportJobDataSourceOverrideParametersOutputTypeDef,
-    _OptionalAssetBundleImportJobDataSourceOverrideParametersOutputTypeDef,
-):
-    pass
-
-
-DataSourceTypeDef = TypedDict(
-    "DataSourceTypeDef",
-    {
-        "Arn": str,
-        "DataSourceId": str,
-        "Name": str,
-        "Type": DataSourceTypeType,
-        "Status": ResourceStatusType,
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "DataSourceParameters": DataSourceParametersOutputTypeDef,
-        "AlternateDataSourceParameters": List[DataSourceParametersOutputTypeDef],
-        "VpcConnectionProperties": VpcConnectionPropertiesOutputTypeDef,
-        "SslProperties": SslPropertiesOutputTypeDef,
-        "ErrorInfo": DataSourceErrorInfoTypeDef,
-        "SecretArn": str,
-    },
-    total=False,
-)
-
 _RequiredAssetBundleImportJobDataSourceOverrideParametersTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobDataSourceOverrideParametersTypeDef",
     {
         "DataSourceId": str,
     },
 )
 _OptionalAssetBundleImportJobDataSourceOverrideParametersTypeDef = TypedDict(
@@ -16522,20 +13417,40 @@
 )
 
 
 class CredentialPairTypeDef(_RequiredCredentialPairTypeDef, _OptionalCredentialPairTypeDef):
     pass
 
 
+DataSourceTypeDef = TypedDict(
+    "DataSourceTypeDef",
+    {
+        "Arn": str,
+        "DataSourceId": str,
+        "Name": str,
+        "Type": DataSourceTypeType,
+        "Status": ResourceStatusType,
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "DataSourceParameters": DataSourceParametersTypeDef,
+        "AlternateDataSourceParameters": List[DataSourceParametersTypeDef],
+        "VpcConnectionProperties": VpcConnectionPropertiesTypeDef,
+        "SslProperties": SslPropertiesTypeDef,
+        "ErrorInfo": DataSourceErrorInfoTypeDef,
+        "SecretArn": str,
+    },
+    total=False,
+)
+
 ThemeConfigurationOutputTypeDef = TypedDict(
     "ThemeConfigurationOutputTypeDef",
     {
         "DataColorPalette": DataColorPaletteOutputTypeDef,
-        "UIColorPalette": UIColorPaletteOutputTypeDef,
-        "Sheet": SheetStyleOutputTypeDef,
+        "UIColorPalette": UIColorPaletteTypeDef,
+        "Sheet": SheetStyleTypeDef,
         "Typography": TypographyOutputTypeDef,
     },
     total=False,
 )
 
 ThemeConfigurationTypeDef = TypedDict(
     "ThemeConfigurationTypeDef",
@@ -16544,33 +13459,14 @@
         "UIColorPalette": UIColorPaletteTypeDef,
         "Sheet": SheetStyleTypeDef,
         "Typography": TypographyTypeDef,
     },
     total=False,
 )
 
-ComparisonFormatConfigurationOutputTypeDef = TypedDict(
-    "ComparisonFormatConfigurationOutputTypeDef",
-    {
-        "NumberDisplayFormatConfiguration": NumberDisplayFormatConfigurationOutputTypeDef,
-        "PercentageDisplayFormatConfiguration": PercentageDisplayFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-NumericFormatConfigurationOutputTypeDef = TypedDict(
-    "NumericFormatConfigurationOutputTypeDef",
-    {
-        "NumberDisplayFormatConfiguration": NumberDisplayFormatConfigurationOutputTypeDef,
-        "CurrencyDisplayFormatConfiguration": CurrencyDisplayFormatConfigurationOutputTypeDef,
-        "PercentageDisplayFormatConfiguration": PercentageDisplayFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ComparisonFormatConfigurationTypeDef = TypedDict(
     "ComparisonFormatConfigurationTypeDef",
     {
         "NumberDisplayFormatConfiguration": NumberDisplayFormatConfigurationTypeDef,
         "PercentageDisplayFormatConfiguration": PercentageDisplayFormatConfigurationTypeDef,
     },
     total=False,
@@ -16582,158 +13478,14 @@
         "NumberDisplayFormatConfiguration": NumberDisplayFormatConfigurationTypeDef,
         "CurrencyDisplayFormatConfiguration": CurrencyDisplayFormatConfigurationTypeDef,
         "PercentageDisplayFormatConfiguration": PercentageDisplayFormatConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredAggregationSortConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAggregationSortConfigurationOutputTypeDef",
-    {
-        "Column": ColumnIdentifierOutputTypeDef,
-        "SortDirection": SortDirectionType,
-    },
-)
-_OptionalAggregationSortConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAggregationSortConfigurationOutputTypeDef",
-    {
-        "AggregationFunction": AggregationFunctionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class AggregationSortConfigurationOutputTypeDef(
-    _RequiredAggregationSortConfigurationOutputTypeDef,
-    _OptionalAggregationSortConfigurationOutputTypeDef,
-):
-    pass
-
-
-_RequiredColumnSortOutputTypeDef = TypedDict(
-    "_RequiredColumnSortOutputTypeDef",
-    {
-        "SortBy": ColumnIdentifierOutputTypeDef,
-        "Direction": SortDirectionType,
-    },
-)
-_OptionalColumnSortOutputTypeDef = TypedDict(
-    "_OptionalColumnSortOutputTypeDef",
-    {
-        "AggregationFunction": AggregationFunctionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ColumnSortOutputTypeDef(_RequiredColumnSortOutputTypeDef, _OptionalColumnSortOutputTypeDef):
-    pass
-
-
-_RequiredColumnTooltipItemOutputTypeDef = TypedDict(
-    "_RequiredColumnTooltipItemOutputTypeDef",
-    {
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalColumnTooltipItemOutputTypeDef = TypedDict(
-    "_OptionalColumnTooltipItemOutputTypeDef",
-    {
-        "Label": str,
-        "Visibility": VisibilityType,
-        "Aggregation": AggregationFunctionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ColumnTooltipItemOutputTypeDef(
-    _RequiredColumnTooltipItemOutputTypeDef, _OptionalColumnTooltipItemOutputTypeDef
-):
-    pass
-
-
-_RequiredNumericEqualityFilterOutputTypeDef = TypedDict(
-    "_RequiredNumericEqualityFilterOutputTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-        "MatchOperator": NumericEqualityMatchOperatorType,
-        "NullOption": FilterNullOptionType,
-    },
-)
-_OptionalNumericEqualityFilterOutputTypeDef = TypedDict(
-    "_OptionalNumericEqualityFilterOutputTypeDef",
-    {
-        "Value": float,
-        "SelectAllOptions": Literal["FILTER_ALL_VALUES"],
-        "AggregationFunction": AggregationFunctionOutputTypeDef,
-        "ParameterName": str,
-    },
-    total=False,
-)
-
-
-class NumericEqualityFilterOutputTypeDef(
-    _RequiredNumericEqualityFilterOutputTypeDef, _OptionalNumericEqualityFilterOutputTypeDef
-):
-    pass
-
-
-_RequiredNumericRangeFilterOutputTypeDef = TypedDict(
-    "_RequiredNumericRangeFilterOutputTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-        "NullOption": FilterNullOptionType,
-    },
-)
-_OptionalNumericRangeFilterOutputTypeDef = TypedDict(
-    "_OptionalNumericRangeFilterOutputTypeDef",
-    {
-        "IncludeMinimum": bool,
-        "IncludeMaximum": bool,
-        "RangeMinimum": NumericRangeFilterValueOutputTypeDef,
-        "RangeMaximum": NumericRangeFilterValueOutputTypeDef,
-        "SelectAllOptions": Literal["FILTER_ALL_VALUES"],
-        "AggregationFunction": AggregationFunctionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class NumericRangeFilterOutputTypeDef(
-    _RequiredNumericRangeFilterOutputTypeDef, _OptionalNumericRangeFilterOutputTypeDef
-):
-    pass
-
-
-_RequiredReferenceLineDynamicDataConfigurationOutputTypeDef = TypedDict(
-    "_RequiredReferenceLineDynamicDataConfigurationOutputTypeDef",
-    {
-        "Column": ColumnIdentifierOutputTypeDef,
-        "Calculation": NumericalAggregationFunctionOutputTypeDef,
-    },
-)
-_OptionalReferenceLineDynamicDataConfigurationOutputTypeDef = TypedDict(
-    "_OptionalReferenceLineDynamicDataConfigurationOutputTypeDef",
-    {
-        "MeasureAggregationFunction": AggregationFunctionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ReferenceLineDynamicDataConfigurationOutputTypeDef(
-    _RequiredReferenceLineDynamicDataConfigurationOutputTypeDef,
-    _OptionalReferenceLineDynamicDataConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredAggregationSortConfigurationTypeDef = TypedDict(
     "_RequiredAggregationSortConfigurationTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "SortDirection": SortDirectionType,
     },
 )
@@ -16884,18 +13636,18 @@
     "_OptionalTopicFilterOutputTypeDef",
     {
         "FilterDescription": str,
         "FilterClass": FilterClassType,
         "FilterSynonyms": List[str],
         "FilterType": NamedFilterTypeType,
         "CategoryFilter": TopicCategoryFilterOutputTypeDef,
-        "NumericEqualityFilter": TopicNumericEqualityFilterOutputTypeDef,
-        "NumericRangeFilter": TopicNumericRangeFilterOutputTypeDef,
-        "DateRangeFilter": TopicDateRangeFilterOutputTypeDef,
-        "RelativeDateFilter": TopicRelativeDateFilterOutputTypeDef,
+        "NumericEqualityFilter": TopicNumericEqualityFilterTypeDef,
+        "NumericRangeFilter": TopicNumericRangeFilterTypeDef,
+        "DateRangeFilter": TopicDateRangeFilterTypeDef,
+        "RelativeDateFilter": TopicRelativeDateFilterTypeDef,
     },
     total=False,
 )
 
 
 class TopicFilterOutputTypeDef(
     _RequiredTopicFilterOutputTypeDef, _OptionalTopicFilterOutputTypeDef
@@ -16986,21 +13738,14 @@
     {
         "Files": List[SnapshotFileOutputTypeDef],
         "S3Results": List[SnapshotJobS3ResultTypeDef],
     },
     total=False,
 )
 
-DefaultSectionBasedLayoutConfigurationOutputTypeDef = TypedDict(
-    "DefaultSectionBasedLayoutConfigurationOutputTypeDef",
-    {
-        "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsOutputTypeDef,
-    },
-)
-
 DefaultSectionBasedLayoutConfigurationTypeDef = TypedDict(
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
@@ -17009,15 +13754,15 @@
     {
         "Elements": List[FreeFormLayoutElementOutputTypeDef],
     },
 )
 _OptionalFreeFormLayoutConfigurationOutputTypeDef = TypedDict(
     "_OptionalFreeFormLayoutConfigurationOutputTypeDef",
     {
-        "CanvasSizeOptions": FreeFormLayoutCanvasSizeOptionsOutputTypeDef,
+        "CanvasSizeOptions": FreeFormLayoutCanvasSizeOptionsTypeDef,
     },
     total=False,
 )
 
 
 class FreeFormLayoutConfigurationOutputTypeDef(
     _RequiredFreeFormLayoutConfigurationOutputTypeDef,
@@ -17112,35 +13857,35 @@
         "DecimalParameterDeclaration": DecimalParameterDeclarationOutputTypeDef,
         "IntegerParameterDeclaration": IntegerParameterDeclarationOutputTypeDef,
         "DateTimeParameterDeclaration": DateTimeParameterDeclarationOutputTypeDef,
     },
     total=False,
 )
 
-ColumnHierarchyOutputTypeDef = TypedDict(
-    "ColumnHierarchyOutputTypeDef",
-    {
-        "ExplicitHierarchy": ExplicitHierarchyOutputTypeDef,
-        "DateTimeHierarchy": DateTimeHierarchyOutputTypeDef,
-        "PredefinedHierarchy": PredefinedHierarchyOutputTypeDef,
-    },
-    total=False,
-)
-
 ParameterDeclarationTypeDef = TypedDict(
     "ParameterDeclarationTypeDef",
     {
         "StringParameterDeclaration": StringParameterDeclarationTypeDef,
         "DecimalParameterDeclaration": DecimalParameterDeclarationTypeDef,
         "IntegerParameterDeclaration": IntegerParameterDeclarationTypeDef,
         "DateTimeParameterDeclaration": DateTimeParameterDeclarationTypeDef,
     },
     total=False,
 )
 
+ColumnHierarchyOutputTypeDef = TypedDict(
+    "ColumnHierarchyOutputTypeDef",
+    {
+        "ExplicitHierarchy": ExplicitHierarchyOutputTypeDef,
+        "DateTimeHierarchy": DateTimeHierarchyOutputTypeDef,
+        "PredefinedHierarchy": PredefinedHierarchyOutputTypeDef,
+    },
+    total=False,
+)
+
 ColumnHierarchyTypeDef = TypedDict(
     "ColumnHierarchyTypeDef",
     {
         "ExplicitHierarchy": ExplicitHierarchyTypeDef,
         "DateTimeHierarchy": DateTimeHierarchyTypeDef,
         "PredefinedHierarchy": PredefinedHierarchyTypeDef,
     },
@@ -17157,15 +13902,15 @@
     },
 )
 
 _RequiredLogicalTableOutputTypeDef = TypedDict(
     "_RequiredLogicalTableOutputTypeDef",
     {
         "Alias": str,
-        "Source": LogicalTableSourceOutputTypeDef,
+        "Source": LogicalTableSourceTypeDef,
     },
 )
 _OptionalLogicalTableOutputTypeDef = TypedDict(
     "_OptionalLogicalTableOutputTypeDef",
     {
         "DataTransforms": List[TransformOperationOutputTypeDef],
     },
@@ -17225,69 +13970,80 @@
         "ParameterValueConfigurations": Sequence[SetParameterValueConfigurationTypeDef],
     },
 )
 
 AxisDisplayOptionsOutputTypeDef = TypedDict(
     "AxisDisplayOptionsOutputTypeDef",
     {
-        "TickLabelOptions": AxisTickLabelOptionsOutputTypeDef,
+        "TickLabelOptions": AxisTickLabelOptionsTypeDef,
         "AxisLineVisibility": VisibilityType,
         "GridLineVisibility": VisibilityType,
         "DataOptions": AxisDataOptionsOutputTypeDef,
-        "ScrollbarOptions": ScrollBarOptionsOutputTypeDef,
+        "ScrollbarOptions": ScrollBarOptionsTypeDef,
+        "AxisOffset": str,
+    },
+    total=False,
+)
+
+AxisDisplayOptionsTypeDef = TypedDict(
+    "AxisDisplayOptionsTypeDef",
+    {
+        "TickLabelOptions": AxisTickLabelOptionsTypeDef,
+        "AxisLineVisibility": VisibilityType,
+        "GridLineVisibility": VisibilityType,
+        "DataOptions": AxisDataOptionsTypeDef,
+        "ScrollbarOptions": ScrollBarOptionsTypeDef,
         "AxisOffset": str,
     },
     total=False,
 )
 
-_RequiredFilterDateTimePickerControlOutputTypeDef = TypedDict(
-    "_RequiredFilterDateTimePickerControlOutputTypeDef",
+_RequiredFilterDateTimePickerControlTypeDef = TypedDict(
+    "_RequiredFilterDateTimePickerControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
     },
 )
-_OptionalFilterDateTimePickerControlOutputTypeDef = TypedDict(
-    "_OptionalFilterDateTimePickerControlOutputTypeDef",
+_OptionalFilterDateTimePickerControlTypeDef = TypedDict(
+    "_OptionalFilterDateTimePickerControlTypeDef",
     {
-        "DisplayOptions": DateTimePickerControlDisplayOptionsOutputTypeDef,
+        "DisplayOptions": DateTimePickerControlDisplayOptionsTypeDef,
         "Type": SheetControlDateTimePickerTypeType,
     },
     total=False,
 )
 
 
-class FilterDateTimePickerControlOutputTypeDef(
-    _RequiredFilterDateTimePickerControlOutputTypeDef,
-    _OptionalFilterDateTimePickerControlOutputTypeDef,
+class FilterDateTimePickerControlTypeDef(
+    _RequiredFilterDateTimePickerControlTypeDef, _OptionalFilterDateTimePickerControlTypeDef
 ):
     pass
 
 
-_RequiredParameterDateTimePickerControlOutputTypeDef = TypedDict(
-    "_RequiredParameterDateTimePickerControlOutputTypeDef",
+_RequiredParameterDateTimePickerControlTypeDef = TypedDict(
+    "_RequiredParameterDateTimePickerControlTypeDef",
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
     },
 )
-_OptionalParameterDateTimePickerControlOutputTypeDef = TypedDict(
-    "_OptionalParameterDateTimePickerControlOutputTypeDef",
+_OptionalParameterDateTimePickerControlTypeDef = TypedDict(
+    "_OptionalParameterDateTimePickerControlTypeDef",
     {
-        "DisplayOptions": DateTimePickerControlDisplayOptionsOutputTypeDef,
+        "DisplayOptions": DateTimePickerControlDisplayOptionsTypeDef,
     },
     total=False,
 )
 
 
-class ParameterDateTimePickerControlOutputTypeDef(
-    _RequiredParameterDateTimePickerControlOutputTypeDef,
-    _OptionalParameterDateTimePickerControlOutputTypeDef,
+class ParameterDateTimePickerControlTypeDef(
+    _RequiredParameterDateTimePickerControlTypeDef, _OptionalParameterDateTimePickerControlTypeDef
 ):
     pass
 
 
 _RequiredFilterDropDownControlOutputTypeDef = TypedDict(
     "_RequiredFilterDropDownControlOutputTypeDef",
     {
@@ -17295,432 +14051,181 @@
         "Title": str,
         "SourceFilterId": str,
     },
 )
 _OptionalFilterDropDownControlOutputTypeDef = TypedDict(
     "_OptionalFilterDropDownControlOutputTypeDef",
     {
-        "DisplayOptions": DropDownControlDisplayOptionsOutputTypeDef,
+        "DisplayOptions": DropDownControlDisplayOptionsTypeDef,
         "Type": SheetControlListTypeType,
         "SelectableValues": FilterSelectableValuesOutputTypeDef,
         "CascadingControlConfiguration": CascadingControlConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 
 class FilterDropDownControlOutputTypeDef(
     _RequiredFilterDropDownControlOutputTypeDef, _OptionalFilterDropDownControlOutputTypeDef
 ):
     pass
 
 
-_RequiredParameterDropDownControlOutputTypeDef = TypedDict(
-    "_RequiredParameterDropDownControlOutputTypeDef",
-    {
-        "ParameterControlId": str,
-        "Title": str,
-        "SourceParameterName": str,
-    },
-)
-_OptionalParameterDropDownControlOutputTypeDef = TypedDict(
-    "_OptionalParameterDropDownControlOutputTypeDef",
-    {
-        "DisplayOptions": DropDownControlDisplayOptionsOutputTypeDef,
-        "Type": SheetControlListTypeType,
-        "SelectableValues": ParameterSelectableValuesOutputTypeDef,
-        "CascadingControlConfiguration": CascadingControlConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ParameterDropDownControlOutputTypeDef(
-    _RequiredParameterDropDownControlOutputTypeDef, _OptionalParameterDropDownControlOutputTypeDef
-):
-    pass
-
-
-_RequiredFilterListControlOutputTypeDef = TypedDict(
-    "_RequiredFilterListControlOutputTypeDef",
+_RequiredFilterDropDownControlTypeDef = TypedDict(
+    "_RequiredFilterDropDownControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
     },
 )
-_OptionalFilterListControlOutputTypeDef = TypedDict(
-    "_OptionalFilterListControlOutputTypeDef",
+_OptionalFilterDropDownControlTypeDef = TypedDict(
+    "_OptionalFilterDropDownControlTypeDef",
     {
-        "DisplayOptions": ListControlDisplayOptionsOutputTypeDef,
+        "DisplayOptions": DropDownControlDisplayOptionsTypeDef,
         "Type": SheetControlListTypeType,
-        "SelectableValues": FilterSelectableValuesOutputTypeDef,
-        "CascadingControlConfiguration": CascadingControlConfigurationOutputTypeDef,
+        "SelectableValues": FilterSelectableValuesTypeDef,
+        "CascadingControlConfiguration": CascadingControlConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class FilterListControlOutputTypeDef(
-    _RequiredFilterListControlOutputTypeDef, _OptionalFilterListControlOutputTypeDef
+class FilterDropDownControlTypeDef(
+    _RequiredFilterDropDownControlTypeDef, _OptionalFilterDropDownControlTypeDef
 ):
     pass
 
 
-_RequiredParameterListControlOutputTypeDef = TypedDict(
-    "_RequiredParameterListControlOutputTypeDef",
+_RequiredParameterDropDownControlOutputTypeDef = TypedDict(
+    "_RequiredParameterDropDownControlOutputTypeDef",
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
     },
 )
-_OptionalParameterListControlOutputTypeDef = TypedDict(
-    "_OptionalParameterListControlOutputTypeDef",
+_OptionalParameterDropDownControlOutputTypeDef = TypedDict(
+    "_OptionalParameterDropDownControlOutputTypeDef",
     {
-        "DisplayOptions": ListControlDisplayOptionsOutputTypeDef,
+        "DisplayOptions": DropDownControlDisplayOptionsTypeDef,
         "Type": SheetControlListTypeType,
         "SelectableValues": ParameterSelectableValuesOutputTypeDef,
         "CascadingControlConfiguration": CascadingControlConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 
-class ParameterListControlOutputTypeDef(
-    _RequiredParameterListControlOutputTypeDef, _OptionalParameterListControlOutputTypeDef
-):
-    pass
-
-
-_RequiredFilterRelativeDateTimeControlOutputTypeDef = TypedDict(
-    "_RequiredFilterRelativeDateTimeControlOutputTypeDef",
-    {
-        "FilterControlId": str,
-        "Title": str,
-        "SourceFilterId": str,
-    },
-)
-_OptionalFilterRelativeDateTimeControlOutputTypeDef = TypedDict(
-    "_OptionalFilterRelativeDateTimeControlOutputTypeDef",
-    {
-        "DisplayOptions": RelativeDateTimeControlDisplayOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class FilterRelativeDateTimeControlOutputTypeDef(
-    _RequiredFilterRelativeDateTimeControlOutputTypeDef,
-    _OptionalFilterRelativeDateTimeControlOutputTypeDef,
-):
-    pass
-
-
-_RequiredFilterSliderControlOutputTypeDef = TypedDict(
-    "_RequiredFilterSliderControlOutputTypeDef",
-    {
-        "FilterControlId": str,
-        "Title": str,
-        "SourceFilterId": str,
-        "MaximumValue": float,
-        "MinimumValue": float,
-        "StepSize": float,
-    },
-)
-_OptionalFilterSliderControlOutputTypeDef = TypedDict(
-    "_OptionalFilterSliderControlOutputTypeDef",
-    {
-        "DisplayOptions": SliderControlDisplayOptionsOutputTypeDef,
-        "Type": SheetControlSliderTypeType,
-    },
-    total=False,
-)
-
-
-class FilterSliderControlOutputTypeDef(
-    _RequiredFilterSliderControlOutputTypeDef, _OptionalFilterSliderControlOutputTypeDef
-):
-    pass
-
-
-_RequiredParameterSliderControlOutputTypeDef = TypedDict(
-    "_RequiredParameterSliderControlOutputTypeDef",
-    {
-        "ParameterControlId": str,
-        "Title": str,
-        "SourceParameterName": str,
-        "MaximumValue": float,
-        "MinimumValue": float,
-        "StepSize": float,
-    },
-)
-_OptionalParameterSliderControlOutputTypeDef = TypedDict(
-    "_OptionalParameterSliderControlOutputTypeDef",
-    {
-        "DisplayOptions": SliderControlDisplayOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ParameterSliderControlOutputTypeDef(
-    _RequiredParameterSliderControlOutputTypeDef, _OptionalParameterSliderControlOutputTypeDef
-):
-    pass
-
-
-_RequiredFilterTextAreaControlOutputTypeDef = TypedDict(
-    "_RequiredFilterTextAreaControlOutputTypeDef",
-    {
-        "FilterControlId": str,
-        "Title": str,
-        "SourceFilterId": str,
-    },
-)
-_OptionalFilterTextAreaControlOutputTypeDef = TypedDict(
-    "_OptionalFilterTextAreaControlOutputTypeDef",
-    {
-        "Delimiter": str,
-        "DisplayOptions": TextAreaControlDisplayOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class FilterTextAreaControlOutputTypeDef(
-    _RequiredFilterTextAreaControlOutputTypeDef, _OptionalFilterTextAreaControlOutputTypeDef
-):
-    pass
-
-
-_RequiredParameterTextAreaControlOutputTypeDef = TypedDict(
-    "_RequiredParameterTextAreaControlOutputTypeDef",
-    {
-        "ParameterControlId": str,
-        "Title": str,
-        "SourceParameterName": str,
-    },
-)
-_OptionalParameterTextAreaControlOutputTypeDef = TypedDict(
-    "_OptionalParameterTextAreaControlOutputTypeDef",
-    {
-        "Delimiter": str,
-        "DisplayOptions": TextAreaControlDisplayOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ParameterTextAreaControlOutputTypeDef(
-    _RequiredParameterTextAreaControlOutputTypeDef, _OptionalParameterTextAreaControlOutputTypeDef
-):
-    pass
-
-
-_RequiredFilterTextFieldControlOutputTypeDef = TypedDict(
-    "_RequiredFilterTextFieldControlOutputTypeDef",
-    {
-        "FilterControlId": str,
-        "Title": str,
-        "SourceFilterId": str,
-    },
-)
-_OptionalFilterTextFieldControlOutputTypeDef = TypedDict(
-    "_OptionalFilterTextFieldControlOutputTypeDef",
-    {
-        "DisplayOptions": TextFieldControlDisplayOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class FilterTextFieldControlOutputTypeDef(
-    _RequiredFilterTextFieldControlOutputTypeDef, _OptionalFilterTextFieldControlOutputTypeDef
+class ParameterDropDownControlOutputTypeDef(
+    _RequiredParameterDropDownControlOutputTypeDef, _OptionalParameterDropDownControlOutputTypeDef
 ):
     pass
 
 
-_RequiredParameterTextFieldControlOutputTypeDef = TypedDict(
-    "_RequiredParameterTextFieldControlOutputTypeDef",
+_RequiredParameterDropDownControlTypeDef = TypedDict(
+    "_RequiredParameterDropDownControlTypeDef",
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
     },
 )
-_OptionalParameterTextFieldControlOutputTypeDef = TypedDict(
-    "_OptionalParameterTextFieldControlOutputTypeDef",
+_OptionalParameterDropDownControlTypeDef = TypedDict(
+    "_OptionalParameterDropDownControlTypeDef",
     {
-        "DisplayOptions": TextFieldControlDisplayOptionsOutputTypeDef,
+        "DisplayOptions": DropDownControlDisplayOptionsTypeDef,
+        "Type": SheetControlListTypeType,
+        "SelectableValues": ParameterSelectableValuesTypeDef,
+        "CascadingControlConfiguration": CascadingControlConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class ParameterTextFieldControlOutputTypeDef(
-    _RequiredParameterTextFieldControlOutputTypeDef, _OptionalParameterTextFieldControlOutputTypeDef
+class ParameterDropDownControlTypeDef(
+    _RequiredParameterDropDownControlTypeDef, _OptionalParameterDropDownControlTypeDef
 ):
     pass
 
 
-SmallMultiplesOptionsOutputTypeDef = TypedDict(
-    "SmallMultiplesOptionsOutputTypeDef",
-    {
-        "MaxVisibleRows": int,
-        "MaxVisibleColumns": int,
-        "PanelConfiguration": PanelConfigurationOutputTypeDef,
-        "XAxis": SmallMultiplesAxisPropertiesOutputTypeDef,
-        "YAxis": SmallMultiplesAxisPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
-TableFieldLinkConfigurationOutputTypeDef = TypedDict(
-    "TableFieldLinkConfigurationOutputTypeDef",
-    {
-        "Target": URLTargetConfigurationType,
-        "Content": TableFieldLinkContentConfigurationOutputTypeDef,
-    },
-)
-
-AxisDisplayOptionsTypeDef = TypedDict(
-    "AxisDisplayOptionsTypeDef",
-    {
-        "TickLabelOptions": AxisTickLabelOptionsTypeDef,
-        "AxisLineVisibility": VisibilityType,
-        "GridLineVisibility": VisibilityType,
-        "DataOptions": AxisDataOptionsTypeDef,
-        "ScrollbarOptions": ScrollBarOptionsTypeDef,
-        "AxisOffset": str,
-    },
-    total=False,
-)
-
-_RequiredFilterDateTimePickerControlTypeDef = TypedDict(
-    "_RequiredFilterDateTimePickerControlTypeDef",
+_RequiredFilterListControlOutputTypeDef = TypedDict(
+    "_RequiredFilterListControlOutputTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
     },
 )
-_OptionalFilterDateTimePickerControlTypeDef = TypedDict(
-    "_OptionalFilterDateTimePickerControlTypeDef",
-    {
-        "DisplayOptions": DateTimePickerControlDisplayOptionsTypeDef,
-        "Type": SheetControlDateTimePickerTypeType,
-    },
-    total=False,
-)
-
-
-class FilterDateTimePickerControlTypeDef(
-    _RequiredFilterDateTimePickerControlTypeDef, _OptionalFilterDateTimePickerControlTypeDef
-):
-    pass
-
-
-_RequiredParameterDateTimePickerControlTypeDef = TypedDict(
-    "_RequiredParameterDateTimePickerControlTypeDef",
-    {
-        "ParameterControlId": str,
-        "Title": str,
-        "SourceParameterName": str,
-    },
-)
-_OptionalParameterDateTimePickerControlTypeDef = TypedDict(
-    "_OptionalParameterDateTimePickerControlTypeDef",
+_OptionalFilterListControlOutputTypeDef = TypedDict(
+    "_OptionalFilterListControlOutputTypeDef",
     {
-        "DisplayOptions": DateTimePickerControlDisplayOptionsTypeDef,
+        "DisplayOptions": ListControlDisplayOptionsTypeDef,
+        "Type": SheetControlListTypeType,
+        "SelectableValues": FilterSelectableValuesOutputTypeDef,
+        "CascadingControlConfiguration": CascadingControlConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 
-class ParameterDateTimePickerControlTypeDef(
-    _RequiredParameterDateTimePickerControlTypeDef, _OptionalParameterDateTimePickerControlTypeDef
+class FilterListControlOutputTypeDef(
+    _RequiredFilterListControlOutputTypeDef, _OptionalFilterListControlOutputTypeDef
 ):
     pass
 
 
-_RequiredFilterDropDownControlTypeDef = TypedDict(
-    "_RequiredFilterDropDownControlTypeDef",
+_RequiredFilterListControlTypeDef = TypedDict(
+    "_RequiredFilterListControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
     },
 )
-_OptionalFilterDropDownControlTypeDef = TypedDict(
-    "_OptionalFilterDropDownControlTypeDef",
+_OptionalFilterListControlTypeDef = TypedDict(
+    "_OptionalFilterListControlTypeDef",
     {
-        "DisplayOptions": DropDownControlDisplayOptionsTypeDef,
+        "DisplayOptions": ListControlDisplayOptionsTypeDef,
         "Type": SheetControlListTypeType,
         "SelectableValues": FilterSelectableValuesTypeDef,
         "CascadingControlConfiguration": CascadingControlConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class FilterDropDownControlTypeDef(
-    _RequiredFilterDropDownControlTypeDef, _OptionalFilterDropDownControlTypeDef
+class FilterListControlTypeDef(
+    _RequiredFilterListControlTypeDef, _OptionalFilterListControlTypeDef
 ):
     pass
 
 
-_RequiredParameterDropDownControlTypeDef = TypedDict(
-    "_RequiredParameterDropDownControlTypeDef",
+_RequiredParameterListControlOutputTypeDef = TypedDict(
+    "_RequiredParameterListControlOutputTypeDef",
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
     },
 )
-_OptionalParameterDropDownControlTypeDef = TypedDict(
-    "_OptionalParameterDropDownControlTypeDef",
-    {
-        "DisplayOptions": DropDownControlDisplayOptionsTypeDef,
-        "Type": SheetControlListTypeType,
-        "SelectableValues": ParameterSelectableValuesTypeDef,
-        "CascadingControlConfiguration": CascadingControlConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class ParameterDropDownControlTypeDef(
-    _RequiredParameterDropDownControlTypeDef, _OptionalParameterDropDownControlTypeDef
-):
-    pass
-
-
-_RequiredFilterListControlTypeDef = TypedDict(
-    "_RequiredFilterListControlTypeDef",
-    {
-        "FilterControlId": str,
-        "Title": str,
-        "SourceFilterId": str,
-    },
-)
-_OptionalFilterListControlTypeDef = TypedDict(
-    "_OptionalFilterListControlTypeDef",
+_OptionalParameterListControlOutputTypeDef = TypedDict(
+    "_OptionalParameterListControlOutputTypeDef",
     {
         "DisplayOptions": ListControlDisplayOptionsTypeDef,
         "Type": SheetControlListTypeType,
-        "SelectableValues": FilterSelectableValuesTypeDef,
-        "CascadingControlConfiguration": CascadingControlConfigurationTypeDef,
+        "SelectableValues": ParameterSelectableValuesOutputTypeDef,
+        "CascadingControlConfiguration": CascadingControlConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 
-class FilterListControlTypeDef(
-    _RequiredFilterListControlTypeDef, _OptionalFilterListControlTypeDef
+class ParameterListControlOutputTypeDef(
+    _RequiredParameterListControlOutputTypeDef, _OptionalParameterListControlOutputTypeDef
 ):
     pass
 
 
 _RequiredParameterListControlTypeDef = TypedDict(
     "_RequiredParameterListControlTypeDef",
     {
@@ -17940,75 +14445,24 @@
 PivotTableOptionsOutputTypeDef = TypedDict(
     "PivotTableOptionsOutputTypeDef",
     {
         "MetricPlacement": PivotTableMetricPlacementType,
         "SingleMetricVisibility": VisibilityType,
         "ColumnNamesVisibility": VisibilityType,
         "ToggleButtonsVisibility": VisibilityType,
-        "ColumnHeaderStyle": TableCellStyleOutputTypeDef,
-        "RowHeaderStyle": TableCellStyleOutputTypeDef,
-        "CellStyle": TableCellStyleOutputTypeDef,
-        "RowFieldNamesStyle": TableCellStyleOutputTypeDef,
+        "ColumnHeaderStyle": TableCellStyleTypeDef,
+        "RowHeaderStyle": TableCellStyleTypeDef,
+        "CellStyle": TableCellStyleTypeDef,
+        "RowFieldNamesStyle": TableCellStyleTypeDef,
         "RowAlternateColorOptions": RowAlternateColorOptionsOutputTypeDef,
         "CollapsedRowDimensionsVisibility": VisibilityType,
     },
     total=False,
 )
 
-PivotTotalOptionsOutputTypeDef = TypedDict(
-    "PivotTotalOptionsOutputTypeDef",
-    {
-        "TotalsVisibility": VisibilityType,
-        "Placement": TableTotalsPlacementType,
-        "ScrollStatus": TableTotalsScrollStatusType,
-        "CustomLabel": str,
-        "TotalCellStyle": TableCellStyleOutputTypeDef,
-        "ValueCellStyle": TableCellStyleOutputTypeDef,
-        "MetricHeaderCellStyle": TableCellStyleOutputTypeDef,
-    },
-    total=False,
-)
-
-SubtotalOptionsOutputTypeDef = TypedDict(
-    "SubtotalOptionsOutputTypeDef",
-    {
-        "TotalsVisibility": VisibilityType,
-        "CustomLabel": str,
-        "FieldLevel": PivotTableSubtotalLevelType,
-        "FieldLevelOptions": List[PivotTableFieldSubtotalOptionsOutputTypeDef],
-        "TotalCellStyle": TableCellStyleOutputTypeDef,
-        "ValueCellStyle": TableCellStyleOutputTypeDef,
-        "MetricHeaderCellStyle": TableCellStyleOutputTypeDef,
-    },
-    total=False,
-)
-
-TableOptionsOutputTypeDef = TypedDict(
-    "TableOptionsOutputTypeDef",
-    {
-        "Orientation": TableOrientationType,
-        "HeaderStyle": TableCellStyleOutputTypeDef,
-        "CellStyle": TableCellStyleOutputTypeDef,
-        "RowAlternateColorOptions": RowAlternateColorOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-TotalOptionsOutputTypeDef = TypedDict(
-    "TotalOptionsOutputTypeDef",
-    {
-        "TotalsVisibility": VisibilityType,
-        "Placement": TableTotalsPlacementType,
-        "ScrollStatus": TableTotalsScrollStatusType,
-        "CustomLabel": str,
-        "TotalCellStyle": TableCellStyleOutputTypeDef,
-    },
-    total=False,
-)
-
 PivotTableOptionsTypeDef = TypedDict(
     "PivotTableOptionsTypeDef",
     {
         "MetricPlacement": PivotTableMetricPlacementType,
         "SingleMetricVisibility": VisibilityType,
         "ColumnNamesVisibility": VisibilityType,
         "ToggleButtonsVisibility": VisibilityType,
@@ -18032,28 +14486,53 @@
         "TotalCellStyle": TableCellStyleTypeDef,
         "ValueCellStyle": TableCellStyleTypeDef,
         "MetricHeaderCellStyle": TableCellStyleTypeDef,
     },
     total=False,
 )
 
+SubtotalOptionsOutputTypeDef = TypedDict(
+    "SubtotalOptionsOutputTypeDef",
+    {
+        "TotalsVisibility": VisibilityType,
+        "CustomLabel": str,
+        "FieldLevel": PivotTableSubtotalLevelType,
+        "FieldLevelOptions": List[PivotTableFieldSubtotalOptionsTypeDef],
+        "TotalCellStyle": TableCellStyleTypeDef,
+        "ValueCellStyle": TableCellStyleTypeDef,
+        "MetricHeaderCellStyle": TableCellStyleTypeDef,
+    },
+    total=False,
+)
+
 SubtotalOptionsTypeDef = TypedDict(
     "SubtotalOptionsTypeDef",
     {
         "TotalsVisibility": VisibilityType,
         "CustomLabel": str,
         "FieldLevel": PivotTableSubtotalLevelType,
         "FieldLevelOptions": Sequence[PivotTableFieldSubtotalOptionsTypeDef],
         "TotalCellStyle": TableCellStyleTypeDef,
         "ValueCellStyle": TableCellStyleTypeDef,
         "MetricHeaderCellStyle": TableCellStyleTypeDef,
     },
     total=False,
 )
 
+TableOptionsOutputTypeDef = TypedDict(
+    "TableOptionsOutputTypeDef",
+    {
+        "Orientation": TableOrientationType,
+        "HeaderStyle": TableCellStyleTypeDef,
+        "CellStyle": TableCellStyleTypeDef,
+        "RowAlternateColorOptions": RowAlternateColorOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 TableOptionsTypeDef = TypedDict(
     "TableOptionsTypeDef",
     {
         "Orientation": TableOrientationType,
         "HeaderStyle": TableCellStyleTypeDef,
         "CellStyle": TableCellStyleTypeDef,
         "RowAlternateColorOptions": RowAlternateColorOptionsTypeDef,
@@ -18081,24 +14560,24 @@
     total=False,
 )
 
 GaugeChartPrimaryValueConditionalFormattingOutputTypeDef = TypedDict(
     "GaugeChartPrimaryValueConditionalFormattingOutputTypeDef",
     {
         "TextColor": ConditionalFormattingColorOutputTypeDef,
-        "Icon": ConditionalFormattingIconOutputTypeDef,
+        "Icon": ConditionalFormattingIconTypeDef,
     },
     total=False,
 )
 
 KPIPrimaryValueConditionalFormattingOutputTypeDef = TypedDict(
     "KPIPrimaryValueConditionalFormattingOutputTypeDef",
     {
         "TextColor": ConditionalFormattingColorOutputTypeDef,
-        "Icon": ConditionalFormattingIconOutputTypeDef,
+        "Icon": ConditionalFormattingIconTypeDef,
     },
     total=False,
 )
 
 KPIProgressBarConditionalFormattingOutputTypeDef = TypedDict(
     "KPIProgressBarConditionalFormattingOutputTypeDef",
     {
@@ -18124,15 +14603,15 @@
 )
 
 TextConditionalFormatOutputTypeDef = TypedDict(
     "TextConditionalFormatOutputTypeDef",
     {
         "BackgroundColor": ConditionalFormattingColorOutputTypeDef,
         "TextColor": ConditionalFormattingColorOutputTypeDef,
-        "Icon": ConditionalFormattingIconOutputTypeDef,
+        "Icon": ConditionalFormattingIconTypeDef,
     },
     total=False,
 )
 
 GaugeChartArcConditionalFormattingTypeDef = TypedDict(
     "GaugeChartArcConditionalFormattingTypeDef",
     {
@@ -18208,15 +14687,15 @@
 )
 
 DescribeDataSetRefreshPropertiesResponseTypeDef = TypedDict(
     "DescribeDataSetRefreshPropertiesResponseTypeDef",
     {
         "RequestId": str,
         "Status": int,
-        "DataSetRefreshProperties": DataSetRefreshPropertiesOutputTypeDef,
+        "DataSetRefreshProperties": DataSetRefreshPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDataSetRefreshPropertiesRequestRequestTypeDef = TypedDict(
     "PutDataSetRefreshPropertiesRequestRequestTypeDef",
     {
@@ -18226,50 +14705,29 @@
     },
 )
 
 AssetBundleImportJobOverrideParametersOutputTypeDef = TypedDict(
     "AssetBundleImportJobOverrideParametersOutputTypeDef",
     {
         "ResourceIdOverrideConfiguration": (
-            AssetBundleImportJobResourceIdOverrideConfigurationOutputTypeDef
+            AssetBundleImportJobResourceIdOverrideConfigurationTypeDef
         ),
         "VPCConnections": List[AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef],
         "RefreshSchedules": List[
             AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef
         ],
-        "DataSources": List[AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef],
-        "DataSets": List[AssetBundleImportJobDataSetOverrideParametersOutputTypeDef],
-        "Themes": List[AssetBundleImportJobThemeOverrideParametersOutputTypeDef],
-        "Analyses": List[AssetBundleImportJobAnalysisOverrideParametersOutputTypeDef],
-        "Dashboards": List[AssetBundleImportJobDashboardOverrideParametersOutputTypeDef],
+        "DataSources": List[AssetBundleImportJobDataSourceOverrideParametersTypeDef],
+        "DataSets": List[AssetBundleImportJobDataSetOverrideParametersTypeDef],
+        "Themes": List[AssetBundleImportJobThemeOverrideParametersTypeDef],
+        "Analyses": List[AssetBundleImportJobAnalysisOverrideParametersTypeDef],
+        "Dashboards": List[AssetBundleImportJobDashboardOverrideParametersTypeDef],
     },
     total=False,
 )
 
-DescribeDataSourceResponseTypeDef = TypedDict(
-    "DescribeDataSourceResponseTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataSourcesResponseTypeDef = TypedDict(
-    "ListDataSourcesResponseTypeDef",
-    {
-        "DataSources": List[DataSourceTypeDef],
-        "NextToken": str,
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AssetBundleImportJobOverrideParametersTypeDef = TypedDict(
     "AssetBundleImportJobOverrideParametersTypeDef",
     {
         "ResourceIdOverrideConfiguration": (
             AssetBundleImportJobResourceIdOverrideConfigurationTypeDef
         ),
         "VPCConnections": Sequence[AssetBundleImportJobVPCConnectionOverrideParametersTypeDef],
@@ -18289,14 +14747,35 @@
         "CredentialPair": CredentialPairTypeDef,
         "CopySourceArn": str,
         "SecretArn": str,
     },
     total=False,
 )
 
+DescribeDataSourceResponseTypeDef = TypedDict(
+    "DescribeDataSourceResponseTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDataSourcesResponseTypeDef = TypedDict(
+    "ListDataSourcesResponseTypeDef",
+    {
+        "DataSources": List[DataSourceTypeDef],
+        "NextToken": str,
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ThemeVersionTypeDef = TypedDict(
     "ThemeVersionTypeDef",
     {
         "VersionNumber": int,
         "Arn": str,
         "Description": str,
         "BaseThemeId": str,
@@ -18356,59 +14835,14 @@
 
 class UpdateThemeRequestRequestTypeDef(
     _RequiredUpdateThemeRequestRequestTypeDef, _OptionalUpdateThemeRequestRequestTypeDef
 ):
     pass
 
 
-ComparisonConfigurationOutputTypeDef = TypedDict(
-    "ComparisonConfigurationOutputTypeDef",
-    {
-        "ComparisonMethod": ComparisonMethodType,
-        "ComparisonFormat": ComparisonFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-DateTimeFormatConfigurationOutputTypeDef = TypedDict(
-    "DateTimeFormatConfigurationOutputTypeDef",
-    {
-        "DateTimeFormat": str,
-        "NullValueFormatConfiguration": NullValueFormatConfigurationOutputTypeDef,
-        "NumericFormatConfiguration": NumericFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-NumberFormatConfigurationOutputTypeDef = TypedDict(
-    "NumberFormatConfigurationOutputTypeDef",
-    {
-        "FormatConfiguration": NumericFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-ReferenceLineValueLabelConfigurationOutputTypeDef = TypedDict(
-    "ReferenceLineValueLabelConfigurationOutputTypeDef",
-    {
-        "RelativePosition": ReferenceLineValueLabelRelativePositionType,
-        "FormatConfiguration": NumericFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-StringFormatConfigurationOutputTypeDef = TypedDict(
-    "StringFormatConfigurationOutputTypeDef",
-    {
-        "NullValueFormatConfiguration": NullValueFormatConfigurationOutputTypeDef,
-        "NumericFormatConfiguration": NumericFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ComparisonConfigurationTypeDef = TypedDict(
     "ComparisonConfigurationTypeDef",
     {
         "ComparisonMethod": ComparisonMethodType,
         "ComparisonFormat": ComparisonFormatConfigurationTypeDef,
     },
     total=False,
@@ -18450,16 +14884,16 @@
     total=False,
 )
 
 _RequiredTopBottomFilterOutputTypeDef = TypedDict(
     "_RequiredTopBottomFilterOutputTypeDef",
     {
         "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-        "AggregationSortConfigurations": List[AggregationSortConfigurationOutputTypeDef],
+        "Column": ColumnIdentifierTypeDef,
+        "AggregationSortConfigurations": List[AggregationSortConfigurationTypeDef],
     },
 )
 _OptionalTopBottomFilterOutputTypeDef = TypedDict(
     "_OptionalTopBottomFilterOutputTypeDef",
     {
         "Limit": int,
         "TimeGranularity": TimeGranularityType,
@@ -18471,52 +14905,14 @@
 
 class TopBottomFilterOutputTypeDef(
     _RequiredTopBottomFilterOutputTypeDef, _OptionalTopBottomFilterOutputTypeDef
 ):
     pass
 
 
-FieldSortOptionsOutputTypeDef = TypedDict(
-    "FieldSortOptionsOutputTypeDef",
-    {
-        "FieldSort": FieldSortOutputTypeDef,
-        "ColumnSort": ColumnSortOutputTypeDef,
-    },
-    total=False,
-)
-
-PivotTableSortByOutputTypeDef = TypedDict(
-    "PivotTableSortByOutputTypeDef",
-    {
-        "Field": FieldSortOutputTypeDef,
-        "Column": ColumnSortOutputTypeDef,
-        "DataPath": DataPathSortOutputTypeDef,
-    },
-    total=False,
-)
-
-TooltipItemOutputTypeDef = TypedDict(
-    "TooltipItemOutputTypeDef",
-    {
-        "FieldTooltipItem": FieldTooltipItemOutputTypeDef,
-        "ColumnTooltipItem": ColumnTooltipItemOutputTypeDef,
-    },
-    total=False,
-)
-
-ReferenceLineDataConfigurationOutputTypeDef = TypedDict(
-    "ReferenceLineDataConfigurationOutputTypeDef",
-    {
-        "StaticConfiguration": ReferenceLineStaticDataConfigurationOutputTypeDef,
-        "DynamicConfiguration": ReferenceLineDynamicDataConfigurationOutputTypeDef,
-        "AxisBinding": AxisBindingType,
-    },
-    total=False,
-)
-
 _RequiredTopBottomFilterTypeDef = TypedDict(
     "_RequiredTopBottomFilterTypeDef",
     {
         "FilterId": str,
         "Column": ColumnIdentifierTypeDef,
         "AggregationSortConfigurations": Sequence[AggregationSortConfigurationTypeDef],
     },
@@ -18541,14 +14937,24 @@
     {
         "FieldSort": FieldSortTypeDef,
         "ColumnSort": ColumnSortTypeDef,
     },
     total=False,
 )
 
+PivotTableSortByOutputTypeDef = TypedDict(
+    "PivotTableSortByOutputTypeDef",
+    {
+        "Field": FieldSortTypeDef,
+        "Column": ColumnSortTypeDef,
+        "DataPath": DataPathSortOutputTypeDef,
+    },
+    total=False,
+)
+
 PivotTableSortByTypeDef = TypedDict(
     "PivotTableSortByTypeDef",
     {
         "Field": FieldSortTypeDef,
         "Column": ColumnSortTypeDef,
         "DataPath": DataPathSortTypeDef,
     },
@@ -18581,15 +14987,15 @@
     },
 )
 _OptionalDatasetMetadataOutputTypeDef = TypedDict(
     "_OptionalDatasetMetadataOutputTypeDef",
     {
         "DatasetName": str,
         "DatasetDescription": str,
-        "DataAggregation": DataAggregationOutputTypeDef,
+        "DataAggregation": DataAggregationTypeDef,
         "Filters": List[TopicFilterOutputTypeDef],
         "Columns": List[TopicColumnOutputTypeDef],
         "CalculatedFields": List[TopicCalculatedFieldOutputTypeDef],
         "NamedEntities": List[TopicNamedEntityOutputTypeDef],
     },
     total=False,
 )
@@ -18655,22 +15061,14 @@
     "AnonymousUserSnapshotJobResultTypeDef",
     {
         "FileGroups": List[SnapshotJobResultFileGroupTypeDef],
     },
     total=False,
 )
 
-DefaultPaginatedLayoutConfigurationOutputTypeDef = TypedDict(
-    "DefaultPaginatedLayoutConfigurationOutputTypeDef",
-    {
-        "SectionBased": DefaultSectionBasedLayoutConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 DefaultPaginatedLayoutConfigurationTypeDef = TypedDict(
     "DefaultPaginatedLayoutConfigurationTypeDef",
     {
         "SectionBased": DefaultSectionBasedLayoutConfigurationTypeDef,
     },
     total=False,
 )
@@ -18729,18 +15127,18 @@
         "PhysicalTableMap": Dict[str, PhysicalTableOutputTypeDef],
         "LogicalTableMap": Dict[str, LogicalTableOutputTypeDef],
         "OutputColumns": List[OutputColumnTypeDef],
         "ImportMode": DataSetImportModeType,
         "ConsumedSpiceCapacityInBytes": int,
         "ColumnGroups": List[ColumnGroupOutputTypeDef],
         "FieldFolders": Dict[str, FieldFolderOutputTypeDef],
-        "RowLevelPermissionDataSet": RowLevelPermissionDataSetOutputTypeDef,
+        "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
         "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationOutputTypeDef,
         "ColumnLevelPermissionRules": List[ColumnLevelPermissionRuleOutputTypeDef],
-        "DataSetUsageConfiguration": DataSetUsageConfigurationOutputTypeDef,
+        "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
         "DatasetParameters": List[DatasetParameterOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateDataSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSetRequestRequestTypeDef",
@@ -18818,16 +15216,16 @@
     },
 )
 
 VisualCustomActionOperationOutputTypeDef = TypedDict(
     "VisualCustomActionOperationOutputTypeDef",
     {
         "FilterOperation": CustomActionFilterOperationOutputTypeDef,
-        "NavigationOperation": CustomActionNavigationOperationOutputTypeDef,
-        "URLOperation": CustomActionURLOperationOutputTypeDef,
+        "NavigationOperation": CustomActionNavigationOperationTypeDef,
+        "URLOperation": CustomActionURLOperationTypeDef,
         "SetParametersOperation": CustomActionSetParametersOperationOutputTypeDef,
     },
     total=False,
 )
 
 VisualCustomActionOperationTypeDef = TypedDict(
     "VisualCustomActionOperationTypeDef",
@@ -18840,60 +15238,38 @@
     total=False,
 )
 
 LineSeriesAxisDisplayOptionsOutputTypeDef = TypedDict(
     "LineSeriesAxisDisplayOptionsOutputTypeDef",
     {
         "AxisOptions": AxisDisplayOptionsOutputTypeDef,
-        "MissingDataConfigurations": List[MissingDataConfigurationOutputTypeDef],
-    },
-    total=False,
-)
-
-FilterControlOutputTypeDef = TypedDict(
-    "FilterControlOutputTypeDef",
-    {
-        "DateTimePicker": FilterDateTimePickerControlOutputTypeDef,
-        "List": FilterListControlOutputTypeDef,
-        "Dropdown": FilterDropDownControlOutputTypeDef,
-        "TextField": FilterTextFieldControlOutputTypeDef,
-        "TextArea": FilterTextAreaControlOutputTypeDef,
-        "Slider": FilterSliderControlOutputTypeDef,
-        "RelativeDateTime": FilterRelativeDateTimeControlOutputTypeDef,
-    },
-    total=False,
-)
-
-ParameterControlOutputTypeDef = TypedDict(
-    "ParameterControlOutputTypeDef",
-    {
-        "DateTimePicker": ParameterDateTimePickerControlOutputTypeDef,
-        "List": ParameterListControlOutputTypeDef,
-        "Dropdown": ParameterDropDownControlOutputTypeDef,
-        "TextField": ParameterTextFieldControlOutputTypeDef,
-        "TextArea": ParameterTextAreaControlOutputTypeDef,
-        "Slider": ParameterSliderControlOutputTypeDef,
+        "MissingDataConfigurations": List[MissingDataConfigurationTypeDef],
     },
     total=False,
 )
 
-TableFieldURLConfigurationOutputTypeDef = TypedDict(
-    "TableFieldURLConfigurationOutputTypeDef",
+LineSeriesAxisDisplayOptionsTypeDef = TypedDict(
+    "LineSeriesAxisDisplayOptionsTypeDef",
     {
-        "LinkConfiguration": TableFieldLinkConfigurationOutputTypeDef,
-        "ImageConfiguration": TableFieldImageConfigurationOutputTypeDef,
+        "AxisOptions": AxisDisplayOptionsTypeDef,
+        "MissingDataConfigurations": Sequence[MissingDataConfigurationTypeDef],
     },
     total=False,
 )
 
-LineSeriesAxisDisplayOptionsTypeDef = TypedDict(
-    "LineSeriesAxisDisplayOptionsTypeDef",
+FilterControlOutputTypeDef = TypedDict(
+    "FilterControlOutputTypeDef",
     {
-        "AxisOptions": AxisDisplayOptionsTypeDef,
-        "MissingDataConfigurations": Sequence[MissingDataConfigurationTypeDef],
+        "DateTimePicker": FilterDateTimePickerControlTypeDef,
+        "List": FilterListControlOutputTypeDef,
+        "Dropdown": FilterDropDownControlOutputTypeDef,
+        "TextField": FilterTextFieldControlTypeDef,
+        "TextArea": FilterTextAreaControlTypeDef,
+        "Slider": FilterSliderControlTypeDef,
+        "RelativeDateTime": FilterRelativeDateTimeControlTypeDef,
     },
     total=False,
 )
 
 FilterControlTypeDef = TypedDict(
     "FilterControlTypeDef",
     {
@@ -18904,14 +15280,27 @@
         "TextArea": FilterTextAreaControlTypeDef,
         "Slider": FilterSliderControlTypeDef,
         "RelativeDateTime": FilterRelativeDateTimeControlTypeDef,
     },
     total=False,
 )
 
+ParameterControlOutputTypeDef = TypedDict(
+    "ParameterControlOutputTypeDef",
+    {
+        "DateTimePicker": ParameterDateTimePickerControlTypeDef,
+        "List": ParameterListControlOutputTypeDef,
+        "Dropdown": ParameterDropDownControlOutputTypeDef,
+        "TextField": ParameterTextFieldControlTypeDef,
+        "TextArea": ParameterTextAreaControlTypeDef,
+        "Slider": ParameterSliderControlTypeDef,
+    },
+    total=False,
+)
+
 ParameterControlTypeDef = TypedDict(
     "ParameterControlTypeDef",
     {
         "DateTimePicker": ParameterDateTimePickerControlTypeDef,
         "List": ParameterListControlTypeDef,
         "Dropdown": ParameterDropDownControlTypeDef,
         "TextField": ParameterTextFieldControlTypeDef,
@@ -18931,16 +15320,16 @@
 )
 
 PivotTableTotalOptionsOutputTypeDef = TypedDict(
     "PivotTableTotalOptionsOutputTypeDef",
     {
         "RowSubtotalOptions": SubtotalOptionsOutputTypeDef,
         "ColumnSubtotalOptions": SubtotalOptionsOutputTypeDef,
-        "RowTotalOptions": PivotTotalOptionsOutputTypeDef,
-        "ColumnTotalOptions": PivotTotalOptionsOutputTypeDef,
+        "RowTotalOptions": PivotTotalOptionsTypeDef,
+        "ColumnTotalOptions": PivotTotalOptionsTypeDef,
     },
     total=False,
 )
 
 PivotTableTotalOptionsTypeDef = TypedDict(
     "PivotTableTotalOptionsTypeDef",
     {
@@ -18998,16 +15387,16 @@
         "FieldId": str,
     },
 )
 _OptionalPivotTableCellConditionalFormattingOutputTypeDef = TypedDict(
     "_OptionalPivotTableCellConditionalFormattingOutputTypeDef",
     {
         "TextFormat": TextConditionalFormatOutputTypeDef,
-        "Scope": PivotTableConditionalFormattingScopeOutputTypeDef,
-        "Scopes": List[PivotTableConditionalFormattingScopeOutputTypeDef],
+        "Scope": PivotTableConditionalFormattingScopeTypeDef,
+        "Scopes": List[PivotTableConditionalFormattingScopeTypeDef],
     },
     total=False,
 )
 
 
 class PivotTableCellConditionalFormattingOutputTypeDef(
     _RequiredPivotTableCellConditionalFormattingOutputTypeDef,
@@ -19232,202 +15621,14 @@
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
         "Type": ThemeTypeType,
     },
     total=False,
 )
 
-GaugeChartOptionsOutputTypeDef = TypedDict(
-    "GaugeChartOptionsOutputTypeDef",
-    {
-        "PrimaryValueDisplayType": PrimaryValueDisplayTypeType,
-        "Comparison": ComparisonConfigurationOutputTypeDef,
-        "ArcAxis": ArcAxisConfigurationOutputTypeDef,
-        "Arc": ArcConfigurationOutputTypeDef,
-        "PrimaryValueFontConfiguration": FontConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-KPIOptionsOutputTypeDef = TypedDict(
-    "KPIOptionsOutputTypeDef",
-    {
-        "ProgressBar": ProgressBarOptionsOutputTypeDef,
-        "TrendArrows": TrendArrowOptionsOutputTypeDef,
-        "SecondaryValue": SecondaryValueOptionsOutputTypeDef,
-        "Comparison": ComparisonConfigurationOutputTypeDef,
-        "PrimaryValueDisplayType": PrimaryValueDisplayTypeType,
-        "PrimaryValueFontConfiguration": FontConfigurationOutputTypeDef,
-        "SecondaryValueFontConfiguration": FontConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDateDimensionFieldOutputTypeDef = TypedDict(
-    "_RequiredDateDimensionFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalDateDimensionFieldOutputTypeDef = TypedDict(
-    "_OptionalDateDimensionFieldOutputTypeDef",
-    {
-        "DateGranularity": TimeGranularityType,
-        "HierarchyId": str,
-        "FormatConfiguration": DateTimeFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class DateDimensionFieldOutputTypeDef(
-    _RequiredDateDimensionFieldOutputTypeDef, _OptionalDateDimensionFieldOutputTypeDef
-):
-    pass
-
-
-_RequiredDateMeasureFieldOutputTypeDef = TypedDict(
-    "_RequiredDateMeasureFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalDateMeasureFieldOutputTypeDef = TypedDict(
-    "_OptionalDateMeasureFieldOutputTypeDef",
-    {
-        "AggregationFunction": DateAggregationFunctionType,
-        "FormatConfiguration": DateTimeFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class DateMeasureFieldOutputTypeDef(
-    _RequiredDateMeasureFieldOutputTypeDef, _OptionalDateMeasureFieldOutputTypeDef
-):
-    pass
-
-
-_RequiredNumericalDimensionFieldOutputTypeDef = TypedDict(
-    "_RequiredNumericalDimensionFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalNumericalDimensionFieldOutputTypeDef = TypedDict(
-    "_OptionalNumericalDimensionFieldOutputTypeDef",
-    {
-        "HierarchyId": str,
-        "FormatConfiguration": NumberFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class NumericalDimensionFieldOutputTypeDef(
-    _RequiredNumericalDimensionFieldOutputTypeDef, _OptionalNumericalDimensionFieldOutputTypeDef
-):
-    pass
-
-
-_RequiredNumericalMeasureFieldOutputTypeDef = TypedDict(
-    "_RequiredNumericalMeasureFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalNumericalMeasureFieldOutputTypeDef = TypedDict(
-    "_OptionalNumericalMeasureFieldOutputTypeDef",
-    {
-        "AggregationFunction": NumericalAggregationFunctionOutputTypeDef,
-        "FormatConfiguration": NumberFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class NumericalMeasureFieldOutputTypeDef(
-    _RequiredNumericalMeasureFieldOutputTypeDef, _OptionalNumericalMeasureFieldOutputTypeDef
-):
-    pass
-
-
-ReferenceLineLabelConfigurationOutputTypeDef = TypedDict(
-    "ReferenceLineLabelConfigurationOutputTypeDef",
-    {
-        "ValueLabelConfiguration": ReferenceLineValueLabelConfigurationOutputTypeDef,
-        "CustomLabelConfiguration": ReferenceLineCustomLabelConfigurationOutputTypeDef,
-        "FontConfiguration": FontConfigurationOutputTypeDef,
-        "FontColor": str,
-        "HorizontalPosition": ReferenceLineLabelHorizontalPositionType,
-        "VerticalPosition": ReferenceLineLabelVerticalPositionType,
-    },
-    total=False,
-)
-
-_RequiredCategoricalDimensionFieldOutputTypeDef = TypedDict(
-    "_RequiredCategoricalDimensionFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalCategoricalDimensionFieldOutputTypeDef = TypedDict(
-    "_OptionalCategoricalDimensionFieldOutputTypeDef",
-    {
-        "HierarchyId": str,
-        "FormatConfiguration": StringFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CategoricalDimensionFieldOutputTypeDef(
-    _RequiredCategoricalDimensionFieldOutputTypeDef, _OptionalCategoricalDimensionFieldOutputTypeDef
-):
-    pass
-
-
-_RequiredCategoricalMeasureFieldOutputTypeDef = TypedDict(
-    "_RequiredCategoricalMeasureFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalCategoricalMeasureFieldOutputTypeDef = TypedDict(
-    "_OptionalCategoricalMeasureFieldOutputTypeDef",
-    {
-        "AggregationFunction": CategoricalAggregationFunctionType,
-        "FormatConfiguration": StringFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CategoricalMeasureFieldOutputTypeDef(
-    _RequiredCategoricalMeasureFieldOutputTypeDef, _OptionalCategoricalMeasureFieldOutputTypeDef
-):
-    pass
-
-
-FormatConfigurationOutputTypeDef = TypedDict(
-    "FormatConfigurationOutputTypeDef",
-    {
-        "StringFormatConfiguration": StringFormatConfigurationOutputTypeDef,
-        "NumberFormatConfiguration": NumberFormatConfigurationOutputTypeDef,
-        "DateTimeFormatConfiguration": DateTimeFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 GaugeChartOptionsTypeDef = TypedDict(
     "GaugeChartOptionsTypeDef",
     {
         "PrimaryValueDisplayType": PrimaryValueDisplayTypeType,
         "Comparison": ComparisonConfigurationTypeDef,
         "ArcAxis": ArcAxisConfigurationTypeDef,
         "Arc": ArcConfigurationTypeDef,
@@ -19610,362 +15811,362 @@
     total=False,
 )
 
 FilterOutputTypeDef = TypedDict(
     "FilterOutputTypeDef",
     {
         "CategoryFilter": CategoryFilterOutputTypeDef,
-        "NumericRangeFilter": NumericRangeFilterOutputTypeDef,
-        "NumericEqualityFilter": NumericEqualityFilterOutputTypeDef,
+        "NumericRangeFilter": NumericRangeFilterTypeDef,
+        "NumericEqualityFilter": NumericEqualityFilterTypeDef,
         "TimeEqualityFilter": TimeEqualityFilterOutputTypeDef,
         "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
-        "RelativeDatesFilter": RelativeDatesFilterOutputTypeDef,
+        "RelativeDatesFilter": RelativeDatesFilterTypeDef,
         "TopBottomFilter": TopBottomFilterOutputTypeDef,
     },
     total=False,
 )
 
-BarChartSortConfigurationOutputTypeDef = TypedDict(
-    "BarChartSortConfigurationOutputTypeDef",
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "ColorSort": List[FieldSortOptionsOutputTypeDef],
-        "ColorItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "SmallMultiplesSort": List[FieldSortOptionsOutputTypeDef],
-        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
+        "CategoryFilter": CategoryFilterTypeDef,
+        "NumericRangeFilter": NumericRangeFilterTypeDef,
+        "NumericEqualityFilter": NumericEqualityFilterTypeDef,
+        "TimeEqualityFilter": TimeEqualityFilterTypeDef,
+        "TimeRangeFilter": TimeRangeFilterTypeDef,
+        "RelativeDatesFilter": RelativeDatesFilterTypeDef,
+        "TopBottomFilter": TopBottomFilterTypeDef,
     },
     total=False,
 )
 
-BoxPlotSortConfigurationOutputTypeDef = TypedDict(
-    "BoxPlotSortConfigurationOutputTypeDef",
+BarChartSortConfigurationOutputTypeDef = TypedDict(
+    "BarChartSortConfigurationOutputTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "PaginationConfiguration": PaginationConfigurationOutputTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "ColorSort": List[FieldSortOptionsTypeDef],
+        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
+        "SmallMultiplesSort": List[FieldSortOptionsTypeDef],
+        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-ComboChartSortConfigurationOutputTypeDef = TypedDict(
-    "ComboChartSortConfigurationOutputTypeDef",
+BarChartSortConfigurationTypeDef = TypedDict(
+    "BarChartSortConfigurationTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "ColorSort": List[FieldSortOptionsOutputTypeDef],
-        "ColorItemsLimit": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "ColorSort": Sequence[FieldSortOptionsTypeDef],
+        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
+        "SmallMultiplesSort": Sequence[FieldSortOptionsTypeDef],
+        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-FilledMapSortConfigurationOutputTypeDef = TypedDict(
-    "FilledMapSortConfigurationOutputTypeDef",
+BoxPlotSortConfigurationOutputTypeDef = TypedDict(
+    "BoxPlotSortConfigurationOutputTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "PaginationConfiguration": PaginationConfigurationTypeDef,
     },
     total=False,
 )
 
-FunnelChartSortConfigurationOutputTypeDef = TypedDict(
-    "FunnelChartSortConfigurationOutputTypeDef",
+BoxPlotSortConfigurationTypeDef = TypedDict(
+    "BoxPlotSortConfigurationTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "PaginationConfiguration": PaginationConfigurationTypeDef,
     },
     total=False,
 )
 
-HeatMapSortConfigurationOutputTypeDef = TypedDict(
-    "HeatMapSortConfigurationOutputTypeDef",
+ComboChartSortConfigurationOutputTypeDef = TypedDict(
+    "ComboChartSortConfigurationOutputTypeDef",
     {
-        "HeatMapRowSort": List[FieldSortOptionsOutputTypeDef],
-        "HeatMapColumnSort": List[FieldSortOptionsOutputTypeDef],
-        "HeatMapRowItemsLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
-        "HeatMapColumnItemsLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "ColorSort": List[FieldSortOptionsTypeDef],
+        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-KPISortConfigurationOutputTypeDef = TypedDict(
-    "KPISortConfigurationOutputTypeDef",
+ComboChartSortConfigurationTypeDef = TypedDict(
+    "ComboChartSortConfigurationTypeDef",
     {
-        "TrendGroupSort": List[FieldSortOptionsOutputTypeDef],
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "ColorSort": Sequence[FieldSortOptionsTypeDef],
+        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-LineChartSortConfigurationOutputTypeDef = TypedDict(
-    "LineChartSortConfigurationOutputTypeDef",
+FilledMapSortConfigurationOutputTypeDef = TypedDict(
+    "FilledMapSortConfigurationOutputTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "CategoryItemsLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
-        "ColorItemsLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
-        "SmallMultiplesSort": List[FieldSortOptionsOutputTypeDef],
-        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
     },
     total=False,
 )
 
-PieChartSortConfigurationOutputTypeDef = TypedDict(
-    "PieChartSortConfigurationOutputTypeDef",
+FilledMapSortConfigurationTypeDef = TypedDict(
+    "FilledMapSortConfigurationTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "SmallMultiplesSort": List[FieldSortOptionsOutputTypeDef],
-        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
     },
     total=False,
 )
 
-RadarChartSortConfigurationOutputTypeDef = TypedDict(
-    "RadarChartSortConfigurationOutputTypeDef",
+FunnelChartSortConfigurationOutputTypeDef = TypedDict(
+    "FunnelChartSortConfigurationOutputTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "ColorSort": List[FieldSortOptionsOutputTypeDef],
-        "ColorItemsLimit": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-SankeyDiagramSortConfigurationOutputTypeDef = TypedDict(
-    "SankeyDiagramSortConfigurationOutputTypeDef",
+FunnelChartSortConfigurationTypeDef = TypedDict(
+    "FunnelChartSortConfigurationTypeDef",
     {
-        "WeightSort": List[FieldSortOptionsOutputTypeDef],
-        "SourceItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "DestinationItemsLimit": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-TableSortConfigurationOutputTypeDef = TypedDict(
-    "TableSortConfigurationOutputTypeDef",
+HeatMapSortConfigurationOutputTypeDef = TypedDict(
+    "HeatMapSortConfigurationOutputTypeDef",
     {
-        "RowSort": List[FieldSortOptionsOutputTypeDef],
-        "PaginationConfiguration": PaginationConfigurationOutputTypeDef,
+        "HeatMapRowSort": List[FieldSortOptionsTypeDef],
+        "HeatMapColumnSort": List[FieldSortOptionsTypeDef],
+        "HeatMapRowItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "HeatMapColumnItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-TreeMapSortConfigurationOutputTypeDef = TypedDict(
-    "TreeMapSortConfigurationOutputTypeDef",
+HeatMapSortConfigurationTypeDef = TypedDict(
+    "HeatMapSortConfigurationTypeDef",
     {
-        "TreeMapSort": List[FieldSortOptionsOutputTypeDef],
-        "TreeMapGroupItemsLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
+        "HeatMapRowSort": Sequence[FieldSortOptionsTypeDef],
+        "HeatMapColumnSort": Sequence[FieldSortOptionsTypeDef],
+        "HeatMapRowItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "HeatMapColumnItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-WaterfallChartSortConfigurationOutputTypeDef = TypedDict(
-    "WaterfallChartSortConfigurationOutputTypeDef",
+KPISortConfigurationOutputTypeDef = TypedDict(
+    "KPISortConfigurationOutputTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "BreakdownItemsLimit": ItemsLimitConfigurationOutputTypeDef,
+        "TrendGroupSort": List[FieldSortOptionsTypeDef],
     },
     total=False,
 )
 
-WordCloudSortConfigurationOutputTypeDef = TypedDict(
-    "WordCloudSortConfigurationOutputTypeDef",
+KPISortConfigurationTypeDef = TypedDict(
+    "KPISortConfigurationTypeDef",
     {
-        "CategoryItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
+        "TrendGroupSort": Sequence[FieldSortOptionsTypeDef],
     },
     total=False,
 )
 
-PivotFieldSortOptionsOutputTypeDef = TypedDict(
-    "PivotFieldSortOptionsOutputTypeDef",
+LineChartSortConfigurationOutputTypeDef = TypedDict(
+    "LineChartSortConfigurationOutputTypeDef",
     {
-        "FieldId": str,
-        "SortBy": PivotTableSortByOutputTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "CategoryItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "ColorItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "SmallMultiplesSort": List[FieldSortOptionsTypeDef],
+        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
+    total=False,
 )
 
-FieldBasedTooltipOutputTypeDef = TypedDict(
-    "FieldBasedTooltipOutputTypeDef",
+LineChartSortConfigurationTypeDef = TypedDict(
+    "LineChartSortConfigurationTypeDef",
     {
-        "AggregationVisibility": VisibilityType,
-        "TooltipTitleType": TooltipTitleTypeType,
-        "TooltipFields": List[TooltipItemOutputTypeDef],
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "CategoryItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "ColorItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "SmallMultiplesSort": Sequence[FieldSortOptionsTypeDef],
+        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
+PieChartSortConfigurationOutputTypeDef = TypedDict(
+    "PieChartSortConfigurationOutputTypeDef",
     {
-        "CategoryFilter": CategoryFilterTypeDef,
-        "NumericRangeFilter": NumericRangeFilterTypeDef,
-        "NumericEqualityFilter": NumericEqualityFilterTypeDef,
-        "TimeEqualityFilter": TimeEqualityFilterTypeDef,
-        "TimeRangeFilter": TimeRangeFilterTypeDef,
-        "RelativeDatesFilter": RelativeDatesFilterTypeDef,
-        "TopBottomFilter": TopBottomFilterTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "SmallMultiplesSort": List[FieldSortOptionsTypeDef],
+        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-BarChartSortConfigurationTypeDef = TypedDict(
-    "BarChartSortConfigurationTypeDef",
+PieChartSortConfigurationTypeDef = TypedDict(
+    "PieChartSortConfigurationTypeDef",
     {
         "CategorySort": Sequence[FieldSortOptionsTypeDef],
         "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
-        "ColorSort": Sequence[FieldSortOptionsTypeDef],
-        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
         "SmallMultiplesSort": Sequence[FieldSortOptionsTypeDef],
         "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-BoxPlotSortConfigurationTypeDef = TypedDict(
-    "BoxPlotSortConfigurationTypeDef",
+RadarChartSortConfigurationOutputTypeDef = TypedDict(
+    "RadarChartSortConfigurationOutputTypeDef",
     {
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
-        "PaginationConfiguration": PaginationConfigurationTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "ColorSort": List[FieldSortOptionsTypeDef],
+        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-ComboChartSortConfigurationTypeDef = TypedDict(
-    "ComboChartSortConfigurationTypeDef",
+RadarChartSortConfigurationTypeDef = TypedDict(
+    "RadarChartSortConfigurationTypeDef",
     {
         "CategorySort": Sequence[FieldSortOptionsTypeDef],
         "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
         "ColorSort": Sequence[FieldSortOptionsTypeDef],
         "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-FilledMapSortConfigurationTypeDef = TypedDict(
-    "FilledMapSortConfigurationTypeDef",
-    {
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
-    },
-    total=False,
-)
-
-FunnelChartSortConfigurationTypeDef = TypedDict(
-    "FunnelChartSortConfigurationTypeDef",
+SankeyDiagramSortConfigurationOutputTypeDef = TypedDict(
+    "SankeyDiagramSortConfigurationOutputTypeDef",
     {
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "WeightSort": List[FieldSortOptionsTypeDef],
+        "SourceItemsLimit": ItemsLimitConfigurationTypeDef,
+        "DestinationItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-HeatMapSortConfigurationTypeDef = TypedDict(
-    "HeatMapSortConfigurationTypeDef",
+SankeyDiagramSortConfigurationTypeDef = TypedDict(
+    "SankeyDiagramSortConfigurationTypeDef",
     {
-        "HeatMapRowSort": Sequence[FieldSortOptionsTypeDef],
-        "HeatMapColumnSort": Sequence[FieldSortOptionsTypeDef],
-        "HeatMapRowItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
-        "HeatMapColumnItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "WeightSort": Sequence[FieldSortOptionsTypeDef],
+        "SourceItemsLimit": ItemsLimitConfigurationTypeDef,
+        "DestinationItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-KPISortConfigurationTypeDef = TypedDict(
-    "KPISortConfigurationTypeDef",
+TableSortConfigurationOutputTypeDef = TypedDict(
+    "TableSortConfigurationOutputTypeDef",
     {
-        "TrendGroupSort": Sequence[FieldSortOptionsTypeDef],
+        "RowSort": List[FieldSortOptionsTypeDef],
+        "PaginationConfiguration": PaginationConfigurationTypeDef,
     },
     total=False,
 )
 
-LineChartSortConfigurationTypeDef = TypedDict(
-    "LineChartSortConfigurationTypeDef",
+TableSortConfigurationTypeDef = TypedDict(
+    "TableSortConfigurationTypeDef",
     {
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
-        "CategoryItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
-        "ColorItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
-        "SmallMultiplesSort": Sequence[FieldSortOptionsTypeDef],
-        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "RowSort": Sequence[FieldSortOptionsTypeDef],
+        "PaginationConfiguration": PaginationConfigurationTypeDef,
     },
     total=False,
 )
 
-PieChartSortConfigurationTypeDef = TypedDict(
-    "PieChartSortConfigurationTypeDef",
+TreeMapSortConfigurationOutputTypeDef = TypedDict(
+    "TreeMapSortConfigurationOutputTypeDef",
     {
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
-        "SmallMultiplesSort": Sequence[FieldSortOptionsTypeDef],
-        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "TreeMapSort": List[FieldSortOptionsTypeDef],
+        "TreeMapGroupItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-RadarChartSortConfigurationTypeDef = TypedDict(
-    "RadarChartSortConfigurationTypeDef",
+TreeMapSortConfigurationTypeDef = TypedDict(
+    "TreeMapSortConfigurationTypeDef",
     {
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
-        "ColorSort": Sequence[FieldSortOptionsTypeDef],
-        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
+        "TreeMapSort": Sequence[FieldSortOptionsTypeDef],
+        "TreeMapGroupItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-SankeyDiagramSortConfigurationTypeDef = TypedDict(
-    "SankeyDiagramSortConfigurationTypeDef",
+WaterfallChartSortConfigurationOutputTypeDef = TypedDict(
+    "WaterfallChartSortConfigurationOutputTypeDef",
     {
-        "WeightSort": Sequence[FieldSortOptionsTypeDef],
-        "SourceItemsLimit": ItemsLimitConfigurationTypeDef,
-        "DestinationItemsLimit": ItemsLimitConfigurationTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "BreakdownItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-TableSortConfigurationTypeDef = TypedDict(
-    "TableSortConfigurationTypeDef",
+WaterfallChartSortConfigurationTypeDef = TypedDict(
+    "WaterfallChartSortConfigurationTypeDef",
     {
-        "RowSort": Sequence[FieldSortOptionsTypeDef],
-        "PaginationConfiguration": PaginationConfigurationTypeDef,
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "BreakdownItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-TreeMapSortConfigurationTypeDef = TypedDict(
-    "TreeMapSortConfigurationTypeDef",
+WordCloudSortConfigurationOutputTypeDef = TypedDict(
+    "WordCloudSortConfigurationOutputTypeDef",
     {
-        "TreeMapSort": Sequence[FieldSortOptionsTypeDef],
-        "TreeMapGroupItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
     },
     total=False,
 )
 
-WaterfallChartSortConfigurationTypeDef = TypedDict(
-    "WaterfallChartSortConfigurationTypeDef",
+WordCloudSortConfigurationTypeDef = TypedDict(
+    "WordCloudSortConfigurationTypeDef",
     {
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
         "CategorySort": Sequence[FieldSortOptionsTypeDef],
-        "BreakdownItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-WordCloudSortConfigurationTypeDef = TypedDict(
-    "WordCloudSortConfigurationTypeDef",
+PivotFieldSortOptionsOutputTypeDef = TypedDict(
+    "PivotFieldSortOptionsOutputTypeDef",
     {
-        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "FieldId": str,
+        "SortBy": PivotTableSortByOutputTypeDef,
     },
-    total=False,
 )
 
 PivotFieldSortOptionsTypeDef = TypedDict(
     "PivotFieldSortOptionsTypeDef",
     {
         "FieldId": str,
         "SortBy": PivotTableSortByTypeDef,
     },
 )
 
+FieldBasedTooltipOutputTypeDef = TypedDict(
+    "FieldBasedTooltipOutputTypeDef",
+    {
+        "AggregationVisibility": VisibilityType,
+        "TooltipTitleType": TooltipTitleTypeType,
+        "TooltipFields": List[TooltipItemTypeDef],
+    },
+    total=False,
+)
+
 FieldBasedTooltipTypeDef = TypedDict(
     "FieldBasedTooltipTypeDef",
     {
         "AggregationVisibility": VisibilityType,
         "TooltipTitleType": TooltipTitleTypeType,
         "TooltipFields": Sequence[TooltipItemTypeDef],
     },
@@ -19996,24 +16197,14 @@
     "SnapshotJobResultTypeDef",
     {
         "AnonymousUsers": List[AnonymousUserSnapshotJobResultTypeDef],
     },
     total=False,
 )
 
-DefaultNewSheetConfigurationOutputTypeDef = TypedDict(
-    "DefaultNewSheetConfigurationOutputTypeDef",
-    {
-        "InteractiveLayoutConfiguration": DefaultInteractiveLayoutConfigurationOutputTypeDef,
-        "PaginatedLayoutConfiguration": DefaultPaginatedLayoutConfigurationOutputTypeDef,
-        "SheetContentType": SheetContentTypeType,
-    },
-    total=False,
-)
-
 DefaultNewSheetConfigurationTypeDef = TypedDict(
     "DefaultNewSheetConfigurationTypeDef",
     {
         "InteractiveLayoutConfiguration": DefaultInteractiveLayoutConfigurationTypeDef,
         "PaginatedLayoutConfiguration": DefaultPaginatedLayoutConfigurationTypeDef,
         "SheetContentType": SheetContentTypeType,
     },
@@ -20034,15 +16225,15 @@
         "SectionId": str,
         "Layout": SectionLayoutConfigurationOutputTypeDef,
     },
 )
 _OptionalHeaderFooterSectionConfigurationOutputTypeDef = TypedDict(
     "_OptionalHeaderFooterSectionConfigurationOutputTypeDef",
     {
-        "Style": SectionStyleOutputTypeDef,
+        "Style": SectionStyleTypeDef,
     },
     total=False,
 )
 
 
 class HeaderFooterSectionConfigurationOutputTypeDef(
     _RequiredHeaderFooterSectionConfigurationOutputTypeDef,
@@ -20136,38 +16327,14 @@
 
 class VisualCustomActionTypeDef(
     _RequiredVisualCustomActionTypeDef, _OptionalVisualCustomActionTypeDef
 ):
     pass
 
 
-_RequiredTableFieldOptionOutputTypeDef = TypedDict(
-    "_RequiredTableFieldOptionOutputTypeDef",
-    {
-        "FieldId": str,
-    },
-)
-_OptionalTableFieldOptionOutputTypeDef = TypedDict(
-    "_OptionalTableFieldOptionOutputTypeDef",
-    {
-        "Width": str,
-        "CustomLabel": str,
-        "Visibility": VisibilityType,
-        "URLStyling": TableFieldURLConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class TableFieldOptionOutputTypeDef(
-    _RequiredTableFieldOptionOutputTypeDef, _OptionalTableFieldOptionOutputTypeDef
-):
-    pass
-
-
 _RequiredTableFieldOptionTypeDef = TypedDict(
     "_RequiredTableFieldOptionTypeDef",
     {
         "FieldId": str,
     },
 )
 _OptionalTableFieldOptionTypeDef = TypedDict(
@@ -20272,145 +16439,79 @@
         "Theme": ThemeTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredReferenceLineOutputTypeDef = TypedDict(
-    "_RequiredReferenceLineOutputTypeDef",
+_RequiredReferenceLineTypeDef = TypedDict(
+    "_RequiredReferenceLineTypeDef",
     {
-        "DataConfiguration": ReferenceLineDataConfigurationOutputTypeDef,
+        "DataConfiguration": ReferenceLineDataConfigurationTypeDef,
     },
 )
-_OptionalReferenceLineOutputTypeDef = TypedDict(
-    "_OptionalReferenceLineOutputTypeDef",
+_OptionalReferenceLineTypeDef = TypedDict(
+    "_OptionalReferenceLineTypeDef",
     {
         "Status": WidgetStatusType,
-        "StyleConfiguration": ReferenceLineStyleConfigurationOutputTypeDef,
-        "LabelConfiguration": ReferenceLineLabelConfigurationOutputTypeDef,
+        "StyleConfiguration": ReferenceLineStyleConfigurationTypeDef,
+        "LabelConfiguration": ReferenceLineLabelConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class ReferenceLineOutputTypeDef(
-    _RequiredReferenceLineOutputTypeDef, _OptionalReferenceLineOutputTypeDef
-):
+class ReferenceLineTypeDef(_RequiredReferenceLineTypeDef, _OptionalReferenceLineTypeDef):
     pass
 
 
-DimensionFieldOutputTypeDef = TypedDict(
-    "DimensionFieldOutputTypeDef",
+DimensionFieldTypeDef = TypedDict(
+    "DimensionFieldTypeDef",
     {
-        "NumericalDimensionField": NumericalDimensionFieldOutputTypeDef,
-        "CategoricalDimensionField": CategoricalDimensionFieldOutputTypeDef,
-        "DateDimensionField": DateDimensionFieldOutputTypeDef,
+        "NumericalDimensionField": NumericalDimensionFieldTypeDef,
+        "CategoricalDimensionField": CategoricalDimensionFieldTypeDef,
+        "DateDimensionField": DateDimensionFieldTypeDef,
     },
     total=False,
 )
 
-MeasureFieldOutputTypeDef = TypedDict(
-    "MeasureFieldOutputTypeDef",
+MeasureFieldTypeDef = TypedDict(
+    "MeasureFieldTypeDef",
     {
-        "NumericalMeasureField": NumericalMeasureFieldOutputTypeDef,
-        "CategoricalMeasureField": CategoricalMeasureFieldOutputTypeDef,
-        "DateMeasureField": DateMeasureFieldOutputTypeDef,
-        "CalculatedMeasureField": CalculatedMeasureFieldOutputTypeDef,
+        "NumericalMeasureField": NumericalMeasureFieldTypeDef,
+        "CategoricalMeasureField": CategoricalMeasureFieldTypeDef,
+        "DateMeasureField": DateMeasureFieldTypeDef,
+        "CalculatedMeasureField": CalculatedMeasureFieldTypeDef,
     },
     total=False,
 )
 
 _RequiredColumnConfigurationOutputTypeDef = TypedDict(
     "_RequiredColumnConfigurationOutputTypeDef",
     {
-        "Column": ColumnIdentifierOutputTypeDef,
+        "Column": ColumnIdentifierTypeDef,
     },
 )
 _OptionalColumnConfigurationOutputTypeDef = TypedDict(
     "_OptionalColumnConfigurationOutputTypeDef",
     {
-        "FormatConfiguration": FormatConfigurationOutputTypeDef,
+        "FormatConfiguration": FormatConfigurationTypeDef,
         "Role": ColumnRoleType,
         "ColorsConfiguration": ColorsConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 
 class ColumnConfigurationOutputTypeDef(
     _RequiredColumnConfigurationOutputTypeDef, _OptionalColumnConfigurationOutputTypeDef
 ):
     pass
 
 
-_RequiredUnaggregatedFieldOutputTypeDef = TypedDict(
-    "_RequiredUnaggregatedFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalUnaggregatedFieldOutputTypeDef = TypedDict(
-    "_OptionalUnaggregatedFieldOutputTypeDef",
-    {
-        "FormatConfiguration": FormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class UnaggregatedFieldOutputTypeDef(
-    _RequiredUnaggregatedFieldOutputTypeDef, _OptionalUnaggregatedFieldOutputTypeDef
-):
-    pass
-
-
-_RequiredReferenceLineTypeDef = TypedDict(
-    "_RequiredReferenceLineTypeDef",
-    {
-        "DataConfiguration": ReferenceLineDataConfigurationTypeDef,
-    },
-)
-_OptionalReferenceLineTypeDef = TypedDict(
-    "_OptionalReferenceLineTypeDef",
-    {
-        "Status": WidgetStatusType,
-        "StyleConfiguration": ReferenceLineStyleConfigurationTypeDef,
-        "LabelConfiguration": ReferenceLineLabelConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class ReferenceLineTypeDef(_RequiredReferenceLineTypeDef, _OptionalReferenceLineTypeDef):
-    pass
-
-
-DimensionFieldTypeDef = TypedDict(
-    "DimensionFieldTypeDef",
-    {
-        "NumericalDimensionField": NumericalDimensionFieldTypeDef,
-        "CategoricalDimensionField": CategoricalDimensionFieldTypeDef,
-        "DateDimensionField": DateDimensionFieldTypeDef,
-    },
-    total=False,
-)
-
-MeasureFieldTypeDef = TypedDict(
-    "MeasureFieldTypeDef",
-    {
-        "NumericalMeasureField": NumericalMeasureFieldTypeDef,
-        "CategoricalMeasureField": CategoricalMeasureFieldTypeDef,
-        "DateMeasureField": DateMeasureFieldTypeDef,
-        "CalculatedMeasureField": CalculatedMeasureFieldTypeDef,
-    },
-    total=False,
-)
-
 _RequiredColumnConfigurationTypeDef = TypedDict(
     "_RequiredColumnConfigurationTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
     },
 )
 _OptionalColumnConfigurationTypeDef = TypedDict(
@@ -20472,32 +16573,14 @@
 
 class FilterGroupOutputTypeDef(
     _RequiredFilterGroupOutputTypeDef, _OptionalFilterGroupOutputTypeDef
 ):
     pass
 
 
-PivotTableSortConfigurationOutputTypeDef = TypedDict(
-    "PivotTableSortConfigurationOutputTypeDef",
-    {
-        "FieldSortOptions": List[PivotFieldSortOptionsOutputTypeDef],
-    },
-    total=False,
-)
-
-TooltipOptionsOutputTypeDef = TypedDict(
-    "TooltipOptionsOutputTypeDef",
-    {
-        "TooltipVisibility": VisibilityType,
-        "SelectedTooltipType": SelectedTooltipTypeType,
-        "FieldBasedTooltip": FieldBasedTooltipOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredFilterGroupTypeDef = TypedDict(
     "_RequiredFilterGroupTypeDef",
     {
         "FilterGroupId": str,
         "Filters": Sequence[FilterTypeDef],
         "ScopeConfiguration": FilterScopeConfigurationTypeDef,
         "CrossDataset": CrossDatasetTypesType,
@@ -20512,22 +16595,40 @@
 )
 
 
 class FilterGroupTypeDef(_RequiredFilterGroupTypeDef, _OptionalFilterGroupTypeDef):
     pass
 
 
+PivotTableSortConfigurationOutputTypeDef = TypedDict(
+    "PivotTableSortConfigurationOutputTypeDef",
+    {
+        "FieldSortOptions": List[PivotFieldSortOptionsOutputTypeDef],
+    },
+    total=False,
+)
+
 PivotTableSortConfigurationTypeDef = TypedDict(
     "PivotTableSortConfigurationTypeDef",
     {
         "FieldSortOptions": Sequence[PivotFieldSortOptionsTypeDef],
     },
     total=False,
 )
 
+TooltipOptionsOutputTypeDef = TypedDict(
+    "TooltipOptionsOutputTypeDef",
+    {
+        "TooltipVisibility": VisibilityType,
+        "SelectedTooltipType": SelectedTooltipTypeType,
+        "FieldBasedTooltip": FieldBasedTooltipOutputTypeDef,
+    },
+    total=False,
+)
+
 TooltipOptionsTypeDef = TypedDict(
     "TooltipOptionsTypeDef",
     {
         "TooltipVisibility": VisibilityType,
         "SelectedTooltipType": SelectedTooltipTypeType,
         "FieldBasedTooltip": FieldBasedTooltipTypeDef,
     },
@@ -20589,21 +16690,14 @@
         "ErrorInfo": SnapshotJobErrorInfoTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AnalysisDefaultsOutputTypeDef = TypedDict(
-    "AnalysisDefaultsOutputTypeDef",
-    {
-        "DefaultNewSheetConfiguration": DefaultNewSheetConfigurationOutputTypeDef,
-    },
-)
-
 AnalysisDefaultsTypeDef = TypedDict(
     "AnalysisDefaultsTypeDef",
     {
         "DefaultNewSheetConfiguration": DefaultNewSheetConfigurationTypeDef,
     },
 )
 
@@ -20613,16 +16707,16 @@
         "SectionId": str,
         "Content": BodySectionContentOutputTypeDef,
     },
 )
 _OptionalBodySectionConfigurationOutputTypeDef = TypedDict(
     "_OptionalBodySectionConfigurationOutputTypeDef",
     {
-        "Style": SectionStyleOutputTypeDef,
-        "PageBreakConfiguration": SectionPageBreakConfigurationOutputTypeDef,
+        "Style": SectionStyleTypeDef,
+        "PageBreakConfiguration": SectionPageBreakConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class BodySectionConfigurationOutputTypeDef(
     _RequiredBodySectionConfigurationOutputTypeDef, _OptionalBodySectionConfigurationOutputTypeDef
@@ -20659,17 +16753,17 @@
         "VisualId": str,
         "DataSetIdentifier": str,
     },
 )
 _OptionalCustomContentVisualOutputTypeDef = TypedDict(
     "_OptionalCustomContentVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": CustomContentConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": CustomContentConfigurationTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
 
 class CustomContentVisualOutputTypeDef(
@@ -20744,15 +16838,15 @@
 class EmptyVisualTypeDef(_RequiredEmptyVisualTypeDef, _OptionalEmptyVisualTypeDef):
     pass
 
 
 TableFieldOptionsOutputTypeDef = TypedDict(
     "TableFieldOptionsOutputTypeDef",
     {
-        "SelectedFieldOptions": List[TableFieldOptionOutputTypeDef],
+        "SelectedFieldOptions": List[TableFieldOptionTypeDef],
         "Order": List[str],
     },
     total=False,
 )
 
 TableFieldOptionsTypeDef = TypedDict(
     "TableFieldOptionsTypeDef",
@@ -20805,519 +16899,83 @@
     "TableConditionalFormattingTypeDef",
     {
         "ConditionalFormattingOptions": Sequence[TableConditionalFormattingOptionTypeDef],
     },
     total=False,
 )
 
-_RequiredUniqueValuesComputationOutputTypeDef = TypedDict(
-    "_RequiredUniqueValuesComputationOutputTypeDef",
+_RequiredUniqueValuesComputationTypeDef = TypedDict(
+    "_RequiredUniqueValuesComputationTypeDef",
     {
         "ComputationId": str,
-        "Category": DimensionFieldOutputTypeDef,
+        "Category": DimensionFieldTypeDef,
     },
 )
-_OptionalUniqueValuesComputationOutputTypeDef = TypedDict(
-    "_OptionalUniqueValuesComputationOutputTypeDef",
+_OptionalUniqueValuesComputationTypeDef = TypedDict(
+    "_OptionalUniqueValuesComputationTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
 
-class UniqueValuesComputationOutputTypeDef(
-    _RequiredUniqueValuesComputationOutputTypeDef, _OptionalUniqueValuesComputationOutputTypeDef
+class UniqueValuesComputationTypeDef(
+    _RequiredUniqueValuesComputationTypeDef, _OptionalUniqueValuesComputationTypeDef
 ):
     pass
 
 
 BarChartAggregatedFieldWellsOutputTypeDef = TypedDict(
     "BarChartAggregatedFieldWellsOutputTypeDef",
     {
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-        "Colors": List[DimensionFieldOutputTypeDef],
-        "SmallMultiples": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-BoxPlotAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "BoxPlotAggregatedFieldWellsOutputTypeDef",
-    {
-        "GroupBy": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-ComboChartAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "ComboChartAggregatedFieldWellsOutputTypeDef",
-    {
-        "Category": List[DimensionFieldOutputTypeDef],
-        "BarValues": List[MeasureFieldOutputTypeDef],
-        "Colors": List[DimensionFieldOutputTypeDef],
-        "LineValues": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-FilledMapAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "FilledMapAggregatedFieldWellsOutputTypeDef",
-    {
-        "Geospatial": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-_RequiredForecastComputationOutputTypeDef = TypedDict(
-    "_RequiredForecastComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-    },
-)
-_OptionalForecastComputationOutputTypeDef = TypedDict(
-    "_OptionalForecastComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-        "PeriodsForward": int,
-        "PeriodsBackward": int,
-        "UpperBoundary": float,
-        "LowerBoundary": float,
-        "PredictionInterval": int,
-        "Seasonality": ForecastComputationSeasonalityType,
-        "CustomSeasonalityValue": int,
+        "Category": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+        "Colors": List[DimensionFieldTypeDef],
+        "SmallMultiples": List[DimensionFieldTypeDef],
     },
     total=False,
 )
 
-
-class ForecastComputationOutputTypeDef(
-    _RequiredForecastComputationOutputTypeDef, _OptionalForecastComputationOutputTypeDef
-):
-    pass
-
-
-FunnelChartAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "FunnelChartAggregatedFieldWellsOutputTypeDef",
-    {
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-GaugeChartFieldWellsOutputTypeDef = TypedDict(
-    "GaugeChartFieldWellsOutputTypeDef",
-    {
-        "Values": List[MeasureFieldOutputTypeDef],
-        "TargetValues": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-GeospatialMapAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "GeospatialMapAggregatedFieldWellsOutputTypeDef",
-    {
-        "Geospatial": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-        "Colors": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-_RequiredGrowthRateComputationOutputTypeDef = TypedDict(
-    "_RequiredGrowthRateComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-    },
-)
-_OptionalGrowthRateComputationOutputTypeDef = TypedDict(
-    "_OptionalGrowthRateComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-        "PeriodSize": int,
-    },
-    total=False,
-)
-
-
-class GrowthRateComputationOutputTypeDef(
-    _RequiredGrowthRateComputationOutputTypeDef, _OptionalGrowthRateComputationOutputTypeDef
-):
-    pass
-
-
-HeatMapAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "HeatMapAggregatedFieldWellsOutputTypeDef",
-    {
-        "Rows": List[DimensionFieldOutputTypeDef],
-        "Columns": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-HistogramAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "HistogramAggregatedFieldWellsOutputTypeDef",
-    {
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-KPIFieldWellsOutputTypeDef = TypedDict(
-    "KPIFieldWellsOutputTypeDef",
-    {
-        "Values": List[MeasureFieldOutputTypeDef],
-        "TargetValues": List[MeasureFieldOutputTypeDef],
-        "TrendGroups": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-LineChartAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "LineChartAggregatedFieldWellsOutputTypeDef",
-    {
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-        "Colors": List[DimensionFieldOutputTypeDef],
-        "SmallMultiples": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-_RequiredMaximumMinimumComputationOutputTypeDef = TypedDict(
-    "_RequiredMaximumMinimumComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-        "Type": MaximumMinimumComputationTypeType,
-    },
-)
-_OptionalMaximumMinimumComputationOutputTypeDef = TypedDict(
-    "_OptionalMaximumMinimumComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class MaximumMinimumComputationOutputTypeDef(
-    _RequiredMaximumMinimumComputationOutputTypeDef, _OptionalMaximumMinimumComputationOutputTypeDef
-):
-    pass
-
-
-_RequiredMetricComparisonComputationOutputTypeDef = TypedDict(
-    "_RequiredMetricComparisonComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-        "FromValue": MeasureFieldOutputTypeDef,
-        "TargetValue": MeasureFieldOutputTypeDef,
-    },
-)
-_OptionalMetricComparisonComputationOutputTypeDef = TypedDict(
-    "_OptionalMetricComparisonComputationOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-
-class MetricComparisonComputationOutputTypeDef(
-    _RequiredMetricComparisonComputationOutputTypeDef,
-    _OptionalMetricComparisonComputationOutputTypeDef,
-):
-    pass
-
-
-_RequiredPeriodOverPeriodComputationOutputTypeDef = TypedDict(
-    "_RequiredPeriodOverPeriodComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-    },
-)
-_OptionalPeriodOverPeriodComputationOutputTypeDef = TypedDict(
-    "_OptionalPeriodOverPeriodComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class PeriodOverPeriodComputationOutputTypeDef(
-    _RequiredPeriodOverPeriodComputationOutputTypeDef,
-    _OptionalPeriodOverPeriodComputationOutputTypeDef,
-):
-    pass
-
-
-_RequiredPeriodToDateComputationOutputTypeDef = TypedDict(
-    "_RequiredPeriodToDateComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-    },
-)
-_OptionalPeriodToDateComputationOutputTypeDef = TypedDict(
-    "_OptionalPeriodToDateComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-        "PeriodTimeGranularity": TimeGranularityType,
-    },
-    total=False,
-)
-
-
-class PeriodToDateComputationOutputTypeDef(
-    _RequiredPeriodToDateComputationOutputTypeDef, _OptionalPeriodToDateComputationOutputTypeDef
-):
-    pass
-
-
-PieChartAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "PieChartAggregatedFieldWellsOutputTypeDef",
-    {
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-        "SmallMultiples": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-PivotTableAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "PivotTableAggregatedFieldWellsOutputTypeDef",
-    {
-        "Rows": List[DimensionFieldOutputTypeDef],
-        "Columns": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-RadarChartAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "RadarChartAggregatedFieldWellsOutputTypeDef",
-    {
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Color": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-SankeyDiagramAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "SankeyDiagramAggregatedFieldWellsOutputTypeDef",
-    {
-        "Source": List[DimensionFieldOutputTypeDef],
-        "Destination": List[DimensionFieldOutputTypeDef],
-        "Weight": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef",
-    {
-        "XAxis": List[MeasureFieldOutputTypeDef],
-        "YAxis": List[MeasureFieldOutputTypeDef],
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Size": List[MeasureFieldOutputTypeDef],
-        "Label": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-ScatterPlotUnaggregatedFieldWellsOutputTypeDef = TypedDict(
-    "ScatterPlotUnaggregatedFieldWellsOutputTypeDef",
-    {
-        "XAxis": List[DimensionFieldOutputTypeDef],
-        "YAxis": List[DimensionFieldOutputTypeDef],
-        "Size": List[MeasureFieldOutputTypeDef],
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Label": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-TableAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "TableAggregatedFieldWellsOutputTypeDef",
-    {
-        "GroupBy": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-_RequiredTopBottomMoversComputationOutputTypeDef = TypedDict(
-    "_RequiredTopBottomMoversComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-        "Category": DimensionFieldOutputTypeDef,
-        "Type": TopBottomComputationTypeType,
-    },
-)
-_OptionalTopBottomMoversComputationOutputTypeDef = TypedDict(
-    "_OptionalTopBottomMoversComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-        "MoverSize": int,
-        "SortOrder": TopBottomSortOrderType,
-    },
-    total=False,
-)
-
-
-class TopBottomMoversComputationOutputTypeDef(
-    _RequiredTopBottomMoversComputationOutputTypeDef,
-    _OptionalTopBottomMoversComputationOutputTypeDef,
-):
-    pass
-
-
-_RequiredTopBottomRankedComputationOutputTypeDef = TypedDict(
-    "_RequiredTopBottomRankedComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Category": DimensionFieldOutputTypeDef,
-        "Type": TopBottomComputationTypeType,
-    },
-)
-_OptionalTopBottomRankedComputationOutputTypeDef = TypedDict(
-    "_OptionalTopBottomRankedComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-        "ResultSize": int,
-    },
-    total=False,
-)
-
-
-class TopBottomRankedComputationOutputTypeDef(
-    _RequiredTopBottomRankedComputationOutputTypeDef,
-    _OptionalTopBottomRankedComputationOutputTypeDef,
-):
-    pass
-
-
-_RequiredTotalAggregationComputationOutputTypeDef = TypedDict(
-    "_RequiredTotalAggregationComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Value": MeasureFieldOutputTypeDef,
-    },
-)
-_OptionalTotalAggregationComputationOutputTypeDef = TypedDict(
-    "_OptionalTotalAggregationComputationOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-
-class TotalAggregationComputationOutputTypeDef(
-    _RequiredTotalAggregationComputationOutputTypeDef,
-    _OptionalTotalAggregationComputationOutputTypeDef,
-):
-    pass
-
-
-TreeMapAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "TreeMapAggregatedFieldWellsOutputTypeDef",
-    {
-        "Groups": List[DimensionFieldOutputTypeDef],
-        "Sizes": List[MeasureFieldOutputTypeDef],
-        "Colors": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-WaterfallChartAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "WaterfallChartAggregatedFieldWellsOutputTypeDef",
-    {
-        "Categories": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-        "Breakdowns": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-WordCloudAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "WordCloudAggregatedFieldWellsOutputTypeDef",
-    {
-        "GroupBy": List[DimensionFieldOutputTypeDef],
-        "Size": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-TableUnaggregatedFieldWellsOutputTypeDef = TypedDict(
-    "TableUnaggregatedFieldWellsOutputTypeDef",
+BarChartAggregatedFieldWellsTypeDef = TypedDict(
+    "BarChartAggregatedFieldWellsTypeDef",
     {
-        "Values": List[UnaggregatedFieldOutputTypeDef],
+        "Category": Sequence[DimensionFieldTypeDef],
+        "Values": Sequence[MeasureFieldTypeDef],
+        "Colors": Sequence[DimensionFieldTypeDef],
+        "SmallMultiples": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
-_RequiredUniqueValuesComputationTypeDef = TypedDict(
-    "_RequiredUniqueValuesComputationTypeDef",
-    {
-        "ComputationId": str,
-        "Category": DimensionFieldTypeDef,
-    },
-)
-_OptionalUniqueValuesComputationTypeDef = TypedDict(
-    "_OptionalUniqueValuesComputationTypeDef",
+BoxPlotAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "BoxPlotAggregatedFieldWellsOutputTypeDef",
     {
-        "Name": str,
+        "GroupBy": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
     },
     total=False,
 )
 
-
-class UniqueValuesComputationTypeDef(
-    _RequiredUniqueValuesComputationTypeDef, _OptionalUniqueValuesComputationTypeDef
-):
-    pass
-
-
-BarChartAggregatedFieldWellsTypeDef = TypedDict(
-    "BarChartAggregatedFieldWellsTypeDef",
+BoxPlotAggregatedFieldWellsTypeDef = TypedDict(
+    "BoxPlotAggregatedFieldWellsTypeDef",
     {
-        "Category": Sequence[DimensionFieldTypeDef],
+        "GroupBy": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
-        "Colors": Sequence[DimensionFieldTypeDef],
-        "SmallMultiples": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
-BoxPlotAggregatedFieldWellsTypeDef = TypedDict(
-    "BoxPlotAggregatedFieldWellsTypeDef",
+ComboChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "ComboChartAggregatedFieldWellsOutputTypeDef",
     {
-        "GroupBy": Sequence[DimensionFieldTypeDef],
-        "Values": Sequence[MeasureFieldTypeDef],
+        "Category": List[DimensionFieldTypeDef],
+        "BarValues": List[MeasureFieldTypeDef],
+        "Colors": List[DimensionFieldTypeDef],
+        "LineValues": List[MeasureFieldTypeDef],
     },
     total=False,
 )
 
 ComboChartAggregatedFieldWellsTypeDef = TypedDict(
     "ComboChartAggregatedFieldWellsTypeDef",
     {
@@ -21325,14 +16983,23 @@
         "BarValues": Sequence[MeasureFieldTypeDef],
         "Colors": Sequence[DimensionFieldTypeDef],
         "LineValues": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+FilledMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "FilledMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Geospatial": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 FilledMapAggregatedFieldWellsTypeDef = TypedDict(
     "FilledMapAggregatedFieldWellsTypeDef",
     {
         "Geospatial": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
@@ -21364,32 +17031,60 @@
 
 class ForecastComputationTypeDef(
     _RequiredForecastComputationTypeDef, _OptionalForecastComputationTypeDef
 ):
     pass
 
 
+FunnelChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "FunnelChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 FunnelChartAggregatedFieldWellsTypeDef = TypedDict(
     "FunnelChartAggregatedFieldWellsTypeDef",
     {
         "Category": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+GaugeChartFieldWellsOutputTypeDef = TypedDict(
+    "GaugeChartFieldWellsOutputTypeDef",
+    {
+        "Values": List[MeasureFieldTypeDef],
+        "TargetValues": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 GaugeChartFieldWellsTypeDef = TypedDict(
     "GaugeChartFieldWellsTypeDef",
     {
         "Values": Sequence[MeasureFieldTypeDef],
         "TargetValues": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+GeospatialMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "GeospatialMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Geospatial": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+        "Colors": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 GeospatialMapAggregatedFieldWellsTypeDef = TypedDict(
     "GeospatialMapAggregatedFieldWellsTypeDef",
     {
         "Geospatial": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
         "Colors": Sequence[DimensionFieldTypeDef],
     },
@@ -21416,42 +17111,81 @@
 
 class GrowthRateComputationTypeDef(
     _RequiredGrowthRateComputationTypeDef, _OptionalGrowthRateComputationTypeDef
 ):
     pass
 
 
+HeatMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "HeatMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Rows": List[DimensionFieldTypeDef],
+        "Columns": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 HeatMapAggregatedFieldWellsTypeDef = TypedDict(
     "HeatMapAggregatedFieldWellsTypeDef",
     {
         "Rows": Sequence[DimensionFieldTypeDef],
         "Columns": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+HistogramAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "HistogramAggregatedFieldWellsOutputTypeDef",
+    {
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 HistogramAggregatedFieldWellsTypeDef = TypedDict(
     "HistogramAggregatedFieldWellsTypeDef",
     {
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+KPIFieldWellsOutputTypeDef = TypedDict(
+    "KPIFieldWellsOutputTypeDef",
+    {
+        "Values": List[MeasureFieldTypeDef],
+        "TargetValues": List[MeasureFieldTypeDef],
+        "TrendGroups": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 KPIFieldWellsTypeDef = TypedDict(
     "KPIFieldWellsTypeDef",
     {
         "Values": Sequence[MeasureFieldTypeDef],
         "TargetValues": Sequence[MeasureFieldTypeDef],
         "TrendGroups": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
+LineChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "LineChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+        "Colors": List[DimensionFieldTypeDef],
+        "SmallMultiples": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 LineChartAggregatedFieldWellsTypeDef = TypedDict(
     "LineChartAggregatedFieldWellsTypeDef",
     {
         "Category": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
         "Colors": Sequence[DimensionFieldTypeDef],
         "SmallMultiples": Sequence[DimensionFieldTypeDef],
@@ -21550,78 +17284,151 @@
 
 class PeriodToDateComputationTypeDef(
     _RequiredPeriodToDateComputationTypeDef, _OptionalPeriodToDateComputationTypeDef
 ):
     pass
 
 
+PieChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "PieChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+        "SmallMultiples": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 PieChartAggregatedFieldWellsTypeDef = TypedDict(
     "PieChartAggregatedFieldWellsTypeDef",
     {
         "Category": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
         "SmallMultiples": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
+PivotTableAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "PivotTableAggregatedFieldWellsOutputTypeDef",
+    {
+        "Rows": List[DimensionFieldTypeDef],
+        "Columns": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 PivotTableAggregatedFieldWellsTypeDef = TypedDict(
     "PivotTableAggregatedFieldWellsTypeDef",
     {
         "Rows": Sequence[DimensionFieldTypeDef],
         "Columns": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+RadarChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "RadarChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": List[DimensionFieldTypeDef],
+        "Color": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 RadarChartAggregatedFieldWellsTypeDef = TypedDict(
     "RadarChartAggregatedFieldWellsTypeDef",
     {
         "Category": Sequence[DimensionFieldTypeDef],
         "Color": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+SankeyDiagramAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "SankeyDiagramAggregatedFieldWellsOutputTypeDef",
+    {
+        "Source": List[DimensionFieldTypeDef],
+        "Destination": List[DimensionFieldTypeDef],
+        "Weight": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 SankeyDiagramAggregatedFieldWellsTypeDef = TypedDict(
     "SankeyDiagramAggregatedFieldWellsTypeDef",
     {
         "Source": Sequence[DimensionFieldTypeDef],
         "Destination": Sequence[DimensionFieldTypeDef],
         "Weight": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef",
+    {
+        "XAxis": List[MeasureFieldTypeDef],
+        "YAxis": List[MeasureFieldTypeDef],
+        "Category": List[DimensionFieldTypeDef],
+        "Size": List[MeasureFieldTypeDef],
+        "Label": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 ScatterPlotCategoricallyAggregatedFieldWellsTypeDef = TypedDict(
     "ScatterPlotCategoricallyAggregatedFieldWellsTypeDef",
     {
         "XAxis": Sequence[MeasureFieldTypeDef],
         "YAxis": Sequence[MeasureFieldTypeDef],
         "Category": Sequence[DimensionFieldTypeDef],
         "Size": Sequence[MeasureFieldTypeDef],
         "Label": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
+ScatterPlotUnaggregatedFieldWellsOutputTypeDef = TypedDict(
+    "ScatterPlotUnaggregatedFieldWellsOutputTypeDef",
+    {
+        "XAxis": List[DimensionFieldTypeDef],
+        "YAxis": List[DimensionFieldTypeDef],
+        "Size": List[MeasureFieldTypeDef],
+        "Category": List[DimensionFieldTypeDef],
+        "Label": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 ScatterPlotUnaggregatedFieldWellsTypeDef = TypedDict(
     "ScatterPlotUnaggregatedFieldWellsTypeDef",
     {
         "XAxis": Sequence[DimensionFieldTypeDef],
         "YAxis": Sequence[DimensionFieldTypeDef],
         "Size": Sequence[MeasureFieldTypeDef],
         "Category": Sequence[DimensionFieldTypeDef],
         "Label": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
+TableAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "TableAggregatedFieldWellsOutputTypeDef",
+    {
+        "GroupBy": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 TableAggregatedFieldWellsTypeDef = TypedDict(
     "TableAggregatedFieldWellsTypeDef",
     {
         "GroupBy": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
@@ -21697,58 +17504,95 @@
 
 class TotalAggregationComputationTypeDef(
     _RequiredTotalAggregationComputationTypeDef, _OptionalTotalAggregationComputationTypeDef
 ):
     pass
 
 
+TreeMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "TreeMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Groups": List[DimensionFieldTypeDef],
+        "Sizes": List[MeasureFieldTypeDef],
+        "Colors": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 TreeMapAggregatedFieldWellsTypeDef = TypedDict(
     "TreeMapAggregatedFieldWellsTypeDef",
     {
         "Groups": Sequence[DimensionFieldTypeDef],
         "Sizes": Sequence[MeasureFieldTypeDef],
         "Colors": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+WaterfallChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "WaterfallChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Categories": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+        "Breakdowns": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 WaterfallChartAggregatedFieldWellsTypeDef = TypedDict(
     "WaterfallChartAggregatedFieldWellsTypeDef",
     {
         "Categories": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
         "Breakdowns": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
+WordCloudAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "WordCloudAggregatedFieldWellsOutputTypeDef",
+    {
+        "GroupBy": List[DimensionFieldTypeDef],
+        "Size": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 WordCloudAggregatedFieldWellsTypeDef = TypedDict(
     "WordCloudAggregatedFieldWellsTypeDef",
     {
         "GroupBy": Sequence[DimensionFieldTypeDef],
         "Size": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+TableUnaggregatedFieldWellsOutputTypeDef = TypedDict(
+    "TableUnaggregatedFieldWellsOutputTypeDef",
+    {
+        "Values": List[UnaggregatedFieldTypeDef],
+    },
+    total=False,
+)
+
 TableUnaggregatedFieldWellsTypeDef = TypedDict(
     "TableUnaggregatedFieldWellsTypeDef",
     {
         "Values": Sequence[UnaggregatedFieldTypeDef],
     },
     total=False,
 )
 
 SectionBasedLayoutConfigurationOutputTypeDef = TypedDict(
     "SectionBasedLayoutConfigurationOutputTypeDef",
     {
         "HeaderSections": List[HeaderFooterSectionConfigurationOutputTypeDef],
         "BodySections": List[BodySectionConfigurationOutputTypeDef],
         "FooterSections": List[HeaderFooterSectionConfigurationOutputTypeDef],
-        "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsOutputTypeDef,
+        "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
 SectionBasedLayoutConfigurationTypeDef = TypedDict(
     "SectionBasedLayoutConfigurationTypeDef",
     {
         "HeaderSections": Sequence[HeaderFooterSectionConfigurationTypeDef],
@@ -21762,315 +17606,265 @@
     "BarChartFieldWellsOutputTypeDef",
     {
         "BarChartAggregatedFieldWells": BarChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-BoxPlotFieldWellsOutputTypeDef = TypedDict(
-    "BoxPlotFieldWellsOutputTypeDef",
-    {
-        "BoxPlotAggregatedFieldWells": BoxPlotAggregatedFieldWellsOutputTypeDef,
-    },
-    total=False,
-)
-
-ComboChartFieldWellsOutputTypeDef = TypedDict(
-    "ComboChartFieldWellsOutputTypeDef",
-    {
-        "ComboChartAggregatedFieldWells": ComboChartAggregatedFieldWellsOutputTypeDef,
-    },
-    total=False,
-)
-
-FilledMapFieldWellsOutputTypeDef = TypedDict(
-    "FilledMapFieldWellsOutputTypeDef",
-    {
-        "FilledMapAggregatedFieldWells": FilledMapAggregatedFieldWellsOutputTypeDef,
-    },
-    total=False,
-)
-
-FunnelChartFieldWellsOutputTypeDef = TypedDict(
-    "FunnelChartFieldWellsOutputTypeDef",
-    {
-        "FunnelChartAggregatedFieldWells": FunnelChartAggregatedFieldWellsOutputTypeDef,
-    },
-    total=False,
-)
-
-GaugeChartConfigurationOutputTypeDef = TypedDict(
-    "GaugeChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": GaugeChartFieldWellsOutputTypeDef,
-        "GaugeChartOptions": GaugeChartOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "TooltipOptions": TooltipOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-GeospatialMapFieldWellsOutputTypeDef = TypedDict(
-    "GeospatialMapFieldWellsOutputTypeDef",
+BarChartFieldWellsTypeDef = TypedDict(
+    "BarChartFieldWellsTypeDef",
     {
-        "GeospatialMapAggregatedFieldWells": GeospatialMapAggregatedFieldWellsOutputTypeDef,
+        "BarChartAggregatedFieldWells": BarChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-HeatMapFieldWellsOutputTypeDef = TypedDict(
-    "HeatMapFieldWellsOutputTypeDef",
+BoxPlotFieldWellsOutputTypeDef = TypedDict(
+    "BoxPlotFieldWellsOutputTypeDef",
     {
-        "HeatMapAggregatedFieldWells": HeatMapAggregatedFieldWellsOutputTypeDef,
+        "BoxPlotAggregatedFieldWells": BoxPlotAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-HistogramFieldWellsOutputTypeDef = TypedDict(
-    "HistogramFieldWellsOutputTypeDef",
+BoxPlotFieldWellsTypeDef = TypedDict(
+    "BoxPlotFieldWellsTypeDef",
     {
-        "HistogramAggregatedFieldWells": HistogramAggregatedFieldWellsOutputTypeDef,
+        "BoxPlotAggregatedFieldWells": BoxPlotAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-KPIConfigurationOutputTypeDef = TypedDict(
-    "KPIConfigurationOutputTypeDef",
+ComboChartFieldWellsOutputTypeDef = TypedDict(
+    "ComboChartFieldWellsOutputTypeDef",
     {
-        "FieldWells": KPIFieldWellsOutputTypeDef,
-        "SortConfiguration": KPISortConfigurationOutputTypeDef,
-        "KPIOptions": KPIOptionsOutputTypeDef,
+        "ComboChartAggregatedFieldWells": ComboChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-LineChartFieldWellsOutputTypeDef = TypedDict(
-    "LineChartFieldWellsOutputTypeDef",
+ComboChartFieldWellsTypeDef = TypedDict(
+    "ComboChartFieldWellsTypeDef",
     {
-        "LineChartAggregatedFieldWells": LineChartAggregatedFieldWellsOutputTypeDef,
+        "ComboChartAggregatedFieldWells": ComboChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-PieChartFieldWellsOutputTypeDef = TypedDict(
-    "PieChartFieldWellsOutputTypeDef",
+FilledMapFieldWellsOutputTypeDef = TypedDict(
+    "FilledMapFieldWellsOutputTypeDef",
     {
-        "PieChartAggregatedFieldWells": PieChartAggregatedFieldWellsOutputTypeDef,
+        "FilledMapAggregatedFieldWells": FilledMapAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-PivotTableFieldWellsOutputTypeDef = TypedDict(
-    "PivotTableFieldWellsOutputTypeDef",
+FilledMapFieldWellsTypeDef = TypedDict(
+    "FilledMapFieldWellsTypeDef",
     {
-        "PivotTableAggregatedFieldWells": PivotTableAggregatedFieldWellsOutputTypeDef,
+        "FilledMapAggregatedFieldWells": FilledMapAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-RadarChartFieldWellsOutputTypeDef = TypedDict(
-    "RadarChartFieldWellsOutputTypeDef",
+FunnelChartFieldWellsOutputTypeDef = TypedDict(
+    "FunnelChartFieldWellsOutputTypeDef",
     {
-        "RadarChartAggregatedFieldWells": RadarChartAggregatedFieldWellsOutputTypeDef,
+        "FunnelChartAggregatedFieldWells": FunnelChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-SankeyDiagramFieldWellsOutputTypeDef = TypedDict(
-    "SankeyDiagramFieldWellsOutputTypeDef",
+FunnelChartFieldWellsTypeDef = TypedDict(
+    "FunnelChartFieldWellsTypeDef",
     {
-        "SankeyDiagramAggregatedFieldWells": SankeyDiagramAggregatedFieldWellsOutputTypeDef,
+        "FunnelChartAggregatedFieldWells": FunnelChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-ScatterPlotFieldWellsOutputTypeDef = TypedDict(
-    "ScatterPlotFieldWellsOutputTypeDef",
+GaugeChartConfigurationOutputTypeDef = TypedDict(
+    "GaugeChartConfigurationOutputTypeDef",
     {
-        "ScatterPlotCategoricallyAggregatedFieldWells": (
-            ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef
-        ),
-        "ScatterPlotUnaggregatedFieldWells": ScatterPlotUnaggregatedFieldWellsOutputTypeDef,
+        "FieldWells": GaugeChartFieldWellsOutputTypeDef,
+        "GaugeChartOptions": GaugeChartOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "TooltipOptions": TooltipOptionsOutputTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
     },
     total=False,
 )
 
-ComputationOutputTypeDef = TypedDict(
-    "ComputationOutputTypeDef",
+GaugeChartConfigurationTypeDef = TypedDict(
+    "GaugeChartConfigurationTypeDef",
     {
-        "TopBottomRanked": TopBottomRankedComputationOutputTypeDef,
-        "TopBottomMovers": TopBottomMoversComputationOutputTypeDef,
-        "TotalAggregation": TotalAggregationComputationOutputTypeDef,
-        "MaximumMinimum": MaximumMinimumComputationOutputTypeDef,
-        "MetricComparison": MetricComparisonComputationOutputTypeDef,
-        "PeriodOverPeriod": PeriodOverPeriodComputationOutputTypeDef,
-        "PeriodToDate": PeriodToDateComputationOutputTypeDef,
-        "GrowthRate": GrowthRateComputationOutputTypeDef,
-        "UniqueValues": UniqueValuesComputationOutputTypeDef,
-        "Forecast": ForecastComputationOutputTypeDef,
+        "FieldWells": GaugeChartFieldWellsTypeDef,
+        "GaugeChartOptions": GaugeChartOptionsTypeDef,
+        "DataLabels": DataLabelOptionsTypeDef,
+        "TooltipOptions": TooltipOptionsTypeDef,
+        "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
-TreeMapFieldWellsOutputTypeDef = TypedDict(
-    "TreeMapFieldWellsOutputTypeDef",
+GeospatialMapFieldWellsOutputTypeDef = TypedDict(
+    "GeospatialMapFieldWellsOutputTypeDef",
     {
-        "TreeMapAggregatedFieldWells": TreeMapAggregatedFieldWellsOutputTypeDef,
+        "GeospatialMapAggregatedFieldWells": GeospatialMapAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-WaterfallChartFieldWellsOutputTypeDef = TypedDict(
-    "WaterfallChartFieldWellsOutputTypeDef",
+GeospatialMapFieldWellsTypeDef = TypedDict(
+    "GeospatialMapFieldWellsTypeDef",
     {
-        "WaterfallChartAggregatedFieldWells": WaterfallChartAggregatedFieldWellsOutputTypeDef,
+        "GeospatialMapAggregatedFieldWells": GeospatialMapAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-WordCloudFieldWellsOutputTypeDef = TypedDict(
-    "WordCloudFieldWellsOutputTypeDef",
+HeatMapFieldWellsOutputTypeDef = TypedDict(
+    "HeatMapFieldWellsOutputTypeDef",
     {
-        "WordCloudAggregatedFieldWells": WordCloudAggregatedFieldWellsOutputTypeDef,
+        "HeatMapAggregatedFieldWells": HeatMapAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-TableFieldWellsOutputTypeDef = TypedDict(
-    "TableFieldWellsOutputTypeDef",
+HeatMapFieldWellsTypeDef = TypedDict(
+    "HeatMapFieldWellsTypeDef",
     {
-        "TableAggregatedFieldWells": TableAggregatedFieldWellsOutputTypeDef,
-        "TableUnaggregatedFieldWells": TableUnaggregatedFieldWellsOutputTypeDef,
+        "HeatMapAggregatedFieldWells": HeatMapAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-BarChartFieldWellsTypeDef = TypedDict(
-    "BarChartFieldWellsTypeDef",
+HistogramFieldWellsOutputTypeDef = TypedDict(
+    "HistogramFieldWellsOutputTypeDef",
     {
-        "BarChartAggregatedFieldWells": BarChartAggregatedFieldWellsTypeDef,
+        "HistogramAggregatedFieldWells": HistogramAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-BoxPlotFieldWellsTypeDef = TypedDict(
-    "BoxPlotFieldWellsTypeDef",
+HistogramFieldWellsTypeDef = TypedDict(
+    "HistogramFieldWellsTypeDef",
     {
-        "BoxPlotAggregatedFieldWells": BoxPlotAggregatedFieldWellsTypeDef,
+        "HistogramAggregatedFieldWells": HistogramAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-ComboChartFieldWellsTypeDef = TypedDict(
-    "ComboChartFieldWellsTypeDef",
+KPIConfigurationOutputTypeDef = TypedDict(
+    "KPIConfigurationOutputTypeDef",
     {
-        "ComboChartAggregatedFieldWells": ComboChartAggregatedFieldWellsTypeDef,
+        "FieldWells": KPIFieldWellsOutputTypeDef,
+        "SortConfiguration": KPISortConfigurationOutputTypeDef,
+        "KPIOptions": KPIOptionsTypeDef,
     },
     total=False,
 )
 
-FilledMapFieldWellsTypeDef = TypedDict(
-    "FilledMapFieldWellsTypeDef",
+KPIConfigurationTypeDef = TypedDict(
+    "KPIConfigurationTypeDef",
     {
-        "FilledMapAggregatedFieldWells": FilledMapAggregatedFieldWellsTypeDef,
+        "FieldWells": KPIFieldWellsTypeDef,
+        "SortConfiguration": KPISortConfigurationTypeDef,
+        "KPIOptions": KPIOptionsTypeDef,
     },
     total=False,
 )
 
-FunnelChartFieldWellsTypeDef = TypedDict(
-    "FunnelChartFieldWellsTypeDef",
+LineChartFieldWellsOutputTypeDef = TypedDict(
+    "LineChartFieldWellsOutputTypeDef",
     {
-        "FunnelChartAggregatedFieldWells": FunnelChartAggregatedFieldWellsTypeDef,
+        "LineChartAggregatedFieldWells": LineChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-GaugeChartConfigurationTypeDef = TypedDict(
-    "GaugeChartConfigurationTypeDef",
+LineChartFieldWellsTypeDef = TypedDict(
+    "LineChartFieldWellsTypeDef",
     {
-        "FieldWells": GaugeChartFieldWellsTypeDef,
-        "GaugeChartOptions": GaugeChartOptionsTypeDef,
-        "DataLabels": DataLabelOptionsTypeDef,
-        "TooltipOptions": TooltipOptionsTypeDef,
-        "VisualPalette": VisualPaletteTypeDef,
+        "LineChartAggregatedFieldWells": LineChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-GeospatialMapFieldWellsTypeDef = TypedDict(
-    "GeospatialMapFieldWellsTypeDef",
+PieChartFieldWellsOutputTypeDef = TypedDict(
+    "PieChartFieldWellsOutputTypeDef",
     {
-        "GeospatialMapAggregatedFieldWells": GeospatialMapAggregatedFieldWellsTypeDef,
+        "PieChartAggregatedFieldWells": PieChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-HeatMapFieldWellsTypeDef = TypedDict(
-    "HeatMapFieldWellsTypeDef",
+PieChartFieldWellsTypeDef = TypedDict(
+    "PieChartFieldWellsTypeDef",
     {
-        "HeatMapAggregatedFieldWells": HeatMapAggregatedFieldWellsTypeDef,
+        "PieChartAggregatedFieldWells": PieChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-HistogramFieldWellsTypeDef = TypedDict(
-    "HistogramFieldWellsTypeDef",
+PivotTableFieldWellsOutputTypeDef = TypedDict(
+    "PivotTableFieldWellsOutputTypeDef",
     {
-        "HistogramAggregatedFieldWells": HistogramAggregatedFieldWellsTypeDef,
+        "PivotTableAggregatedFieldWells": PivotTableAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-KPIConfigurationTypeDef = TypedDict(
-    "KPIConfigurationTypeDef",
+PivotTableFieldWellsTypeDef = TypedDict(
+    "PivotTableFieldWellsTypeDef",
     {
-        "FieldWells": KPIFieldWellsTypeDef,
-        "SortConfiguration": KPISortConfigurationTypeDef,
-        "KPIOptions": KPIOptionsTypeDef,
+        "PivotTableAggregatedFieldWells": PivotTableAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-LineChartFieldWellsTypeDef = TypedDict(
-    "LineChartFieldWellsTypeDef",
+RadarChartFieldWellsOutputTypeDef = TypedDict(
+    "RadarChartFieldWellsOutputTypeDef",
     {
-        "LineChartAggregatedFieldWells": LineChartAggregatedFieldWellsTypeDef,
+        "RadarChartAggregatedFieldWells": RadarChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-PieChartFieldWellsTypeDef = TypedDict(
-    "PieChartFieldWellsTypeDef",
+RadarChartFieldWellsTypeDef = TypedDict(
+    "RadarChartFieldWellsTypeDef",
     {
-        "PieChartAggregatedFieldWells": PieChartAggregatedFieldWellsTypeDef,
+        "RadarChartAggregatedFieldWells": RadarChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-PivotTableFieldWellsTypeDef = TypedDict(
-    "PivotTableFieldWellsTypeDef",
+SankeyDiagramFieldWellsOutputTypeDef = TypedDict(
+    "SankeyDiagramFieldWellsOutputTypeDef",
     {
-        "PivotTableAggregatedFieldWells": PivotTableAggregatedFieldWellsTypeDef,
+        "SankeyDiagramAggregatedFieldWells": SankeyDiagramAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-RadarChartFieldWellsTypeDef = TypedDict(
-    "RadarChartFieldWellsTypeDef",
+SankeyDiagramFieldWellsTypeDef = TypedDict(
+    "SankeyDiagramFieldWellsTypeDef",
     {
-        "RadarChartAggregatedFieldWells": RadarChartAggregatedFieldWellsTypeDef,
+        "SankeyDiagramAggregatedFieldWells": SankeyDiagramAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-SankeyDiagramFieldWellsTypeDef = TypedDict(
-    "SankeyDiagramFieldWellsTypeDef",
+ScatterPlotFieldWellsOutputTypeDef = TypedDict(
+    "ScatterPlotFieldWellsOutputTypeDef",
     {
-        "SankeyDiagramAggregatedFieldWells": SankeyDiagramAggregatedFieldWellsTypeDef,
+        "ScatterPlotCategoricallyAggregatedFieldWells": (
+            ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef
+        ),
+        "ScatterPlotUnaggregatedFieldWells": ScatterPlotUnaggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
 ScatterPlotFieldWellsTypeDef = TypedDict(
     "ScatterPlotFieldWellsTypeDef",
     {
@@ -22095,38 +17889,71 @@
         "GrowthRate": GrowthRateComputationTypeDef,
         "UniqueValues": UniqueValuesComputationTypeDef,
         "Forecast": ForecastComputationTypeDef,
     },
     total=False,
 )
 
+TreeMapFieldWellsOutputTypeDef = TypedDict(
+    "TreeMapFieldWellsOutputTypeDef",
+    {
+        "TreeMapAggregatedFieldWells": TreeMapAggregatedFieldWellsOutputTypeDef,
+    },
+    total=False,
+)
+
 TreeMapFieldWellsTypeDef = TypedDict(
     "TreeMapFieldWellsTypeDef",
     {
         "TreeMapAggregatedFieldWells": TreeMapAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
+WaterfallChartFieldWellsOutputTypeDef = TypedDict(
+    "WaterfallChartFieldWellsOutputTypeDef",
+    {
+        "WaterfallChartAggregatedFieldWells": WaterfallChartAggregatedFieldWellsOutputTypeDef,
+    },
+    total=False,
+)
+
 WaterfallChartFieldWellsTypeDef = TypedDict(
     "WaterfallChartFieldWellsTypeDef",
     {
         "WaterfallChartAggregatedFieldWells": WaterfallChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
+WordCloudFieldWellsOutputTypeDef = TypedDict(
+    "WordCloudFieldWellsOutputTypeDef",
+    {
+        "WordCloudAggregatedFieldWells": WordCloudAggregatedFieldWellsOutputTypeDef,
+    },
+    total=False,
+)
+
 WordCloudFieldWellsTypeDef = TypedDict(
     "WordCloudFieldWellsTypeDef",
     {
         "WordCloudAggregatedFieldWells": WordCloudAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
+TableFieldWellsOutputTypeDef = TypedDict(
+    "TableFieldWellsOutputTypeDef",
+    {
+        "TableAggregatedFieldWells": TableAggregatedFieldWellsOutputTypeDef,
+        "TableUnaggregatedFieldWells": TableUnaggregatedFieldWellsOutputTypeDef,
+    },
+    total=False,
+)
+
 TableFieldWellsTypeDef = TypedDict(
     "TableFieldWellsTypeDef",
     {
         "TableAggregatedFieldWells": TableAggregatedFieldWellsTypeDef,
         "TableUnaggregatedFieldWells": TableUnaggregatedFieldWellsTypeDef,
     },
     total=False,
@@ -22156,362 +17983,29 @@
     "BarChartConfigurationOutputTypeDef",
     {
         "FieldWells": BarChartFieldWellsOutputTypeDef,
         "SortConfiguration": BarChartSortConfigurationOutputTypeDef,
         "Orientation": BarChartOrientationType,
         "BarsArrangement": BarsArrangementType,
         "VisualPalette": VisualPaletteOutputTypeDef,
-        "SmallMultiplesOptions": SmallMultiplesOptionsOutputTypeDef,
+        "SmallMultiplesOptions": SmallMultiplesOptionsTypeDef,
         "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
         "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
         "ValueAxis": AxisDisplayOptionsOutputTypeDef,
         "ValueLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
         "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "ReferenceLines": List[ReferenceLineOutputTypeDef],
-        "ContributionAnalysisDefaults": List[ContributionAnalysisDefaultOutputTypeDef],
-    },
-    total=False,
-)
-
-BoxPlotChartConfigurationOutputTypeDef = TypedDict(
-    "BoxPlotChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": BoxPlotFieldWellsOutputTypeDef,
-        "SortConfiguration": BoxPlotSortConfigurationOutputTypeDef,
-        "BoxPlotOptions": BoxPlotOptionsOutputTypeDef,
-        "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
-        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "PrimaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "ReferenceLines": List[ReferenceLineOutputTypeDef],
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-ComboChartConfigurationOutputTypeDef = TypedDict(
-    "ComboChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": ComboChartFieldWellsOutputTypeDef,
-        "SortConfiguration": ComboChartSortConfigurationOutputTypeDef,
-        "BarsArrangement": BarsArrangementType,
-        "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
-        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "PrimaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "SecondaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "SecondaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "BarDataLabels": DataLabelOptionsOutputTypeDef,
-        "LineDataLabels": DataLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "ReferenceLines": List[ReferenceLineOutputTypeDef],
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-FilledMapConfigurationOutputTypeDef = TypedDict(
-    "FilledMapConfigurationOutputTypeDef",
-    {
-        "FieldWells": FilledMapFieldWellsOutputTypeDef,
-        "SortConfiguration": FilledMapSortConfigurationOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "WindowOptions": GeospatialWindowOptionsOutputTypeDef,
-        "MapStyleOptions": GeospatialMapStyleOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-FunnelChartConfigurationOutputTypeDef = TypedDict(
-    "FunnelChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": FunnelChartFieldWellsOutputTypeDef,
-        "SortConfiguration": FunnelChartSortConfigurationOutputTypeDef,
-        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ValueLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "DataLabelOptions": FunnelChartDataLabelOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGaugeChartVisualOutputTypeDef = TypedDict(
-    "_RequiredGaugeChartVisualOutputTypeDef",
-    {
-        "VisualId": str,
-    },
-)
-_OptionalGaugeChartVisualOutputTypeDef = TypedDict(
-    "_OptionalGaugeChartVisualOutputTypeDef",
-    {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": GaugeChartConfigurationOutputTypeDef,
-        "ConditionalFormatting": GaugeChartConditionalFormattingOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class GaugeChartVisualOutputTypeDef(
-    _RequiredGaugeChartVisualOutputTypeDef, _OptionalGaugeChartVisualOutputTypeDef
-):
-    pass
-
-
-GeospatialMapConfigurationOutputTypeDef = TypedDict(
-    "GeospatialMapConfigurationOutputTypeDef",
-    {
-        "FieldWells": GeospatialMapFieldWellsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "WindowOptions": GeospatialWindowOptionsOutputTypeDef,
-        "MapStyleOptions": GeospatialMapStyleOptionsOutputTypeDef,
-        "PointStyleOptions": GeospatialPointStyleOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-HeatMapConfigurationOutputTypeDef = TypedDict(
-    "HeatMapConfigurationOutputTypeDef",
-    {
-        "FieldWells": HeatMapFieldWellsOutputTypeDef,
-        "SortConfiguration": HeatMapSortConfigurationOutputTypeDef,
-        "RowLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ColumnLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ColorScale": ColorScaleOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-HistogramConfigurationOutputTypeDef = TypedDict(
-    "HistogramConfigurationOutputTypeDef",
-    {
-        "FieldWells": HistogramFieldWellsOutputTypeDef,
-        "XAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "XAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "YAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "BinOptions": HistogramBinOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredKPIVisualOutputTypeDef = TypedDict(
-    "_RequiredKPIVisualOutputTypeDef",
-    {
-        "VisualId": str,
-    },
-)
-_OptionalKPIVisualOutputTypeDef = TypedDict(
-    "_OptionalKPIVisualOutputTypeDef",
-    {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": KPIConfigurationOutputTypeDef,
-        "ConditionalFormatting": KPIConditionalFormattingOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class KPIVisualOutputTypeDef(_RequiredKPIVisualOutputTypeDef, _OptionalKPIVisualOutputTypeDef):
-    pass
-
-
-LineChartConfigurationOutputTypeDef = TypedDict(
-    "LineChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": LineChartFieldWellsOutputTypeDef,
-        "SortConfiguration": LineChartSortConfigurationOutputTypeDef,
-        "ForecastConfigurations": List[ForecastConfigurationOutputTypeDef],
-        "Type": LineChartTypeType,
-        "SmallMultiplesOptions": SmallMultiplesOptionsOutputTypeDef,
-        "XAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "XAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "PrimaryYAxisDisplayOptions": LineSeriesAxisDisplayOptionsOutputTypeDef,
-        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "SecondaryYAxisDisplayOptions": LineSeriesAxisDisplayOptionsOutputTypeDef,
-        "SecondaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "DefaultSeriesSettings": LineChartDefaultSeriesSettingsOutputTypeDef,
-        "Series": List[SeriesItemOutputTypeDef],
-        "Legend": LegendOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "ReferenceLines": List[ReferenceLineOutputTypeDef],
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "ContributionAnalysisDefaults": List[ContributionAnalysisDefaultOutputTypeDef],
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-PieChartConfigurationOutputTypeDef = TypedDict(
-    "PieChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": PieChartFieldWellsOutputTypeDef,
-        "SortConfiguration": PieChartSortConfigurationOutputTypeDef,
-        "DonutOptions": DonutOptionsOutputTypeDef,
-        "SmallMultiplesOptions": SmallMultiplesOptionsOutputTypeDef,
-        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ValueLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
         "DataLabels": DataLabelOptionsOutputTypeDef,
         "Tooltip": TooltipOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
+        "ReferenceLines": List[ReferenceLineTypeDef],
         "ContributionAnalysisDefaults": List[ContributionAnalysisDefaultOutputTypeDef],
     },
     total=False,
 )
 
-PivotTableConfigurationOutputTypeDef = TypedDict(
-    "PivotTableConfigurationOutputTypeDef",
-    {
-        "FieldWells": PivotTableFieldWellsOutputTypeDef,
-        "SortConfiguration": PivotTableSortConfigurationOutputTypeDef,
-        "TableOptions": PivotTableOptionsOutputTypeDef,
-        "TotalOptions": PivotTableTotalOptionsOutputTypeDef,
-        "FieldOptions": PivotTableFieldOptionsOutputTypeDef,
-        "PaginatedReportOptions": PivotTablePaginatedReportOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-RadarChartConfigurationOutputTypeDef = TypedDict(
-    "RadarChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": RadarChartFieldWellsOutputTypeDef,
-        "SortConfiguration": RadarChartSortConfigurationOutputTypeDef,
-        "Shape": RadarChartShapeType,
-        "BaseSeriesSettings": RadarChartSeriesSettingsOutputTypeDef,
-        "StartAngle": float,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-        "AlternateBandColorsVisibility": VisibilityType,
-        "AlternateBandEvenColor": str,
-        "AlternateBandOddColor": str,
-        "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
-        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ColorAxis": AxisDisplayOptionsOutputTypeDef,
-        "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "AxesRangeScale": RadarChartAxesRangeScaleType,
-    },
-    total=False,
-)
-
-SankeyDiagramChartConfigurationOutputTypeDef = TypedDict(
-    "SankeyDiagramChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": SankeyDiagramFieldWellsOutputTypeDef,
-        "SortConfiguration": SankeyDiagramSortConfigurationOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-ScatterPlotConfigurationOutputTypeDef = TypedDict(
-    "ScatterPlotConfigurationOutputTypeDef",
-    {
-        "FieldWells": ScatterPlotFieldWellsOutputTypeDef,
-        "XAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "XAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "YAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "YAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-InsightConfigurationOutputTypeDef = TypedDict(
-    "InsightConfigurationOutputTypeDef",
-    {
-        "Computations": List[ComputationOutputTypeDef],
-        "CustomNarrative": CustomNarrativeOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-TreeMapConfigurationOutputTypeDef = TypedDict(
-    "TreeMapConfigurationOutputTypeDef",
-    {
-        "FieldWells": TreeMapFieldWellsOutputTypeDef,
-        "SortConfiguration": TreeMapSortConfigurationOutputTypeDef,
-        "GroupLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "SizeLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ColorScale": ColorScaleOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-WaterfallChartConfigurationOutputTypeDef = TypedDict(
-    "WaterfallChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": WaterfallChartFieldWellsOutputTypeDef,
-        "SortConfiguration": WaterfallChartSortConfigurationOutputTypeDef,
-        "WaterfallChartOptions": WaterfallChartOptionsOutputTypeDef,
-        "CategoryAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "CategoryAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "PrimaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-WordCloudChartConfigurationOutputTypeDef = TypedDict(
-    "WordCloudChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": WordCloudFieldWellsOutputTypeDef,
-        "SortConfiguration": WordCloudSortConfigurationOutputTypeDef,
-        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "WordCloudOptions": WordCloudOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-TableConfigurationOutputTypeDef = TypedDict(
-    "TableConfigurationOutputTypeDef",
-    {
-        "FieldWells": TableFieldWellsOutputTypeDef,
-        "SortConfiguration": TableSortConfigurationOutputTypeDef,
-        "TableOptions": TableOptionsOutputTypeDef,
-        "TotalOptions": TotalOptionsOutputTypeDef,
-        "FieldOptions": TableFieldOptionsOutputTypeDef,
-        "PaginatedReportOptions": TablePaginatedReportOptionsOutputTypeDef,
-        "TableInlineVisualizations": List[TableInlineVisualizationOutputTypeDef],
-    },
-    total=False,
-)
-
 BarChartConfigurationTypeDef = TypedDict(
     "BarChartConfigurationTypeDef",
     {
         "FieldWells": BarChartFieldWellsTypeDef,
         "SortConfiguration": BarChartSortConfigurationTypeDef,
         "Orientation": BarChartOrientationType,
         "BarsArrangement": BarsArrangementType,
@@ -22527,14 +18021,32 @@
         "Tooltip": TooltipOptionsTypeDef,
         "ReferenceLines": Sequence[ReferenceLineTypeDef],
         "ContributionAnalysisDefaults": Sequence[ContributionAnalysisDefaultTypeDef],
     },
     total=False,
 )
 
+BoxPlotChartConfigurationOutputTypeDef = TypedDict(
+    "BoxPlotChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": BoxPlotFieldWellsOutputTypeDef,
+        "SortConfiguration": BoxPlotSortConfigurationOutputTypeDef,
+        "BoxPlotOptions": BoxPlotOptionsTypeDef,
+        "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
+        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "PrimaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "ReferenceLines": List[ReferenceLineTypeDef],
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 BoxPlotChartConfigurationTypeDef = TypedDict(
     "BoxPlotChartConfigurationTypeDef",
     {
         "FieldWells": BoxPlotFieldWellsTypeDef,
         "SortConfiguration": BoxPlotSortConfigurationTypeDef,
         "BoxPlotOptions": BoxPlotOptionsTypeDef,
         "CategoryAxis": AxisDisplayOptionsTypeDef,
@@ -22545,14 +18057,37 @@
         "Tooltip": TooltipOptionsTypeDef,
         "ReferenceLines": Sequence[ReferenceLineTypeDef],
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+ComboChartConfigurationOutputTypeDef = TypedDict(
+    "ComboChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": ComboChartFieldWellsOutputTypeDef,
+        "SortConfiguration": ComboChartSortConfigurationOutputTypeDef,
+        "BarsArrangement": BarsArrangementType,
+        "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
+        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "PrimaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "SecondaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "SecondaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "BarDataLabels": DataLabelOptionsOutputTypeDef,
+        "LineDataLabels": DataLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "ReferenceLines": List[ReferenceLineTypeDef],
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 ComboChartConfigurationTypeDef = TypedDict(
     "ComboChartConfigurationTypeDef",
     {
         "FieldWells": ComboChartFieldWellsTypeDef,
         "SortConfiguration": ComboChartSortConfigurationTypeDef,
         "BarsArrangement": BarsArrangementType,
         "CategoryAxis": AxisDisplayOptionsTypeDef,
@@ -22568,41 +18103,93 @@
         "Tooltip": TooltipOptionsTypeDef,
         "ReferenceLines": Sequence[ReferenceLineTypeDef],
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+FilledMapConfigurationOutputTypeDef = TypedDict(
+    "FilledMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": FilledMapFieldWellsOutputTypeDef,
+        "SortConfiguration": FilledMapSortConfigurationOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "WindowOptions": GeospatialWindowOptionsTypeDef,
+        "MapStyleOptions": GeospatialMapStyleOptionsTypeDef,
+    },
+    total=False,
+)
+
 FilledMapConfigurationTypeDef = TypedDict(
     "FilledMapConfigurationTypeDef",
     {
         "FieldWells": FilledMapFieldWellsTypeDef,
         "SortConfiguration": FilledMapSortConfigurationTypeDef,
         "Legend": LegendOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
         "WindowOptions": GeospatialWindowOptionsTypeDef,
         "MapStyleOptions": GeospatialMapStyleOptionsTypeDef,
     },
     total=False,
 )
 
+FunnelChartConfigurationOutputTypeDef = TypedDict(
+    "FunnelChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": FunnelChartFieldWellsOutputTypeDef,
+        "SortConfiguration": FunnelChartSortConfigurationOutputTypeDef,
+        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ValueLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "DataLabelOptions": FunnelChartDataLabelOptionsTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 FunnelChartConfigurationTypeDef = TypedDict(
     "FunnelChartConfigurationTypeDef",
     {
         "FieldWells": FunnelChartFieldWellsTypeDef,
         "SortConfiguration": FunnelChartSortConfigurationTypeDef,
         "CategoryLabelOptions": ChartAxisLabelOptionsTypeDef,
         "ValueLabelOptions": ChartAxisLabelOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
         "DataLabelOptions": FunnelChartDataLabelOptionsTypeDef,
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+_RequiredGaugeChartVisualOutputTypeDef = TypedDict(
+    "_RequiredGaugeChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+    },
+)
+_OptionalGaugeChartVisualOutputTypeDef = TypedDict(
+    "_OptionalGaugeChartVisualOutputTypeDef",
+    {
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": GaugeChartConfigurationOutputTypeDef,
+        "ConditionalFormatting": GaugeChartConditionalFormattingOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class GaugeChartVisualOutputTypeDef(
+    _RequiredGaugeChartVisualOutputTypeDef, _OptionalGaugeChartVisualOutputTypeDef
+):
+    pass
+
+
 _RequiredGaugeChartVisualTypeDef = TypedDict(
     "_RequiredGaugeChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
 _OptionalGaugeChartVisualTypeDef = TypedDict(
@@ -22618,28 +18205,57 @@
 )
 
 
 class GaugeChartVisualTypeDef(_RequiredGaugeChartVisualTypeDef, _OptionalGaugeChartVisualTypeDef):
     pass
 
 
+GeospatialMapConfigurationOutputTypeDef = TypedDict(
+    "GeospatialMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": GeospatialMapFieldWellsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "WindowOptions": GeospatialWindowOptionsTypeDef,
+        "MapStyleOptions": GeospatialMapStyleOptionsTypeDef,
+        "PointStyleOptions": GeospatialPointStyleOptionsOutputTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 GeospatialMapConfigurationTypeDef = TypedDict(
     "GeospatialMapConfigurationTypeDef",
     {
         "FieldWells": GeospatialMapFieldWellsTypeDef,
         "Legend": LegendOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
         "WindowOptions": GeospatialWindowOptionsTypeDef,
         "MapStyleOptions": GeospatialMapStyleOptionsTypeDef,
         "PointStyleOptions": GeospatialPointStyleOptionsTypeDef,
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+HeatMapConfigurationOutputTypeDef = TypedDict(
+    "HeatMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": HeatMapFieldWellsOutputTypeDef,
+        "SortConfiguration": HeatMapSortConfigurationOutputTypeDef,
+        "RowLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ColumnLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ColorScale": ColorScaleOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 HeatMapConfigurationTypeDef = TypedDict(
     "HeatMapConfigurationTypeDef",
     {
         "FieldWells": HeatMapFieldWellsTypeDef,
         "SortConfiguration": HeatMapSortConfigurationTypeDef,
         "RowLabelOptions": ChartAxisLabelOptionsTypeDef,
         "ColumnLabelOptions": ChartAxisLabelOptionsTypeDef,
@@ -22647,14 +18263,29 @@
         "Legend": LegendOptionsTypeDef,
         "DataLabels": DataLabelOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
     },
     total=False,
 )
 
+HistogramConfigurationOutputTypeDef = TypedDict(
+    "HistogramConfigurationOutputTypeDef",
+    {
+        "FieldWells": HistogramFieldWellsOutputTypeDef,
+        "XAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "XAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "YAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "BinOptions": HistogramBinOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 HistogramConfigurationTypeDef = TypedDict(
     "HistogramConfigurationTypeDef",
     {
         "FieldWells": HistogramFieldWellsTypeDef,
         "XAxisDisplayOptions": AxisDisplayOptionsTypeDef,
         "XAxisLabelOptions": ChartAxisLabelOptionsTypeDef,
         "YAxisDisplayOptions": AxisDisplayOptionsTypeDef,
@@ -22662,14 +18293,38 @@
         "DataLabels": DataLabelOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+_RequiredKPIVisualOutputTypeDef = TypedDict(
+    "_RequiredKPIVisualOutputTypeDef",
+    {
+        "VisualId": str,
+    },
+)
+_OptionalKPIVisualOutputTypeDef = TypedDict(
+    "_OptionalKPIVisualOutputTypeDef",
+    {
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": KPIConfigurationOutputTypeDef,
+        "ConditionalFormatting": KPIConditionalFormattingOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class KPIVisualOutputTypeDef(_RequiredKPIVisualOutputTypeDef, _OptionalKPIVisualOutputTypeDef):
+    pass
+
+
 _RequiredKPIVisualTypeDef = TypedDict(
     "_RequiredKPIVisualTypeDef",
     {
         "VisualId": str,
     },
 )
 _OptionalKPIVisualTypeDef = TypedDict(
@@ -22686,14 +18341,40 @@
 )
 
 
 class KPIVisualTypeDef(_RequiredKPIVisualTypeDef, _OptionalKPIVisualTypeDef):
     pass
 
 
+LineChartConfigurationOutputTypeDef = TypedDict(
+    "LineChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": LineChartFieldWellsOutputTypeDef,
+        "SortConfiguration": LineChartSortConfigurationOutputTypeDef,
+        "ForecastConfigurations": List[ForecastConfigurationOutputTypeDef],
+        "Type": LineChartTypeType,
+        "SmallMultiplesOptions": SmallMultiplesOptionsTypeDef,
+        "XAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "XAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "PrimaryYAxisDisplayOptions": LineSeriesAxisDisplayOptionsOutputTypeDef,
+        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "SecondaryYAxisDisplayOptions": LineSeriesAxisDisplayOptionsOutputTypeDef,
+        "SecondaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "DefaultSeriesSettings": LineChartDefaultSeriesSettingsTypeDef,
+        "Series": List[SeriesItemTypeDef],
+        "Legend": LegendOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "ReferenceLines": List[ReferenceLineTypeDef],
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "ContributionAnalysisDefaults": List[ContributionAnalysisDefaultOutputTypeDef],
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 LineChartConfigurationTypeDef = TypedDict(
     "LineChartConfigurationTypeDef",
     {
         "FieldWells": LineChartFieldWellsTypeDef,
         "SortConfiguration": LineChartSortConfigurationTypeDef,
         "ForecastConfigurations": Sequence[ForecastConfigurationTypeDef],
         "Type": LineChartTypeType,
@@ -22712,14 +18393,32 @@
         "Tooltip": TooltipOptionsTypeDef,
         "ContributionAnalysisDefaults": Sequence[ContributionAnalysisDefaultTypeDef],
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+PieChartConfigurationOutputTypeDef = TypedDict(
+    "PieChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": PieChartFieldWellsOutputTypeDef,
+        "SortConfiguration": PieChartSortConfigurationOutputTypeDef,
+        "DonutOptions": DonutOptionsTypeDef,
+        "SmallMultiplesOptions": SmallMultiplesOptionsTypeDef,
+        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ValueLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+        "ContributionAnalysisDefaults": List[ContributionAnalysisDefaultOutputTypeDef],
+    },
+    total=False,
+)
+
 PieChartConfigurationTypeDef = TypedDict(
     "PieChartConfigurationTypeDef",
     {
         "FieldWells": PieChartFieldWellsTypeDef,
         "SortConfiguration": PieChartSortConfigurationTypeDef,
         "DonutOptions": DonutOptionsTypeDef,
         "SmallMultiplesOptions": SmallMultiplesOptionsTypeDef,
@@ -22730,27 +18429,62 @@
         "Tooltip": TooltipOptionsTypeDef,
         "VisualPalette": VisualPaletteTypeDef,
         "ContributionAnalysisDefaults": Sequence[ContributionAnalysisDefaultTypeDef],
     },
     total=False,
 )
 
+PivotTableConfigurationOutputTypeDef = TypedDict(
+    "PivotTableConfigurationOutputTypeDef",
+    {
+        "FieldWells": PivotTableFieldWellsOutputTypeDef,
+        "SortConfiguration": PivotTableSortConfigurationOutputTypeDef,
+        "TableOptions": PivotTableOptionsOutputTypeDef,
+        "TotalOptions": PivotTableTotalOptionsOutputTypeDef,
+        "FieldOptions": PivotTableFieldOptionsOutputTypeDef,
+        "PaginatedReportOptions": PivotTablePaginatedReportOptionsTypeDef,
+    },
+    total=False,
+)
+
 PivotTableConfigurationTypeDef = TypedDict(
     "PivotTableConfigurationTypeDef",
     {
         "FieldWells": PivotTableFieldWellsTypeDef,
         "SortConfiguration": PivotTableSortConfigurationTypeDef,
         "TableOptions": PivotTableOptionsTypeDef,
         "TotalOptions": PivotTableTotalOptionsTypeDef,
         "FieldOptions": PivotTableFieldOptionsTypeDef,
         "PaginatedReportOptions": PivotTablePaginatedReportOptionsTypeDef,
     },
     total=False,
 )
 
+RadarChartConfigurationOutputTypeDef = TypedDict(
+    "RadarChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": RadarChartFieldWellsOutputTypeDef,
+        "SortConfiguration": RadarChartSortConfigurationOutputTypeDef,
+        "Shape": RadarChartShapeType,
+        "BaseSeriesSettings": RadarChartSeriesSettingsTypeDef,
+        "StartAngle": float,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+        "AlternateBandColorsVisibility": VisibilityType,
+        "AlternateBandEvenColor": str,
+        "AlternateBandOddColor": str,
+        "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
+        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ColorAxis": AxisDisplayOptionsOutputTypeDef,
+        "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "AxesRangeScale": RadarChartAxesRangeScaleType,
+    },
+    total=False,
+)
+
 RadarChartConfigurationTypeDef = TypedDict(
     "RadarChartConfigurationTypeDef",
     {
         "FieldWells": RadarChartFieldWellsTypeDef,
         "SortConfiguration": RadarChartSortConfigurationTypeDef,
         "Shape": RadarChartShapeType,
         "BaseSeriesSettings": RadarChartSeriesSettingsTypeDef,
@@ -22765,24 +18499,50 @@
         "ColorLabelOptions": ChartAxisLabelOptionsTypeDef,
         "Legend": LegendOptionsTypeDef,
         "AxesRangeScale": RadarChartAxesRangeScaleType,
     },
     total=False,
 )
 
+SankeyDiagramChartConfigurationOutputTypeDef = TypedDict(
+    "SankeyDiagramChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": SankeyDiagramFieldWellsOutputTypeDef,
+        "SortConfiguration": SankeyDiagramSortConfigurationOutputTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 SankeyDiagramChartConfigurationTypeDef = TypedDict(
     "SankeyDiagramChartConfigurationTypeDef",
     {
         "FieldWells": SankeyDiagramFieldWellsTypeDef,
         "SortConfiguration": SankeyDiagramSortConfigurationTypeDef,
         "DataLabels": DataLabelOptionsTypeDef,
     },
     total=False,
 )
 
+ScatterPlotConfigurationOutputTypeDef = TypedDict(
+    "ScatterPlotConfigurationOutputTypeDef",
+    {
+        "FieldWells": ScatterPlotFieldWellsOutputTypeDef,
+        "XAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "XAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "YAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "YAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 ScatterPlotConfigurationTypeDef = TypedDict(
     "ScatterPlotConfigurationTypeDef",
     {
         "FieldWells": ScatterPlotFieldWellsTypeDef,
         "XAxisLabelOptions": ChartAxisLabelOptionsTypeDef,
         "XAxisDisplayOptions": AxisDisplayOptionsTypeDef,
         "YAxisLabelOptions": ChartAxisLabelOptionsTypeDef,
@@ -22791,23 +18551,48 @@
         "DataLabels": DataLabelOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+InsightConfigurationOutputTypeDef = TypedDict(
+    "InsightConfigurationOutputTypeDef",
+    {
+        "Computations": List[ComputationTypeDef],
+        "CustomNarrative": CustomNarrativeOptionsTypeDef,
+    },
+    total=False,
+)
+
 InsightConfigurationTypeDef = TypedDict(
     "InsightConfigurationTypeDef",
     {
         "Computations": Sequence[ComputationTypeDef],
         "CustomNarrative": CustomNarrativeOptionsTypeDef,
     },
     total=False,
 )
 
+TreeMapConfigurationOutputTypeDef = TypedDict(
+    "TreeMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": TreeMapFieldWellsOutputTypeDef,
+        "SortConfiguration": TreeMapSortConfigurationOutputTypeDef,
+        "GroupLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "SizeLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ColorScale": ColorScaleOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 TreeMapConfigurationTypeDef = TypedDict(
     "TreeMapConfigurationTypeDef",
     {
         "FieldWells": TreeMapFieldWellsTypeDef,
         "SortConfiguration": TreeMapSortConfigurationTypeDef,
         "GroupLabelOptions": ChartAxisLabelOptionsTypeDef,
         "SizeLabelOptions": ChartAxisLabelOptionsTypeDef,
@@ -22816,14 +18601,31 @@
         "Legend": LegendOptionsTypeDef,
         "DataLabels": DataLabelOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
     },
     total=False,
 )
 
+WaterfallChartConfigurationOutputTypeDef = TypedDict(
+    "WaterfallChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": WaterfallChartFieldWellsOutputTypeDef,
+        "SortConfiguration": WaterfallChartSortConfigurationOutputTypeDef,
+        "WaterfallChartOptions": WaterfallChartOptionsTypeDef,
+        "CategoryAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "CategoryAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "PrimaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 WaterfallChartConfigurationTypeDef = TypedDict(
     "WaterfallChartConfigurationTypeDef",
     {
         "FieldWells": WaterfallChartFieldWellsTypeDef,
         "SortConfiguration": WaterfallChartSortConfigurationTypeDef,
         "WaterfallChartOptions": WaterfallChartOptionsTypeDef,
         "CategoryAxisLabelOptions": ChartAxisLabelOptionsTypeDef,
@@ -22833,25 +18635,50 @@
         "Legend": LegendOptionsTypeDef,
         "DataLabels": DataLabelOptionsTypeDef,
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+WordCloudChartConfigurationOutputTypeDef = TypedDict(
+    "WordCloudChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": WordCloudFieldWellsOutputTypeDef,
+        "SortConfiguration": WordCloudSortConfigurationOutputTypeDef,
+        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "WordCloudOptions": WordCloudOptionsTypeDef,
+    },
+    total=False,
+)
+
 WordCloudChartConfigurationTypeDef = TypedDict(
     "WordCloudChartConfigurationTypeDef",
     {
         "FieldWells": WordCloudFieldWellsTypeDef,
         "SortConfiguration": WordCloudSortConfigurationTypeDef,
         "CategoryLabelOptions": ChartAxisLabelOptionsTypeDef,
         "WordCloudOptions": WordCloudOptionsTypeDef,
     },
     total=False,
 )
 
+TableConfigurationOutputTypeDef = TypedDict(
+    "TableConfigurationOutputTypeDef",
+    {
+        "FieldWells": TableFieldWellsOutputTypeDef,
+        "SortConfiguration": TableSortConfigurationOutputTypeDef,
+        "TableOptions": TableOptionsOutputTypeDef,
+        "TotalOptions": TotalOptionsTypeDef,
+        "FieldOptions": TableFieldOptionsOutputTypeDef,
+        "PaginatedReportOptions": TablePaginatedReportOptionsTypeDef,
+        "TableInlineVisualizations": List[TableInlineVisualizationTypeDef],
+    },
+    total=False,
+)
+
 TableConfigurationTypeDef = TypedDict(
     "TableConfigurationTypeDef",
     {
         "FieldWells": TableFieldWellsTypeDef,
         "SortConfiguration": TableSortConfigurationTypeDef,
         "TableOptions": TableOptionsTypeDef,
         "TotalOptions": TotalOptionsTypeDef,
@@ -22881,897 +18708,897 @@
     {
         "VisualId": str,
     },
 )
 _OptionalBarChartVisualOutputTypeDef = TypedDict(
     "_OptionalBarChartVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
         "ChartConfiguration": BarChartConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
         "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
 
 class BarChartVisualOutputTypeDef(
     _RequiredBarChartVisualOutputTypeDef, _OptionalBarChartVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredBoxPlotVisualOutputTypeDef = TypedDict(
-    "_RequiredBoxPlotVisualOutputTypeDef",
+_RequiredBarChartVisualTypeDef = TypedDict(
+    "_RequiredBarChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalBoxPlotVisualOutputTypeDef = TypedDict(
-    "_OptionalBoxPlotVisualOutputTypeDef",
+_OptionalBarChartVisualTypeDef = TypedDict(
+    "_OptionalBarChartVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": BoxPlotChartConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": BarChartConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
 
-class BoxPlotVisualOutputTypeDef(
-    _RequiredBoxPlotVisualOutputTypeDef, _OptionalBoxPlotVisualOutputTypeDef
-):
+class BarChartVisualTypeDef(_RequiredBarChartVisualTypeDef, _OptionalBarChartVisualTypeDef):
     pass
 
 
-_RequiredComboChartVisualOutputTypeDef = TypedDict(
-    "_RequiredComboChartVisualOutputTypeDef",
+_RequiredBoxPlotVisualOutputTypeDef = TypedDict(
+    "_RequiredBoxPlotVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalComboChartVisualOutputTypeDef = TypedDict(
-    "_OptionalComboChartVisualOutputTypeDef",
+_OptionalBoxPlotVisualOutputTypeDef = TypedDict(
+    "_OptionalBoxPlotVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": ComboChartConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": BoxPlotChartConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
         "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
 
-class ComboChartVisualOutputTypeDef(
-    _RequiredComboChartVisualOutputTypeDef, _OptionalComboChartVisualOutputTypeDef
+class BoxPlotVisualOutputTypeDef(
+    _RequiredBoxPlotVisualOutputTypeDef, _OptionalBoxPlotVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredFilledMapVisualOutputTypeDef = TypedDict(
-    "_RequiredFilledMapVisualOutputTypeDef",
+_RequiredBoxPlotVisualTypeDef = TypedDict(
+    "_RequiredBoxPlotVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalFilledMapVisualOutputTypeDef = TypedDict(
-    "_OptionalFilledMapVisualOutputTypeDef",
+_OptionalBoxPlotVisualTypeDef = TypedDict(
+    "_OptionalBoxPlotVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": FilledMapConfigurationOutputTypeDef,
-        "ConditionalFormatting": FilledMapConditionalFormattingOutputTypeDef,
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
-        "Actions": List[VisualCustomActionOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": BoxPlotChartConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
 
-class FilledMapVisualOutputTypeDef(
-    _RequiredFilledMapVisualOutputTypeDef, _OptionalFilledMapVisualOutputTypeDef
-):
+class BoxPlotVisualTypeDef(_RequiredBoxPlotVisualTypeDef, _OptionalBoxPlotVisualTypeDef):
     pass
 
 
-_RequiredFunnelChartVisualOutputTypeDef = TypedDict(
-    "_RequiredFunnelChartVisualOutputTypeDef",
+_RequiredComboChartVisualOutputTypeDef = TypedDict(
+    "_RequiredComboChartVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalFunnelChartVisualOutputTypeDef = TypedDict(
-    "_OptionalFunnelChartVisualOutputTypeDef",
+_OptionalComboChartVisualOutputTypeDef = TypedDict(
+    "_OptionalComboChartVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": FunnelChartConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": ComboChartConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
         "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
 
-class FunnelChartVisualOutputTypeDef(
-    _RequiredFunnelChartVisualOutputTypeDef, _OptionalFunnelChartVisualOutputTypeDef
+class ComboChartVisualOutputTypeDef(
+    _RequiredComboChartVisualOutputTypeDef, _OptionalComboChartVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredGeospatialMapVisualOutputTypeDef = TypedDict(
-    "_RequiredGeospatialMapVisualOutputTypeDef",
+_RequiredComboChartVisualTypeDef = TypedDict(
+    "_RequiredComboChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalGeospatialMapVisualOutputTypeDef = TypedDict(
-    "_OptionalGeospatialMapVisualOutputTypeDef",
+_OptionalComboChartVisualTypeDef = TypedDict(
+    "_OptionalComboChartVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": GeospatialMapConfigurationOutputTypeDef,
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
-        "Actions": List[VisualCustomActionOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": ComboChartConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
 
-class GeospatialMapVisualOutputTypeDef(
-    _RequiredGeospatialMapVisualOutputTypeDef, _OptionalGeospatialMapVisualOutputTypeDef
-):
+class ComboChartVisualTypeDef(_RequiredComboChartVisualTypeDef, _OptionalComboChartVisualTypeDef):
     pass
 
 
-_RequiredHeatMapVisualOutputTypeDef = TypedDict(
-    "_RequiredHeatMapVisualOutputTypeDef",
+_RequiredFilledMapVisualOutputTypeDef = TypedDict(
+    "_RequiredFilledMapVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalHeatMapVisualOutputTypeDef = TypedDict(
-    "_OptionalHeatMapVisualOutputTypeDef",
+_OptionalFilledMapVisualOutputTypeDef = TypedDict(
+    "_OptionalFilledMapVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": HeatMapConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": FilledMapConfigurationOutputTypeDef,
+        "ConditionalFormatting": FilledMapConditionalFormattingOutputTypeDef,
         "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
         "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
 
-class HeatMapVisualOutputTypeDef(
-    _RequiredHeatMapVisualOutputTypeDef, _OptionalHeatMapVisualOutputTypeDef
+class FilledMapVisualOutputTypeDef(
+    _RequiredFilledMapVisualOutputTypeDef, _OptionalFilledMapVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredHistogramVisualOutputTypeDef = TypedDict(
-    "_RequiredHistogramVisualOutputTypeDef",
+_RequiredFilledMapVisualTypeDef = TypedDict(
+    "_RequiredFilledMapVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalHistogramVisualOutputTypeDef = TypedDict(
-    "_OptionalHistogramVisualOutputTypeDef",
+_OptionalFilledMapVisualTypeDef = TypedDict(
+    "_OptionalFilledMapVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": HistogramConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": FilledMapConfigurationTypeDef,
+        "ConditionalFormatting": FilledMapConditionalFormattingTypeDef,
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "Actions": Sequence[VisualCustomActionTypeDef],
     },
     total=False,
 )
 
 
-class HistogramVisualOutputTypeDef(
-    _RequiredHistogramVisualOutputTypeDef, _OptionalHistogramVisualOutputTypeDef
-):
+class FilledMapVisualTypeDef(_RequiredFilledMapVisualTypeDef, _OptionalFilledMapVisualTypeDef):
     pass
 
 
-_RequiredLineChartVisualOutputTypeDef = TypedDict(
-    "_RequiredLineChartVisualOutputTypeDef",
+_RequiredFunnelChartVisualOutputTypeDef = TypedDict(
+    "_RequiredFunnelChartVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalLineChartVisualOutputTypeDef = TypedDict(
-    "_OptionalLineChartVisualOutputTypeDef",
+_OptionalFunnelChartVisualOutputTypeDef = TypedDict(
+    "_OptionalFunnelChartVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": LineChartConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": FunnelChartConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
         "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
 
-class LineChartVisualOutputTypeDef(
-    _RequiredLineChartVisualOutputTypeDef, _OptionalLineChartVisualOutputTypeDef
+class FunnelChartVisualOutputTypeDef(
+    _RequiredFunnelChartVisualOutputTypeDef, _OptionalFunnelChartVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredPieChartVisualOutputTypeDef = TypedDict(
-    "_RequiredPieChartVisualOutputTypeDef",
+_RequiredFunnelChartVisualTypeDef = TypedDict(
+    "_RequiredFunnelChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalPieChartVisualOutputTypeDef = TypedDict(
-    "_OptionalPieChartVisualOutputTypeDef",
+_OptionalFunnelChartVisualTypeDef = TypedDict(
+    "_OptionalFunnelChartVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": PieChartConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": FunnelChartConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
 
-class PieChartVisualOutputTypeDef(
-    _RequiredPieChartVisualOutputTypeDef, _OptionalPieChartVisualOutputTypeDef
+class FunnelChartVisualTypeDef(
+    _RequiredFunnelChartVisualTypeDef, _OptionalFunnelChartVisualTypeDef
 ):
     pass
 
 
-_RequiredPivotTableVisualOutputTypeDef = TypedDict(
-    "_RequiredPivotTableVisualOutputTypeDef",
+_RequiredGeospatialMapVisualOutputTypeDef = TypedDict(
+    "_RequiredGeospatialMapVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalPivotTableVisualOutputTypeDef = TypedDict(
-    "_OptionalPivotTableVisualOutputTypeDef",
+_OptionalGeospatialMapVisualOutputTypeDef = TypedDict(
+    "_OptionalGeospatialMapVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": PivotTableConfigurationOutputTypeDef,
-        "ConditionalFormatting": PivotTableConditionalFormattingOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": GeospatialMapConfigurationOutputTypeDef,
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
         "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
 
-class PivotTableVisualOutputTypeDef(
-    _RequiredPivotTableVisualOutputTypeDef, _OptionalPivotTableVisualOutputTypeDef
+class GeospatialMapVisualOutputTypeDef(
+    _RequiredGeospatialMapVisualOutputTypeDef, _OptionalGeospatialMapVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredRadarChartVisualOutputTypeDef = TypedDict(
-    "_RequiredRadarChartVisualOutputTypeDef",
+_RequiredGeospatialMapVisualTypeDef = TypedDict(
+    "_RequiredGeospatialMapVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalRadarChartVisualOutputTypeDef = TypedDict(
-    "_OptionalRadarChartVisualOutputTypeDef",
+_OptionalGeospatialMapVisualTypeDef = TypedDict(
+    "_OptionalGeospatialMapVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": RadarChartConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": GeospatialMapConfigurationTypeDef,
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "Actions": Sequence[VisualCustomActionTypeDef],
     },
     total=False,
 )
 
 
-class RadarChartVisualOutputTypeDef(
-    _RequiredRadarChartVisualOutputTypeDef, _OptionalRadarChartVisualOutputTypeDef
+class GeospatialMapVisualTypeDef(
+    _RequiredGeospatialMapVisualTypeDef, _OptionalGeospatialMapVisualTypeDef
 ):
     pass
 
 
-_RequiredSankeyDiagramVisualOutputTypeDef = TypedDict(
-    "_RequiredSankeyDiagramVisualOutputTypeDef",
+_RequiredHeatMapVisualOutputTypeDef = TypedDict(
+    "_RequiredHeatMapVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalSankeyDiagramVisualOutputTypeDef = TypedDict(
-    "_OptionalSankeyDiagramVisualOutputTypeDef",
+_OptionalHeatMapVisualOutputTypeDef = TypedDict(
+    "_OptionalHeatMapVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": SankeyDiagramChartConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": HeatMapConfigurationOutputTypeDef,
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
         "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
 
-class SankeyDiagramVisualOutputTypeDef(
-    _RequiredSankeyDiagramVisualOutputTypeDef, _OptionalSankeyDiagramVisualOutputTypeDef
+class HeatMapVisualOutputTypeDef(
+    _RequiredHeatMapVisualOutputTypeDef, _OptionalHeatMapVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredScatterPlotVisualOutputTypeDef = TypedDict(
-    "_RequiredScatterPlotVisualOutputTypeDef",
+_RequiredHeatMapVisualTypeDef = TypedDict(
+    "_RequiredHeatMapVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalScatterPlotVisualOutputTypeDef = TypedDict(
-    "_OptionalScatterPlotVisualOutputTypeDef",
+_OptionalHeatMapVisualTypeDef = TypedDict(
+    "_OptionalHeatMapVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": ScatterPlotConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": HeatMapConfigurationTypeDef,
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "Actions": Sequence[VisualCustomActionTypeDef],
     },
     total=False,
 )
 
 
-class ScatterPlotVisualOutputTypeDef(
-    _RequiredScatterPlotVisualOutputTypeDef, _OptionalScatterPlotVisualOutputTypeDef
-):
+class HeatMapVisualTypeDef(_RequiredHeatMapVisualTypeDef, _OptionalHeatMapVisualTypeDef):
     pass
 
 
-_RequiredInsightVisualOutputTypeDef = TypedDict(
-    "_RequiredInsightVisualOutputTypeDef",
+_RequiredHistogramVisualOutputTypeDef = TypedDict(
+    "_RequiredHistogramVisualOutputTypeDef",
     {
         "VisualId": str,
-        "DataSetIdentifier": str,
     },
 )
-_OptionalInsightVisualOutputTypeDef = TypedDict(
-    "_OptionalInsightVisualOutputTypeDef",
+_OptionalHistogramVisualOutputTypeDef = TypedDict(
+    "_OptionalHistogramVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "InsightConfiguration": InsightConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": HistogramConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
 
-class InsightVisualOutputTypeDef(
-    _RequiredInsightVisualOutputTypeDef, _OptionalInsightVisualOutputTypeDef
+class HistogramVisualOutputTypeDef(
+    _RequiredHistogramVisualOutputTypeDef, _OptionalHistogramVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredTreeMapVisualOutputTypeDef = TypedDict(
-    "_RequiredTreeMapVisualOutputTypeDef",
+_RequiredHistogramVisualTypeDef = TypedDict(
+    "_RequiredHistogramVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalTreeMapVisualOutputTypeDef = TypedDict(
-    "_OptionalTreeMapVisualOutputTypeDef",
+_OptionalHistogramVisualTypeDef = TypedDict(
+    "_OptionalHistogramVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": TreeMapConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": HistogramConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
     },
     total=False,
 )
 
 
-class TreeMapVisualOutputTypeDef(
-    _RequiredTreeMapVisualOutputTypeDef, _OptionalTreeMapVisualOutputTypeDef
-):
+class HistogramVisualTypeDef(_RequiredHistogramVisualTypeDef, _OptionalHistogramVisualTypeDef):
     pass
 
 
-_RequiredWaterfallVisualOutputTypeDef = TypedDict(
-    "_RequiredWaterfallVisualOutputTypeDef",
+_RequiredLineChartVisualOutputTypeDef = TypedDict(
+    "_RequiredLineChartVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalWaterfallVisualOutputTypeDef = TypedDict(
-    "_OptionalWaterfallVisualOutputTypeDef",
+_OptionalLineChartVisualOutputTypeDef = TypedDict(
+    "_OptionalLineChartVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": WaterfallChartConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": LineChartConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
         "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
 
-class WaterfallVisualOutputTypeDef(
-    _RequiredWaterfallVisualOutputTypeDef, _OptionalWaterfallVisualOutputTypeDef
+class LineChartVisualOutputTypeDef(
+    _RequiredLineChartVisualOutputTypeDef, _OptionalLineChartVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredWordCloudVisualOutputTypeDef = TypedDict(
-    "_RequiredWordCloudVisualOutputTypeDef",
+_RequiredLineChartVisualTypeDef = TypedDict(
+    "_RequiredLineChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalWordCloudVisualOutputTypeDef = TypedDict(
-    "_OptionalWordCloudVisualOutputTypeDef",
+_OptionalLineChartVisualTypeDef = TypedDict(
+    "_OptionalLineChartVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": WordCloudChartConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": LineChartConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
 
-class WordCloudVisualOutputTypeDef(
-    _RequiredWordCloudVisualOutputTypeDef, _OptionalWordCloudVisualOutputTypeDef
-):
+class LineChartVisualTypeDef(_RequiredLineChartVisualTypeDef, _OptionalLineChartVisualTypeDef):
     pass
 
 
-_RequiredTableVisualOutputTypeDef = TypedDict(
-    "_RequiredTableVisualOutputTypeDef",
+_RequiredPieChartVisualOutputTypeDef = TypedDict(
+    "_RequiredPieChartVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalTableVisualOutputTypeDef = TypedDict(
-    "_OptionalTableVisualOutputTypeDef",
+_OptionalPieChartVisualOutputTypeDef = TypedDict(
+    "_OptionalPieChartVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": TableConfigurationOutputTypeDef,
-        "ConditionalFormatting": TableConditionalFormattingOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": PieChartConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
 
-class TableVisualOutputTypeDef(
-    _RequiredTableVisualOutputTypeDef, _OptionalTableVisualOutputTypeDef
+class PieChartVisualOutputTypeDef(
+    _RequiredPieChartVisualOutputTypeDef, _OptionalPieChartVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredBarChartVisualTypeDef = TypedDict(
-    "_RequiredBarChartVisualTypeDef",
+_RequiredPieChartVisualTypeDef = TypedDict(
+    "_RequiredPieChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalBarChartVisualTypeDef = TypedDict(
-    "_OptionalBarChartVisualTypeDef",
+_OptionalPieChartVisualTypeDef = TypedDict(
+    "_OptionalPieChartVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": BarChartConfigurationTypeDef,
+        "ChartConfiguration": PieChartConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
         "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
 
-class BarChartVisualTypeDef(_RequiredBarChartVisualTypeDef, _OptionalBarChartVisualTypeDef):
+class PieChartVisualTypeDef(_RequiredPieChartVisualTypeDef, _OptionalPieChartVisualTypeDef):
     pass
 
 
-_RequiredBoxPlotVisualTypeDef = TypedDict(
-    "_RequiredBoxPlotVisualTypeDef",
+_RequiredPivotTableVisualOutputTypeDef = TypedDict(
+    "_RequiredPivotTableVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalBoxPlotVisualTypeDef = TypedDict(
-    "_OptionalBoxPlotVisualTypeDef",
+_OptionalPivotTableVisualOutputTypeDef = TypedDict(
+    "_OptionalPivotTableVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": BoxPlotChartConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "ChartConfiguration": PivotTableConfigurationOutputTypeDef,
+        "ConditionalFormatting": PivotTableConditionalFormattingOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
 
-class BoxPlotVisualTypeDef(_RequiredBoxPlotVisualTypeDef, _OptionalBoxPlotVisualTypeDef):
+class PivotTableVisualOutputTypeDef(
+    _RequiredPivotTableVisualOutputTypeDef, _OptionalPivotTableVisualOutputTypeDef
+):
     pass
 
 
-_RequiredComboChartVisualTypeDef = TypedDict(
-    "_RequiredComboChartVisualTypeDef",
+_RequiredPivotTableVisualTypeDef = TypedDict(
+    "_RequiredPivotTableVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalComboChartVisualTypeDef = TypedDict(
-    "_OptionalComboChartVisualTypeDef",
+_OptionalPivotTableVisualTypeDef = TypedDict(
+    "_OptionalPivotTableVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": ComboChartConfigurationTypeDef,
+        "ChartConfiguration": PivotTableConfigurationTypeDef,
+        "ConditionalFormatting": PivotTableConditionalFormattingTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
 
-class ComboChartVisualTypeDef(_RequiredComboChartVisualTypeDef, _OptionalComboChartVisualTypeDef):
+class PivotTableVisualTypeDef(_RequiredPivotTableVisualTypeDef, _OptionalPivotTableVisualTypeDef):
     pass
 
 
-_RequiredFilledMapVisualTypeDef = TypedDict(
-    "_RequiredFilledMapVisualTypeDef",
+_RequiredRadarChartVisualOutputTypeDef = TypedDict(
+    "_RequiredRadarChartVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalFilledMapVisualTypeDef = TypedDict(
-    "_OptionalFilledMapVisualTypeDef",
+_OptionalRadarChartVisualOutputTypeDef = TypedDict(
+    "_OptionalRadarChartVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": FilledMapConfigurationTypeDef,
-        "ConditionalFormatting": FilledMapConditionalFormattingTypeDef,
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
-        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ChartConfiguration": RadarChartConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
 
-class FilledMapVisualTypeDef(_RequiredFilledMapVisualTypeDef, _OptionalFilledMapVisualTypeDef):
+class RadarChartVisualOutputTypeDef(
+    _RequiredRadarChartVisualOutputTypeDef, _OptionalRadarChartVisualOutputTypeDef
+):
     pass
 
 
-_RequiredFunnelChartVisualTypeDef = TypedDict(
-    "_RequiredFunnelChartVisualTypeDef",
+_RequiredRadarChartVisualTypeDef = TypedDict(
+    "_RequiredRadarChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalFunnelChartVisualTypeDef = TypedDict(
-    "_OptionalFunnelChartVisualTypeDef",
+_OptionalRadarChartVisualTypeDef = TypedDict(
+    "_OptionalRadarChartVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": FunnelChartConfigurationTypeDef,
+        "ChartConfiguration": RadarChartConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
         "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
 
-class FunnelChartVisualTypeDef(
-    _RequiredFunnelChartVisualTypeDef, _OptionalFunnelChartVisualTypeDef
-):
+class RadarChartVisualTypeDef(_RequiredRadarChartVisualTypeDef, _OptionalRadarChartVisualTypeDef):
     pass
 
 
-_RequiredGeospatialMapVisualTypeDef = TypedDict(
-    "_RequiredGeospatialMapVisualTypeDef",
+_RequiredSankeyDiagramVisualOutputTypeDef = TypedDict(
+    "_RequiredSankeyDiagramVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalGeospatialMapVisualTypeDef = TypedDict(
-    "_OptionalGeospatialMapVisualTypeDef",
+_OptionalSankeyDiagramVisualOutputTypeDef = TypedDict(
+    "_OptionalSankeyDiagramVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": GeospatialMapConfigurationTypeDef,
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
-        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ChartConfiguration": SankeyDiagramChartConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
 
-class GeospatialMapVisualTypeDef(
-    _RequiredGeospatialMapVisualTypeDef, _OptionalGeospatialMapVisualTypeDef
+class SankeyDiagramVisualOutputTypeDef(
+    _RequiredSankeyDiagramVisualOutputTypeDef, _OptionalSankeyDiagramVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredHeatMapVisualTypeDef = TypedDict(
-    "_RequiredHeatMapVisualTypeDef",
+_RequiredSankeyDiagramVisualTypeDef = TypedDict(
+    "_RequiredSankeyDiagramVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalHeatMapVisualTypeDef = TypedDict(
-    "_OptionalHeatMapVisualTypeDef",
+_OptionalSankeyDiagramVisualTypeDef = TypedDict(
+    "_OptionalSankeyDiagramVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": HeatMapConfigurationTypeDef,
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "ChartConfiguration": SankeyDiagramChartConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
     },
     total=False,
 )
 
 
-class HeatMapVisualTypeDef(_RequiredHeatMapVisualTypeDef, _OptionalHeatMapVisualTypeDef):
+class SankeyDiagramVisualTypeDef(
+    _RequiredSankeyDiagramVisualTypeDef, _OptionalSankeyDiagramVisualTypeDef
+):
     pass
 
 
-_RequiredHistogramVisualTypeDef = TypedDict(
-    "_RequiredHistogramVisualTypeDef",
+_RequiredScatterPlotVisualOutputTypeDef = TypedDict(
+    "_RequiredScatterPlotVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalHistogramVisualTypeDef = TypedDict(
-    "_OptionalHistogramVisualTypeDef",
+_OptionalScatterPlotVisualOutputTypeDef = TypedDict(
+    "_OptionalScatterPlotVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": HistogramConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ChartConfiguration": ScatterPlotConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
 
-class HistogramVisualTypeDef(_RequiredHistogramVisualTypeDef, _OptionalHistogramVisualTypeDef):
+class ScatterPlotVisualOutputTypeDef(
+    _RequiredScatterPlotVisualOutputTypeDef, _OptionalScatterPlotVisualOutputTypeDef
+):
     pass
 
 
-_RequiredLineChartVisualTypeDef = TypedDict(
-    "_RequiredLineChartVisualTypeDef",
+_RequiredScatterPlotVisualTypeDef = TypedDict(
+    "_RequiredScatterPlotVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalLineChartVisualTypeDef = TypedDict(
-    "_OptionalLineChartVisualTypeDef",
+_OptionalScatterPlotVisualTypeDef = TypedDict(
+    "_OptionalScatterPlotVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": LineChartConfigurationTypeDef,
+        "ChartConfiguration": ScatterPlotConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
         "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
 
-class LineChartVisualTypeDef(_RequiredLineChartVisualTypeDef, _OptionalLineChartVisualTypeDef):
+class ScatterPlotVisualTypeDef(
+    _RequiredScatterPlotVisualTypeDef, _OptionalScatterPlotVisualTypeDef
+):
     pass
 
 
-_RequiredPieChartVisualTypeDef = TypedDict(
-    "_RequiredPieChartVisualTypeDef",
+_RequiredInsightVisualOutputTypeDef = TypedDict(
+    "_RequiredInsightVisualOutputTypeDef",
     {
         "VisualId": str,
+        "DataSetIdentifier": str,
     },
 )
-_OptionalPieChartVisualTypeDef = TypedDict(
-    "_OptionalPieChartVisualTypeDef",
+_OptionalInsightVisualOutputTypeDef = TypedDict(
+    "_OptionalInsightVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": PieChartConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "InsightConfiguration": InsightConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
 
-class PieChartVisualTypeDef(_RequiredPieChartVisualTypeDef, _OptionalPieChartVisualTypeDef):
+class InsightVisualOutputTypeDef(
+    _RequiredInsightVisualOutputTypeDef, _OptionalInsightVisualOutputTypeDef
+):
     pass
 
 
-_RequiredPivotTableVisualTypeDef = TypedDict(
-    "_RequiredPivotTableVisualTypeDef",
+_RequiredInsightVisualTypeDef = TypedDict(
+    "_RequiredInsightVisualTypeDef",
     {
         "VisualId": str,
+        "DataSetIdentifier": str,
     },
 )
-_OptionalPivotTableVisualTypeDef = TypedDict(
-    "_OptionalPivotTableVisualTypeDef",
+_OptionalInsightVisualTypeDef = TypedDict(
+    "_OptionalInsightVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": PivotTableConfigurationTypeDef,
-        "ConditionalFormatting": PivotTableConditionalFormattingTypeDef,
+        "InsightConfiguration": InsightConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
     },
     total=False,
 )
 
 
-class PivotTableVisualTypeDef(_RequiredPivotTableVisualTypeDef, _OptionalPivotTableVisualTypeDef):
+class InsightVisualTypeDef(_RequiredInsightVisualTypeDef, _OptionalInsightVisualTypeDef):
     pass
 
 
-_RequiredRadarChartVisualTypeDef = TypedDict(
-    "_RequiredRadarChartVisualTypeDef",
+_RequiredTreeMapVisualOutputTypeDef = TypedDict(
+    "_RequiredTreeMapVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalRadarChartVisualTypeDef = TypedDict(
-    "_OptionalRadarChartVisualTypeDef",
+_OptionalTreeMapVisualOutputTypeDef = TypedDict(
+    "_OptionalTreeMapVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": RadarChartConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "ChartConfiguration": TreeMapConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
 
-class RadarChartVisualTypeDef(_RequiredRadarChartVisualTypeDef, _OptionalRadarChartVisualTypeDef):
+class TreeMapVisualOutputTypeDef(
+    _RequiredTreeMapVisualOutputTypeDef, _OptionalTreeMapVisualOutputTypeDef
+):
     pass
 
 
-_RequiredSankeyDiagramVisualTypeDef = TypedDict(
-    "_RequiredSankeyDiagramVisualTypeDef",
+_RequiredTreeMapVisualTypeDef = TypedDict(
+    "_RequiredTreeMapVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalSankeyDiagramVisualTypeDef = TypedDict(
-    "_OptionalSankeyDiagramVisualTypeDef",
+_OptionalTreeMapVisualTypeDef = TypedDict(
+    "_OptionalTreeMapVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": SankeyDiagramChartConfigurationTypeDef,
+        "ChartConfiguration": TreeMapConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
 
-class SankeyDiagramVisualTypeDef(
-    _RequiredSankeyDiagramVisualTypeDef, _OptionalSankeyDiagramVisualTypeDef
-):
+class TreeMapVisualTypeDef(_RequiredTreeMapVisualTypeDef, _OptionalTreeMapVisualTypeDef):
     pass
 
 
-_RequiredScatterPlotVisualTypeDef = TypedDict(
-    "_RequiredScatterPlotVisualTypeDef",
+_RequiredWaterfallVisualOutputTypeDef = TypedDict(
+    "_RequiredWaterfallVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalScatterPlotVisualTypeDef = TypedDict(
-    "_OptionalScatterPlotVisualTypeDef",
+_OptionalWaterfallVisualOutputTypeDef = TypedDict(
+    "_OptionalWaterfallVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": ScatterPlotConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "ChartConfiguration": WaterfallChartConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
 
-class ScatterPlotVisualTypeDef(
-    _RequiredScatterPlotVisualTypeDef, _OptionalScatterPlotVisualTypeDef
+class WaterfallVisualOutputTypeDef(
+    _RequiredWaterfallVisualOutputTypeDef, _OptionalWaterfallVisualOutputTypeDef
 ):
     pass
 
 
-_RequiredInsightVisualTypeDef = TypedDict(
-    "_RequiredInsightVisualTypeDef",
+_RequiredWaterfallVisualTypeDef = TypedDict(
+    "_RequiredWaterfallVisualTypeDef",
     {
         "VisualId": str,
-        "DataSetIdentifier": str,
     },
 )
-_OptionalInsightVisualTypeDef = TypedDict(
-    "_OptionalInsightVisualTypeDef",
+_OptionalWaterfallVisualTypeDef = TypedDict(
+    "_OptionalWaterfallVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "InsightConfiguration": InsightConfigurationTypeDef,
+        "ChartConfiguration": WaterfallChartConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
 
-class InsightVisualTypeDef(_RequiredInsightVisualTypeDef, _OptionalInsightVisualTypeDef):
+class WaterfallVisualTypeDef(_RequiredWaterfallVisualTypeDef, _OptionalWaterfallVisualTypeDef):
     pass
 
 
-_RequiredTreeMapVisualTypeDef = TypedDict(
-    "_RequiredTreeMapVisualTypeDef",
+_RequiredWordCloudVisualOutputTypeDef = TypedDict(
+    "_RequiredWordCloudVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalTreeMapVisualTypeDef = TypedDict(
-    "_OptionalTreeMapVisualTypeDef",
+_OptionalWordCloudVisualOutputTypeDef = TypedDict(
+    "_OptionalWordCloudVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": TreeMapConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "ChartConfiguration": WordCloudChartConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
 
-class TreeMapVisualTypeDef(_RequiredTreeMapVisualTypeDef, _OptionalTreeMapVisualTypeDef):
+class WordCloudVisualOutputTypeDef(
+    _RequiredWordCloudVisualOutputTypeDef, _OptionalWordCloudVisualOutputTypeDef
+):
     pass
 
 
-_RequiredWaterfallVisualTypeDef = TypedDict(
-    "_RequiredWaterfallVisualTypeDef",
+_RequiredWordCloudVisualTypeDef = TypedDict(
+    "_RequiredWordCloudVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalWaterfallVisualTypeDef = TypedDict(
-    "_OptionalWaterfallVisualTypeDef",
+_OptionalWordCloudVisualTypeDef = TypedDict(
+    "_OptionalWordCloudVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": WaterfallChartConfigurationTypeDef,
+        "ChartConfiguration": WordCloudChartConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
         "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
 
-class WaterfallVisualTypeDef(_RequiredWaterfallVisualTypeDef, _OptionalWaterfallVisualTypeDef):
+class WordCloudVisualTypeDef(_RequiredWordCloudVisualTypeDef, _OptionalWordCloudVisualTypeDef):
     pass
 
 
-_RequiredWordCloudVisualTypeDef = TypedDict(
-    "_RequiredWordCloudVisualTypeDef",
+_RequiredTableVisualOutputTypeDef = TypedDict(
+    "_RequiredTableVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalWordCloudVisualTypeDef = TypedDict(
-    "_OptionalWordCloudVisualTypeDef",
+_OptionalTableVisualOutputTypeDef = TypedDict(
+    "_OptionalTableVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": WordCloudChartConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "ChartConfiguration": TableConfigurationOutputTypeDef,
+        "ConditionalFormatting": TableConditionalFormattingOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
 
-class WordCloudVisualTypeDef(_RequiredWordCloudVisualTypeDef, _OptionalWordCloudVisualTypeDef):
+class TableVisualOutputTypeDef(
+    _RequiredTableVisualOutputTypeDef, _OptionalTableVisualOutputTypeDef
+):
     pass
 
 
 _RequiredTableVisualTypeDef = TypedDict(
     "_RequiredTableVisualTypeDef",
     {
         "VisualId": str,
@@ -23865,15 +19692,15 @@
     {
         "Title": str,
         "Description": str,
         "Name": str,
         "ParameterControls": List[ParameterControlOutputTypeDef],
         "FilterControls": List[FilterControlOutputTypeDef],
         "Visuals": List[VisualOutputTypeDef],
-        "TextBoxes": List[SheetTextBoxOutputTypeDef],
+        "TextBoxes": List[SheetTextBoxTypeDef],
         "Layouts": List[LayoutOutputTypeDef],
         "SheetControlLayouts": List[SheetControlLayoutOutputTypeDef],
         "ContentType": SheetContentTypeType,
     },
     total=False,
 )
 
@@ -23911,52 +19738,52 @@
 class SheetDefinitionTypeDef(_RequiredSheetDefinitionTypeDef, _OptionalSheetDefinitionTypeDef):
     pass
 
 
 _RequiredAnalysisDefinitionOutputTypeDef = TypedDict(
     "_RequiredAnalysisDefinitionOutputTypeDef",
     {
-        "DataSetIdentifierDeclarations": List[DataSetIdentifierDeclarationOutputTypeDef],
+        "DataSetIdentifierDeclarations": List[DataSetIdentifierDeclarationTypeDef],
     },
 )
 _OptionalAnalysisDefinitionOutputTypeDef = TypedDict(
     "_OptionalAnalysisDefinitionOutputTypeDef",
     {
         "Sheets": List[SheetDefinitionOutputTypeDef],
-        "CalculatedFields": List[CalculatedFieldOutputTypeDef],
+        "CalculatedFields": List[CalculatedFieldTypeDef],
         "ParameterDeclarations": List[ParameterDeclarationOutputTypeDef],
         "FilterGroups": List[FilterGroupOutputTypeDef],
         "ColumnConfigurations": List[ColumnConfigurationOutputTypeDef],
-        "AnalysisDefaults": AnalysisDefaultsOutputTypeDef,
+        "AnalysisDefaults": AnalysisDefaultsTypeDef,
     },
     total=False,
 )
 
 
 class AnalysisDefinitionOutputTypeDef(
     _RequiredAnalysisDefinitionOutputTypeDef, _OptionalAnalysisDefinitionOutputTypeDef
 ):
     pass
 
 
 _RequiredDashboardVersionDefinitionOutputTypeDef = TypedDict(
     "_RequiredDashboardVersionDefinitionOutputTypeDef",
     {
-        "DataSetIdentifierDeclarations": List[DataSetIdentifierDeclarationOutputTypeDef],
+        "DataSetIdentifierDeclarations": List[DataSetIdentifierDeclarationTypeDef],
     },
 )
 _OptionalDashboardVersionDefinitionOutputTypeDef = TypedDict(
     "_OptionalDashboardVersionDefinitionOutputTypeDef",
     {
         "Sheets": List[SheetDefinitionOutputTypeDef],
-        "CalculatedFields": List[CalculatedFieldOutputTypeDef],
+        "CalculatedFields": List[CalculatedFieldTypeDef],
         "ParameterDeclarations": List[ParameterDeclarationOutputTypeDef],
         "FilterGroups": List[FilterGroupOutputTypeDef],
         "ColumnConfigurations": List[ColumnConfigurationOutputTypeDef],
-        "AnalysisDefaults": AnalysisDefaultsOutputTypeDef,
+        "AnalysisDefaults": AnalysisDefaultsTypeDef,
     },
     total=False,
 )
 
 
 class DashboardVersionDefinitionOutputTypeDef(
     _RequiredDashboardVersionDefinitionOutputTypeDef,
@@ -23971,19 +19798,19 @@
         "DataSetConfigurations": List[DataSetConfigurationOutputTypeDef],
     },
 )
 _OptionalTemplateVersionDefinitionOutputTypeDef = TypedDict(
     "_OptionalTemplateVersionDefinitionOutputTypeDef",
     {
         "Sheets": List[SheetDefinitionOutputTypeDef],
-        "CalculatedFields": List[CalculatedFieldOutputTypeDef],
+        "CalculatedFields": List[CalculatedFieldTypeDef],
         "ParameterDeclarations": List[ParameterDeclarationOutputTypeDef],
         "FilterGroups": List[FilterGroupOutputTypeDef],
         "ColumnConfigurations": List[ColumnConfigurationOutputTypeDef],
-        "AnalysisDefaults": AnalysisDefaultsOutputTypeDef,
+        "AnalysisDefaults": AnalysisDefaultsTypeDef,
     },
     total=False,
 )
 
 
 class TemplateVersionDefinitionOutputTypeDef(
     _RequiredTemplateVersionDefinitionOutputTypeDef, _OptionalTemplateVersionDefinitionOutputTypeDef
@@ -24091,15 +19918,15 @@
         "Errors": List[DashboardErrorTypeDef],
         "Name": str,
         "ResourceStatus": ResourceStatusType,
         "ThemeArn": str,
         "Definition": DashboardVersionDefinitionOutputTypeDef,
         "Status": int,
         "RequestId": str,
-        "DashboardPublishOptions": DashboardPublishOptionsOutputTypeDef,
+        "DashboardPublishOptions": DashboardPublishOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTemplateDefinitionResponseTypeDef = TypedDict(
     "DescribeTemplateDefinitionResponseTypeDef",
     {
```

### Comparing `mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight/type_defs.pyi` & `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight/type_defs.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for quicksight service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_quicksight.type_defs import AccountCustomizationOutputTypeDef
+    from mypy_boto3_quicksight.type_defs import AccountCustomizationTypeDef
 
-    data: AccountCustomizationOutputTypeDef = {...}
+    data: AccountCustomizationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -197,163 +197,114 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AccountCustomizationOutputTypeDef",
     "AccountCustomizationTypeDef",
     "AccountInfoTypeDef",
     "AccountSettingsTypeDef",
     "ActiveIAMPolicyAssignmentTypeDef",
-    "AdHocFilteringOptionOutputTypeDef",
     "AdHocFilteringOptionTypeDef",
-    "AttributeAggregationFunctionOutputTypeDef",
     "AttributeAggregationFunctionTypeDef",
-    "ColumnIdentifierOutputTypeDef",
     "ColumnIdentifierTypeDef",
-    "AmazonElasticsearchParametersOutputTypeDef",
     "AmazonElasticsearchParametersTypeDef",
-    "AmazonOpenSearchParametersOutputTypeDef",
     "AmazonOpenSearchParametersTypeDef",
-    "CalculatedFieldOutputTypeDef",
-    "DataSetIdentifierDeclarationOutputTypeDef",
     "CalculatedFieldTypeDef",
     "DataSetIdentifierDeclarationTypeDef",
     "EntityTypeDef",
     "AnalysisSearchFilterTypeDef",
     "DataSetReferenceTypeDef",
     "AnalysisSummaryTypeDef",
     "SheetTypeDef",
-    "AnchorDateConfigurationOutputTypeDef",
     "AnchorDateConfigurationTypeDef",
     "AnonymousUserDashboardEmbeddingConfigurationTypeDef",
     "DashboardVisualIdTypeDef",
     "AnonymousUserQSearchBarEmbeddingConfigurationTypeDef",
-    "ArcAxisDisplayRangeOutputTypeDef",
     "ArcAxisDisplayRangeTypeDef",
-    "ArcConfigurationOutputTypeDef",
     "ArcConfigurationTypeDef",
-    "ArcOptionsOutputTypeDef",
     "ArcOptionsTypeDef",
     "AssetBundleExportJobAnalysisOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobDashboardOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobDataSetOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobDataSourceOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef",
-    "AssetBundleExportJobResourceIdOverrideConfigurationOutputTypeDef",
+    "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleExportJobThemeOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobVPCConnectionOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobAnalysisOverridePropertiesTypeDef",
     "AssetBundleExportJobDashboardOverridePropertiesTypeDef",
     "AssetBundleExportJobDataSetOverridePropertiesTypeDef",
     "AssetBundleExportJobDataSourceOverridePropertiesTypeDef",
     "AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef",
-    "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleExportJobThemeOverridePropertiesTypeDef",
     "AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef",
     "AssetBundleExportJobErrorTypeDef",
     "AssetBundleExportJobSummaryTypeDef",
-    "AssetBundleImportJobAnalysisOverrideParametersOutputTypeDef",
     "AssetBundleImportJobAnalysisOverrideParametersTypeDef",
-    "AssetBundleImportJobDashboardOverrideParametersOutputTypeDef",
     "AssetBundleImportJobDashboardOverrideParametersTypeDef",
-    "AssetBundleImportJobDataSetOverrideParametersOutputTypeDef",
     "AssetBundleImportJobDataSetOverrideParametersTypeDef",
-    "AssetBundleImportJobDataSourceCredentialPairOutputTypeDef",
     "AssetBundleImportJobDataSourceCredentialPairTypeDef",
-    "SslPropertiesOutputTypeDef",
-    "VpcConnectionPropertiesOutputTypeDef",
     "SslPropertiesTypeDef",
     "VpcConnectionPropertiesTypeDef",
     "AssetBundleImportJobErrorTypeDef",
     "AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef",
-    "AssetBundleImportJobResourceIdOverrideConfigurationOutputTypeDef",
-    "AssetBundleImportJobThemeOverrideParametersOutputTypeDef",
-    "AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef",
-    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
     "AssetBundleImportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleImportJobThemeOverrideParametersTypeDef",
+    "AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef",
+    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
     "AssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
     "AssetBundleImportJobSummaryTypeDef",
     "AssetBundleImportSourceDescriptionTypeDef",
     "AssetBundleImportSourceTypeDef",
-    "AthenaParametersOutputTypeDef",
     "AthenaParametersTypeDef",
-    "AuroraParametersOutputTypeDef",
     "AuroraParametersTypeDef",
-    "AuroraPostgreSqlParametersOutputTypeDef",
     "AuroraPostgreSqlParametersTypeDef",
-    "AwsIotAnalyticsParametersOutputTypeDef",
     "AwsIotAnalyticsParametersTypeDef",
-    "DateAxisOptionsOutputTypeDef",
     "DateAxisOptionsTypeDef",
-    "AxisDisplayMinMaxRangeOutputTypeDef",
     "AxisDisplayMinMaxRangeTypeDef",
-    "AxisLinearScaleOutputTypeDef",
     "AxisLinearScaleTypeDef",
-    "AxisLogarithmicScaleOutputTypeDef",
     "AxisLogarithmicScaleTypeDef",
-    "ItemsLimitConfigurationOutputTypeDef",
     "ItemsLimitConfigurationTypeDef",
-    "BinCountOptionsOutputTypeDef",
     "BinCountOptionsTypeDef",
-    "BinWidthOptionsOutputTypeDef",
     "BinWidthOptionsTypeDef",
     "BookmarksConfigurationsTypeDef",
-    "BorderStyleOutputTypeDef",
     "BorderStyleTypeDef",
-    "BoxPlotStyleOptionsOutputTypeDef",
     "BoxPlotStyleOptionsTypeDef",
-    "PaginationConfigurationOutputTypeDef",
     "PaginationConfigurationTypeDef",
-    "CalculatedColumnOutputTypeDef",
     "CalculatedColumnTypeDef",
-    "CalculatedMeasureFieldOutputTypeDef",
     "CalculatedMeasureFieldTypeDef",
     "CancelIngestionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "CastColumnTypeOperationOutputTypeDef",
     "CastColumnTypeOperationTypeDef",
-    "CustomFilterConfigurationOutputTypeDef",
+    "CustomFilterConfigurationTypeDef",
     "CustomFilterListConfigurationOutputTypeDef",
     "FilterListConfigurationOutputTypeDef",
-    "CustomFilterConfigurationTypeDef",
     "CustomFilterListConfigurationTypeDef",
     "FilterListConfigurationTypeDef",
     "CellValueSynonymOutputTypeDef",
     "CellValueSynonymTypeDef",
-    "SimpleClusterMarkerOutputTypeDef",
     "SimpleClusterMarkerTypeDef",
     "CollectiveConstantOutputTypeDef",
     "CollectiveConstantTypeDef",
-    "DataColorOutputTypeDef",
     "DataColorTypeDef",
-    "CustomColorOutputTypeDef",
     "CustomColorTypeDef",
-    "ColumnDescriptionOutputTypeDef",
     "ColumnDescriptionTypeDef",
-    "ColumnGroupColumnSchemaOutputTypeDef",
     "ColumnGroupColumnSchemaTypeDef",
     "GeoSpatialColumnGroupOutputTypeDef",
     "GeoSpatialColumnGroupTypeDef",
     "ColumnLevelPermissionRuleOutputTypeDef",
     "ColumnLevelPermissionRuleTypeDef",
-    "ColumnSchemaOutputTypeDef",
     "ColumnSchemaTypeDef",
     "ComparativeOrderOutputTypeDef",
     "ComparativeOrderTypeDef",
-    "ConditionalFormattingSolidColorOutputTypeDef",
     "ConditionalFormattingSolidColorTypeDef",
-    "ConditionalFormattingCustomIconOptionsOutputTypeDef",
-    "ConditionalFormattingIconDisplayConfigurationOutputTypeDef",
     "ConditionalFormattingCustomIconOptionsTypeDef",
     "ConditionalFormattingIconDisplayConfigurationTypeDef",
-    "ConditionalFormattingIconSetOutputTypeDef",
     "ConditionalFormattingIconSetTypeDef",
     "TagTypeDef",
     "CreateAccountSubscriptionRequestRequestTypeDef",
     "SignupResponseTypeDef",
     "ResourcePermissionTypeDef",
     "DataSetUsageConfigurationTypeDef",
     "FieldFolderTypeDef",
@@ -367,95 +318,51 @@
     "CreateIAMPolicyAssignmentRequestRequestTypeDef",
     "CreateIngestionRequestRequestTypeDef",
     "CreateTemplateAliasRequestRequestTypeDef",
     "TemplateAliasTypeDef",
     "CreateThemeAliasRequestRequestTypeDef",
     "ThemeAliasTypeDef",
     "TopicRefreshScheduleTypeDef",
-    "DecimalPlacesConfigurationOutputTypeDef",
-    "NegativeValueConfigurationOutputTypeDef",
-    "NullValueFormatConfigurationOutputTypeDef",
     "DecimalPlacesConfigurationTypeDef",
     "NegativeValueConfigurationTypeDef",
     "NullValueFormatConfigurationTypeDef",
-    "LocalNavigationConfigurationOutputTypeDef",
     "LocalNavigationConfigurationTypeDef",
-    "CustomActionURLOperationOutputTypeDef",
     "CustomActionURLOperationTypeDef",
-    "CustomContentConfigurationOutputTypeDef",
     "CustomContentConfigurationTypeDef",
-    "CustomNarrativeOptionsOutputTypeDef",
     "CustomNarrativeOptionsTypeDef",
     "CustomParameterValuesOutputTypeDef",
     "CustomParameterValuesTypeDef",
-    "InputColumnOutputTypeDef",
     "InputColumnTypeDef",
-    "DataPointDrillUpDownOptionOutputTypeDef",
-    "DataPointMenuLabelOptionOutputTypeDef",
-    "DataPointTooltipOptionOutputTypeDef",
-    "ExportToCSVOptionOutputTypeDef",
-    "ExportWithHiddenFieldsOptionOutputTypeDef",
-    "SheetControlsOptionOutputTypeDef",
-    "SheetLayoutElementMaximizationOptionOutputTypeDef",
-    "VisualAxisSortOptionOutputTypeDef",
-    "VisualMenuOptionOutputTypeDef",
     "DataPointDrillUpDownOptionTypeDef",
     "DataPointMenuLabelOptionTypeDef",
     "DataPointTooltipOptionTypeDef",
     "ExportToCSVOptionTypeDef",
     "ExportWithHiddenFieldsOptionTypeDef",
     "SheetControlsOptionTypeDef",
     "SheetLayoutElementMaximizationOptionTypeDef",
     "VisualAxisSortOptionTypeDef",
     "VisualMenuOptionTypeDef",
     "DashboardSearchFilterTypeDef",
     "DashboardSummaryTypeDef",
     "DashboardVersionSummaryTypeDef",
-    "ExportHiddenFieldsOptionOutputTypeDef",
     "ExportHiddenFieldsOptionTypeDef",
-    "DataAggregationOutputTypeDef",
     "DataAggregationTypeDef",
-    "DataBarsOptionsOutputTypeDef",
     "DataBarsOptionsTypeDef",
     "DataColorPaletteOutputTypeDef",
     "DataColorPaletteTypeDef",
-    "DataPathLabelTypeOutputTypeDef",
-    "FieldLabelTypeOutputTypeDef",
-    "MaximumLabelTypeOutputTypeDef",
-    "MinimumLabelTypeOutputTypeDef",
-    "RangeEndsLabelTypeOutputTypeDef",
     "DataPathLabelTypeTypeDef",
     "FieldLabelTypeTypeDef",
     "MaximumLabelTypeTypeDef",
     "MinimumLabelTypeTypeDef",
     "RangeEndsLabelTypeTypeDef",
-    "DataPathValueOutputTypeDef",
     "DataPathValueTypeDef",
     "DataSetSearchFilterTypeDef",
-    "RowLevelPermissionDataSetOutputTypeDef",
-    "DataSetUsageConfigurationOutputTypeDef",
     "FieldFolderOutputTypeDef",
     "OutputColumnTypeDef",
     "DataSourceErrorInfoTypeDef",
-    "DatabricksParametersOutputTypeDef",
-    "ExasolParametersOutputTypeDef",
-    "JiraParametersOutputTypeDef",
-    "MariaDbParametersOutputTypeDef",
-    "MySqlParametersOutputTypeDef",
-    "OracleParametersOutputTypeDef",
-    "PostgreSqlParametersOutputTypeDef",
-    "PrestoParametersOutputTypeDef",
-    "RdsParametersOutputTypeDef",
-    "RedshiftParametersOutputTypeDef",
-    "ServiceNowParametersOutputTypeDef",
-    "SnowflakeParametersOutputTypeDef",
-    "SparkParametersOutputTypeDef",
-    "SqlServerParametersOutputTypeDef",
-    "TeradataParametersOutputTypeDef",
-    "TwitterParametersOutputTypeDef",
     "DatabricksParametersTypeDef",
     "ExasolParametersTypeDef",
     "JiraParametersTypeDef",
     "MariaDbParametersTypeDef",
     "MySqlParametersTypeDef",
     "OracleParametersTypeDef",
     "PostgreSqlParametersTypeDef",
@@ -468,27 +375,23 @@
     "SqlServerParametersTypeDef",
     "TeradataParametersTypeDef",
     "TwitterParametersTypeDef",
     "DataSourceSearchFilterTypeDef",
     "DataSourceSummaryTypeDef",
     "DateTimeDatasetParameterDefaultValuesOutputTypeDef",
     "DateTimeDatasetParameterDefaultValuesTypeDef",
-    "RollingDateConfigurationOutputTypeDef",
     "RollingDateConfigurationTypeDef",
     "DateTimeValueWhenUnsetConfigurationOutputTypeDef",
-    "MappedDataSetParameterOutputTypeDef",
-    "DateTimeValueWhenUnsetConfigurationTypeDef",
     "MappedDataSetParameterTypeDef",
+    "DateTimeValueWhenUnsetConfigurationTypeDef",
     "DateTimeParameterOutputTypeDef",
     "DateTimeParameterTypeDef",
-    "SheetControlInfoIconLabelOptionsOutputTypeDef",
     "SheetControlInfoIconLabelOptionsTypeDef",
     "DecimalDatasetParameterDefaultValuesOutputTypeDef",
     "DecimalDatasetParameterDefaultValuesTypeDef",
-    "DecimalValueWhenUnsetConfigurationOutputTypeDef",
     "DecimalValueWhenUnsetConfigurationTypeDef",
     "DecimalParameterOutputTypeDef",
     "DecimalParameterTypeDef",
     "DeleteAccountCustomizationRequestRequestTypeDef",
     "DeleteAccountSubscriptionRequestRequestTypeDef",
     "DeleteAnalysisRequestRequestTypeDef",
     "DeleteDashboardRequestRequestTypeDef",
@@ -555,105 +458,72 @@
     "TopicRefreshDetailsTypeDef",
     "DescribeTopicRefreshScheduleRequestRequestTypeDef",
     "TopicRefreshScheduleOutputTypeDef",
     "DescribeTopicRequestRequestTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "UserTypeDef",
     "DescribeVPCConnectionRequestRequestTypeDef",
-    "NegativeFormatOutputTypeDef",
     "NegativeFormatTypeDef",
-    "DonutCenterOptionsOutputTypeDef",
     "DonutCenterOptionsTypeDef",
-    "ListControlSelectAllOptionsOutputTypeDef",
     "ListControlSelectAllOptionsTypeDef",
     "ErrorInfoTypeDef",
-    "ExcludePeriodConfigurationOutputTypeDef",
     "ExcludePeriodConfigurationTypeDef",
-    "FieldSortOutputTypeDef",
     "FieldSortTypeDef",
-    "FieldTooltipItemOutputTypeDef",
     "FieldTooltipItemTypeDef",
-    "GeospatialMapStyleOptionsOutputTypeDef",
     "GeospatialMapStyleOptionsTypeDef",
     "FilterSelectableValuesOutputTypeDef",
     "FilterSelectableValuesTypeDef",
-    "FilterOperationOutputTypeDef",
     "SameSheetTargetVisualConfigurationOutputTypeDef",
     "SameSheetTargetVisualConfigurationTypeDef",
     "FilterOperationTypeDef",
     "FolderSearchFilterTypeDef",
     "FolderSummaryTypeDef",
-    "FontSizeOutputTypeDef",
-    "FontWeightOutputTypeDef",
     "FontSizeTypeDef",
     "FontWeightTypeDef",
-    "FontOutputTypeDef",
     "FontTypeDef",
-    "TimeBasedForecastPropertiesOutputTypeDef",
     "TimeBasedForecastPropertiesTypeDef",
     "WhatIfPointScenarioOutputTypeDef",
     "WhatIfRangeScenarioOutputTypeDef",
     "WhatIfPointScenarioTypeDef",
     "WhatIfRangeScenarioTypeDef",
-    "FreeFormLayoutScreenCanvasSizeOptionsOutputTypeDef",
     "FreeFormLayoutScreenCanvasSizeOptionsTypeDef",
-    "FreeFormLayoutElementBackgroundStyleOutputTypeDef",
     "FreeFormLayoutElementBackgroundStyleTypeDef",
-    "FreeFormLayoutElementBorderStyleOutputTypeDef",
     "FreeFormLayoutElementBorderStyleTypeDef",
-    "LoadingAnimationOutputTypeDef",
     "LoadingAnimationTypeDef",
     "SessionTagTypeDef",
-    "GeospatialCoordinateBoundsOutputTypeDef",
     "GeospatialCoordinateBoundsTypeDef",
-    "GeospatialHeatmapDataColorOutputTypeDef",
     "GeospatialHeatmapDataColorTypeDef",
     "GetDashboardEmbedUrlRequestRequestTypeDef",
     "GetSessionEmbedUrlRequestRequestTypeDef",
-    "TableBorderOptionsOutputTypeDef",
     "TableBorderOptionsTypeDef",
-    "GradientStopOutputTypeDef",
     "GradientStopTypeDef",
-    "GridLayoutScreenCanvasSizeOptionsOutputTypeDef",
     "GridLayoutScreenCanvasSizeOptionsTypeDef",
-    "GridLayoutElementOutputTypeDef",
     "GridLayoutElementTypeDef",
     "GroupSearchFilterTypeDef",
-    "GutterStyleOutputTypeDef",
     "GutterStyleTypeDef",
     "IAMPolicyAssignmentSummaryTypeDef",
-    "LookbackWindowOutputTypeDef",
     "LookbackWindowTypeDef",
     "QueueInfoTypeDef",
     "RowInfoTypeDef",
     "IntegerDatasetParameterDefaultValuesOutputTypeDef",
     "IntegerDatasetParameterDefaultValuesTypeDef",
-    "IntegerValueWhenUnsetConfigurationOutputTypeDef",
     "IntegerValueWhenUnsetConfigurationTypeDef",
     "IntegerParameterOutputTypeDef",
     "IntegerParameterTypeDef",
-    "JoinKeyPropertiesOutputTypeDef",
     "JoinKeyPropertiesTypeDef",
-    "ProgressBarOptionsOutputTypeDef",
-    "SecondaryValueOptionsOutputTypeDef",
-    "TrendArrowOptionsOutputTypeDef",
     "ProgressBarOptionsTypeDef",
     "SecondaryValueOptionsTypeDef",
     "TrendArrowOptionsTypeDef",
-    "LineChartLineStyleSettingsOutputTypeDef",
-    "LineChartMarkerStyleSettingsOutputTypeDef",
     "LineChartLineStyleSettingsTypeDef",
     "LineChartMarkerStyleSettingsTypeDef",
-    "MissingDataConfigurationOutputTypeDef",
     "MissingDataConfigurationTypeDef",
     "PaginatorConfigTypeDef",
     "ListAnalysesRequestRequestTypeDef",
     "ListAssetBundleExportJobsRequestRequestTypeDef",
     "ListAssetBundleImportJobsRequestRequestTypeDef",
-    "ListControlSearchOptionsOutputTypeDef",
     "ListControlSearchOptionsTypeDef",
     "ListDashboardVersionsRequestRequestTypeDef",
     "ListDashboardsRequestRequestTypeDef",
     "ListDataSetsRequestRequestTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListFolderMembersRequestRequestTypeDef",
     "MemberIdArnPairTypeDef",
@@ -662,15 +532,14 @@
     "ListGroupsRequestRequestTypeDef",
     "ListIAMPolicyAssignmentsForUserRequestRequestTypeDef",
     "ListIAMPolicyAssignmentsRequestRequestTypeDef",
     "ListIngestionsRequestRequestTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListRefreshSchedulesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListTemplateAliasesRequestRequestTypeDef",
     "ListTemplateVersionsRequestRequestTypeDef",
     "TemplateVersionSummaryTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "ListThemeAliasesRequestRequestTypeDef",
     "ListThemeVersionsRequestRequestTypeDef",
@@ -679,111 +548,77 @@
     "ThemeSummaryTypeDef",
     "ListTopicRefreshSchedulesRequestRequestTypeDef",
     "ListTopicsRequestRequestTypeDef",
     "TopicSummaryTypeDef",
     "ListUserGroupsRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVPCConnectionsRequestRequestTypeDef",
-    "LongFormatTextOutputTypeDef",
     "LongFormatTextTypeDef",
-    "ManifestFileLocationOutputTypeDef",
     "ManifestFileLocationTypeDef",
-    "MarginStyleOutputTypeDef",
     "MarginStyleTypeDef",
     "NamedEntityDefinitionMetricOutputTypeDef",
     "NamedEntityDefinitionMetricTypeDef",
     "NamespaceErrorTypeDef",
     "NetworkInterfaceTypeDef",
     "NewDefaultValuesOutputTypeDef",
     "NewDefaultValuesTypeDef",
-    "NumericRangeFilterValueOutputTypeDef",
     "NumericRangeFilterValueTypeDef",
-    "ThousandSeparatorOptionsOutputTypeDef",
     "ThousandSeparatorOptionsTypeDef",
-    "PercentileAggregationOutputTypeDef",
     "PercentileAggregationTypeDef",
     "StringParameterOutputTypeDef",
     "StringParameterTypeDef",
-    "PercentVisibleRangeOutputTypeDef",
     "PercentVisibleRangeTypeDef",
-    "PivotTableConditionalFormattingScopeOutputTypeDef",
     "PivotTableConditionalFormattingScopeTypeDef",
-    "PivotTablePaginatedReportOptionsOutputTypeDef",
     "PivotTablePaginatedReportOptionsTypeDef",
-    "PivotTableFieldOptionOutputTypeDef",
     "PivotTableFieldOptionTypeDef",
-    "PivotTableFieldSubtotalOptionsOutputTypeDef",
     "PivotTableFieldSubtotalOptionsTypeDef",
     "RowAlternateColorOptionsOutputTypeDef",
     "RowAlternateColorOptionsTypeDef",
     "ProjectOperationOutputTypeDef",
     "ProjectOperationTypeDef",
-    "RadarChartAreaStyleSettingsOutputTypeDef",
     "RadarChartAreaStyleSettingsTypeDef",
-    "RangeConstantOutputTypeDef",
     "RangeConstantTypeDef",
-    "ReferenceLineCustomLabelConfigurationOutputTypeDef",
     "ReferenceLineCustomLabelConfigurationTypeDef",
-    "ReferenceLineStaticDataConfigurationOutputTypeDef",
     "ReferenceLineStaticDataConfigurationTypeDef",
-    "ReferenceLineStyleConfigurationOutputTypeDef",
     "ReferenceLineStyleConfigurationTypeDef",
-    "ScheduleRefreshOnEntityOutputTypeDef",
     "ScheduleRefreshOnEntityTypeDef",
     "RegisterUserRequestRequestTypeDef",
     "StatePersistenceConfigurationsTypeDef",
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
-    "RenameColumnOperationOutputTypeDef",
     "RenameColumnOperationTypeDef",
     "RestoreAnalysisRequestRequestTypeDef",
-    "RowLevelPermissionTagRuleOutputTypeDef",
     "RowLevelPermissionTagRuleTypeDef",
-    "S3BucketConfigurationOutputTypeDef",
     "S3BucketConfigurationTypeDef",
-    "UploadSettingsOutputTypeDef",
     "UploadSettingsTypeDef",
-    "SectionAfterPageBreakOutputTypeDef",
     "SectionAfterPageBreakTypeDef",
-    "SpacingOutputTypeDef",
     "SpacingTypeDef",
     "SheetVisualScopingConfigurationOutputTypeDef",
     "SheetVisualScopingConfigurationTypeDef",
     "SemanticEntityTypeOutputTypeDef",
     "SemanticEntityTypeTypeDef",
     "SemanticTypeOutputTypeDef",
     "SemanticTypeTypeDef",
-    "SheetTextBoxOutputTypeDef",
     "SheetTextBoxTypeDef",
-    "SheetElementConfigurationOverridesOutputTypeDef",
     "SheetElementConfigurationOverridesTypeDef",
-    "ShortFormatTextOutputTypeDef",
     "ShortFormatTextTypeDef",
-    "SmallMultiplesAxisPropertiesOutputTypeDef",
     "SmallMultiplesAxisPropertiesTypeDef",
     "SnapshotAnonymousUserRedactedTypeDef",
     "SnapshotFileSheetSelectionOutputTypeDef",
     "SnapshotFileSheetSelectionTypeDef",
     "SnapshotJobResultErrorInfoTypeDef",
     "StringDatasetParameterDefaultValuesOutputTypeDef",
     "StringDatasetParameterDefaultValuesTypeDef",
-    "StringValueWhenUnsetConfigurationOutputTypeDef",
     "StringValueWhenUnsetConfigurationTypeDef",
-    "TableCellImageSizingConfigurationOutputTypeDef",
     "TableCellImageSizingConfigurationTypeDef",
-    "TablePaginatedReportOptionsOutputTypeDef",
     "TablePaginatedReportOptionsTypeDef",
-    "TableFieldCustomIconContentOutputTypeDef",
     "TableFieldCustomIconContentTypeDef",
     "TemplateSourceTemplateTypeDef",
-    "TextControlPlaceholderOptionsOutputTypeDef",
     "TextControlPlaceholderOptionsTypeDef",
-    "UIColorPaletteOutputTypeDef",
     "UIColorPaletteTypeDef",
     "ThemeErrorTypeDef",
-    "TopicSingularFilterConstantOutputTypeDef",
     "TopicSingularFilterConstantTypeDef",
     "UntagColumnOperationOutputTypeDef",
     "UntagColumnOperationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccountSettingsRequestRequestTypeDef",
     "UpdateDashboardPublishedVersionRequestRequestTypeDef",
     "UpdateFolderRequestRequestTypeDef",
@@ -791,63 +626,51 @@
     "UpdateIAMPolicyAssignmentRequestRequestTypeDef",
     "UpdateIpRestrictionRequestRequestTypeDef",
     "UpdatePublicSharingSettingsRequestRequestTypeDef",
     "UpdateTemplateAliasRequestRequestTypeDef",
     "UpdateThemeAliasRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateVPCConnectionRequestRequestTypeDef",
-    "WaterfallChartOptionsOutputTypeDef",
     "WaterfallChartOptionsTypeDef",
-    "WordCloudOptionsOutputTypeDef",
     "WordCloudOptionsTypeDef",
     "UpdateAccountCustomizationRequestRequestTypeDef",
-    "AxisLabelReferenceOptionsOutputTypeDef",
-    "CascadingControlSourceOutputTypeDef",
-    "CategoryDrillDownFilterOutputTypeDef",
-    "ContributionAnalysisDefaultOutputTypeDef",
-    "DynamicDefaultValueOutputTypeDef",
-    "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
-    "NumericEqualityDrillDownFilterOutputTypeDef",
-    "ParameterSelectableValuesOutputTypeDef",
-    "TimeEqualityFilterOutputTypeDef",
-    "TimeRangeDrillDownFilterOutputTypeDef",
     "AxisLabelReferenceOptionsTypeDef",
     "CascadingControlSourceTypeDef",
+    "CategoryDrillDownFilterOutputTypeDef",
     "CategoryDrillDownFilterTypeDef",
+    "ContributionAnalysisDefaultOutputTypeDef",
     "ContributionAnalysisDefaultTypeDef",
     "DynamicDefaultValueTypeDef",
+    "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
     "FilterOperationSelectedFieldsConfigurationTypeDef",
     "NumericEqualityDrillDownFilterTypeDef",
+    "ParameterSelectableValuesOutputTypeDef",
     "ParameterSelectableValuesTypeDef",
+    "TimeEqualityFilterOutputTypeDef",
     "TimeEqualityFilterTypeDef",
+    "TimeRangeDrillDownFilterOutputTypeDef",
     "TimeRangeDrillDownFilterTypeDef",
     "AnalysisErrorTypeDef",
     "DashboardErrorTypeDef",
     "TemplateErrorTypeDef",
     "SearchAnalysesRequestRequestTypeDef",
     "AnalysisSourceTemplateTypeDef",
     "DashboardSourceTemplateTypeDef",
     "TemplateSourceAnalysisTypeDef",
     "AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef",
     "RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef",
-    "ArcAxisConfigurationOutputTypeDef",
     "ArcAxisConfigurationTypeDef",
     "AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef",
     "AssetBundleCloudFormationOverridePropertyConfigurationTypeDef",
-    "AssetBundleImportJobDataSourceCredentialsOutputTypeDef",
     "AssetBundleImportJobDataSourceCredentialsTypeDef",
     "AxisDisplayRangeOutputTypeDef",
     "AxisDisplayRangeTypeDef",
-    "AxisScaleOutputTypeDef",
     "AxisScaleTypeDef",
-    "HistogramBinOptionsOutputTypeDef",
     "HistogramBinOptionsTypeDef",
-    "TileStyleOutputTypeDef",
     "TileStyleTypeDef",
-    "BoxPlotOptionsOutputTypeDef",
     "BoxPlotOptionsTypeDef",
     "CreateColumnsOperationOutputTypeDef",
     "CreateColumnsOperationTypeDef",
     "CancelIngestionResponseTypeDef",
     "CreateAccountCustomizationResponseTypeDef",
     "CreateAnalysisResponseTypeDef",
     "CreateDashboardResponseTypeDef",
@@ -923,46 +746,45 @@
     "UpdateTemplateResponseTypeDef",
     "UpdateThemeResponseTypeDef",
     "UpdateTopicRefreshScheduleResponseTypeDef",
     "UpdateTopicResponseTypeDef",
     "UpdateVPCConnectionResponseTypeDef",
     "CategoryFilterConfigurationOutputTypeDef",
     "CategoryFilterConfigurationTypeDef",
-    "ClusterMarkerOutputTypeDef",
     "ClusterMarkerTypeDef",
     "TopicCategoryFilterConstantOutputTypeDef",
     "TopicCategoryFilterConstantTypeDef",
     "ColorScaleOutputTypeDef",
     "ColorScaleTypeDef",
     "ColorsConfigurationOutputTypeDef",
     "ColorsConfigurationTypeDef",
-    "ColumnTagOutputTypeDef",
     "ColumnTagTypeDef",
     "ColumnGroupSchemaOutputTypeDef",
     "ColumnGroupSchemaTypeDef",
     "ColumnGroupOutputTypeDef",
     "ColumnGroupTypeDef",
     "DataSetSchemaOutputTypeDef",
     "DataSetSchemaTypeDef",
-    "ConditionalFormattingCustomIconConditionOutputTypeDef",
     "ConditionalFormattingCustomIconConditionTypeDef",
     "CreateAccountCustomizationRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateVPCConnectionRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateAccountSubscriptionResponseTypeDef",
     "CreateFolderRequestRequestTypeDef",
     "UpdateAnalysisPermissionsRequestRequestTypeDef",
     "UpdateDashboardPermissionsRequestRequestTypeDef",
     "UpdateDataSetPermissionsRequestRequestTypeDef",
     "UpdateDataSourcePermissionsRequestRequestTypeDef",
     "UpdateFolderPermissionsRequestRequestTypeDef",
     "UpdateTemplatePermissionsRequestRequestTypeDef",
     "UpdateThemePermissionsRequestRequestTypeDef",
     "UpdateTopicPermissionsRequestRequestTypeDef",
+    "DataSetSummaryTypeDef",
     "CreateFolderMembershipResponseTypeDef",
     "CreateGroupMembershipResponseTypeDef",
     "DescribeGroupMembershipResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "DescribeGroupResponseTypeDef",
     "ListGroupsResponseTypeDef",
@@ -975,42 +797,36 @@
     "UpdateTemplateAliasResponseTypeDef",
     "CreateThemeAliasResponseTypeDef",
     "DescribeThemeAliasResponseTypeDef",
     "ListThemeAliasesResponseTypeDef",
     "UpdateThemeAliasResponseTypeDef",
     "CreateTopicRefreshScheduleRequestRequestTypeDef",
     "UpdateTopicRefreshScheduleRequestRequestTypeDef",
-    "CustomActionNavigationOperationOutputTypeDef",
     "CustomActionNavigationOperationTypeDef",
     "CustomValuesConfigurationOutputTypeDef",
     "CustomValuesConfigurationTypeDef",
     "CustomSqlOutputTypeDef",
-    "RelationalTableOutputTypeDef",
     "CustomSqlTypeDef",
+    "RelationalTableOutputTypeDef",
     "RelationalTableTypeDef",
     "SearchDashboardsRequestRequestTypeDef",
     "ListDashboardsResponseTypeDef",
     "SearchDashboardsResponseTypeDef",
     "ListDashboardVersionsResponseTypeDef",
-    "DashboardVisualPublishOptionsOutputTypeDef",
     "DashboardVisualPublishOptionsTypeDef",
-    "TableInlineVisualizationOutputTypeDef",
     "TableInlineVisualizationTypeDef",
-    "DataLabelTypeOutputTypeDef",
     "DataLabelTypeTypeDef",
-    "DataPathColorOutputTypeDef",
-    "DataPathSortOutputTypeDef",
-    "PivotTableDataPathOptionOutputTypeDef",
-    "PivotTableFieldCollapseStateTargetOutputTypeDef",
     "DataPathColorTypeDef",
+    "DataPathSortOutputTypeDef",
     "DataPathSortTypeDef",
+    "PivotTableDataPathOptionOutputTypeDef",
     "PivotTableDataPathOptionTypeDef",
+    "PivotTableFieldCollapseStateTargetOutputTypeDef",
     "PivotTableFieldCollapseStateTargetTypeDef",
     "SearchDataSetsRequestRequestTypeDef",
-    "DataSetSummaryTypeDef",
     "SearchDataSourcesRequestRequestTypeDef",
     "SearchDataSourcesResponseTypeDef",
     "DateTimeDatasetParameterOutputTypeDef",
     "DateTimeDatasetParameterTypeDef",
     "TimeRangeFilterValueOutputTypeDef",
     "TimeRangeFilterValueTypeDef",
     "DecimalDatasetParameterOutputTypeDef",
@@ -1034,55 +850,43 @@
     "DescribeTopicRefreshResponseTypeDef",
     "DescribeTopicRefreshScheduleResponseTypeDef",
     "TopicRefreshScheduleSummaryTypeDef",
     "DescribeUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "RegisterUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
-    "DisplayFormatOptionsOutputTypeDef",
     "DisplayFormatOptionsTypeDef",
-    "DonutOptionsOutputTypeDef",
     "DonutOptionsTypeDef",
-    "RelativeDatesFilterOutputTypeDef",
     "RelativeDatesFilterTypeDef",
     "FilterOperationTargetVisualsConfigurationOutputTypeDef",
     "FilterOperationTargetVisualsConfigurationTypeDef",
     "SearchFoldersRequestRequestTypeDef",
     "ListFoldersResponseTypeDef",
     "SearchFoldersResponseTypeDef",
-    "FontConfigurationOutputTypeDef",
     "FontConfigurationTypeDef",
     "TypographyOutputTypeDef",
     "TypographyTypeDef",
     "ForecastScenarioOutputTypeDef",
     "ForecastScenarioTypeDef",
-    "FreeFormLayoutCanvasSizeOptionsOutputTypeDef",
     "FreeFormLayoutCanvasSizeOptionsTypeDef",
     "SnapshotAnonymousUserTypeDef",
-    "GeospatialWindowOptionsOutputTypeDef",
     "GeospatialWindowOptionsTypeDef",
     "GeospatialHeatmapColorScaleOutputTypeDef",
     "GeospatialHeatmapColorScaleTypeDef",
-    "TableSideBorderOptionsOutputTypeDef",
     "TableSideBorderOptionsTypeDef",
     "GradientColorOutputTypeDef",
     "GradientColorTypeDef",
-    "GridLayoutCanvasSizeOptionsOutputTypeDef",
     "GridLayoutCanvasSizeOptionsTypeDef",
     "SearchGroupsRequestRequestTypeDef",
     "ListIAMPolicyAssignmentsResponseTypeDef",
-    "IncrementalRefreshOutputTypeDef",
     "IncrementalRefreshTypeDef",
     "IngestionTypeDef",
     "IntegerDatasetParameterOutputTypeDef",
     "IntegerDatasetParameterTypeDef",
-    "JoinInstructionOutputTypeDef",
     "JoinInstructionTypeDef",
-    "LineChartDefaultSeriesSettingsOutputTypeDef",
-    "LineChartSeriesSettingsOutputTypeDef",
     "LineChartDefaultSeriesSettingsTypeDef",
     "LineChartSeriesSettingsTypeDef",
     "ListAnalysesRequestListAnalysesPaginateTypeDef",
     "ListAssetBundleExportJobsRequestListAssetBundleExportJobsPaginateTypeDef",
     "ListAssetBundleImportJobsRequestListAssetBundleImportJobsPaginateTypeDef",
     "ListDashboardVersionsRequestListDashboardVersionsPaginateTypeDef",
     "ListDashboardsRequestListDashboardsPaginateTypeDef",
@@ -1103,222 +907,177 @@
     "ListUsersRequestListUsersPaginateTypeDef",
     "SearchAnalysesRequestSearchAnalysesPaginateTypeDef",
     "SearchDashboardsRequestSearchDashboardsPaginateTypeDef",
     "SearchDataSetsRequestSearchDataSetsPaginateTypeDef",
     "SearchDataSourcesRequestSearchDataSourcesPaginateTypeDef",
     "SearchGroupsRequestSearchGroupsPaginateTypeDef",
     "ListFolderMembersResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTemplateVersionsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "ListThemeVersionsResponseTypeDef",
     "ListThemesResponseTypeDef",
     "ListTopicsResponseTypeDef",
-    "VisualSubtitleLabelOptionsOutputTypeDef",
     "VisualSubtitleLabelOptionsTypeDef",
-    "S3ParametersOutputTypeDef",
     "S3ParametersTypeDef",
-    "TileLayoutStyleOutputTypeDef",
     "TileLayoutStyleTypeDef",
     "NamedEntityDefinitionOutputTypeDef",
     "NamedEntityDefinitionTypeDef",
     "NamespaceInfoV2TypeDef",
     "VPCConnectionSummaryTypeDef",
     "VPCConnectionTypeDef",
     "OverrideDatasetParameterOperationOutputTypeDef",
     "OverrideDatasetParameterOperationTypeDef",
-    "NumericSeparatorConfigurationOutputTypeDef",
     "NumericSeparatorConfigurationTypeDef",
-    "NumericalAggregationFunctionOutputTypeDef",
     "NumericalAggregationFunctionTypeDef",
     "ParametersOutputTypeDef",
     "ParametersTypeDef",
-    "VisibleRangeOptionsOutputTypeDef",
     "VisibleRangeOptionsTypeDef",
-    "RadarChartSeriesSettingsOutputTypeDef",
     "RadarChartSeriesSettingsTypeDef",
-    "TopicRangeFilterConstantOutputTypeDef",
     "TopicRangeFilterConstantTypeDef",
-    "RefreshFrequencyOutputTypeDef",
     "RefreshFrequencyTypeDef",
     "RegisteredUserConsoleFeatureConfigurationsTypeDef",
     "RegisteredUserDashboardFeatureConfigurationsTypeDef",
     "RowLevelPermissionTagConfigurationOutputTypeDef",
     "RowLevelPermissionTagConfigurationTypeDef",
-    "SnapshotS3DestinationConfigurationOutputTypeDef",
     "SnapshotS3DestinationConfigurationTypeDef",
     "S3SourceOutputTypeDef",
     "S3SourceTypeDef",
-    "SectionPageBreakConfigurationOutputTypeDef",
     "SectionPageBreakConfigurationTypeDef",
-    "SectionBasedLayoutPaperCanvasSizeOptionsOutputTypeDef",
-    "SectionStyleOutputTypeDef",
     "SectionBasedLayoutPaperCanvasSizeOptionsTypeDef",
     "SectionStyleTypeDef",
     "SelectedSheetsFilterScopeConfigurationOutputTypeDef",
     "SelectedSheetsFilterScopeConfigurationTypeDef",
-    "SheetElementRenderingRuleOutputTypeDef",
     "SheetElementRenderingRuleTypeDef",
-    "VisualTitleLabelOptionsOutputTypeDef",
     "VisualTitleLabelOptionsTypeDef",
     "SnapshotUserConfigurationRedactedTypeDef",
     "SnapshotFileOutputTypeDef",
     "SnapshotFileTypeDef",
     "StringDatasetParameterOutputTypeDef",
     "StringDatasetParameterTypeDef",
-    "TableFieldImageConfigurationOutputTypeDef",
     "TableFieldImageConfigurationTypeDef",
-    "TopicNumericEqualityFilterOutputTypeDef",
-    "TopicRelativeDateFilterOutputTypeDef",
     "TopicNumericEqualityFilterTypeDef",
     "TopicRelativeDateFilterTypeDef",
     "CascadingControlConfigurationOutputTypeDef",
-    "DateTimeDefaultValuesOutputTypeDef",
-    "DecimalDefaultValuesOutputTypeDef",
-    "IntegerDefaultValuesOutputTypeDef",
-    "StringDefaultValuesOutputTypeDef",
-    "DrillDownFilterOutputTypeDef",
     "CascadingControlConfigurationTypeDef",
+    "DateTimeDefaultValuesOutputTypeDef",
     "DateTimeDefaultValuesTypeDef",
+    "DecimalDefaultValuesOutputTypeDef",
     "DecimalDefaultValuesTypeDef",
+    "IntegerDefaultValuesOutputTypeDef",
     "IntegerDefaultValuesTypeDef",
+    "StringDefaultValuesOutputTypeDef",
     "StringDefaultValuesTypeDef",
+    "DrillDownFilterOutputTypeDef",
     "DrillDownFilterTypeDef",
     "AnalysisTypeDef",
     "DashboardVersionTypeDef",
     "AnalysisSourceEntityTypeDef",
     "DashboardSourceEntityTypeDef",
     "TemplateSourceEntityTypeDef",
     "AnonymousUserEmbeddingExperienceConfigurationTypeDef",
     "DescribeAssetBundleExportJobResponseTypeDef",
     "StartAssetBundleExportJobRequestRequestTypeDef",
     "NumericAxisOptionsOutputTypeDef",
     "NumericAxisOptionsTypeDef",
     "CategoryFilterOutputTypeDef",
     "CategoryFilterTypeDef",
-    "ClusterMarkerConfigurationOutputTypeDef",
     "ClusterMarkerConfigurationTypeDef",
     "TopicCategoryFilterOutputTypeDef",
     "TopicCategoryFilterTypeDef",
     "TagColumnOperationOutputTypeDef",
     "TagColumnOperationTypeDef",
     "DataSetConfigurationOutputTypeDef",
     "DataSetConfigurationTypeDef",
-    "ConditionalFormattingIconOutputTypeDef",
     "ConditionalFormattingIconTypeDef",
+    "ListDataSetsResponseTypeDef",
+    "SearchDataSetsResponseTypeDef",
     "DestinationParameterValueConfigurationOutputTypeDef",
     "DestinationParameterValueConfigurationTypeDef",
-    "DashboardPublishOptionsOutputTypeDef",
     "DashboardPublishOptionsTypeDef",
     "VisualPaletteOutputTypeDef",
-    "PivotTableFieldCollapseStateOptionOutputTypeDef",
     "VisualPaletteTypeDef",
+    "PivotTableFieldCollapseStateOptionOutputTypeDef",
     "PivotTableFieldCollapseStateOptionTypeDef",
-    "ListDataSetsResponseTypeDef",
-    "SearchDataSetsResponseTypeDef",
     "TimeRangeFilterOutputTypeDef",
     "TimeRangeFilterTypeDef",
     "DescribeDashboardPermissionsResponseTypeDef",
     "UpdateDashboardPermissionsResponseTypeDef",
     "ListTopicRefreshSchedulesResponseTypeDef",
-    "DefaultFormattingOutputTypeDef",
     "DefaultFormattingTypeDef",
     "CustomActionFilterOperationOutputTypeDef",
     "CustomActionFilterOperationTypeDef",
-    "AxisLabelOptionsOutputTypeDef",
-    "DataLabelOptionsOutputTypeDef",
-    "FunnelChartDataLabelOptionsOutputTypeDef",
-    "LabelOptionsOutputTypeDef",
-    "PanelTitleOptionsOutputTypeDef",
-    "TableFieldCustomTextContentOutputTypeDef",
     "AxisLabelOptionsTypeDef",
+    "DataLabelOptionsOutputTypeDef",
     "DataLabelOptionsTypeDef",
     "FunnelChartDataLabelOptionsTypeDef",
     "LabelOptionsTypeDef",
     "PanelTitleOptionsTypeDef",
     "TableFieldCustomTextContentTypeDef",
     "ForecastConfigurationOutputTypeDef",
     "ForecastConfigurationTypeDef",
-    "DefaultFreeFormLayoutConfigurationOutputTypeDef",
     "DefaultFreeFormLayoutConfigurationTypeDef",
     "SnapshotUserConfigurationTypeDef",
     "GeospatialHeatmapConfigurationOutputTypeDef",
     "GeospatialHeatmapConfigurationTypeDef",
-    "GlobalTableBorderOptionsOutputTypeDef",
     "GlobalTableBorderOptionsTypeDef",
     "ConditionalFormattingGradientColorOutputTypeDef",
     "ConditionalFormattingGradientColorTypeDef",
-    "DefaultGridLayoutConfigurationOutputTypeDef",
-    "GridLayoutConfigurationOutputTypeDef",
     "DefaultGridLayoutConfigurationTypeDef",
+    "GridLayoutConfigurationOutputTypeDef",
     "GridLayoutConfigurationTypeDef",
-    "RefreshConfigurationOutputTypeDef",
     "RefreshConfigurationTypeDef",
     "DescribeIngestionResponseTypeDef",
     "ListIngestionsResponseTypeDef",
-    "LogicalTableSourceOutputTypeDef",
     "LogicalTableSourceTypeDef",
-    "DataFieldSeriesItemOutputTypeDef",
-    "FieldSeriesItemOutputTypeDef",
     "DataFieldSeriesItemTypeDef",
     "FieldSeriesItemTypeDef",
-    "DataSourceParametersOutputTypeDef",
     "DataSourceParametersTypeDef",
-    "SheetStyleOutputTypeDef",
     "SheetStyleTypeDef",
     "TopicNamedEntityOutputTypeDef",
     "TopicNamedEntityTypeDef",
     "DescribeNamespaceResponseTypeDef",
     "ListNamespacesResponseTypeDef",
     "ListVPCConnectionsResponseTypeDef",
     "DescribeVPCConnectionResponseTypeDef",
-    "CurrencyDisplayFormatConfigurationOutputTypeDef",
-    "NumberDisplayFormatConfigurationOutputTypeDef",
-    "PercentageDisplayFormatConfigurationOutputTypeDef",
     "CurrencyDisplayFormatConfigurationTypeDef",
     "NumberDisplayFormatConfigurationTypeDef",
     "PercentageDisplayFormatConfigurationTypeDef",
-    "AggregationFunctionOutputTypeDef",
     "AggregationFunctionTypeDef",
-    "ScrollBarOptionsOutputTypeDef",
     "ScrollBarOptionsTypeDef",
-    "TopicDateRangeFilterOutputTypeDef",
-    "TopicNumericRangeFilterOutputTypeDef",
     "TopicDateRangeFilterTypeDef",
     "TopicNumericRangeFilterTypeDef",
     "RefreshScheduleOutputTypeDef",
     "RefreshScheduleTypeDef",
     "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
     "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
     "SnapshotDestinationConfigurationOutputTypeDef",
-    "SnapshotJobS3ResultTypeDef",
     "SnapshotDestinationConfigurationTypeDef",
+    "SnapshotJobS3ResultTypeDef",
     "PhysicalTableOutputTypeDef",
     "PhysicalTableTypeDef",
-    "SectionBasedLayoutCanvasSizeOptionsOutputTypeDef",
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
     "FilterScopeConfigurationOutputTypeDef",
     "FilterScopeConfigurationTypeDef",
     "FreeFormLayoutElementOutputTypeDef",
     "FreeFormLayoutElementTypeDef",
     "SnapshotFileGroupOutputTypeDef",
     "SnapshotFileGroupTypeDef",
     "DatasetParameterOutputTypeDef",
     "DatasetParameterTypeDef",
     "DateTimeParameterDeclarationOutputTypeDef",
+    "DateTimeParameterDeclarationTypeDef",
     "DecimalParameterDeclarationOutputTypeDef",
+    "DecimalParameterDeclarationTypeDef",
     "IntegerParameterDeclarationOutputTypeDef",
+    "IntegerParameterDeclarationTypeDef",
     "StringParameterDeclarationOutputTypeDef",
+    "StringParameterDeclarationTypeDef",
     "DateTimeHierarchyOutputTypeDef",
     "ExplicitHierarchyOutputTypeDef",
     "PredefinedHierarchyOutputTypeDef",
-    "DateTimeParameterDeclarationTypeDef",
-    "DecimalParameterDeclarationTypeDef",
-    "IntegerParameterDeclarationTypeDef",
-    "StringParameterDeclarationTypeDef",
     "DateTimeHierarchyTypeDef",
     "ExplicitHierarchyTypeDef",
     "PredefinedHierarchyTypeDef",
     "DescribeAnalysisResponseTypeDef",
     "DashboardTypeDef",
     "GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
     "AxisDataOptionsOutputTypeDef",
@@ -1327,143 +1086,105 @@
     "TransformOperationTypeDef",
     "TemplateVersionTypeDef",
     "SetParameterValueConfigurationOutputTypeDef",
     "SetParameterValueConfigurationTypeDef",
     "PivotTableFieldOptionsOutputTypeDef",
     "PivotTableFieldOptionsTypeDef",
     "TopicCalculatedFieldOutputTypeDef",
-    "TopicColumnOutputTypeDef",
     "TopicCalculatedFieldTypeDef",
+    "TopicColumnOutputTypeDef",
     "TopicColumnTypeDef",
     "ChartAxisLabelOptionsOutputTypeDef",
-    "AxisTickLabelOptionsOutputTypeDef",
-    "DateTimePickerControlDisplayOptionsOutputTypeDef",
-    "DropDownControlDisplayOptionsOutputTypeDef",
-    "LegendOptionsOutputTypeDef",
-    "ListControlDisplayOptionsOutputTypeDef",
-    "RelativeDateTimeControlDisplayOptionsOutputTypeDef",
-    "SliderControlDisplayOptionsOutputTypeDef",
-    "TextAreaControlDisplayOptionsOutputTypeDef",
-    "TextFieldControlDisplayOptionsOutputTypeDef",
-    "PanelConfigurationOutputTypeDef",
-    "TableFieldLinkContentConfigurationOutputTypeDef",
     "ChartAxisLabelOptionsTypeDef",
     "AxisTickLabelOptionsTypeDef",
     "DateTimePickerControlDisplayOptionsTypeDef",
     "DropDownControlDisplayOptionsTypeDef",
     "LegendOptionsTypeDef",
     "ListControlDisplayOptionsTypeDef",
     "RelativeDateTimeControlDisplayOptionsTypeDef",
     "SliderControlDisplayOptionsTypeDef",
     "TextAreaControlDisplayOptionsTypeDef",
     "TextFieldControlDisplayOptionsTypeDef",
     "PanelConfigurationTypeDef",
     "TableFieldLinkContentConfigurationTypeDef",
     "GeospatialPointStyleOptionsOutputTypeDef",
     "GeospatialPointStyleOptionsTypeDef",
-    "TableCellStyleOutputTypeDef",
     "TableCellStyleTypeDef",
     "ConditionalFormattingColorOutputTypeDef",
     "ConditionalFormattingColorTypeDef",
-    "DefaultInteractiveLayoutConfigurationOutputTypeDef",
-    "SheetControlLayoutConfigurationOutputTypeDef",
     "DefaultInteractiveLayoutConfigurationTypeDef",
+    "SheetControlLayoutConfigurationOutputTypeDef",
     "SheetControlLayoutConfigurationTypeDef",
-    "DataSetRefreshPropertiesOutputTypeDef",
     "DataSetRefreshPropertiesTypeDef",
-    "SeriesItemOutputTypeDef",
     "SeriesItemTypeDef",
-    "AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef",
-    "DataSourceTypeDef",
     "AssetBundleImportJobDataSourceOverrideParametersTypeDef",
     "CredentialPairTypeDef",
+    "DataSourceTypeDef",
     "ThemeConfigurationOutputTypeDef",
     "ThemeConfigurationTypeDef",
-    "ComparisonFormatConfigurationOutputTypeDef",
-    "NumericFormatConfigurationOutputTypeDef",
     "ComparisonFormatConfigurationTypeDef",
     "NumericFormatConfigurationTypeDef",
-    "AggregationSortConfigurationOutputTypeDef",
-    "ColumnSortOutputTypeDef",
-    "ColumnTooltipItemOutputTypeDef",
-    "NumericEqualityFilterOutputTypeDef",
-    "NumericRangeFilterOutputTypeDef",
-    "ReferenceLineDynamicDataConfigurationOutputTypeDef",
     "AggregationSortConfigurationTypeDef",
     "ColumnSortTypeDef",
     "ColumnTooltipItemTypeDef",
     "NumericEqualityFilterTypeDef",
     "NumericRangeFilterTypeDef",
     "ReferenceLineDynamicDataConfigurationTypeDef",
     "TopicFilterOutputTypeDef",
     "TopicFilterTypeDef",
     "DescribeRefreshScheduleResponseTypeDef",
     "ListRefreshSchedulesResponseTypeDef",
     "CreateRefreshScheduleRequestRequestTypeDef",
     "UpdateRefreshScheduleRequestRequestTypeDef",
     "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
     "SnapshotJobResultFileGroupTypeDef",
-    "DefaultSectionBasedLayoutConfigurationOutputTypeDef",
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     "FreeFormLayoutConfigurationOutputTypeDef",
     "FreeFormSectionLayoutConfigurationOutputTypeDef",
     "FreeFormLayoutConfigurationTypeDef",
     "FreeFormSectionLayoutConfigurationTypeDef",
     "SnapshotConfigurationOutputTypeDef",
     "SnapshotConfigurationTypeDef",
     "ParameterDeclarationOutputTypeDef",
-    "ColumnHierarchyOutputTypeDef",
     "ParameterDeclarationTypeDef",
+    "ColumnHierarchyOutputTypeDef",
     "ColumnHierarchyTypeDef",
     "DescribeDashboardResponseTypeDef",
     "LogicalTableOutputTypeDef",
     "LogicalTableTypeDef",
     "TemplateTypeDef",
     "CustomActionSetParametersOperationOutputTypeDef",
     "CustomActionSetParametersOperationTypeDef",
     "AxisDisplayOptionsOutputTypeDef",
-    "FilterDateTimePickerControlOutputTypeDef",
-    "ParameterDateTimePickerControlOutputTypeDef",
-    "FilterDropDownControlOutputTypeDef",
-    "ParameterDropDownControlOutputTypeDef",
-    "FilterListControlOutputTypeDef",
-    "ParameterListControlOutputTypeDef",
-    "FilterRelativeDateTimeControlOutputTypeDef",
-    "FilterSliderControlOutputTypeDef",
-    "ParameterSliderControlOutputTypeDef",
-    "FilterTextAreaControlOutputTypeDef",
-    "ParameterTextAreaControlOutputTypeDef",
-    "FilterTextFieldControlOutputTypeDef",
-    "ParameterTextFieldControlOutputTypeDef",
-    "SmallMultiplesOptionsOutputTypeDef",
-    "TableFieldLinkConfigurationOutputTypeDef",
     "AxisDisplayOptionsTypeDef",
     "FilterDateTimePickerControlTypeDef",
     "ParameterDateTimePickerControlTypeDef",
+    "FilterDropDownControlOutputTypeDef",
     "FilterDropDownControlTypeDef",
+    "ParameterDropDownControlOutputTypeDef",
     "ParameterDropDownControlTypeDef",
+    "FilterListControlOutputTypeDef",
     "FilterListControlTypeDef",
+    "ParameterListControlOutputTypeDef",
     "ParameterListControlTypeDef",
     "FilterRelativeDateTimeControlTypeDef",
     "FilterSliderControlTypeDef",
     "ParameterSliderControlTypeDef",
     "FilterTextAreaControlTypeDef",
     "ParameterTextAreaControlTypeDef",
     "FilterTextFieldControlTypeDef",
     "ParameterTextFieldControlTypeDef",
     "SmallMultiplesOptionsTypeDef",
     "TableFieldLinkConfigurationTypeDef",
     "PivotTableOptionsOutputTypeDef",
-    "PivotTotalOptionsOutputTypeDef",
-    "SubtotalOptionsOutputTypeDef",
-    "TableOptionsOutputTypeDef",
-    "TotalOptionsOutputTypeDef",
     "PivotTableOptionsTypeDef",
     "PivotTotalOptionsTypeDef",
+    "SubtotalOptionsOutputTypeDef",
     "SubtotalOptionsTypeDef",
+    "TableOptionsOutputTypeDef",
     "TableOptionsTypeDef",
     "TotalOptionsTypeDef",
     "GaugeChartArcConditionalFormattingOutputTypeDef",
     "GaugeChartPrimaryValueConditionalFormattingOutputTypeDef",
     "KPIPrimaryValueConditionalFormattingOutputTypeDef",
     "KPIProgressBarConditionalFormattingOutputTypeDef",
     "ShapeConditionalFormatOutputTypeDef",
@@ -1477,63 +1198,53 @@
     "TableRowConditionalFormattingTypeDef",
     "TextConditionalFormatTypeDef",
     "SheetControlLayoutOutputTypeDef",
     "SheetControlLayoutTypeDef",
     "DescribeDataSetRefreshPropertiesResponseTypeDef",
     "PutDataSetRefreshPropertiesRequestRequestTypeDef",
     "AssetBundleImportJobOverrideParametersOutputTypeDef",
-    "DescribeDataSourceResponseTypeDef",
-    "ListDataSourcesResponseTypeDef",
     "AssetBundleImportJobOverrideParametersTypeDef",
     "DataSourceCredentialsTypeDef",
+    "DescribeDataSourceResponseTypeDef",
+    "ListDataSourcesResponseTypeDef",
     "ThemeVersionTypeDef",
     "CreateThemeRequestRequestTypeDef",
     "UpdateThemeRequestRequestTypeDef",
-    "ComparisonConfigurationOutputTypeDef",
-    "DateTimeFormatConfigurationOutputTypeDef",
-    "NumberFormatConfigurationOutputTypeDef",
-    "ReferenceLineValueLabelConfigurationOutputTypeDef",
-    "StringFormatConfigurationOutputTypeDef",
     "ComparisonConfigurationTypeDef",
     "DateTimeFormatConfigurationTypeDef",
     "NumberFormatConfigurationTypeDef",
     "ReferenceLineValueLabelConfigurationTypeDef",
     "StringFormatConfigurationTypeDef",
     "TopBottomFilterOutputTypeDef",
-    "FieldSortOptionsOutputTypeDef",
-    "PivotTableSortByOutputTypeDef",
-    "TooltipItemOutputTypeDef",
-    "ReferenceLineDataConfigurationOutputTypeDef",
     "TopBottomFilterTypeDef",
     "FieldSortOptionsTypeDef",
+    "PivotTableSortByOutputTypeDef",
     "PivotTableSortByTypeDef",
     "TooltipItemTypeDef",
     "ReferenceLineDataConfigurationTypeDef",
     "DatasetMetadataOutputTypeDef",
     "DatasetMetadataTypeDef",
     "GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
     "AnonymousUserSnapshotJobResultTypeDef",
-    "DefaultPaginatedLayoutConfigurationOutputTypeDef",
     "DefaultPaginatedLayoutConfigurationTypeDef",
     "SectionLayoutConfigurationOutputTypeDef",
     "SectionLayoutConfigurationTypeDef",
     "DescribeDashboardSnapshotJobResponseTypeDef",
     "StartDashboardSnapshotJobRequestRequestTypeDef",
     "DataSetTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "UpdateDataSetRequestRequestTypeDef",
     "DescribeTemplateResponseTypeDef",
     "VisualCustomActionOperationOutputTypeDef",
     "VisualCustomActionOperationTypeDef",
     "LineSeriesAxisDisplayOptionsOutputTypeDef",
-    "FilterControlOutputTypeDef",
-    "ParameterControlOutputTypeDef",
-    "TableFieldURLConfigurationOutputTypeDef",
     "LineSeriesAxisDisplayOptionsTypeDef",
+    "FilterControlOutputTypeDef",
     "FilterControlTypeDef",
+    "ParameterControlOutputTypeDef",
     "ParameterControlTypeDef",
     "TableFieldURLConfigurationTypeDef",
     "PivotTableTotalOptionsOutputTypeDef",
     "PivotTableTotalOptionsTypeDef",
     "GaugeChartConditionalFormattingOptionOutputTypeDef",
     "KPIConditionalFormattingOptionOutputTypeDef",
     "FilledMapShapeConditionalFormattingOutputTypeDef",
@@ -1545,116 +1256,99 @@
     "PivotTableCellConditionalFormattingTypeDef",
     "TableCellConditionalFormattingTypeDef",
     "DescribeAssetBundleImportJobResponseTypeDef",
     "StartAssetBundleImportJobRequestRequestTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "ThemeTypeDef",
-    "GaugeChartOptionsOutputTypeDef",
-    "KPIOptionsOutputTypeDef",
-    "DateDimensionFieldOutputTypeDef",
-    "DateMeasureFieldOutputTypeDef",
-    "NumericalDimensionFieldOutputTypeDef",
-    "NumericalMeasureFieldOutputTypeDef",
-    "ReferenceLineLabelConfigurationOutputTypeDef",
-    "CategoricalDimensionFieldOutputTypeDef",
-    "CategoricalMeasureFieldOutputTypeDef",
-    "FormatConfigurationOutputTypeDef",
     "GaugeChartOptionsTypeDef",
     "KPIOptionsTypeDef",
     "DateDimensionFieldTypeDef",
     "DateMeasureFieldTypeDef",
     "NumericalDimensionFieldTypeDef",
     "NumericalMeasureFieldTypeDef",
     "ReferenceLineLabelConfigurationTypeDef",
     "CategoricalDimensionFieldTypeDef",
     "CategoricalMeasureFieldTypeDef",
     "FormatConfigurationTypeDef",
     "FilterOutputTypeDef",
-    "BarChartSortConfigurationOutputTypeDef",
-    "BoxPlotSortConfigurationOutputTypeDef",
-    "ComboChartSortConfigurationOutputTypeDef",
-    "FilledMapSortConfigurationOutputTypeDef",
-    "FunnelChartSortConfigurationOutputTypeDef",
-    "HeatMapSortConfigurationOutputTypeDef",
-    "KPISortConfigurationOutputTypeDef",
-    "LineChartSortConfigurationOutputTypeDef",
-    "PieChartSortConfigurationOutputTypeDef",
-    "RadarChartSortConfigurationOutputTypeDef",
-    "SankeyDiagramSortConfigurationOutputTypeDef",
-    "TableSortConfigurationOutputTypeDef",
-    "TreeMapSortConfigurationOutputTypeDef",
-    "WaterfallChartSortConfigurationOutputTypeDef",
-    "WordCloudSortConfigurationOutputTypeDef",
-    "PivotFieldSortOptionsOutputTypeDef",
-    "FieldBasedTooltipOutputTypeDef",
     "FilterTypeDef",
+    "BarChartSortConfigurationOutputTypeDef",
     "BarChartSortConfigurationTypeDef",
+    "BoxPlotSortConfigurationOutputTypeDef",
     "BoxPlotSortConfigurationTypeDef",
+    "ComboChartSortConfigurationOutputTypeDef",
     "ComboChartSortConfigurationTypeDef",
+    "FilledMapSortConfigurationOutputTypeDef",
     "FilledMapSortConfigurationTypeDef",
+    "FunnelChartSortConfigurationOutputTypeDef",
     "FunnelChartSortConfigurationTypeDef",
+    "HeatMapSortConfigurationOutputTypeDef",
     "HeatMapSortConfigurationTypeDef",
+    "KPISortConfigurationOutputTypeDef",
     "KPISortConfigurationTypeDef",
+    "LineChartSortConfigurationOutputTypeDef",
     "LineChartSortConfigurationTypeDef",
+    "PieChartSortConfigurationOutputTypeDef",
     "PieChartSortConfigurationTypeDef",
+    "RadarChartSortConfigurationOutputTypeDef",
     "RadarChartSortConfigurationTypeDef",
+    "SankeyDiagramSortConfigurationOutputTypeDef",
     "SankeyDiagramSortConfigurationTypeDef",
+    "TableSortConfigurationOutputTypeDef",
     "TableSortConfigurationTypeDef",
+    "TreeMapSortConfigurationOutputTypeDef",
     "TreeMapSortConfigurationTypeDef",
+    "WaterfallChartSortConfigurationOutputTypeDef",
     "WaterfallChartSortConfigurationTypeDef",
+    "WordCloudSortConfigurationOutputTypeDef",
     "WordCloudSortConfigurationTypeDef",
+    "PivotFieldSortOptionsOutputTypeDef",
     "PivotFieldSortOptionsTypeDef",
+    "FieldBasedTooltipOutputTypeDef",
     "FieldBasedTooltipTypeDef",
     "TopicDetailsOutputTypeDef",
     "TopicDetailsTypeDef",
     "SnapshotJobResultTypeDef",
-    "DefaultNewSheetConfigurationOutputTypeDef",
     "DefaultNewSheetConfigurationTypeDef",
     "BodySectionContentOutputTypeDef",
     "HeaderFooterSectionConfigurationOutputTypeDef",
     "BodySectionContentTypeDef",
     "HeaderFooterSectionConfigurationTypeDef",
     "DescribeDataSetResponseTypeDef",
     "VisualCustomActionOutputTypeDef",
     "VisualCustomActionTypeDef",
-    "TableFieldOptionOutputTypeDef",
     "TableFieldOptionTypeDef",
     "GaugeChartConditionalFormattingOutputTypeDef",
     "KPIConditionalFormattingOutputTypeDef",
     "FilledMapConditionalFormattingOptionOutputTypeDef",
     "PivotTableConditionalFormattingOptionOutputTypeDef",
     "TableConditionalFormattingOptionOutputTypeDef",
     "GaugeChartConditionalFormattingTypeDef",
     "KPIConditionalFormattingTypeDef",
     "FilledMapConditionalFormattingOptionTypeDef",
     "PivotTableConditionalFormattingOptionTypeDef",
     "TableConditionalFormattingOptionTypeDef",
     "DescribeThemeResponseTypeDef",
-    "ReferenceLineOutputTypeDef",
-    "DimensionFieldOutputTypeDef",
-    "MeasureFieldOutputTypeDef",
-    "ColumnConfigurationOutputTypeDef",
-    "UnaggregatedFieldOutputTypeDef",
     "ReferenceLineTypeDef",
     "DimensionFieldTypeDef",
     "MeasureFieldTypeDef",
+    "ColumnConfigurationOutputTypeDef",
     "ColumnConfigurationTypeDef",
     "UnaggregatedFieldTypeDef",
     "FilterGroupOutputTypeDef",
-    "PivotTableSortConfigurationOutputTypeDef",
-    "TooltipOptionsOutputTypeDef",
     "FilterGroupTypeDef",
+    "PivotTableSortConfigurationOutputTypeDef",
     "PivotTableSortConfigurationTypeDef",
+    "TooltipOptionsOutputTypeDef",
     "TooltipOptionsTypeDef",
     "DescribeTopicResponseTypeDef",
     "CreateTopicRequestRequestTypeDef",
     "UpdateTopicRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobResultResponseTypeDef",
-    "AnalysisDefaultsOutputTypeDef",
     "AnalysisDefaultsTypeDef",
     "BodySectionConfigurationOutputTypeDef",
     "BodySectionConfigurationTypeDef",
     "CustomContentVisualOutputTypeDef",
     "EmptyVisualOutputTypeDef",
     "CustomContentVisualTypeDef",
     "EmptyVisualTypeDef",
@@ -1662,205 +1356,194 @@
     "TableFieldOptionsTypeDef",
     "FilledMapConditionalFormattingOutputTypeDef",
     "PivotTableConditionalFormattingOutputTypeDef",
     "TableConditionalFormattingOutputTypeDef",
     "FilledMapConditionalFormattingTypeDef",
     "PivotTableConditionalFormattingTypeDef",
     "TableConditionalFormattingTypeDef",
-    "UniqueValuesComputationOutputTypeDef",
-    "BarChartAggregatedFieldWellsOutputTypeDef",
-    "BoxPlotAggregatedFieldWellsOutputTypeDef",
-    "ComboChartAggregatedFieldWellsOutputTypeDef",
-    "FilledMapAggregatedFieldWellsOutputTypeDef",
-    "ForecastComputationOutputTypeDef",
-    "FunnelChartAggregatedFieldWellsOutputTypeDef",
-    "GaugeChartFieldWellsOutputTypeDef",
-    "GeospatialMapAggregatedFieldWellsOutputTypeDef",
-    "GrowthRateComputationOutputTypeDef",
-    "HeatMapAggregatedFieldWellsOutputTypeDef",
-    "HistogramAggregatedFieldWellsOutputTypeDef",
-    "KPIFieldWellsOutputTypeDef",
-    "LineChartAggregatedFieldWellsOutputTypeDef",
-    "MaximumMinimumComputationOutputTypeDef",
-    "MetricComparisonComputationOutputTypeDef",
-    "PeriodOverPeriodComputationOutputTypeDef",
-    "PeriodToDateComputationOutputTypeDef",
-    "PieChartAggregatedFieldWellsOutputTypeDef",
-    "PivotTableAggregatedFieldWellsOutputTypeDef",
-    "RadarChartAggregatedFieldWellsOutputTypeDef",
-    "SankeyDiagramAggregatedFieldWellsOutputTypeDef",
-    "ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef",
-    "ScatterPlotUnaggregatedFieldWellsOutputTypeDef",
-    "TableAggregatedFieldWellsOutputTypeDef",
-    "TopBottomMoversComputationOutputTypeDef",
-    "TopBottomRankedComputationOutputTypeDef",
-    "TotalAggregationComputationOutputTypeDef",
-    "TreeMapAggregatedFieldWellsOutputTypeDef",
-    "WaterfallChartAggregatedFieldWellsOutputTypeDef",
-    "WordCloudAggregatedFieldWellsOutputTypeDef",
-    "TableUnaggregatedFieldWellsOutputTypeDef",
     "UniqueValuesComputationTypeDef",
+    "BarChartAggregatedFieldWellsOutputTypeDef",
     "BarChartAggregatedFieldWellsTypeDef",
+    "BoxPlotAggregatedFieldWellsOutputTypeDef",
     "BoxPlotAggregatedFieldWellsTypeDef",
+    "ComboChartAggregatedFieldWellsOutputTypeDef",
     "ComboChartAggregatedFieldWellsTypeDef",
+    "FilledMapAggregatedFieldWellsOutputTypeDef",
     "FilledMapAggregatedFieldWellsTypeDef",
     "ForecastComputationTypeDef",
+    "FunnelChartAggregatedFieldWellsOutputTypeDef",
     "FunnelChartAggregatedFieldWellsTypeDef",
+    "GaugeChartFieldWellsOutputTypeDef",
     "GaugeChartFieldWellsTypeDef",
+    "GeospatialMapAggregatedFieldWellsOutputTypeDef",
     "GeospatialMapAggregatedFieldWellsTypeDef",
     "GrowthRateComputationTypeDef",
+    "HeatMapAggregatedFieldWellsOutputTypeDef",
     "HeatMapAggregatedFieldWellsTypeDef",
+    "HistogramAggregatedFieldWellsOutputTypeDef",
     "HistogramAggregatedFieldWellsTypeDef",
+    "KPIFieldWellsOutputTypeDef",
     "KPIFieldWellsTypeDef",
+    "LineChartAggregatedFieldWellsOutputTypeDef",
     "LineChartAggregatedFieldWellsTypeDef",
     "MaximumMinimumComputationTypeDef",
     "MetricComparisonComputationTypeDef",
     "PeriodOverPeriodComputationTypeDef",
     "PeriodToDateComputationTypeDef",
+    "PieChartAggregatedFieldWellsOutputTypeDef",
     "PieChartAggregatedFieldWellsTypeDef",
+    "PivotTableAggregatedFieldWellsOutputTypeDef",
     "PivotTableAggregatedFieldWellsTypeDef",
+    "RadarChartAggregatedFieldWellsOutputTypeDef",
     "RadarChartAggregatedFieldWellsTypeDef",
+    "SankeyDiagramAggregatedFieldWellsOutputTypeDef",
     "SankeyDiagramAggregatedFieldWellsTypeDef",
+    "ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef",
     "ScatterPlotCategoricallyAggregatedFieldWellsTypeDef",
+    "ScatterPlotUnaggregatedFieldWellsOutputTypeDef",
     "ScatterPlotUnaggregatedFieldWellsTypeDef",
+    "TableAggregatedFieldWellsOutputTypeDef",
     "TableAggregatedFieldWellsTypeDef",
     "TopBottomMoversComputationTypeDef",
     "TopBottomRankedComputationTypeDef",
     "TotalAggregationComputationTypeDef",
+    "TreeMapAggregatedFieldWellsOutputTypeDef",
     "TreeMapAggregatedFieldWellsTypeDef",
+    "WaterfallChartAggregatedFieldWellsOutputTypeDef",
     "WaterfallChartAggregatedFieldWellsTypeDef",
+    "WordCloudAggregatedFieldWellsOutputTypeDef",
     "WordCloudAggregatedFieldWellsTypeDef",
+    "TableUnaggregatedFieldWellsOutputTypeDef",
     "TableUnaggregatedFieldWellsTypeDef",
     "SectionBasedLayoutConfigurationOutputTypeDef",
     "SectionBasedLayoutConfigurationTypeDef",
     "BarChartFieldWellsOutputTypeDef",
-    "BoxPlotFieldWellsOutputTypeDef",
-    "ComboChartFieldWellsOutputTypeDef",
-    "FilledMapFieldWellsOutputTypeDef",
-    "FunnelChartFieldWellsOutputTypeDef",
-    "GaugeChartConfigurationOutputTypeDef",
-    "GeospatialMapFieldWellsOutputTypeDef",
-    "HeatMapFieldWellsOutputTypeDef",
-    "HistogramFieldWellsOutputTypeDef",
-    "KPIConfigurationOutputTypeDef",
-    "LineChartFieldWellsOutputTypeDef",
-    "PieChartFieldWellsOutputTypeDef",
-    "PivotTableFieldWellsOutputTypeDef",
-    "RadarChartFieldWellsOutputTypeDef",
-    "SankeyDiagramFieldWellsOutputTypeDef",
-    "ScatterPlotFieldWellsOutputTypeDef",
-    "ComputationOutputTypeDef",
-    "TreeMapFieldWellsOutputTypeDef",
-    "WaterfallChartFieldWellsOutputTypeDef",
-    "WordCloudFieldWellsOutputTypeDef",
-    "TableFieldWellsOutputTypeDef",
     "BarChartFieldWellsTypeDef",
+    "BoxPlotFieldWellsOutputTypeDef",
     "BoxPlotFieldWellsTypeDef",
+    "ComboChartFieldWellsOutputTypeDef",
     "ComboChartFieldWellsTypeDef",
+    "FilledMapFieldWellsOutputTypeDef",
     "FilledMapFieldWellsTypeDef",
+    "FunnelChartFieldWellsOutputTypeDef",
     "FunnelChartFieldWellsTypeDef",
+    "GaugeChartConfigurationOutputTypeDef",
     "GaugeChartConfigurationTypeDef",
+    "GeospatialMapFieldWellsOutputTypeDef",
     "GeospatialMapFieldWellsTypeDef",
+    "HeatMapFieldWellsOutputTypeDef",
     "HeatMapFieldWellsTypeDef",
+    "HistogramFieldWellsOutputTypeDef",
     "HistogramFieldWellsTypeDef",
+    "KPIConfigurationOutputTypeDef",
     "KPIConfigurationTypeDef",
+    "LineChartFieldWellsOutputTypeDef",
     "LineChartFieldWellsTypeDef",
+    "PieChartFieldWellsOutputTypeDef",
     "PieChartFieldWellsTypeDef",
+    "PivotTableFieldWellsOutputTypeDef",
     "PivotTableFieldWellsTypeDef",
+    "RadarChartFieldWellsOutputTypeDef",
     "RadarChartFieldWellsTypeDef",
+    "SankeyDiagramFieldWellsOutputTypeDef",
     "SankeyDiagramFieldWellsTypeDef",
+    "ScatterPlotFieldWellsOutputTypeDef",
     "ScatterPlotFieldWellsTypeDef",
     "ComputationTypeDef",
+    "TreeMapFieldWellsOutputTypeDef",
     "TreeMapFieldWellsTypeDef",
+    "WaterfallChartFieldWellsOutputTypeDef",
     "WaterfallChartFieldWellsTypeDef",
+    "WordCloudFieldWellsOutputTypeDef",
     "WordCloudFieldWellsTypeDef",
+    "TableFieldWellsOutputTypeDef",
     "TableFieldWellsTypeDef",
     "LayoutConfigurationOutputTypeDef",
     "LayoutConfigurationTypeDef",
     "BarChartConfigurationOutputTypeDef",
-    "BoxPlotChartConfigurationOutputTypeDef",
-    "ComboChartConfigurationOutputTypeDef",
-    "FilledMapConfigurationOutputTypeDef",
-    "FunnelChartConfigurationOutputTypeDef",
-    "GaugeChartVisualOutputTypeDef",
-    "GeospatialMapConfigurationOutputTypeDef",
-    "HeatMapConfigurationOutputTypeDef",
-    "HistogramConfigurationOutputTypeDef",
-    "KPIVisualOutputTypeDef",
-    "LineChartConfigurationOutputTypeDef",
-    "PieChartConfigurationOutputTypeDef",
-    "PivotTableConfigurationOutputTypeDef",
-    "RadarChartConfigurationOutputTypeDef",
-    "SankeyDiagramChartConfigurationOutputTypeDef",
-    "ScatterPlotConfigurationOutputTypeDef",
-    "InsightConfigurationOutputTypeDef",
-    "TreeMapConfigurationOutputTypeDef",
-    "WaterfallChartConfigurationOutputTypeDef",
-    "WordCloudChartConfigurationOutputTypeDef",
-    "TableConfigurationOutputTypeDef",
     "BarChartConfigurationTypeDef",
+    "BoxPlotChartConfigurationOutputTypeDef",
     "BoxPlotChartConfigurationTypeDef",
+    "ComboChartConfigurationOutputTypeDef",
     "ComboChartConfigurationTypeDef",
+    "FilledMapConfigurationOutputTypeDef",
     "FilledMapConfigurationTypeDef",
+    "FunnelChartConfigurationOutputTypeDef",
     "FunnelChartConfigurationTypeDef",
+    "GaugeChartVisualOutputTypeDef",
     "GaugeChartVisualTypeDef",
+    "GeospatialMapConfigurationOutputTypeDef",
     "GeospatialMapConfigurationTypeDef",
+    "HeatMapConfigurationOutputTypeDef",
     "HeatMapConfigurationTypeDef",
+    "HistogramConfigurationOutputTypeDef",
     "HistogramConfigurationTypeDef",
+    "KPIVisualOutputTypeDef",
     "KPIVisualTypeDef",
+    "LineChartConfigurationOutputTypeDef",
     "LineChartConfigurationTypeDef",
+    "PieChartConfigurationOutputTypeDef",
     "PieChartConfigurationTypeDef",
+    "PivotTableConfigurationOutputTypeDef",
     "PivotTableConfigurationTypeDef",
+    "RadarChartConfigurationOutputTypeDef",
     "RadarChartConfigurationTypeDef",
+    "SankeyDiagramChartConfigurationOutputTypeDef",
     "SankeyDiagramChartConfigurationTypeDef",
+    "ScatterPlotConfigurationOutputTypeDef",
     "ScatterPlotConfigurationTypeDef",
+    "InsightConfigurationOutputTypeDef",
     "InsightConfigurationTypeDef",
+    "TreeMapConfigurationOutputTypeDef",
     "TreeMapConfigurationTypeDef",
+    "WaterfallChartConfigurationOutputTypeDef",
     "WaterfallChartConfigurationTypeDef",
+    "WordCloudChartConfigurationOutputTypeDef",
     "WordCloudChartConfigurationTypeDef",
+    "TableConfigurationOutputTypeDef",
     "TableConfigurationTypeDef",
     "LayoutOutputTypeDef",
     "LayoutTypeDef",
     "BarChartVisualOutputTypeDef",
-    "BoxPlotVisualOutputTypeDef",
-    "ComboChartVisualOutputTypeDef",
-    "FilledMapVisualOutputTypeDef",
-    "FunnelChartVisualOutputTypeDef",
-    "GeospatialMapVisualOutputTypeDef",
-    "HeatMapVisualOutputTypeDef",
-    "HistogramVisualOutputTypeDef",
-    "LineChartVisualOutputTypeDef",
-    "PieChartVisualOutputTypeDef",
-    "PivotTableVisualOutputTypeDef",
-    "RadarChartVisualOutputTypeDef",
-    "SankeyDiagramVisualOutputTypeDef",
-    "ScatterPlotVisualOutputTypeDef",
-    "InsightVisualOutputTypeDef",
-    "TreeMapVisualOutputTypeDef",
-    "WaterfallVisualOutputTypeDef",
-    "WordCloudVisualOutputTypeDef",
-    "TableVisualOutputTypeDef",
     "BarChartVisualTypeDef",
+    "BoxPlotVisualOutputTypeDef",
     "BoxPlotVisualTypeDef",
+    "ComboChartVisualOutputTypeDef",
     "ComboChartVisualTypeDef",
+    "FilledMapVisualOutputTypeDef",
     "FilledMapVisualTypeDef",
+    "FunnelChartVisualOutputTypeDef",
     "FunnelChartVisualTypeDef",
+    "GeospatialMapVisualOutputTypeDef",
     "GeospatialMapVisualTypeDef",
+    "HeatMapVisualOutputTypeDef",
     "HeatMapVisualTypeDef",
+    "HistogramVisualOutputTypeDef",
     "HistogramVisualTypeDef",
+    "LineChartVisualOutputTypeDef",
     "LineChartVisualTypeDef",
+    "PieChartVisualOutputTypeDef",
     "PieChartVisualTypeDef",
+    "PivotTableVisualOutputTypeDef",
     "PivotTableVisualTypeDef",
+    "RadarChartVisualOutputTypeDef",
     "RadarChartVisualTypeDef",
+    "SankeyDiagramVisualOutputTypeDef",
     "SankeyDiagramVisualTypeDef",
+    "ScatterPlotVisualOutputTypeDef",
     "ScatterPlotVisualTypeDef",
+    "InsightVisualOutputTypeDef",
     "InsightVisualTypeDef",
+    "TreeMapVisualOutputTypeDef",
     "TreeMapVisualTypeDef",
+    "WaterfallVisualOutputTypeDef",
     "WaterfallVisualTypeDef",
+    "WordCloudVisualOutputTypeDef",
     "WordCloudVisualTypeDef",
+    "TableVisualOutputTypeDef",
     "TableVisualTypeDef",
     "VisualOutputTypeDef",
     "VisualTypeDef",
     "SheetDefinitionOutputTypeDef",
     "SheetDefinitionTypeDef",
     "AnalysisDefinitionOutputTypeDef",
     "DashboardVersionDefinitionOutputTypeDef",
@@ -1875,23 +1558,14 @@
     "UpdateAnalysisRequestRequestTypeDef",
     "CreateDashboardRequestRequestTypeDef",
     "UpdateDashboardRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
 )
 
-AccountCustomizationOutputTypeDef = TypedDict(
-    "AccountCustomizationOutputTypeDef",
-    {
-        "DefaultTheme": str,
-        "DefaultEmailCustomizationTemplate": str,
-    },
-    total=False,
-)
-
 AccountCustomizationTypeDef = TypedDict(
     "AccountCustomizationTypeDef",
     {
         "DefaultTheme": str,
         "DefaultEmailCustomizationTemplate": str,
     },
     total=False,
@@ -1927,109 +1601,53 @@
     {
         "AssignmentName": str,
         "PolicyArn": str,
     },
     total=False,
 )
 
-AdHocFilteringOptionOutputTypeDef = TypedDict(
-    "AdHocFilteringOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
 AdHocFilteringOptionTypeDef = TypedDict(
     "AdHocFilteringOptionTypeDef",
     {
         "AvailabilityStatus": DashboardBehaviorType,
     },
     total=False,
 )
 
-AttributeAggregationFunctionOutputTypeDef = TypedDict(
-    "AttributeAggregationFunctionOutputTypeDef",
-    {
-        "SimpleAttributeAggregation": Literal["UNIQUE_VALUE"],
-        "ValueForMultipleValues": str,
-    },
-    total=False,
-)
-
 AttributeAggregationFunctionTypeDef = TypedDict(
     "AttributeAggregationFunctionTypeDef",
     {
         "SimpleAttributeAggregation": Literal["UNIQUE_VALUE"],
         "ValueForMultipleValues": str,
     },
     total=False,
 )
 
-ColumnIdentifierOutputTypeDef = TypedDict(
-    "ColumnIdentifierOutputTypeDef",
-    {
-        "DataSetIdentifier": str,
-        "ColumnName": str,
-    },
-)
-
 ColumnIdentifierTypeDef = TypedDict(
     "ColumnIdentifierTypeDef",
     {
         "DataSetIdentifier": str,
         "ColumnName": str,
     },
 )
 
-AmazonElasticsearchParametersOutputTypeDef = TypedDict(
-    "AmazonElasticsearchParametersOutputTypeDef",
-    {
-        "Domain": str,
-    },
-)
-
 AmazonElasticsearchParametersTypeDef = TypedDict(
     "AmazonElasticsearchParametersTypeDef",
     {
         "Domain": str,
     },
 )
 
-AmazonOpenSearchParametersOutputTypeDef = TypedDict(
-    "AmazonOpenSearchParametersOutputTypeDef",
-    {
-        "Domain": str,
-    },
-)
-
 AmazonOpenSearchParametersTypeDef = TypedDict(
     "AmazonOpenSearchParametersTypeDef",
     {
         "Domain": str,
     },
 )
 
-CalculatedFieldOutputTypeDef = TypedDict(
-    "CalculatedFieldOutputTypeDef",
-    {
-        "DataSetIdentifier": str,
-        "Name": str,
-        "Expression": str,
-    },
-)
-
-DataSetIdentifierDeclarationOutputTypeDef = TypedDict(
-    "DataSetIdentifierDeclarationOutputTypeDef",
-    {
-        "Identifier": str,
-        "DataSetArn": str,
-    },
-)
-
 CalculatedFieldTypeDef = TypedDict(
     "CalculatedFieldTypeDef",
     {
         "DataSetIdentifier": str,
         "Name": str,
         "Expression": str,
     },
@@ -2087,23 +1705,14 @@
     {
         "SheetId": str,
         "Name": str,
     },
     total=False,
 )
 
-AnchorDateConfigurationOutputTypeDef = TypedDict(
-    "AnchorDateConfigurationOutputTypeDef",
-    {
-        "AnchorOption": Literal["NOW"],
-        "ParameterName": str,
-    },
-    total=False,
-)
-
 AnchorDateConfigurationTypeDef = TypedDict(
     "AnchorDateConfigurationTypeDef",
     {
         "AnchorOption": Literal["NOW"],
         "ParameterName": str,
     },
     total=False,
@@ -2128,58 +1737,32 @@
 AnonymousUserQSearchBarEmbeddingConfigurationTypeDef = TypedDict(
     "AnonymousUserQSearchBarEmbeddingConfigurationTypeDef",
     {
         "InitialTopicId": str,
     },
 )
 
-ArcAxisDisplayRangeOutputTypeDef = TypedDict(
-    "ArcAxisDisplayRangeOutputTypeDef",
-    {
-        "Min": float,
-        "Max": float,
-    },
-    total=False,
-)
-
 ArcAxisDisplayRangeTypeDef = TypedDict(
     "ArcAxisDisplayRangeTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-ArcConfigurationOutputTypeDef = TypedDict(
-    "ArcConfigurationOutputTypeDef",
-    {
-        "ArcAngle": float,
-        "ArcThickness": ArcThicknessOptionsType,
-    },
-    total=False,
-)
-
 ArcConfigurationTypeDef = TypedDict(
     "ArcConfigurationTypeDef",
     {
         "ArcAngle": float,
         "ArcThickness": ArcThicknessOptionsType,
     },
     total=False,
 )
 
-ArcOptionsOutputTypeDef = TypedDict(
-    "ArcOptionsOutputTypeDef",
-    {
-        "ArcThickness": ArcThicknessType,
-    },
-    total=False,
-)
-
 ArcOptionsTypeDef = TypedDict(
     "ArcOptionsTypeDef",
     {
         "ArcThickness": ArcThicknessType,
     },
     total=False,
 )
@@ -2280,16 +1863,16 @@
 
 class AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef(
     _RequiredAssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef,
     _OptionalAssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef,
 ):
     pass
 
-AssetBundleExportJobResourceIdOverrideConfigurationOutputTypeDef = TypedDict(
-    "AssetBundleExportJobResourceIdOverrideConfigurationOutputTypeDef",
+AssetBundleExportJobResourceIdOverrideConfigurationTypeDef = TypedDict(
+    "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
     {
         "PrefixForAllResources": bool,
     },
     total=False,
 )
 
 _RequiredAssetBundleExportJobThemeOverridePropertiesOutputTypeDef = TypedDict(
@@ -2428,22 +2011,14 @@
 
 class AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef(
     _RequiredAssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef,
     _OptionalAssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef,
 ):
     pass
 
-AssetBundleExportJobResourceIdOverrideConfigurationTypeDef = TypedDict(
-    "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
-    {
-        "PrefixForAllResources": bool,
-    },
-    total=False,
-)
-
 _RequiredAssetBundleExportJobThemeOverridePropertiesTypeDef = TypedDict(
     "_RequiredAssetBundleExportJobThemeOverridePropertiesTypeDef",
     {
         "Properties": Sequence[Literal["Name"]],
     },
 )
 _OptionalAssetBundleExportJobThemeOverridePropertiesTypeDef = TypedDict(
@@ -2499,34 +2074,14 @@
         "AssetBundleExportJobId": str,
         "IncludeAllDependencies": bool,
         "ExportFormat": AssetBundleExportFormatType,
     },
     total=False,
 )
 
-_RequiredAssetBundleImportJobAnalysisOverrideParametersOutputTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobAnalysisOverrideParametersOutputTypeDef",
-    {
-        "AnalysisId": str,
-    },
-)
-_OptionalAssetBundleImportJobAnalysisOverrideParametersOutputTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobAnalysisOverrideParametersOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-class AssetBundleImportJobAnalysisOverrideParametersOutputTypeDef(
-    _RequiredAssetBundleImportJobAnalysisOverrideParametersOutputTypeDef,
-    _OptionalAssetBundleImportJobAnalysisOverrideParametersOutputTypeDef,
-):
-    pass
-
 _RequiredAssetBundleImportJobAnalysisOverrideParametersTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobAnalysisOverrideParametersTypeDef",
     {
         "AnalysisId": str,
     },
 )
 _OptionalAssetBundleImportJobAnalysisOverrideParametersTypeDef = TypedDict(
@@ -2539,34 +2094,14 @@
 
 class AssetBundleImportJobAnalysisOverrideParametersTypeDef(
     _RequiredAssetBundleImportJobAnalysisOverrideParametersTypeDef,
     _OptionalAssetBundleImportJobAnalysisOverrideParametersTypeDef,
 ):
     pass
 
-_RequiredAssetBundleImportJobDashboardOverrideParametersOutputTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobDashboardOverrideParametersOutputTypeDef",
-    {
-        "DashboardId": str,
-    },
-)
-_OptionalAssetBundleImportJobDashboardOverrideParametersOutputTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobDashboardOverrideParametersOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-class AssetBundleImportJobDashboardOverrideParametersOutputTypeDef(
-    _RequiredAssetBundleImportJobDashboardOverrideParametersOutputTypeDef,
-    _OptionalAssetBundleImportJobDashboardOverrideParametersOutputTypeDef,
-):
-    pass
-
 _RequiredAssetBundleImportJobDashboardOverrideParametersTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobDashboardOverrideParametersTypeDef",
     {
         "DashboardId": str,
     },
 )
 _OptionalAssetBundleImportJobDashboardOverrideParametersTypeDef = TypedDict(
@@ -2579,34 +2114,14 @@
 
 class AssetBundleImportJobDashboardOverrideParametersTypeDef(
     _RequiredAssetBundleImportJobDashboardOverrideParametersTypeDef,
     _OptionalAssetBundleImportJobDashboardOverrideParametersTypeDef,
 ):
     pass
 
-_RequiredAssetBundleImportJobDataSetOverrideParametersOutputTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobDataSetOverrideParametersOutputTypeDef",
-    {
-        "DataSetId": str,
-    },
-)
-_OptionalAssetBundleImportJobDataSetOverrideParametersOutputTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobDataSetOverrideParametersOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-class AssetBundleImportJobDataSetOverrideParametersOutputTypeDef(
-    _RequiredAssetBundleImportJobDataSetOverrideParametersOutputTypeDef,
-    _OptionalAssetBundleImportJobDataSetOverrideParametersOutputTypeDef,
-):
-    pass
-
 _RequiredAssetBundleImportJobDataSetOverrideParametersTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobDataSetOverrideParametersTypeDef",
     {
         "DataSetId": str,
     },
 )
 _OptionalAssetBundleImportJobDataSetOverrideParametersTypeDef = TypedDict(
@@ -2619,45 +2134,22 @@
 
 class AssetBundleImportJobDataSetOverrideParametersTypeDef(
     _RequiredAssetBundleImportJobDataSetOverrideParametersTypeDef,
     _OptionalAssetBundleImportJobDataSetOverrideParametersTypeDef,
 ):
     pass
 
-AssetBundleImportJobDataSourceCredentialPairOutputTypeDef = TypedDict(
-    "AssetBundleImportJobDataSourceCredentialPairOutputTypeDef",
-    {
-        "Username": str,
-        "Password": str,
-    },
-)
-
 AssetBundleImportJobDataSourceCredentialPairTypeDef = TypedDict(
     "AssetBundleImportJobDataSourceCredentialPairTypeDef",
     {
         "Username": str,
         "Password": str,
     },
 )
 
-SslPropertiesOutputTypeDef = TypedDict(
-    "SslPropertiesOutputTypeDef",
-    {
-        "DisableSsl": bool,
-    },
-    total=False,
-)
-
-VpcConnectionPropertiesOutputTypeDef = TypedDict(
-    "VpcConnectionPropertiesOutputTypeDef",
-    {
-        "VpcConnectionArn": str,
-    },
-)
-
 SslPropertiesTypeDef = TypedDict(
     "SslPropertiesTypeDef",
     {
         "DisableSsl": bool,
     },
     total=False,
 )
@@ -2696,39 +2188,39 @@
 
 class AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef(
     _RequiredAssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef,
     _OptionalAssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef,
 ):
     pass
 
-AssetBundleImportJobResourceIdOverrideConfigurationOutputTypeDef = TypedDict(
-    "AssetBundleImportJobResourceIdOverrideConfigurationOutputTypeDef",
+AssetBundleImportJobResourceIdOverrideConfigurationTypeDef = TypedDict(
+    "AssetBundleImportJobResourceIdOverrideConfigurationTypeDef",
     {
         "PrefixForAllResources": str,
     },
     total=False,
 )
 
-_RequiredAssetBundleImportJobThemeOverrideParametersOutputTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobThemeOverrideParametersOutputTypeDef",
+_RequiredAssetBundleImportJobThemeOverrideParametersTypeDef = TypedDict(
+    "_RequiredAssetBundleImportJobThemeOverrideParametersTypeDef",
     {
         "ThemeId": str,
     },
 )
-_OptionalAssetBundleImportJobThemeOverrideParametersOutputTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobThemeOverrideParametersOutputTypeDef",
+_OptionalAssetBundleImportJobThemeOverrideParametersTypeDef = TypedDict(
+    "_OptionalAssetBundleImportJobThemeOverrideParametersTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-class AssetBundleImportJobThemeOverrideParametersOutputTypeDef(
-    _RequiredAssetBundleImportJobThemeOverrideParametersOutputTypeDef,
-    _OptionalAssetBundleImportJobThemeOverrideParametersOutputTypeDef,
+class AssetBundleImportJobThemeOverrideParametersTypeDef(
+    _RequiredAssetBundleImportJobThemeOverrideParametersTypeDef,
+    _OptionalAssetBundleImportJobThemeOverrideParametersTypeDef,
 ):
     pass
 
 _RequiredAssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef",
     {
         "VPCConnectionId": str,
@@ -2769,42 +2261,14 @@
 
 class AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef(
     _RequiredAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
     _OptionalAssetBundleImportJobRefreshScheduleOverrideParametersTypeDef,
 ):
     pass
 
-AssetBundleImportJobResourceIdOverrideConfigurationTypeDef = TypedDict(
-    "AssetBundleImportJobResourceIdOverrideConfigurationTypeDef",
-    {
-        "PrefixForAllResources": str,
-    },
-    total=False,
-)
-
-_RequiredAssetBundleImportJobThemeOverrideParametersTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobThemeOverrideParametersTypeDef",
-    {
-        "ThemeId": str,
-    },
-)
-_OptionalAssetBundleImportJobThemeOverrideParametersTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobThemeOverrideParametersTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-class AssetBundleImportJobThemeOverrideParametersTypeDef(
-    _RequiredAssetBundleImportJobThemeOverrideParametersTypeDef,
-    _OptionalAssetBundleImportJobThemeOverrideParametersTypeDef,
-):
-    pass
-
 _RequiredAssetBundleImportJobVPCConnectionOverrideParametersTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
     {
         "VPCConnectionId": str,
     },
 )
 _OptionalAssetBundleImportJobVPCConnectionOverrideParametersTypeDef = TypedDict(
@@ -2851,193 +2315,99 @@
     {
         "Body": Union[str, bytes, IO[Any], StreamingBody],
         "S3Uri": str,
     },
     total=False,
 )
 
-AthenaParametersOutputTypeDef = TypedDict(
-    "AthenaParametersOutputTypeDef",
-    {
-        "WorkGroup": str,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
 AthenaParametersTypeDef = TypedDict(
     "AthenaParametersTypeDef",
     {
         "WorkGroup": str,
         "RoleArn": str,
     },
     total=False,
 )
 
-AuroraParametersOutputTypeDef = TypedDict(
-    "AuroraParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
 AuroraParametersTypeDef = TypedDict(
     "AuroraParametersTypeDef",
     {
         "Host": str,
         "Port": int,
         "Database": str,
     },
 )
 
-AuroraPostgreSqlParametersOutputTypeDef = TypedDict(
-    "AuroraPostgreSqlParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
 AuroraPostgreSqlParametersTypeDef = TypedDict(
     "AuroraPostgreSqlParametersTypeDef",
     {
         "Host": str,
         "Port": int,
         "Database": str,
     },
 )
 
-AwsIotAnalyticsParametersOutputTypeDef = TypedDict(
-    "AwsIotAnalyticsParametersOutputTypeDef",
-    {
-        "DataSetName": str,
-    },
-)
-
 AwsIotAnalyticsParametersTypeDef = TypedDict(
     "AwsIotAnalyticsParametersTypeDef",
     {
         "DataSetName": str,
     },
 )
 
-DateAxisOptionsOutputTypeDef = TypedDict(
-    "DateAxisOptionsOutputTypeDef",
-    {
-        "MissingDateVisibility": VisibilityType,
-    },
-    total=False,
-)
-
 DateAxisOptionsTypeDef = TypedDict(
     "DateAxisOptionsTypeDef",
     {
         "MissingDateVisibility": VisibilityType,
     },
     total=False,
 )
 
-AxisDisplayMinMaxRangeOutputTypeDef = TypedDict(
-    "AxisDisplayMinMaxRangeOutputTypeDef",
-    {
-        "Minimum": float,
-        "Maximum": float,
-    },
-    total=False,
-)
-
 AxisDisplayMinMaxRangeTypeDef = TypedDict(
     "AxisDisplayMinMaxRangeTypeDef",
     {
         "Minimum": float,
         "Maximum": float,
     },
     total=False,
 )
 
-AxisLinearScaleOutputTypeDef = TypedDict(
-    "AxisLinearScaleOutputTypeDef",
-    {
-        "StepCount": int,
-        "StepSize": float,
-    },
-    total=False,
-)
-
 AxisLinearScaleTypeDef = TypedDict(
     "AxisLinearScaleTypeDef",
     {
         "StepCount": int,
         "StepSize": float,
     },
     total=False,
 )
 
-AxisLogarithmicScaleOutputTypeDef = TypedDict(
-    "AxisLogarithmicScaleOutputTypeDef",
-    {
-        "Base": float,
-    },
-    total=False,
-)
-
 AxisLogarithmicScaleTypeDef = TypedDict(
     "AxisLogarithmicScaleTypeDef",
     {
         "Base": float,
     },
     total=False,
 )
 
-ItemsLimitConfigurationOutputTypeDef = TypedDict(
-    "ItemsLimitConfigurationOutputTypeDef",
-    {
-        "ItemsLimit": int,
-        "OtherCategories": OtherCategoriesType,
-    },
-    total=False,
-)
-
 ItemsLimitConfigurationTypeDef = TypedDict(
     "ItemsLimitConfigurationTypeDef",
     {
         "ItemsLimit": int,
         "OtherCategories": OtherCategoriesType,
     },
     total=False,
 )
 
-BinCountOptionsOutputTypeDef = TypedDict(
-    "BinCountOptionsOutputTypeDef",
-    {
-        "Value": int,
-    },
-    total=False,
-)
-
 BinCountOptionsTypeDef = TypedDict(
     "BinCountOptionsTypeDef",
     {
         "Value": int,
     },
     total=False,
 )
 
-BinWidthOptionsOutputTypeDef = TypedDict(
-    "BinWidthOptionsOutputTypeDef",
-    {
-        "Value": float,
-        "BinCountLimit": int,
-    },
-    total=False,
-)
-
 BinWidthOptionsTypeDef = TypedDict(
     "BinWidthOptionsTypeDef",
     {
         "Value": float,
         "BinCountLimit": int,
     },
     total=False,
@@ -3046,88 +2416,47 @@
 BookmarksConfigurationsTypeDef = TypedDict(
     "BookmarksConfigurationsTypeDef",
     {
         "Enabled": bool,
     },
 )
 
-BorderStyleOutputTypeDef = TypedDict(
-    "BorderStyleOutputTypeDef",
-    {
-        "Show": bool,
-    },
-    total=False,
-)
-
 BorderStyleTypeDef = TypedDict(
     "BorderStyleTypeDef",
     {
         "Show": bool,
     },
     total=False,
 )
 
-BoxPlotStyleOptionsOutputTypeDef = TypedDict(
-    "BoxPlotStyleOptionsOutputTypeDef",
-    {
-        "FillStyle": BoxPlotFillStyleType,
-    },
-    total=False,
-)
-
 BoxPlotStyleOptionsTypeDef = TypedDict(
     "BoxPlotStyleOptionsTypeDef",
     {
         "FillStyle": BoxPlotFillStyleType,
     },
     total=False,
 )
 
-PaginationConfigurationOutputTypeDef = TypedDict(
-    "PaginationConfigurationOutputTypeDef",
-    {
-        "PageSize": int,
-        "PageNumber": int,
-    },
-)
-
 PaginationConfigurationTypeDef = TypedDict(
     "PaginationConfigurationTypeDef",
     {
         "PageSize": int,
         "PageNumber": int,
     },
 )
 
-CalculatedColumnOutputTypeDef = TypedDict(
-    "CalculatedColumnOutputTypeDef",
-    {
-        "ColumnName": str,
-        "ColumnId": str,
-        "Expression": str,
-    },
-)
-
 CalculatedColumnTypeDef = TypedDict(
     "CalculatedColumnTypeDef",
     {
         "ColumnName": str,
         "ColumnId": str,
         "Expression": str,
     },
 )
 
-CalculatedMeasureFieldOutputTypeDef = TypedDict(
-    "CalculatedMeasureFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Expression": str,
-    },
-)
-
 CalculatedMeasureFieldTypeDef = TypedDict(
     "CalculatedMeasureFieldTypeDef",
     {
         "FieldId": str,
         "Expression": str,
     },
 )
@@ -3148,34 +2477,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredCastColumnTypeOperationOutputTypeDef = TypedDict(
-    "_RequiredCastColumnTypeOperationOutputTypeDef",
-    {
-        "ColumnName": str,
-        "NewColumnType": ColumnDataTypeType,
-    },
-)
-_OptionalCastColumnTypeOperationOutputTypeDef = TypedDict(
-    "_OptionalCastColumnTypeOperationOutputTypeDef",
-    {
-        "Format": str,
-    },
-    total=False,
-)
-
-class CastColumnTypeOperationOutputTypeDef(
-    _RequiredCastColumnTypeOperationOutputTypeDef, _OptionalCastColumnTypeOperationOutputTypeDef
-):
-    pass
-
 _RequiredCastColumnTypeOperationTypeDef = TypedDict(
     "_RequiredCastColumnTypeOperationTypeDef",
     {
         "ColumnName": str,
         "NewColumnType": ColumnDataTypeType,
     },
 )
@@ -3188,33 +2497,33 @@
 )
 
 class CastColumnTypeOperationTypeDef(
     _RequiredCastColumnTypeOperationTypeDef, _OptionalCastColumnTypeOperationTypeDef
 ):
     pass
 
-_RequiredCustomFilterConfigurationOutputTypeDef = TypedDict(
-    "_RequiredCustomFilterConfigurationOutputTypeDef",
+_RequiredCustomFilterConfigurationTypeDef = TypedDict(
+    "_RequiredCustomFilterConfigurationTypeDef",
     {
         "MatchOperator": CategoryFilterMatchOperatorType,
         "NullOption": FilterNullOptionType,
     },
 )
-_OptionalCustomFilterConfigurationOutputTypeDef = TypedDict(
-    "_OptionalCustomFilterConfigurationOutputTypeDef",
+_OptionalCustomFilterConfigurationTypeDef = TypedDict(
+    "_OptionalCustomFilterConfigurationTypeDef",
     {
         "CategoryValue": str,
         "SelectAllOptions": Literal["FILTER_ALL_VALUES"],
         "ParameterName": str,
     },
     total=False,
 )
 
-class CustomFilterConfigurationOutputTypeDef(
-    _RequiredCustomFilterConfigurationOutputTypeDef, _OptionalCustomFilterConfigurationOutputTypeDef
+class CustomFilterConfigurationTypeDef(
+    _RequiredCustomFilterConfigurationTypeDef, _OptionalCustomFilterConfigurationTypeDef
 ):
     pass
 
 _RequiredCustomFilterListConfigurationOutputTypeDef = TypedDict(
     "_RequiredCustomFilterListConfigurationOutputTypeDef",
     {
         "MatchOperator": CategoryFilterMatchOperatorType,
@@ -3252,36 +2561,14 @@
 )
 
 class FilterListConfigurationOutputTypeDef(
     _RequiredFilterListConfigurationOutputTypeDef, _OptionalFilterListConfigurationOutputTypeDef
 ):
     pass
 
-_RequiredCustomFilterConfigurationTypeDef = TypedDict(
-    "_RequiredCustomFilterConfigurationTypeDef",
-    {
-        "MatchOperator": CategoryFilterMatchOperatorType,
-        "NullOption": FilterNullOptionType,
-    },
-)
-_OptionalCustomFilterConfigurationTypeDef = TypedDict(
-    "_OptionalCustomFilterConfigurationTypeDef",
-    {
-        "CategoryValue": str,
-        "SelectAllOptions": Literal["FILTER_ALL_VALUES"],
-        "ParameterName": str,
-    },
-    total=False,
-)
-
-class CustomFilterConfigurationTypeDef(
-    _RequiredCustomFilterConfigurationTypeDef, _OptionalCustomFilterConfigurationTypeDef
-):
-    pass
-
 _RequiredCustomFilterListConfigurationTypeDef = TypedDict(
     "_RequiredCustomFilterListConfigurationTypeDef",
     {
         "MatchOperator": CategoryFilterMatchOperatorType,
         "NullOption": FilterNullOptionType,
     },
 )
@@ -3333,22 +2620,14 @@
     {
         "CellValue": str,
         "Synonyms": Sequence[str],
     },
     total=False,
 )
 
-SimpleClusterMarkerOutputTypeDef = TypedDict(
-    "SimpleClusterMarkerOutputTypeDef",
-    {
-        "Color": str,
-    },
-    total=False,
-)
-
 SimpleClusterMarkerTypeDef = TypedDict(
     "SimpleClusterMarkerTypeDef",
     {
         "Color": str,
     },
     total=False,
 )
@@ -3365,52 +2644,23 @@
     "CollectiveConstantTypeDef",
     {
         "ValueList": Sequence[str],
     },
     total=False,
 )
 
-DataColorOutputTypeDef = TypedDict(
-    "DataColorOutputTypeDef",
-    {
-        "Color": str,
-        "DataValue": float,
-    },
-    total=False,
-)
-
 DataColorTypeDef = TypedDict(
     "DataColorTypeDef",
     {
         "Color": str,
         "DataValue": float,
     },
     total=False,
 )
 
-_RequiredCustomColorOutputTypeDef = TypedDict(
-    "_RequiredCustomColorOutputTypeDef",
-    {
-        "Color": str,
-    },
-)
-_OptionalCustomColorOutputTypeDef = TypedDict(
-    "_OptionalCustomColorOutputTypeDef",
-    {
-        "FieldValue": str,
-        "SpecialValue": SpecialValueType,
-    },
-    total=False,
-)
-
-class CustomColorOutputTypeDef(
-    _RequiredCustomColorOutputTypeDef, _OptionalCustomColorOutputTypeDef
-):
-    pass
-
 _RequiredCustomColorTypeDef = TypedDict(
     "_RequiredCustomColorTypeDef",
     {
         "Color": str,
     },
 )
 _OptionalCustomColorTypeDef = TypedDict(
@@ -3421,38 +2671,22 @@
     },
     total=False,
 )
 
 class CustomColorTypeDef(_RequiredCustomColorTypeDef, _OptionalCustomColorTypeDef):
     pass
 
-ColumnDescriptionOutputTypeDef = TypedDict(
-    "ColumnDescriptionOutputTypeDef",
-    {
-        "Text": str,
-    },
-    total=False,
-)
-
 ColumnDescriptionTypeDef = TypedDict(
     "ColumnDescriptionTypeDef",
     {
         "Text": str,
     },
     total=False,
 )
 
-ColumnGroupColumnSchemaOutputTypeDef = TypedDict(
-    "ColumnGroupColumnSchemaOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
 ColumnGroupColumnSchemaTypeDef = TypedDict(
     "ColumnGroupColumnSchemaTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -3511,24 +2745,14 @@
     {
         "Principals": Sequence[str],
         "ColumnNames": Sequence[str],
     },
     total=False,
 )
 
-ColumnSchemaOutputTypeDef = TypedDict(
-    "ColumnSchemaOutputTypeDef",
-    {
-        "Name": str,
-        "DataType": str,
-        "GeographicRole": str,
-    },
-    total=False,
-)
-
 ColumnSchemaTypeDef = TypedDict(
     "ColumnSchemaTypeDef",
     {
         "Name": str,
         "DataType": str,
         "GeographicRole": str,
     },
@@ -3551,34 +2775,14 @@
         "UseOrdering": ColumnOrderingTypeType,
         "SpecifedOrder": Sequence[str],
         "TreatUndefinedSpecifiedValues": UndefinedSpecifiedValueTypeType,
     },
     total=False,
 )
 
-_RequiredConditionalFormattingSolidColorOutputTypeDef = TypedDict(
-    "_RequiredConditionalFormattingSolidColorOutputTypeDef",
-    {
-        "Expression": str,
-    },
-)
-_OptionalConditionalFormattingSolidColorOutputTypeDef = TypedDict(
-    "_OptionalConditionalFormattingSolidColorOutputTypeDef",
-    {
-        "Color": str,
-    },
-    total=False,
-)
-
-class ConditionalFormattingSolidColorOutputTypeDef(
-    _RequiredConditionalFormattingSolidColorOutputTypeDef,
-    _OptionalConditionalFormattingSolidColorOutputTypeDef,
-):
-    pass
-
 _RequiredConditionalFormattingSolidColorTypeDef = TypedDict(
     "_RequiredConditionalFormattingSolidColorTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalConditionalFormattingSolidColorTypeDef = TypedDict(
@@ -3590,31 +2794,14 @@
 )
 
 class ConditionalFormattingSolidColorTypeDef(
     _RequiredConditionalFormattingSolidColorTypeDef, _OptionalConditionalFormattingSolidColorTypeDef
 ):
     pass
 
-ConditionalFormattingCustomIconOptionsOutputTypeDef = TypedDict(
-    "ConditionalFormattingCustomIconOptionsOutputTypeDef",
-    {
-        "Icon": IconType,
-        "UnicodeIcon": str,
-    },
-    total=False,
-)
-
-ConditionalFormattingIconDisplayConfigurationOutputTypeDef = TypedDict(
-    "ConditionalFormattingIconDisplayConfigurationOutputTypeDef",
-    {
-        "IconDisplayOption": Literal["ICON_ONLY"],
-    },
-    total=False,
-)
-
 ConditionalFormattingCustomIconOptionsTypeDef = TypedDict(
     "ConditionalFormattingCustomIconOptionsTypeDef",
     {
         "Icon": IconType,
         "UnicodeIcon": str,
     },
     total=False,
@@ -3624,34 +2811,14 @@
     "ConditionalFormattingIconDisplayConfigurationTypeDef",
     {
         "IconDisplayOption": Literal["ICON_ONLY"],
     },
     total=False,
 )
 
-_RequiredConditionalFormattingIconSetOutputTypeDef = TypedDict(
-    "_RequiredConditionalFormattingIconSetOutputTypeDef",
-    {
-        "Expression": str,
-    },
-)
-_OptionalConditionalFormattingIconSetOutputTypeDef = TypedDict(
-    "_OptionalConditionalFormattingIconSetOutputTypeDef",
-    {
-        "IconSetType": ConditionalFormattingIconSetTypeType,
-    },
-    total=False,
-)
-
-class ConditionalFormattingIconSetOutputTypeDef(
-    _RequiredConditionalFormattingIconSetOutputTypeDef,
-    _OptionalConditionalFormattingIconSetOutputTypeDef,
-):
-    pass
-
 _RequiredConditionalFormattingIconSetTypeDef = TypedDict(
     "_RequiredConditionalFormattingIconSetTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalConditionalFormattingIconSetTypeDef = TypedDict(
@@ -3941,35 +3108,14 @@
 )
 
 class TopicRefreshScheduleTypeDef(
     _RequiredTopicRefreshScheduleTypeDef, _OptionalTopicRefreshScheduleTypeDef
 ):
     pass
 
-DecimalPlacesConfigurationOutputTypeDef = TypedDict(
-    "DecimalPlacesConfigurationOutputTypeDef",
-    {
-        "DecimalPlaces": int,
-    },
-)
-
-NegativeValueConfigurationOutputTypeDef = TypedDict(
-    "NegativeValueConfigurationOutputTypeDef",
-    {
-        "DisplayMode": NegativeValueDisplayModeType,
-    },
-)
-
-NullValueFormatConfigurationOutputTypeDef = TypedDict(
-    "NullValueFormatConfigurationOutputTypeDef",
-    {
-        "NullString": str,
-    },
-)
-
 DecimalPlacesConfigurationTypeDef = TypedDict(
     "DecimalPlacesConfigurationTypeDef",
     {
         "DecimalPlaces": int,
     },
 )
 
@@ -3983,71 +3129,39 @@
 NullValueFormatConfigurationTypeDef = TypedDict(
     "NullValueFormatConfigurationTypeDef",
     {
         "NullString": str,
     },
 )
 
-LocalNavigationConfigurationOutputTypeDef = TypedDict(
-    "LocalNavigationConfigurationOutputTypeDef",
-    {
-        "TargetSheetId": str,
-    },
-)
-
 LocalNavigationConfigurationTypeDef = TypedDict(
     "LocalNavigationConfigurationTypeDef",
     {
         "TargetSheetId": str,
     },
 )
 
-CustomActionURLOperationOutputTypeDef = TypedDict(
-    "CustomActionURLOperationOutputTypeDef",
-    {
-        "URLTemplate": str,
-        "URLTarget": URLTargetConfigurationType,
-    },
-)
-
 CustomActionURLOperationTypeDef = TypedDict(
     "CustomActionURLOperationTypeDef",
     {
         "URLTemplate": str,
         "URLTarget": URLTargetConfigurationType,
     },
 )
 
-CustomContentConfigurationOutputTypeDef = TypedDict(
-    "CustomContentConfigurationOutputTypeDef",
-    {
-        "ContentUrl": str,
-        "ContentType": CustomContentTypeType,
-        "ImageScaling": CustomContentImageScalingConfigurationType,
-    },
-    total=False,
-)
-
 CustomContentConfigurationTypeDef = TypedDict(
     "CustomContentConfigurationTypeDef",
     {
         "ContentUrl": str,
         "ContentType": CustomContentTypeType,
         "ImageScaling": CustomContentImageScalingConfigurationType,
     },
     total=False,
 )
 
-CustomNarrativeOptionsOutputTypeDef = TypedDict(
-    "CustomNarrativeOptionsOutputTypeDef",
-    {
-        "Narrative": str,
-    },
-)
-
 CustomNarrativeOptionsTypeDef = TypedDict(
     "CustomNarrativeOptionsTypeDef",
     {
         "Narrative": str,
     },
 )
 
@@ -4069,102 +3183,22 @@
         "IntegerValues": Sequence[int],
         "DecimalValues": Sequence[float],
         "DateTimeValues": Sequence[Union[datetime, str]],
     },
     total=False,
 )
 
-InputColumnOutputTypeDef = TypedDict(
-    "InputColumnOutputTypeDef",
-    {
-        "Name": str,
-        "Type": InputColumnDataTypeType,
-    },
-)
-
 InputColumnTypeDef = TypedDict(
     "InputColumnTypeDef",
     {
         "Name": str,
         "Type": InputColumnDataTypeType,
     },
 )
 
-DataPointDrillUpDownOptionOutputTypeDef = TypedDict(
-    "DataPointDrillUpDownOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-DataPointMenuLabelOptionOutputTypeDef = TypedDict(
-    "DataPointMenuLabelOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-DataPointTooltipOptionOutputTypeDef = TypedDict(
-    "DataPointTooltipOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-ExportToCSVOptionOutputTypeDef = TypedDict(
-    "ExportToCSVOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-ExportWithHiddenFieldsOptionOutputTypeDef = TypedDict(
-    "ExportWithHiddenFieldsOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-SheetControlsOptionOutputTypeDef = TypedDict(
-    "SheetControlsOptionOutputTypeDef",
-    {
-        "VisibilityState": DashboardUIStateType,
-    },
-    total=False,
-)
-
-SheetLayoutElementMaximizationOptionOutputTypeDef = TypedDict(
-    "SheetLayoutElementMaximizationOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-VisualAxisSortOptionOutputTypeDef = TypedDict(
-    "VisualAxisSortOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
-VisualMenuOptionOutputTypeDef = TypedDict(
-    "VisualMenuOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
 DataPointDrillUpDownOptionTypeDef = TypedDict(
     "DataPointDrillUpDownOptionTypeDef",
     {
         "AvailabilityStatus": DashboardBehaviorType,
     },
     total=False,
 )
@@ -4276,68 +3310,31 @@
         "Status": ResourceStatusType,
         "SourceEntityArn": str,
         "Description": str,
     },
     total=False,
 )
 
-ExportHiddenFieldsOptionOutputTypeDef = TypedDict(
-    "ExportHiddenFieldsOptionOutputTypeDef",
-    {
-        "AvailabilityStatus": DashboardBehaviorType,
-    },
-    total=False,
-)
-
 ExportHiddenFieldsOptionTypeDef = TypedDict(
     "ExportHiddenFieldsOptionTypeDef",
     {
         "AvailabilityStatus": DashboardBehaviorType,
     },
     total=False,
 )
 
-DataAggregationOutputTypeDef = TypedDict(
-    "DataAggregationOutputTypeDef",
-    {
-        "DatasetRowDateGranularity": TopicTimeGranularityType,
-        "DefaultDateColumnName": str,
-    },
-    total=False,
-)
-
 DataAggregationTypeDef = TypedDict(
     "DataAggregationTypeDef",
     {
         "DatasetRowDateGranularity": TopicTimeGranularityType,
         "DefaultDateColumnName": str,
     },
     total=False,
 )
 
-_RequiredDataBarsOptionsOutputTypeDef = TypedDict(
-    "_RequiredDataBarsOptionsOutputTypeDef",
-    {
-        "FieldId": str,
-    },
-)
-_OptionalDataBarsOptionsOutputTypeDef = TypedDict(
-    "_OptionalDataBarsOptionsOutputTypeDef",
-    {
-        "PositiveColor": str,
-        "NegativeColor": str,
-    },
-    total=False,
-)
-
-class DataBarsOptionsOutputTypeDef(
-    _RequiredDataBarsOptionsOutputTypeDef, _OptionalDataBarsOptionsOutputTypeDef
-):
-    pass
-
 _RequiredDataBarsOptionsTypeDef = TypedDict(
     "_RequiredDataBarsOptionsTypeDef",
     {
         "FieldId": str,
     },
 )
 _OptionalDataBarsOptionsTypeDef = TypedDict(
@@ -4368,57 +3365,14 @@
         "Colors": Sequence[str],
         "MinMaxGradient": Sequence[str],
         "EmptyFillColor": str,
     },
     total=False,
 )
 
-DataPathLabelTypeOutputTypeDef = TypedDict(
-    "DataPathLabelTypeOutputTypeDef",
-    {
-        "FieldId": str,
-        "FieldValue": str,
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-FieldLabelTypeOutputTypeDef = TypedDict(
-    "FieldLabelTypeOutputTypeDef",
-    {
-        "FieldId": str,
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-MaximumLabelTypeOutputTypeDef = TypedDict(
-    "MaximumLabelTypeOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-MinimumLabelTypeOutputTypeDef = TypedDict(
-    "MinimumLabelTypeOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-RangeEndsLabelTypeOutputTypeDef = TypedDict(
-    "RangeEndsLabelTypeOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 DataPathLabelTypeTypeDef = TypedDict(
     "DataPathLabelTypeTypeDef",
     {
         "FieldId": str,
         "FieldValue": str,
         "Visibility": VisibilityType,
     },
@@ -4454,22 +3408,14 @@
     "RangeEndsLabelTypeTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
 
-DataPathValueOutputTypeDef = TypedDict(
-    "DataPathValueOutputTypeDef",
-    {
-        "FieldId": str,
-        "FieldValue": str,
-    },
-)
-
 DataPathValueTypeDef = TypedDict(
     "DataPathValueTypeDef",
     {
         "FieldId": str,
         "FieldValue": str,
     },
 )
@@ -4479,45 +3425,14 @@
     {
         "Operator": FilterOperatorType,
         "Name": DataSetFilterAttributeType,
         "Value": str,
     },
 )
 
-_RequiredRowLevelPermissionDataSetOutputTypeDef = TypedDict(
-    "_RequiredRowLevelPermissionDataSetOutputTypeDef",
-    {
-        "Arn": str,
-        "PermissionPolicy": RowLevelPermissionPolicyType,
-    },
-)
-_OptionalRowLevelPermissionDataSetOutputTypeDef = TypedDict(
-    "_OptionalRowLevelPermissionDataSetOutputTypeDef",
-    {
-        "Namespace": str,
-        "FormatVersion": RowLevelPermissionFormatVersionType,
-        "Status": StatusType,
-    },
-    total=False,
-)
-
-class RowLevelPermissionDataSetOutputTypeDef(
-    _RequiredRowLevelPermissionDataSetOutputTypeDef, _OptionalRowLevelPermissionDataSetOutputTypeDef
-):
-    pass
-
-DataSetUsageConfigurationOutputTypeDef = TypedDict(
-    "DataSetUsageConfigurationOutputTypeDef",
-    {
-        "DisableUseAsDirectQuerySource": bool,
-        "DisableUseAsImportedSource": bool,
-    },
-    total=False,
-)
-
 FieldFolderOutputTypeDef = TypedDict(
     "FieldFolderOutputTypeDef",
     {
         "description": str,
         "columns": List[str],
     },
     total=False,
@@ -4538,162 +3453,14 @@
     {
         "Type": DataSourceErrorInfoTypeType,
         "Message": str,
     },
     total=False,
 )
 
-DatabricksParametersOutputTypeDef = TypedDict(
-    "DatabricksParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "SqlEndpointPath": str,
-    },
-)
-
-ExasolParametersOutputTypeDef = TypedDict(
-    "ExasolParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-    },
-)
-
-JiraParametersOutputTypeDef = TypedDict(
-    "JiraParametersOutputTypeDef",
-    {
-        "SiteBaseUrl": str,
-    },
-)
-
-MariaDbParametersOutputTypeDef = TypedDict(
-    "MariaDbParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
-MySqlParametersOutputTypeDef = TypedDict(
-    "MySqlParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
-OracleParametersOutputTypeDef = TypedDict(
-    "OracleParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
-PostgreSqlParametersOutputTypeDef = TypedDict(
-    "PostgreSqlParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
-PrestoParametersOutputTypeDef = TypedDict(
-    "PrestoParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Catalog": str,
-    },
-)
-
-RdsParametersOutputTypeDef = TypedDict(
-    "RdsParametersOutputTypeDef",
-    {
-        "InstanceId": str,
-        "Database": str,
-    },
-)
-
-_RequiredRedshiftParametersOutputTypeDef = TypedDict(
-    "_RequiredRedshiftParametersOutputTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalRedshiftParametersOutputTypeDef = TypedDict(
-    "_OptionalRedshiftParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "ClusterId": str,
-    },
-    total=False,
-)
-
-class RedshiftParametersOutputTypeDef(
-    _RequiredRedshiftParametersOutputTypeDef, _OptionalRedshiftParametersOutputTypeDef
-):
-    pass
-
-ServiceNowParametersOutputTypeDef = TypedDict(
-    "ServiceNowParametersOutputTypeDef",
-    {
-        "SiteBaseUrl": str,
-    },
-)
-
-SnowflakeParametersOutputTypeDef = TypedDict(
-    "SnowflakeParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Database": str,
-        "Warehouse": str,
-    },
-)
-
-SparkParametersOutputTypeDef = TypedDict(
-    "SparkParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-    },
-)
-
-SqlServerParametersOutputTypeDef = TypedDict(
-    "SqlServerParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
-TeradataParametersOutputTypeDef = TypedDict(
-    "TeradataParametersOutputTypeDef",
-    {
-        "Host": str,
-        "Port": int,
-        "Database": str,
-    },
-)
-
-TwitterParametersOutputTypeDef = TypedDict(
-    "TwitterParametersOutputTypeDef",
-    {
-        "Query": str,
-        "MaxRows": int,
-    },
-)
-
 DatabricksParametersTypeDef = TypedDict(
     "DatabricksParametersTypeDef",
     {
         "Host": str,
         "Port": int,
         "SqlEndpointPath": str,
     },
@@ -4872,33 +3639,14 @@
     "DateTimeDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": Sequence[Union[datetime, str]],
     },
     total=False,
 )
 
-_RequiredRollingDateConfigurationOutputTypeDef = TypedDict(
-    "_RequiredRollingDateConfigurationOutputTypeDef",
-    {
-        "Expression": str,
-    },
-)
-_OptionalRollingDateConfigurationOutputTypeDef = TypedDict(
-    "_OptionalRollingDateConfigurationOutputTypeDef",
-    {
-        "DataSetIdentifier": str,
-    },
-    total=False,
-)
-
-class RollingDateConfigurationOutputTypeDef(
-    _RequiredRollingDateConfigurationOutputTypeDef, _OptionalRollingDateConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredRollingDateConfigurationTypeDef = TypedDict(
     "_RequiredRollingDateConfigurationTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalRollingDateConfigurationTypeDef = TypedDict(
@@ -4919,16 +3667,16 @@
     {
         "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
         "CustomValue": datetime,
     },
     total=False,
 )
 
-MappedDataSetParameterOutputTypeDef = TypedDict(
-    "MappedDataSetParameterOutputTypeDef",
+MappedDataSetParameterTypeDef = TypedDict(
+    "MappedDataSetParameterTypeDef",
     {
         "DataSetIdentifier": str,
         "DataSetParameterName": str,
     },
 )
 
 DateTimeValueWhenUnsetConfigurationTypeDef = TypedDict(
@@ -4936,22 +3684,14 @@
     {
         "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
         "CustomValue": Union[datetime, str],
     },
     total=False,
 )
 
-MappedDataSetParameterTypeDef = TypedDict(
-    "MappedDataSetParameterTypeDef",
-    {
-        "DataSetIdentifier": str,
-        "DataSetParameterName": str,
-    },
-)
-
 DateTimeParameterOutputTypeDef = TypedDict(
     "DateTimeParameterOutputTypeDef",
     {
         "Name": str,
         "Values": List[datetime],
     },
 )
@@ -4960,23 +3700,14 @@
     "DateTimeParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[Union[datetime, str]],
     },
 )
 
-SheetControlInfoIconLabelOptionsOutputTypeDef = TypedDict(
-    "SheetControlInfoIconLabelOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "InfoIconText": str,
-    },
-    total=False,
-)
-
 SheetControlInfoIconLabelOptionsTypeDef = TypedDict(
     "SheetControlInfoIconLabelOptionsTypeDef",
     {
         "Visibility": VisibilityType,
         "InfoIconText": str,
     },
     total=False,
@@ -4994,23 +3725,14 @@
     "DecimalDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": Sequence[float],
     },
     total=False,
 )
 
-DecimalValueWhenUnsetConfigurationOutputTypeDef = TypedDict(
-    "DecimalValueWhenUnsetConfigurationOutputTypeDef",
-    {
-        "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
-        "CustomValue": float,
-    },
-    total=False,
-)
-
 DecimalValueWhenUnsetConfigurationTypeDef = TypedDict(
     "DecimalValueWhenUnsetConfigurationTypeDef",
     {
         "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
         "CustomValue": float,
     },
     total=False,
@@ -5797,56 +4519,31 @@
     "DescribeVPCConnectionRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "VPCConnectionId": str,
     },
 )
 
-NegativeFormatOutputTypeDef = TypedDict(
-    "NegativeFormatOutputTypeDef",
-    {
-        "Prefix": str,
-        "Suffix": str,
-    },
-    total=False,
-)
-
 NegativeFormatTypeDef = TypedDict(
     "NegativeFormatTypeDef",
     {
         "Prefix": str,
         "Suffix": str,
     },
     total=False,
 )
 
-DonutCenterOptionsOutputTypeDef = TypedDict(
-    "DonutCenterOptionsOutputTypeDef",
-    {
-        "LabelVisibility": VisibilityType,
-    },
-    total=False,
-)
-
 DonutCenterOptionsTypeDef = TypedDict(
     "DonutCenterOptionsTypeDef",
     {
         "LabelVisibility": VisibilityType,
     },
     total=False,
 )
 
-ListControlSelectAllOptionsOutputTypeDef = TypedDict(
-    "ListControlSelectAllOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 ListControlSelectAllOptionsTypeDef = TypedDict(
     "ListControlSelectAllOptionsTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
@@ -5856,35 +4553,14 @@
     {
         "Type": IngestionErrorTypeType,
         "Message": str,
     },
     total=False,
 )
 
-_RequiredExcludePeriodConfigurationOutputTypeDef = TypedDict(
-    "_RequiredExcludePeriodConfigurationOutputTypeDef",
-    {
-        "Amount": int,
-        "Granularity": TimeGranularityType,
-    },
-)
-_OptionalExcludePeriodConfigurationOutputTypeDef = TypedDict(
-    "_OptionalExcludePeriodConfigurationOutputTypeDef",
-    {
-        "Status": WidgetStatusType,
-    },
-    total=False,
-)
-
-class ExcludePeriodConfigurationOutputTypeDef(
-    _RequiredExcludePeriodConfigurationOutputTypeDef,
-    _OptionalExcludePeriodConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredExcludePeriodConfigurationTypeDef = TypedDict(
     "_RequiredExcludePeriodConfigurationTypeDef",
     {
         "Amount": int,
         "Granularity": TimeGranularityType,
     },
 )
@@ -5897,50 +4573,22 @@
 )
 
 class ExcludePeriodConfigurationTypeDef(
     _RequiredExcludePeriodConfigurationTypeDef, _OptionalExcludePeriodConfigurationTypeDef
 ):
     pass
 
-FieldSortOutputTypeDef = TypedDict(
-    "FieldSortOutputTypeDef",
-    {
-        "FieldId": str,
-        "Direction": SortDirectionType,
-    },
-)
-
 FieldSortTypeDef = TypedDict(
     "FieldSortTypeDef",
     {
         "FieldId": str,
         "Direction": SortDirectionType,
     },
 )
 
-_RequiredFieldTooltipItemOutputTypeDef = TypedDict(
-    "_RequiredFieldTooltipItemOutputTypeDef",
-    {
-        "FieldId": str,
-    },
-)
-_OptionalFieldTooltipItemOutputTypeDef = TypedDict(
-    "_OptionalFieldTooltipItemOutputTypeDef",
-    {
-        "Label": str,
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-class FieldTooltipItemOutputTypeDef(
-    _RequiredFieldTooltipItemOutputTypeDef, _OptionalFieldTooltipItemOutputTypeDef
-):
-    pass
-
 _RequiredFieldTooltipItemTypeDef = TypedDict(
     "_RequiredFieldTooltipItemTypeDef",
     {
         "FieldId": str,
     },
 )
 _OptionalFieldTooltipItemTypeDef = TypedDict(
@@ -5951,22 +4599,14 @@
     },
     total=False,
 )
 
 class FieldTooltipItemTypeDef(_RequiredFieldTooltipItemTypeDef, _OptionalFieldTooltipItemTypeDef):
     pass
 
-GeospatialMapStyleOptionsOutputTypeDef = TypedDict(
-    "GeospatialMapStyleOptionsOutputTypeDef",
-    {
-        "BaseMapStyle": BaseMapStyleTypeType,
-    },
-    total=False,
-)
-
 GeospatialMapStyleOptionsTypeDef = TypedDict(
     "GeospatialMapStyleOptionsTypeDef",
     {
         "BaseMapStyle": BaseMapStyleTypeType,
     },
     total=False,
 )
@@ -5983,21 +4623,14 @@
     "FilterSelectableValuesTypeDef",
     {
         "Values": Sequence[str],
     },
     total=False,
 )
 
-FilterOperationOutputTypeDef = TypedDict(
-    "FilterOperationOutputTypeDef",
-    {
-        "ConditionExpression": str,
-    },
-)
-
 SameSheetTargetVisualConfigurationOutputTypeDef = TypedDict(
     "SameSheetTargetVisualConfigurationOutputTypeDef",
     {
         "TargetVisuals": List[str],
         "TargetVisualOptions": Literal["ALL_VISUALS"],
     },
     total=False,
@@ -6038,30 +4671,14 @@
         "FolderType": Literal["SHARED"],
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
-FontSizeOutputTypeDef = TypedDict(
-    "FontSizeOutputTypeDef",
-    {
-        "Relative": RelativeFontSizeType,
-    },
-    total=False,
-)
-
-FontWeightOutputTypeDef = TypedDict(
-    "FontWeightOutputTypeDef",
-    {
-        "Name": FontWeightNameType,
-    },
-    total=False,
-)
-
 FontSizeTypeDef = TypedDict(
     "FontSizeTypeDef",
     {
         "Relative": RelativeFontSizeType,
     },
     total=False,
 )
@@ -6070,43 +4687,22 @@
     "FontWeightTypeDef",
     {
         "Name": FontWeightNameType,
     },
     total=False,
 )
 
-FontOutputTypeDef = TypedDict(
-    "FontOutputTypeDef",
-    {
-        "FontFamily": str,
-    },
-    total=False,
-)
-
 FontTypeDef = TypedDict(
     "FontTypeDef",
     {
         "FontFamily": str,
     },
     total=False,
 )
 
-TimeBasedForecastPropertiesOutputTypeDef = TypedDict(
-    "TimeBasedForecastPropertiesOutputTypeDef",
-    {
-        "PeriodsForward": int,
-        "PeriodsBackward": int,
-        "UpperBoundary": float,
-        "LowerBoundary": float,
-        "PredictionInterval": int,
-        "Seasonality": int,
-    },
-    total=False,
-)
-
 TimeBasedForecastPropertiesTypeDef = TypedDict(
     "TimeBasedForecastPropertiesTypeDef",
     {
         "PeriodsForward": int,
         "PeriodsBackward": int,
         "UpperBoundary": float,
         "LowerBoundary": float,
@@ -6146,72 +4742,39 @@
     {
         "StartDate": Union[datetime, str],
         "EndDate": Union[datetime, str],
         "Value": float,
     },
 )
 
-FreeFormLayoutScreenCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "FreeFormLayoutScreenCanvasSizeOptionsOutputTypeDef",
-    {
-        "OptimizedViewPortWidth": str,
-    },
-)
-
 FreeFormLayoutScreenCanvasSizeOptionsTypeDef = TypedDict(
     "FreeFormLayoutScreenCanvasSizeOptionsTypeDef",
     {
         "OptimizedViewPortWidth": str,
     },
 )
 
-FreeFormLayoutElementBackgroundStyleOutputTypeDef = TypedDict(
-    "FreeFormLayoutElementBackgroundStyleOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "Color": str,
-    },
-    total=False,
-)
-
 FreeFormLayoutElementBackgroundStyleTypeDef = TypedDict(
     "FreeFormLayoutElementBackgroundStyleTypeDef",
     {
         "Visibility": VisibilityType,
         "Color": str,
     },
     total=False,
 )
 
-FreeFormLayoutElementBorderStyleOutputTypeDef = TypedDict(
-    "FreeFormLayoutElementBorderStyleOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "Color": str,
-    },
-    total=False,
-)
-
 FreeFormLayoutElementBorderStyleTypeDef = TypedDict(
     "FreeFormLayoutElementBorderStyleTypeDef",
     {
         "Visibility": VisibilityType,
         "Color": str,
     },
     total=False,
 )
 
-LoadingAnimationOutputTypeDef = TypedDict(
-    "LoadingAnimationOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 LoadingAnimationTypeDef = TypedDict(
     "LoadingAnimationTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
@@ -6220,41 +4783,24 @@
     "SessionTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-GeospatialCoordinateBoundsOutputTypeDef = TypedDict(
-    "GeospatialCoordinateBoundsOutputTypeDef",
-    {
-        "North": float,
-        "South": float,
-        "West": float,
-        "East": float,
-    },
-)
-
 GeospatialCoordinateBoundsTypeDef = TypedDict(
     "GeospatialCoordinateBoundsTypeDef",
     {
         "North": float,
         "South": float,
         "West": float,
         "East": float,
     },
 )
 
-GeospatialHeatmapDataColorOutputTypeDef = TypedDict(
-    "GeospatialHeatmapDataColorOutputTypeDef",
-    {
-        "Color": str,
-    },
-)
-
 GeospatialHeatmapDataColorTypeDef = TypedDict(
     "GeospatialHeatmapDataColorTypeDef",
     {
         "Color": str,
     },
 )
 
@@ -6304,54 +4850,24 @@
 
 class GetSessionEmbedUrlRequestRequestTypeDef(
     _RequiredGetSessionEmbedUrlRequestRequestTypeDef,
     _OptionalGetSessionEmbedUrlRequestRequestTypeDef,
 ):
     pass
 
-TableBorderOptionsOutputTypeDef = TypedDict(
-    "TableBorderOptionsOutputTypeDef",
-    {
-        "Color": str,
-        "Thickness": int,
-        "Style": TableBorderStyleType,
-    },
-    total=False,
-)
-
 TableBorderOptionsTypeDef = TypedDict(
     "TableBorderOptionsTypeDef",
     {
         "Color": str,
         "Thickness": int,
         "Style": TableBorderStyleType,
     },
     total=False,
 )
 
-_RequiredGradientStopOutputTypeDef = TypedDict(
-    "_RequiredGradientStopOutputTypeDef",
-    {
-        "GradientOffset": float,
-    },
-)
-_OptionalGradientStopOutputTypeDef = TypedDict(
-    "_OptionalGradientStopOutputTypeDef",
-    {
-        "DataValue": float,
-        "Color": str,
-    },
-    total=False,
-)
-
-class GradientStopOutputTypeDef(
-    _RequiredGradientStopOutputTypeDef, _OptionalGradientStopOutputTypeDef
-):
-    pass
-
 _RequiredGradientStopTypeDef = TypedDict(
     "_RequiredGradientStopTypeDef",
     {
         "GradientOffset": float,
     },
 )
 _OptionalGradientStopTypeDef = TypedDict(
@@ -6362,34 +4878,14 @@
     },
     total=False,
 )
 
 class GradientStopTypeDef(_RequiredGradientStopTypeDef, _OptionalGradientStopTypeDef):
     pass
 
-_RequiredGridLayoutScreenCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "_RequiredGridLayoutScreenCanvasSizeOptionsOutputTypeDef",
-    {
-        "ResizeOption": ResizeOptionType,
-    },
-)
-_OptionalGridLayoutScreenCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "_OptionalGridLayoutScreenCanvasSizeOptionsOutputTypeDef",
-    {
-        "OptimizedViewPortWidth": str,
-    },
-    total=False,
-)
-
-class GridLayoutScreenCanvasSizeOptionsOutputTypeDef(
-    _RequiredGridLayoutScreenCanvasSizeOptionsOutputTypeDef,
-    _OptionalGridLayoutScreenCanvasSizeOptionsOutputTypeDef,
-):
-    pass
-
 _RequiredGridLayoutScreenCanvasSizeOptionsTypeDef = TypedDict(
     "_RequiredGridLayoutScreenCanvasSizeOptionsTypeDef",
     {
         "ResizeOption": ResizeOptionType,
     },
 )
 _OptionalGridLayoutScreenCanvasSizeOptionsTypeDef = TypedDict(
@@ -6402,37 +4898,14 @@
 
 class GridLayoutScreenCanvasSizeOptionsTypeDef(
     _RequiredGridLayoutScreenCanvasSizeOptionsTypeDef,
     _OptionalGridLayoutScreenCanvasSizeOptionsTypeDef,
 ):
     pass
 
-_RequiredGridLayoutElementOutputTypeDef = TypedDict(
-    "_RequiredGridLayoutElementOutputTypeDef",
-    {
-        "ElementId": str,
-        "ElementType": LayoutElementTypeType,
-        "ColumnSpan": int,
-        "RowSpan": int,
-    },
-)
-_OptionalGridLayoutElementOutputTypeDef = TypedDict(
-    "_OptionalGridLayoutElementOutputTypeDef",
-    {
-        "ColumnIndex": int,
-        "RowIndex": int,
-    },
-    total=False,
-)
-
-class GridLayoutElementOutputTypeDef(
-    _RequiredGridLayoutElementOutputTypeDef, _OptionalGridLayoutElementOutputTypeDef
-):
-    pass
-
 _RequiredGridLayoutElementTypeDef = TypedDict(
     "_RequiredGridLayoutElementTypeDef",
     {
         "ElementId": str,
         "ElementType": LayoutElementTypeType,
         "ColumnSpan": int,
         "RowSpan": int,
@@ -6457,22 +4930,14 @@
     {
         "Operator": Literal["StartsWith"],
         "Name": Literal["GROUP_NAME"],
         "Value": str,
     },
 )
 
-GutterStyleOutputTypeDef = TypedDict(
-    "GutterStyleOutputTypeDef",
-    {
-        "Show": bool,
-    },
-    total=False,
-)
-
 GutterStyleTypeDef = TypedDict(
     "GutterStyleTypeDef",
     {
         "Show": bool,
     },
     total=False,
 )
@@ -6482,23 +4947,14 @@
     {
         "AssignmentName": str,
         "AssignmentStatus": AssignmentStatusType,
     },
     total=False,
 )
 
-LookbackWindowOutputTypeDef = TypedDict(
-    "LookbackWindowOutputTypeDef",
-    {
-        "ColumnName": str,
-        "Size": int,
-        "SizeUnit": LookbackWindowSizeUnitType,
-    },
-)
-
 LookbackWindowTypeDef = TypedDict(
     "LookbackWindowTypeDef",
     {
         "ColumnName": str,
         "Size": int,
         "SizeUnit": LookbackWindowSizeUnitType,
     },
@@ -6534,23 +4990,14 @@
     "IntegerDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": Sequence[int],
     },
     total=False,
 )
 
-IntegerValueWhenUnsetConfigurationOutputTypeDef = TypedDict(
-    "IntegerValueWhenUnsetConfigurationOutputTypeDef",
-    {
-        "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
-        "CustomValue": int,
-    },
-    total=False,
-)
-
 IntegerValueWhenUnsetConfigurationTypeDef = TypedDict(
     "IntegerValueWhenUnsetConfigurationTypeDef",
     {
         "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
         "CustomValue": int,
     },
     total=False,
@@ -6568,54 +5015,22 @@
     "IntegerParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[int],
     },
 )
 
-JoinKeyPropertiesOutputTypeDef = TypedDict(
-    "JoinKeyPropertiesOutputTypeDef",
-    {
-        "UniqueKey": bool,
-    },
-    total=False,
-)
-
 JoinKeyPropertiesTypeDef = TypedDict(
     "JoinKeyPropertiesTypeDef",
     {
         "UniqueKey": bool,
     },
     total=False,
 )
 
-ProgressBarOptionsOutputTypeDef = TypedDict(
-    "ProgressBarOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-SecondaryValueOptionsOutputTypeDef = TypedDict(
-    "SecondaryValueOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-TrendArrowOptionsOutputTypeDef = TypedDict(
-    "TrendArrowOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 ProgressBarOptionsTypeDef = TypedDict(
     "ProgressBarOptionsTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
@@ -6632,36 +5047,14 @@
     "TrendArrowOptionsTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
 
-LineChartLineStyleSettingsOutputTypeDef = TypedDict(
-    "LineChartLineStyleSettingsOutputTypeDef",
-    {
-        "LineVisibility": VisibilityType,
-        "LineInterpolation": LineInterpolationType,
-        "LineStyle": LineChartLineStyleType,
-        "LineWidth": str,
-    },
-    total=False,
-)
-
-LineChartMarkerStyleSettingsOutputTypeDef = TypedDict(
-    "LineChartMarkerStyleSettingsOutputTypeDef",
-    {
-        "MarkerVisibility": VisibilityType,
-        "MarkerShape": LineChartMarkerShapeType,
-        "MarkerSize": str,
-        "MarkerColor": str,
-    },
-    total=False,
-)
-
 LineChartLineStyleSettingsTypeDef = TypedDict(
     "LineChartLineStyleSettingsTypeDef",
     {
         "LineVisibility": VisibilityType,
         "LineInterpolation": LineInterpolationType,
         "LineStyle": LineChartLineStyleType,
         "LineWidth": str,
@@ -6676,22 +5069,14 @@
         "MarkerShape": LineChartMarkerShapeType,
         "MarkerSize": str,
         "MarkerColor": str,
     },
     total=False,
 )
 
-MissingDataConfigurationOutputTypeDef = TypedDict(
-    "MissingDataConfigurationOutputTypeDef",
-    {
-        "TreatmentOption": MissingDataTreatmentOptionType,
-    },
-    total=False,
-)
-
 MissingDataConfigurationTypeDef = TypedDict(
     "MissingDataConfigurationTypeDef",
     {
         "TreatmentOption": MissingDataTreatmentOptionType,
     },
     total=False,
 )
@@ -6764,22 +5149,14 @@
 
 class ListAssetBundleImportJobsRequestRequestTypeDef(
     _RequiredListAssetBundleImportJobsRequestRequestTypeDef,
     _OptionalListAssetBundleImportJobsRequestRequestTypeDef,
 ):
     pass
 
-ListControlSearchOptionsOutputTypeDef = TypedDict(
-    "ListControlSearchOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 ListControlSearchOptionsTypeDef = TypedDict(
     "ListControlSearchOptionsTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
@@ -7058,22 +5435,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredListTemplateAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateAliasesRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TemplateId": str,
     },
 )
@@ -7345,56 +5714,31 @@
 
 class ListVPCConnectionsRequestRequestTypeDef(
     _RequiredListVPCConnectionsRequestRequestTypeDef,
     _OptionalListVPCConnectionsRequestRequestTypeDef,
 ):
     pass
 
-LongFormatTextOutputTypeDef = TypedDict(
-    "LongFormatTextOutputTypeDef",
-    {
-        "PlainText": str,
-        "RichText": str,
-    },
-    total=False,
-)
-
 LongFormatTextTypeDef = TypedDict(
     "LongFormatTextTypeDef",
     {
         "PlainText": str,
         "RichText": str,
     },
     total=False,
 )
 
-ManifestFileLocationOutputTypeDef = TypedDict(
-    "ManifestFileLocationOutputTypeDef",
-    {
-        "Bucket": str,
-        "Key": str,
-    },
-)
-
 ManifestFileLocationTypeDef = TypedDict(
     "ManifestFileLocationTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
-MarginStyleOutputTypeDef = TypedDict(
-    "MarginStyleOutputTypeDef",
-    {
-        "Show": bool,
-    },
-    total=False,
-)
-
 MarginStyleTypeDef = TypedDict(
     "MarginStyleTypeDef",
     {
         "Show": bool,
     },
     total=False,
 )
@@ -7456,58 +5800,32 @@
         "DecimalStaticValues": Sequence[float],
         "DateTimeStaticValues": Sequence[Union[datetime, str]],
         "IntegerStaticValues": Sequence[int],
     },
     total=False,
 )
 
-NumericRangeFilterValueOutputTypeDef = TypedDict(
-    "NumericRangeFilterValueOutputTypeDef",
-    {
-        "StaticValue": float,
-        "Parameter": str,
-    },
-    total=False,
-)
-
 NumericRangeFilterValueTypeDef = TypedDict(
     "NumericRangeFilterValueTypeDef",
     {
         "StaticValue": float,
         "Parameter": str,
     },
     total=False,
 )
 
-ThousandSeparatorOptionsOutputTypeDef = TypedDict(
-    "ThousandSeparatorOptionsOutputTypeDef",
-    {
-        "Symbol": NumericSeparatorSymbolType,
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 ThousandSeparatorOptionsTypeDef = TypedDict(
     "ThousandSeparatorOptionsTypeDef",
     {
         "Symbol": NumericSeparatorSymbolType,
         "Visibility": VisibilityType,
     },
     total=False,
 )
 
-PercentileAggregationOutputTypeDef = TypedDict(
-    "PercentileAggregationOutputTypeDef",
-    {
-        "PercentileValue": float,
-    },
-    total=False,
-)
-
 PercentileAggregationTypeDef = TypedDict(
     "PercentileAggregationTypeDef",
     {
         "PercentileValue": float,
     },
     total=False,
 )
@@ -7524,86 +5842,40 @@
     "StringParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
-PercentVisibleRangeOutputTypeDef = TypedDict(
-    "PercentVisibleRangeOutputTypeDef",
-    {
-        "From": float,
-        "To": float,
-    },
-    total=False,
-)
-
 PercentVisibleRangeTypeDef = TypedDict(
     "PercentVisibleRangeTypeDef",
     {
         "From": float,
         "To": float,
     },
     total=False,
 )
 
-PivotTableConditionalFormattingScopeOutputTypeDef = TypedDict(
-    "PivotTableConditionalFormattingScopeOutputTypeDef",
-    {
-        "Role": PivotTableConditionalFormattingScopeRoleType,
-    },
-    total=False,
-)
-
 PivotTableConditionalFormattingScopeTypeDef = TypedDict(
     "PivotTableConditionalFormattingScopeTypeDef",
     {
         "Role": PivotTableConditionalFormattingScopeRoleType,
     },
     total=False,
 )
 
-PivotTablePaginatedReportOptionsOutputTypeDef = TypedDict(
-    "PivotTablePaginatedReportOptionsOutputTypeDef",
-    {
-        "VerticalOverflowVisibility": VisibilityType,
-        "OverflowColumnHeaderVisibility": VisibilityType,
-    },
-    total=False,
-)
-
 PivotTablePaginatedReportOptionsTypeDef = TypedDict(
     "PivotTablePaginatedReportOptionsTypeDef",
     {
         "VerticalOverflowVisibility": VisibilityType,
         "OverflowColumnHeaderVisibility": VisibilityType,
     },
     total=False,
 )
 
-_RequiredPivotTableFieldOptionOutputTypeDef = TypedDict(
-    "_RequiredPivotTableFieldOptionOutputTypeDef",
-    {
-        "FieldId": str,
-    },
-)
-_OptionalPivotTableFieldOptionOutputTypeDef = TypedDict(
-    "_OptionalPivotTableFieldOptionOutputTypeDef",
-    {
-        "CustomLabel": str,
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
-class PivotTableFieldOptionOutputTypeDef(
-    _RequiredPivotTableFieldOptionOutputTypeDef, _OptionalPivotTableFieldOptionOutputTypeDef
-):
-    pass
-
 _RequiredPivotTableFieldOptionTypeDef = TypedDict(
     "_RequiredPivotTableFieldOptionTypeDef",
     {
         "FieldId": str,
     },
 )
 _OptionalPivotTableFieldOptionTypeDef = TypedDict(
@@ -7616,22 +5888,14 @@
 )
 
 class PivotTableFieldOptionTypeDef(
     _RequiredPivotTableFieldOptionTypeDef, _OptionalPivotTableFieldOptionTypeDef
 ):
     pass
 
-PivotTableFieldSubtotalOptionsOutputTypeDef = TypedDict(
-    "PivotTableFieldSubtotalOptionsOutputTypeDef",
-    {
-        "FieldId": str,
-    },
-    total=False,
-)
-
 PivotTableFieldSubtotalOptionsTypeDef = TypedDict(
     "PivotTableFieldSubtotalOptionsTypeDef",
     {
         "FieldId": str,
     },
     total=False,
 )
@@ -7664,103 +5928,54 @@
 ProjectOperationTypeDef = TypedDict(
     "ProjectOperationTypeDef",
     {
         "ProjectedColumns": Sequence[str],
     },
 )
 
-RadarChartAreaStyleSettingsOutputTypeDef = TypedDict(
-    "RadarChartAreaStyleSettingsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 RadarChartAreaStyleSettingsTypeDef = TypedDict(
     "RadarChartAreaStyleSettingsTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
 
-RangeConstantOutputTypeDef = TypedDict(
-    "RangeConstantOutputTypeDef",
-    {
-        "Minimum": str,
-        "Maximum": str,
-    },
-    total=False,
-)
-
 RangeConstantTypeDef = TypedDict(
     "RangeConstantTypeDef",
     {
         "Minimum": str,
         "Maximum": str,
     },
     total=False,
 )
 
-ReferenceLineCustomLabelConfigurationOutputTypeDef = TypedDict(
-    "ReferenceLineCustomLabelConfigurationOutputTypeDef",
-    {
-        "CustomLabel": str,
-    },
-)
-
 ReferenceLineCustomLabelConfigurationTypeDef = TypedDict(
     "ReferenceLineCustomLabelConfigurationTypeDef",
     {
         "CustomLabel": str,
     },
 )
 
-ReferenceLineStaticDataConfigurationOutputTypeDef = TypedDict(
-    "ReferenceLineStaticDataConfigurationOutputTypeDef",
-    {
-        "Value": float,
-    },
-)
-
 ReferenceLineStaticDataConfigurationTypeDef = TypedDict(
     "ReferenceLineStaticDataConfigurationTypeDef",
     {
         "Value": float,
     },
 )
 
-ReferenceLineStyleConfigurationOutputTypeDef = TypedDict(
-    "ReferenceLineStyleConfigurationOutputTypeDef",
-    {
-        "Pattern": ReferenceLinePatternTypeType,
-        "Color": str,
-    },
-    total=False,
-)
-
 ReferenceLineStyleConfigurationTypeDef = TypedDict(
     "ReferenceLineStyleConfigurationTypeDef",
     {
         "Pattern": ReferenceLinePatternTypeType,
         "Color": str,
     },
     total=False,
 )
 
-ScheduleRefreshOnEntityOutputTypeDef = TypedDict(
-    "ScheduleRefreshOnEntityOutputTypeDef",
-    {
-        "DayOfWeek": DayOfWeekType,
-        "DayOfMonth": str,
-    },
-    total=False,
-)
-
 ScheduleRefreshOnEntityTypeDef = TypedDict(
     "ScheduleRefreshOnEntityTypeDef",
     {
         "DayOfWeek": DayOfWeekType,
         "DayOfMonth": str,
     },
     total=False,
@@ -7806,22 +6021,14 @@
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
     {
         "InitialTopicId": str,
     },
     total=False,
 )
 
-RenameColumnOperationOutputTypeDef = TypedDict(
-    "RenameColumnOperationOutputTypeDef",
-    {
-        "ColumnName": str,
-        "NewColumnName": str,
-    },
-)
-
 RenameColumnOperationTypeDef = TypedDict(
     "RenameColumnOperationTypeDef",
     {
         "ColumnName": str,
         "NewColumnName": str,
     },
 )
@@ -7830,35 +6037,14 @@
     "RestoreAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
 
-_RequiredRowLevelPermissionTagRuleOutputTypeDef = TypedDict(
-    "_RequiredRowLevelPermissionTagRuleOutputTypeDef",
-    {
-        "TagKey": str,
-        "ColumnName": str,
-    },
-)
-_OptionalRowLevelPermissionTagRuleOutputTypeDef = TypedDict(
-    "_OptionalRowLevelPermissionTagRuleOutputTypeDef",
-    {
-        "TagMultiValueDelimiter": str,
-        "MatchAllValue": str,
-    },
-    total=False,
-)
-
-class RowLevelPermissionTagRuleOutputTypeDef(
-    _RequiredRowLevelPermissionTagRuleOutputTypeDef, _OptionalRowLevelPermissionTagRuleOutputTypeDef
-):
-    pass
-
 _RequiredRowLevelPermissionTagRuleTypeDef = TypedDict(
     "_RequiredRowLevelPermissionTagRuleTypeDef",
     {
         "TagKey": str,
         "ColumnName": str,
     },
 )
@@ -7872,83 +6058,43 @@
 )
 
 class RowLevelPermissionTagRuleTypeDef(
     _RequiredRowLevelPermissionTagRuleTypeDef, _OptionalRowLevelPermissionTagRuleTypeDef
 ):
     pass
 
-S3BucketConfigurationOutputTypeDef = TypedDict(
-    "S3BucketConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-        "BucketPrefix": str,
-        "BucketRegion": str,
-    },
-)
-
 S3BucketConfigurationTypeDef = TypedDict(
     "S3BucketConfigurationTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
         "BucketRegion": str,
     },
 )
 
-UploadSettingsOutputTypeDef = TypedDict(
-    "UploadSettingsOutputTypeDef",
-    {
-        "Format": FileFormatType,
-        "StartFromRow": int,
-        "ContainsHeader": bool,
-        "TextQualifier": TextQualifierType,
-        "Delimiter": str,
-    },
-    total=False,
-)
-
 UploadSettingsTypeDef = TypedDict(
     "UploadSettingsTypeDef",
     {
         "Format": FileFormatType,
         "StartFromRow": int,
         "ContainsHeader": bool,
         "TextQualifier": TextQualifierType,
         "Delimiter": str,
     },
     total=False,
 )
 
-SectionAfterPageBreakOutputTypeDef = TypedDict(
-    "SectionAfterPageBreakOutputTypeDef",
-    {
-        "Status": SectionPageBreakStatusType,
-    },
-    total=False,
-)
-
 SectionAfterPageBreakTypeDef = TypedDict(
     "SectionAfterPageBreakTypeDef",
     {
         "Status": SectionPageBreakStatusType,
     },
     total=False,
 )
 
-SpacingOutputTypeDef = TypedDict(
-    "SpacingOutputTypeDef",
-    {
-        "Top": str,
-        "Bottom": str,
-        "Left": str,
-        "Right": str,
-    },
-    total=False,
-)
-
 SpacingTypeDef = TypedDict(
     "SpacingTypeDef",
     {
         "Top": str,
         "Bottom": str,
         "Left": str,
         "Right": str,
@@ -8041,33 +6187,14 @@
         "TruthyCellValueSynonyms": Sequence[str],
         "FalseyCellValue": str,
         "FalseyCellValueSynonyms": Sequence[str],
     },
     total=False,
 )
 
-_RequiredSheetTextBoxOutputTypeDef = TypedDict(
-    "_RequiredSheetTextBoxOutputTypeDef",
-    {
-        "SheetTextBoxId": str,
-    },
-)
-_OptionalSheetTextBoxOutputTypeDef = TypedDict(
-    "_OptionalSheetTextBoxOutputTypeDef",
-    {
-        "Content": str,
-    },
-    total=False,
-)
-
-class SheetTextBoxOutputTypeDef(
-    _RequiredSheetTextBoxOutputTypeDef, _OptionalSheetTextBoxOutputTypeDef
-):
-    pass
-
 _RequiredSheetTextBoxTypeDef = TypedDict(
     "_RequiredSheetTextBoxTypeDef",
     {
         "SheetTextBoxId": str,
     },
 )
 _OptionalSheetTextBoxTypeDef = TypedDict(
@@ -8077,57 +6204,31 @@
     },
     total=False,
 )
 
 class SheetTextBoxTypeDef(_RequiredSheetTextBoxTypeDef, _OptionalSheetTextBoxTypeDef):
     pass
 
-SheetElementConfigurationOverridesOutputTypeDef = TypedDict(
-    "SheetElementConfigurationOverridesOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 SheetElementConfigurationOverridesTypeDef = TypedDict(
     "SheetElementConfigurationOverridesTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
 
-ShortFormatTextOutputTypeDef = TypedDict(
-    "ShortFormatTextOutputTypeDef",
-    {
-        "PlainText": str,
-        "RichText": str,
-    },
-    total=False,
-)
-
 ShortFormatTextTypeDef = TypedDict(
     "ShortFormatTextTypeDef",
     {
         "PlainText": str,
         "RichText": str,
     },
     total=False,
 )
 
-SmallMultiplesAxisPropertiesOutputTypeDef = TypedDict(
-    "SmallMultiplesAxisPropertiesOutputTypeDef",
-    {
-        "Scale": SmallMultiplesAxisScaleType,
-        "Placement": SmallMultiplesAxisPlacementType,
-    },
-    total=False,
-)
-
 SmallMultiplesAxisPropertiesTypeDef = TypedDict(
     "SmallMultiplesAxisPropertiesTypeDef",
     {
         "Scale": SmallMultiplesAxisScaleType,
         "Placement": SmallMultiplesAxisPlacementType,
     },
     total=False,
@@ -8203,74 +6304,40 @@
     "StringDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": Sequence[str],
     },
     total=False,
 )
 
-StringValueWhenUnsetConfigurationOutputTypeDef = TypedDict(
-    "StringValueWhenUnsetConfigurationOutputTypeDef",
-    {
-        "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
-        "CustomValue": str,
-    },
-    total=False,
-)
-
 StringValueWhenUnsetConfigurationTypeDef = TypedDict(
     "StringValueWhenUnsetConfigurationTypeDef",
     {
         "ValueWhenUnsetOption": ValueWhenUnsetOptionType,
         "CustomValue": str,
     },
     total=False,
 )
 
-TableCellImageSizingConfigurationOutputTypeDef = TypedDict(
-    "TableCellImageSizingConfigurationOutputTypeDef",
-    {
-        "TableCellImageScalingConfiguration": TableCellImageScalingConfigurationType,
-    },
-    total=False,
-)
-
 TableCellImageSizingConfigurationTypeDef = TypedDict(
     "TableCellImageSizingConfigurationTypeDef",
     {
         "TableCellImageScalingConfiguration": TableCellImageScalingConfigurationType,
     },
     total=False,
 )
 
-TablePaginatedReportOptionsOutputTypeDef = TypedDict(
-    "TablePaginatedReportOptionsOutputTypeDef",
-    {
-        "VerticalOverflowVisibility": VisibilityType,
-        "OverflowColumnHeaderVisibility": VisibilityType,
-    },
-    total=False,
-)
-
 TablePaginatedReportOptionsTypeDef = TypedDict(
     "TablePaginatedReportOptionsTypeDef",
     {
         "VerticalOverflowVisibility": VisibilityType,
         "OverflowColumnHeaderVisibility": VisibilityType,
     },
     total=False,
 )
 
-TableFieldCustomIconContentOutputTypeDef = TypedDict(
-    "TableFieldCustomIconContentOutputTypeDef",
-    {
-        "Icon": Literal["LINK"],
-    },
-    total=False,
-)
-
 TableFieldCustomIconContentTypeDef = TypedDict(
     "TableFieldCustomIconContentTypeDef",
     {
         "Icon": Literal["LINK"],
     },
     total=False,
 )
@@ -8278,53 +6345,22 @@
 TemplateSourceTemplateTypeDef = TypedDict(
     "TemplateSourceTemplateTypeDef",
     {
         "Arn": str,
     },
 )
 
-TextControlPlaceholderOptionsOutputTypeDef = TypedDict(
-    "TextControlPlaceholderOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-    },
-    total=False,
-)
-
 TextControlPlaceholderOptionsTypeDef = TypedDict(
     "TextControlPlaceholderOptionsTypeDef",
     {
         "Visibility": VisibilityType,
     },
     total=False,
 )
 
-UIColorPaletteOutputTypeDef = TypedDict(
-    "UIColorPaletteOutputTypeDef",
-    {
-        "PrimaryForeground": str,
-        "PrimaryBackground": str,
-        "SecondaryForeground": str,
-        "SecondaryBackground": str,
-        "Accent": str,
-        "AccentForeground": str,
-        "Danger": str,
-        "DangerForeground": str,
-        "Warning": str,
-        "WarningForeground": str,
-        "Success": str,
-        "SuccessForeground": str,
-        "Dimension": str,
-        "DimensionForeground": str,
-        "Measure": str,
-        "MeasureForeground": str,
-    },
-    total=False,
-)
-
 UIColorPaletteTypeDef = TypedDict(
     "UIColorPaletteTypeDef",
     {
         "PrimaryForeground": str,
         "PrimaryBackground": str,
         "SecondaryForeground": str,
         "SecondaryBackground": str,
@@ -8349,23 +6385,14 @@
     {
         "Type": Literal["INTERNAL_FAILURE"],
         "Message": str,
     },
     total=False,
 )
 
-TopicSingularFilterConstantOutputTypeDef = TypedDict(
-    "TopicSingularFilterConstantOutputTypeDef",
-    {
-        "ConstantType": ConstantTypeType,
-        "SingularConstant": str,
-    },
-    total=False,
-)
-
 TopicSingularFilterConstantTypeDef = TypedDict(
     "TopicSingularFilterConstantTypeDef",
     {
         "ConstantType": ConstantTypeType,
         "SingularConstant": str,
     },
     total=False,
@@ -8589,43 +6616,22 @@
 
 class UpdateVPCConnectionRequestRequestTypeDef(
     _RequiredUpdateVPCConnectionRequestRequestTypeDef,
     _OptionalUpdateVPCConnectionRequestRequestTypeDef,
 ):
     pass
 
-WaterfallChartOptionsOutputTypeDef = TypedDict(
-    "WaterfallChartOptionsOutputTypeDef",
-    {
-        "TotalBarLabel": str,
-    },
-    total=False,
-)
-
 WaterfallChartOptionsTypeDef = TypedDict(
     "WaterfallChartOptionsTypeDef",
     {
         "TotalBarLabel": str,
     },
     total=False,
 )
 
-WordCloudOptionsOutputTypeDef = TypedDict(
-    "WordCloudOptionsOutputTypeDef",
-    {
-        "WordOrientation": WordCloudWordOrientationType,
-        "WordScaling": WordCloudWordScalingType,
-        "CloudLayout": WordCloudCloudLayoutType,
-        "WordCasing": WordCloudWordCasingType,
-        "WordPadding": WordCloudWordPaddingType,
-        "MaximumStringLength": int,
-    },
-    total=False,
-)
-
 WordCloudOptionsTypeDef = TypedDict(
     "WordCloudOptionsTypeDef",
     {
         "WordOrientation": WordCloudWordOrientationType,
         "WordScaling": WordCloudWordScalingType,
         "CloudLayout": WordCloudCloudLayoutType,
         "WordCasing": WordCloudWordCasingType,
@@ -8652,148 +6658,52 @@
 
 class UpdateAccountCustomizationRequestRequestTypeDef(
     _RequiredUpdateAccountCustomizationRequestRequestTypeDef,
     _OptionalUpdateAccountCustomizationRequestRequestTypeDef,
 ):
     pass
 
-AxisLabelReferenceOptionsOutputTypeDef = TypedDict(
-    "AxisLabelReferenceOptionsOutputTypeDef",
+AxisLabelReferenceOptionsTypeDef = TypedDict(
+    "AxisLabelReferenceOptionsTypeDef",
     {
         "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
+        "Column": ColumnIdentifierTypeDef,
     },
 )
 
-CascadingControlSourceOutputTypeDef = TypedDict(
-    "CascadingControlSourceOutputTypeDef",
+CascadingControlSourceTypeDef = TypedDict(
+    "CascadingControlSourceTypeDef",
     {
         "SourceSheetControlId": str,
-        "ColumnToMatch": ColumnIdentifierOutputTypeDef,
+        "ColumnToMatch": ColumnIdentifierTypeDef,
     },
     total=False,
 )
 
 CategoryDrillDownFilterOutputTypeDef = TypedDict(
     "CategoryDrillDownFilterOutputTypeDef",
     {
-        "Column": ColumnIdentifierOutputTypeDef,
+        "Column": ColumnIdentifierTypeDef,
         "CategoryValues": List[str],
     },
 )
 
-ContributionAnalysisDefaultOutputTypeDef = TypedDict(
-    "ContributionAnalysisDefaultOutputTypeDef",
-    {
-        "MeasureFieldId": str,
-        "ContributorDimensions": List[ColumnIdentifierOutputTypeDef],
-    },
-)
-
-_RequiredDynamicDefaultValueOutputTypeDef = TypedDict(
-    "_RequiredDynamicDefaultValueOutputTypeDef",
-    {
-        "DefaultValueColumn": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalDynamicDefaultValueOutputTypeDef = TypedDict(
-    "_OptionalDynamicDefaultValueOutputTypeDef",
-    {
-        "UserNameColumn": ColumnIdentifierOutputTypeDef,
-        "GroupNameColumn": ColumnIdentifierOutputTypeDef,
-    },
-    total=False,
-)
-
-class DynamicDefaultValueOutputTypeDef(
-    _RequiredDynamicDefaultValueOutputTypeDef, _OptionalDynamicDefaultValueOutputTypeDef
-):
-    pass
-
-FilterOperationSelectedFieldsConfigurationOutputTypeDef = TypedDict(
-    "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
-    {
-        "SelectedFields": List[str],
-        "SelectedFieldOptions": Literal["ALL_FIELDS"],
-        "SelectedColumns": List[ColumnIdentifierOutputTypeDef],
-    },
-    total=False,
-)
-
-NumericEqualityDrillDownFilterOutputTypeDef = TypedDict(
-    "NumericEqualityDrillDownFilterOutputTypeDef",
-    {
-        "Column": ColumnIdentifierOutputTypeDef,
-        "Value": float,
-    },
-)
-
-ParameterSelectableValuesOutputTypeDef = TypedDict(
-    "ParameterSelectableValuesOutputTypeDef",
-    {
-        "Values": List[str],
-        "LinkToDataSetColumn": ColumnIdentifierOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredTimeEqualityFilterOutputTypeDef = TypedDict(
-    "_RequiredTimeEqualityFilterOutputTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalTimeEqualityFilterOutputTypeDef = TypedDict(
-    "_OptionalTimeEqualityFilterOutputTypeDef",
-    {
-        "Value": datetime,
-        "ParameterName": str,
-        "TimeGranularity": TimeGranularityType,
-    },
-    total=False,
-)
-
-class TimeEqualityFilterOutputTypeDef(
-    _RequiredTimeEqualityFilterOutputTypeDef, _OptionalTimeEqualityFilterOutputTypeDef
-):
-    pass
-
-TimeRangeDrillDownFilterOutputTypeDef = TypedDict(
-    "TimeRangeDrillDownFilterOutputTypeDef",
-    {
-        "Column": ColumnIdentifierOutputTypeDef,
-        "RangeMinimum": datetime,
-        "RangeMaximum": datetime,
-        "TimeGranularity": TimeGranularityType,
-    },
-)
-
-AxisLabelReferenceOptionsTypeDef = TypedDict(
-    "AxisLabelReferenceOptionsTypeDef",
+CategoryDrillDownFilterTypeDef = TypedDict(
+    "CategoryDrillDownFilterTypeDef",
     {
-        "FieldId": str,
         "Column": ColumnIdentifierTypeDef,
+        "CategoryValues": Sequence[str],
     },
 )
 
-CascadingControlSourceTypeDef = TypedDict(
-    "CascadingControlSourceTypeDef",
-    {
-        "SourceSheetControlId": str,
-        "ColumnToMatch": ColumnIdentifierTypeDef,
-    },
-    total=False,
-)
-
-CategoryDrillDownFilterTypeDef = TypedDict(
-    "CategoryDrillDownFilterTypeDef",
+ContributionAnalysisDefaultOutputTypeDef = TypedDict(
+    "ContributionAnalysisDefaultOutputTypeDef",
     {
-        "Column": ColumnIdentifierTypeDef,
-        "CategoryValues": Sequence[str],
+        "MeasureFieldId": str,
+        "ContributorDimensions": List[ColumnIdentifierTypeDef],
     },
 )
 
 ContributionAnalysisDefaultTypeDef = TypedDict(
     "ContributionAnalysisDefaultTypeDef",
     {
         "MeasureFieldId": str,
@@ -8817,14 +6727,24 @@
 )
 
 class DynamicDefaultValueTypeDef(
     _RequiredDynamicDefaultValueTypeDef, _OptionalDynamicDefaultValueTypeDef
 ):
     pass
 
+FilterOperationSelectedFieldsConfigurationOutputTypeDef = TypedDict(
+    "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
+    {
+        "SelectedFields": List[str],
+        "SelectedFieldOptions": Literal["ALL_FIELDS"],
+        "SelectedColumns": List[ColumnIdentifierTypeDef],
+    },
+    total=False,
+)
+
 FilterOperationSelectedFieldsConfigurationTypeDef = TypedDict(
     "FilterOperationSelectedFieldsConfigurationTypeDef",
     {
         "SelectedFields": Sequence[str],
         "SelectedFieldOptions": Literal["ALL_FIELDS"],
         "SelectedColumns": Sequence[ColumnIdentifierTypeDef],
     },
@@ -8835,23 +6755,54 @@
     "NumericEqualityDrillDownFilterTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "Value": float,
     },
 )
 
+ParameterSelectableValuesOutputTypeDef = TypedDict(
+    "ParameterSelectableValuesOutputTypeDef",
+    {
+        "Values": List[str],
+        "LinkToDataSetColumn": ColumnIdentifierTypeDef,
+    },
+    total=False,
+)
+
 ParameterSelectableValuesTypeDef = TypedDict(
     "ParameterSelectableValuesTypeDef",
     {
         "Values": Sequence[str],
         "LinkToDataSetColumn": ColumnIdentifierTypeDef,
     },
     total=False,
 )
 
+_RequiredTimeEqualityFilterOutputTypeDef = TypedDict(
+    "_RequiredTimeEqualityFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+    },
+)
+_OptionalTimeEqualityFilterOutputTypeDef = TypedDict(
+    "_OptionalTimeEqualityFilterOutputTypeDef",
+    {
+        "Value": datetime,
+        "ParameterName": str,
+        "TimeGranularity": TimeGranularityType,
+    },
+    total=False,
+)
+
+class TimeEqualityFilterOutputTypeDef(
+    _RequiredTimeEqualityFilterOutputTypeDef, _OptionalTimeEqualityFilterOutputTypeDef
+):
+    pass
+
 _RequiredTimeEqualityFilterTypeDef = TypedDict(
     "_RequiredTimeEqualityFilterTypeDef",
     {
         "FilterId": str,
         "Column": ColumnIdentifierTypeDef,
     },
 )
@@ -8866,14 +6817,24 @@
 )
 
 class TimeEqualityFilterTypeDef(
     _RequiredTimeEqualityFilterTypeDef, _OptionalTimeEqualityFilterTypeDef
 ):
     pass
 
+TimeRangeDrillDownFilterOutputTypeDef = TypedDict(
+    "TimeRangeDrillDownFilterOutputTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+        "RangeMinimum": datetime,
+        "RangeMaximum": datetime,
+        "TimeGranularity": TimeGranularityType,
+    },
+)
+
 TimeRangeDrillDownFilterTypeDef = TypedDict(
     "TimeRangeDrillDownFilterTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "RangeMinimum": Union[datetime, str],
         "RangeMaximum": Union[datetime, str],
         "TimeGranularity": TimeGranularityType,
@@ -8965,37 +6926,28 @@
 RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef = TypedDict(
     "RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef",
     {
         "InitialDashboardVisualId": DashboardVisualIdTypeDef,
     },
 )
 
-ArcAxisConfigurationOutputTypeDef = TypedDict(
-    "ArcAxisConfigurationOutputTypeDef",
-    {
-        "Range": ArcAxisDisplayRangeOutputTypeDef,
-        "ReserveRange": int,
-    },
-    total=False,
-)
-
 ArcAxisConfigurationTypeDef = TypedDict(
     "ArcAxisConfigurationTypeDef",
     {
         "Range": ArcAxisDisplayRangeTypeDef,
         "ReserveRange": int,
     },
     total=False,
 )
 
 AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef = TypedDict(
     "AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef",
     {
         "ResourceIdOverrideConfiguration": (
-            AssetBundleExportJobResourceIdOverrideConfigurationOutputTypeDef
+            AssetBundleExportJobResourceIdOverrideConfigurationTypeDef
         ),
         "VPCConnections": List[AssetBundleExportJobVPCConnectionOverridePropertiesOutputTypeDef],
         "RefreshSchedules": List[
             AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef
         ],
         "DataSources": List[AssetBundleExportJobDataSourceOverridePropertiesOutputTypeDef],
         "DataSets": List[AssetBundleExportJobDataSetOverridePropertiesOutputTypeDef],
@@ -9019,130 +6971,83 @@
         "Themes": Sequence[AssetBundleExportJobThemeOverridePropertiesTypeDef],
         "Analyses": Sequence[AssetBundleExportJobAnalysisOverridePropertiesTypeDef],
         "Dashboards": Sequence[AssetBundleExportJobDashboardOverridePropertiesTypeDef],
     },
     total=False,
 )
 
-AssetBundleImportJobDataSourceCredentialsOutputTypeDef = TypedDict(
-    "AssetBundleImportJobDataSourceCredentialsOutputTypeDef",
-    {
-        "CredentialPair": AssetBundleImportJobDataSourceCredentialPairOutputTypeDef,
-        "SecretArn": str,
-    },
-    total=False,
-)
-
 AssetBundleImportJobDataSourceCredentialsTypeDef = TypedDict(
     "AssetBundleImportJobDataSourceCredentialsTypeDef",
     {
         "CredentialPair": AssetBundleImportJobDataSourceCredentialPairTypeDef,
         "SecretArn": str,
     },
     total=False,
 )
 
 AxisDisplayRangeOutputTypeDef = TypedDict(
     "AxisDisplayRangeOutputTypeDef",
     {
-        "MinMax": AxisDisplayMinMaxRangeOutputTypeDef,
+        "MinMax": AxisDisplayMinMaxRangeTypeDef,
         "DataDriven": Dict[str, Any],
     },
     total=False,
 )
 
 AxisDisplayRangeTypeDef = TypedDict(
     "AxisDisplayRangeTypeDef",
     {
         "MinMax": AxisDisplayMinMaxRangeTypeDef,
         "DataDriven": Mapping[str, Any],
     },
     total=False,
 )
 
-AxisScaleOutputTypeDef = TypedDict(
-    "AxisScaleOutputTypeDef",
-    {
-        "Linear": AxisLinearScaleOutputTypeDef,
-        "Logarithmic": AxisLogarithmicScaleOutputTypeDef,
-    },
-    total=False,
-)
-
 AxisScaleTypeDef = TypedDict(
     "AxisScaleTypeDef",
     {
         "Linear": AxisLinearScaleTypeDef,
         "Logarithmic": AxisLogarithmicScaleTypeDef,
     },
     total=False,
 )
 
-HistogramBinOptionsOutputTypeDef = TypedDict(
-    "HistogramBinOptionsOutputTypeDef",
-    {
-        "SelectedBinType": HistogramBinTypeType,
-        "BinCount": BinCountOptionsOutputTypeDef,
-        "BinWidth": BinWidthOptionsOutputTypeDef,
-        "StartValue": float,
-    },
-    total=False,
-)
-
 HistogramBinOptionsTypeDef = TypedDict(
     "HistogramBinOptionsTypeDef",
     {
         "SelectedBinType": HistogramBinTypeType,
         "BinCount": BinCountOptionsTypeDef,
         "BinWidth": BinWidthOptionsTypeDef,
         "StartValue": float,
     },
     total=False,
 )
 
-TileStyleOutputTypeDef = TypedDict(
-    "TileStyleOutputTypeDef",
-    {
-        "Border": BorderStyleOutputTypeDef,
-    },
-    total=False,
-)
-
 TileStyleTypeDef = TypedDict(
     "TileStyleTypeDef",
     {
         "Border": BorderStyleTypeDef,
     },
     total=False,
 )
 
-BoxPlotOptionsOutputTypeDef = TypedDict(
-    "BoxPlotOptionsOutputTypeDef",
-    {
-        "StyleOptions": BoxPlotStyleOptionsOutputTypeDef,
-        "OutlierVisibility": VisibilityType,
-        "AllDataPointsVisibility": VisibilityType,
-    },
-    total=False,
-)
-
 BoxPlotOptionsTypeDef = TypedDict(
     "BoxPlotOptionsTypeDef",
     {
         "StyleOptions": BoxPlotStyleOptionsTypeDef,
         "OutlierVisibility": VisibilityType,
         "AllDataPointsVisibility": VisibilityType,
     },
     total=False,
 )
 
 CreateColumnsOperationOutputTypeDef = TypedDict(
     "CreateColumnsOperationOutputTypeDef",
     {
-        "Columns": List[CalculatedColumnOutputTypeDef],
+        "Columns": List[CalculatedColumnTypeDef],
     },
 )
 
 CreateColumnsOperationTypeDef = TypedDict(
     "CreateColumnsOperationTypeDef",
     {
         "Columns": Sequence[CalculatedColumnTypeDef],
@@ -9162,15 +7067,15 @@
 
 CreateAccountCustomizationResponseTypeDef = TypedDict(
     "CreateAccountCustomizationResponseTypeDef",
     {
         "Arn": str,
         "AwsAccountId": str,
         "Namespace": str,
-        "AccountCustomization": AccountCustomizationOutputTypeDef,
+        "AccountCustomization": AccountCustomizationTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAnalysisResponseTypeDef = TypedDict(
@@ -9590,15 +7495,15 @@
 
 DescribeAccountCustomizationResponseTypeDef = TypedDict(
     "DescribeAccountCustomizationResponseTypeDef",
     {
         "Arn": str,
         "AwsAccountId": str,
         "Namespace": str,
-        "AccountCustomization": AccountCustomizationOutputTypeDef,
+        "AccountCustomization": AccountCustomizationTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountSettingsResponseTypeDef = TypedDict(
@@ -9802,15 +7707,15 @@
 
 UpdateAccountCustomizationResponseTypeDef = TypedDict(
     "UpdateAccountCustomizationResponseTypeDef",
     {
         "Arn": str,
         "AwsAccountId": str,
         "Namespace": str,
-        "AccountCustomization": AccountCustomizationOutputTypeDef,
+        "AccountCustomization": AccountCustomizationTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountSettingsResponseTypeDef = TypedDict(
@@ -10024,37 +7929,29 @@
 )
 
 CategoryFilterConfigurationOutputTypeDef = TypedDict(
     "CategoryFilterConfigurationOutputTypeDef",
     {
         "FilterListConfiguration": FilterListConfigurationOutputTypeDef,
         "CustomFilterListConfiguration": CustomFilterListConfigurationOutputTypeDef,
-        "CustomFilterConfiguration": CustomFilterConfigurationOutputTypeDef,
+        "CustomFilterConfiguration": CustomFilterConfigurationTypeDef,
     },
     total=False,
 )
 
 CategoryFilterConfigurationTypeDef = TypedDict(
     "CategoryFilterConfigurationTypeDef",
     {
         "FilterListConfiguration": FilterListConfigurationTypeDef,
         "CustomFilterListConfiguration": CustomFilterListConfigurationTypeDef,
         "CustomFilterConfiguration": CustomFilterConfigurationTypeDef,
     },
     total=False,
 )
 
-ClusterMarkerOutputTypeDef = TypedDict(
-    "ClusterMarkerOutputTypeDef",
-    {
-        "SimpleClusterMarker": SimpleClusterMarkerOutputTypeDef,
-    },
-    total=False,
-)
-
 ClusterMarkerTypeDef = TypedDict(
     "ClusterMarkerTypeDef",
     {
         "SimpleClusterMarker": SimpleClusterMarkerTypeDef,
     },
     total=False,
 )
@@ -10078,22 +7975,22 @@
     },
     total=False,
 )
 
 _RequiredColorScaleOutputTypeDef = TypedDict(
     "_RequiredColorScaleOutputTypeDef",
     {
-        "Colors": List[DataColorOutputTypeDef],
+        "Colors": List[DataColorTypeDef],
         "ColorFillType": ColorFillTypeType,
     },
 )
 _OptionalColorScaleOutputTypeDef = TypedDict(
     "_OptionalColorScaleOutputTypeDef",
     {
-        "NullValueColor": DataColorOutputTypeDef,
+        "NullValueColor": DataColorTypeDef,
     },
     total=False,
 )
 
 class ColorScaleOutputTypeDef(_RequiredColorScaleOutputTypeDef, _OptionalColorScaleOutputTypeDef):
     pass
 
@@ -10114,50 +8011,41 @@
 
 class ColorScaleTypeDef(_RequiredColorScaleTypeDef, _OptionalColorScaleTypeDef):
     pass
 
 ColorsConfigurationOutputTypeDef = TypedDict(
     "ColorsConfigurationOutputTypeDef",
     {
-        "CustomColors": List[CustomColorOutputTypeDef],
+        "CustomColors": List[CustomColorTypeDef],
     },
     total=False,
 )
 
 ColorsConfigurationTypeDef = TypedDict(
     "ColorsConfigurationTypeDef",
     {
         "CustomColors": Sequence[CustomColorTypeDef],
     },
     total=False,
 )
 
-ColumnTagOutputTypeDef = TypedDict(
-    "ColumnTagOutputTypeDef",
-    {
-        "ColumnGeographicRole": GeoSpatialDataRoleType,
-        "ColumnDescription": ColumnDescriptionOutputTypeDef,
-    },
-    total=False,
-)
-
 ColumnTagTypeDef = TypedDict(
     "ColumnTagTypeDef",
     {
         "ColumnGeographicRole": GeoSpatialDataRoleType,
         "ColumnDescription": ColumnDescriptionTypeDef,
     },
     total=False,
 )
 
 ColumnGroupSchemaOutputTypeDef = TypedDict(
     "ColumnGroupSchemaOutputTypeDef",
     {
         "Name": str,
-        "ColumnGroupColumnSchemaList": List[ColumnGroupColumnSchemaOutputTypeDef],
+        "ColumnGroupColumnSchemaList": List[ColumnGroupColumnSchemaTypeDef],
     },
     total=False,
 )
 
 ColumnGroupSchemaTypeDef = TypedDict(
     "ColumnGroupSchemaTypeDef",
     {
@@ -10182,49 +8070,27 @@
     },
     total=False,
 )
 
 DataSetSchemaOutputTypeDef = TypedDict(
     "DataSetSchemaOutputTypeDef",
     {
-        "ColumnSchemaList": List[ColumnSchemaOutputTypeDef],
+        "ColumnSchemaList": List[ColumnSchemaTypeDef],
     },
     total=False,
 )
 
 DataSetSchemaTypeDef = TypedDict(
     "DataSetSchemaTypeDef",
     {
         "ColumnSchemaList": Sequence[ColumnSchemaTypeDef],
     },
     total=False,
 )
 
-_RequiredConditionalFormattingCustomIconConditionOutputTypeDef = TypedDict(
-    "_RequiredConditionalFormattingCustomIconConditionOutputTypeDef",
-    {
-        "Expression": str,
-        "IconOptions": ConditionalFormattingCustomIconOptionsOutputTypeDef,
-    },
-)
-_OptionalConditionalFormattingCustomIconConditionOutputTypeDef = TypedDict(
-    "_OptionalConditionalFormattingCustomIconConditionOutputTypeDef",
-    {
-        "Color": str,
-        "DisplayConfiguration": ConditionalFormattingIconDisplayConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class ConditionalFormattingCustomIconConditionOutputTypeDef(
-    _RequiredConditionalFormattingCustomIconConditionOutputTypeDef,
-    _OptionalConditionalFormattingCustomIconConditionOutputTypeDef,
-):
-    pass
-
 _RequiredConditionalFormattingCustomIconConditionTypeDef = TypedDict(
     "_RequiredConditionalFormattingCustomIconConditionTypeDef",
     {
         "Expression": str,
         "IconOptions": ConditionalFormattingCustomIconOptionsTypeDef,
     },
 )
@@ -10308,14 +8174,24 @@
 
 class CreateVPCConnectionRequestRequestTypeDef(
     _RequiredCreateVPCConnectionRequestRequestTypeDef,
     _OptionalCreateVPCConnectionRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "RequestId": str,
+        "Status": int,
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
@@ -10528,14 +8404,30 @@
 
 class UpdateTopicPermissionsRequestRequestTypeDef(
     _RequiredUpdateTopicPermissionsRequestRequestTypeDef,
     _OptionalUpdateTopicPermissionsRequestRequestTypeDef,
 ):
     pass
 
+DataSetSummaryTypeDef = TypedDict(
+    "DataSetSummaryTypeDef",
+    {
+        "Arn": str,
+        "DataSetId": str,
+        "Name": str,
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "ImportMode": DataSetImportModeType,
+        "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
+        "RowLevelPermissionTagConfigurationApplied": bool,
+        "ColumnLevelPermissionRulesApplied": bool,
+    },
+    total=False,
+)
+
 CreateFolderMembershipResponseTypeDef = TypedDict(
     "CreateFolderMembershipResponseTypeDef",
     {
         "Status": int,
         "FolderMember": FolderMemberTypeDef,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -10747,22 +8639,14 @@
         "AwsAccountId": str,
         "TopicId": str,
         "DatasetId": str,
         "RefreshSchedule": TopicRefreshScheduleTypeDef,
     },
 )
 
-CustomActionNavigationOperationOutputTypeDef = TypedDict(
-    "CustomActionNavigationOperationOutputTypeDef",
-    {
-        "LocalNavigationConfiguration": LocalNavigationConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 CustomActionNavigationOperationTypeDef = TypedDict(
     "CustomActionNavigationOperationTypeDef",
     {
         "LocalNavigationConfiguration": LocalNavigationConfigurationTypeDef,
     },
     total=False,
 )
@@ -10812,61 +8696,61 @@
         "Name": str,
         "SqlQuery": str,
     },
 )
 _OptionalCustomSqlOutputTypeDef = TypedDict(
     "_OptionalCustomSqlOutputTypeDef",
     {
-        "Columns": List[InputColumnOutputTypeDef],
+        "Columns": List[InputColumnTypeDef],
     },
     total=False,
 )
 
 class CustomSqlOutputTypeDef(_RequiredCustomSqlOutputTypeDef, _OptionalCustomSqlOutputTypeDef):
     pass
 
-_RequiredRelationalTableOutputTypeDef = TypedDict(
-    "_RequiredRelationalTableOutputTypeDef",
+_RequiredCustomSqlTypeDef = TypedDict(
+    "_RequiredCustomSqlTypeDef",
     {
         "DataSourceArn": str,
         "Name": str,
-        "InputColumns": List[InputColumnOutputTypeDef],
+        "SqlQuery": str,
     },
 )
-_OptionalRelationalTableOutputTypeDef = TypedDict(
-    "_OptionalRelationalTableOutputTypeDef",
+_OptionalCustomSqlTypeDef = TypedDict(
+    "_OptionalCustomSqlTypeDef",
     {
-        "Catalog": str,
-        "Schema": str,
+        "Columns": Sequence[InputColumnTypeDef],
     },
     total=False,
 )
 
-class RelationalTableOutputTypeDef(
-    _RequiredRelationalTableOutputTypeDef, _OptionalRelationalTableOutputTypeDef
-):
+class CustomSqlTypeDef(_RequiredCustomSqlTypeDef, _OptionalCustomSqlTypeDef):
     pass
 
-_RequiredCustomSqlTypeDef = TypedDict(
-    "_RequiredCustomSqlTypeDef",
+_RequiredRelationalTableOutputTypeDef = TypedDict(
+    "_RequiredRelationalTableOutputTypeDef",
     {
         "DataSourceArn": str,
         "Name": str,
-        "SqlQuery": str,
+        "InputColumns": List[InputColumnTypeDef],
     },
 )
-_OptionalCustomSqlTypeDef = TypedDict(
-    "_OptionalCustomSqlTypeDef",
+_OptionalRelationalTableOutputTypeDef = TypedDict(
+    "_OptionalRelationalTableOutputTypeDef",
     {
-        "Columns": Sequence[InputColumnTypeDef],
+        "Catalog": str,
+        "Schema": str,
     },
     total=False,
 )
 
-class CustomSqlTypeDef(_RequiredCustomSqlTypeDef, _OptionalCustomSqlTypeDef):
+class RelationalTableOutputTypeDef(
+    _RequiredRelationalTableOutputTypeDef, _OptionalRelationalTableOutputTypeDef
+):
     pass
 
 _RequiredRelationalTableTypeDef = TypedDict(
     "_RequiredRelationalTableTypeDef",
     {
         "DataSourceArn": str,
         "Name": str,
@@ -10935,102 +8819,80 @@
         "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DashboardVisualPublishOptionsOutputTypeDef = TypedDict(
-    "DashboardVisualPublishOptionsOutputTypeDef",
-    {
-        "ExportHiddenFieldsOption": ExportHiddenFieldsOptionOutputTypeDef,
-    },
-    total=False,
-)
-
 DashboardVisualPublishOptionsTypeDef = TypedDict(
     "DashboardVisualPublishOptionsTypeDef",
     {
         "ExportHiddenFieldsOption": ExportHiddenFieldsOptionTypeDef,
     },
     total=False,
 )
 
-TableInlineVisualizationOutputTypeDef = TypedDict(
-    "TableInlineVisualizationOutputTypeDef",
-    {
-        "DataBars": DataBarsOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 TableInlineVisualizationTypeDef = TypedDict(
     "TableInlineVisualizationTypeDef",
     {
         "DataBars": DataBarsOptionsTypeDef,
     },
     total=False,
 )
 
-DataLabelTypeOutputTypeDef = TypedDict(
-    "DataLabelTypeOutputTypeDef",
-    {
-        "FieldLabelType": FieldLabelTypeOutputTypeDef,
-        "DataPathLabelType": DataPathLabelTypeOutputTypeDef,
-        "RangeEndsLabelType": RangeEndsLabelTypeOutputTypeDef,
-        "MinimumLabelType": MinimumLabelTypeOutputTypeDef,
-        "MaximumLabelType": MaximumLabelTypeOutputTypeDef,
-    },
-    total=False,
-)
-
 DataLabelTypeTypeDef = TypedDict(
     "DataLabelTypeTypeDef",
     {
         "FieldLabelType": FieldLabelTypeTypeDef,
         "DataPathLabelType": DataPathLabelTypeTypeDef,
         "RangeEndsLabelType": RangeEndsLabelTypeTypeDef,
         "MinimumLabelType": MinimumLabelTypeTypeDef,
         "MaximumLabelType": MaximumLabelTypeTypeDef,
     },
     total=False,
 )
 
-_RequiredDataPathColorOutputTypeDef = TypedDict(
-    "_RequiredDataPathColorOutputTypeDef",
+_RequiredDataPathColorTypeDef = TypedDict(
+    "_RequiredDataPathColorTypeDef",
     {
-        "Element": DataPathValueOutputTypeDef,
+        "Element": DataPathValueTypeDef,
         "Color": str,
     },
 )
-_OptionalDataPathColorOutputTypeDef = TypedDict(
-    "_OptionalDataPathColorOutputTypeDef",
+_OptionalDataPathColorTypeDef = TypedDict(
+    "_OptionalDataPathColorTypeDef",
     {
         "TimeGranularity": TimeGranularityType,
     },
     total=False,
 )
 
-class DataPathColorOutputTypeDef(
-    _RequiredDataPathColorOutputTypeDef, _OptionalDataPathColorOutputTypeDef
-):
+class DataPathColorTypeDef(_RequiredDataPathColorTypeDef, _OptionalDataPathColorTypeDef):
     pass
 
 DataPathSortOutputTypeDef = TypedDict(
     "DataPathSortOutputTypeDef",
     {
         "Direction": SortDirectionType,
-        "SortPaths": List[DataPathValueOutputTypeDef],
+        "SortPaths": List[DataPathValueTypeDef],
+    },
+)
+
+DataPathSortTypeDef = TypedDict(
+    "DataPathSortTypeDef",
+    {
+        "Direction": SortDirectionType,
+        "SortPaths": Sequence[DataPathValueTypeDef],
     },
 )
 
 _RequiredPivotTableDataPathOptionOutputTypeDef = TypedDict(
     "_RequiredPivotTableDataPathOptionOutputTypeDef",
     {
-        "DataPathList": List[DataPathValueOutputTypeDef],
+        "DataPathList": List[DataPathValueTypeDef],
     },
 )
 _OptionalPivotTableDataPathOptionOutputTypeDef = TypedDict(
     "_OptionalPivotTableDataPathOptionOutputTypeDef",
     {
         "Width": str,
     },
@@ -11038,49 +8900,14 @@
 )
 
 class PivotTableDataPathOptionOutputTypeDef(
     _RequiredPivotTableDataPathOptionOutputTypeDef, _OptionalPivotTableDataPathOptionOutputTypeDef
 ):
     pass
 
-PivotTableFieldCollapseStateTargetOutputTypeDef = TypedDict(
-    "PivotTableFieldCollapseStateTargetOutputTypeDef",
-    {
-        "FieldId": str,
-        "FieldDataPathValues": List[DataPathValueOutputTypeDef],
-    },
-    total=False,
-)
-
-_RequiredDataPathColorTypeDef = TypedDict(
-    "_RequiredDataPathColorTypeDef",
-    {
-        "Element": DataPathValueTypeDef,
-        "Color": str,
-    },
-)
-_OptionalDataPathColorTypeDef = TypedDict(
-    "_OptionalDataPathColorTypeDef",
-    {
-        "TimeGranularity": TimeGranularityType,
-    },
-    total=False,
-)
-
-class DataPathColorTypeDef(_RequiredDataPathColorTypeDef, _OptionalDataPathColorTypeDef):
-    pass
-
-DataPathSortTypeDef = TypedDict(
-    "DataPathSortTypeDef",
-    {
-        "Direction": SortDirectionType,
-        "SortPaths": Sequence[DataPathValueTypeDef],
-    },
-)
-
 _RequiredPivotTableDataPathOptionTypeDef = TypedDict(
     "_RequiredPivotTableDataPathOptionTypeDef",
     {
         "DataPathList": Sequence[DataPathValueTypeDef],
     },
 )
 _OptionalPivotTableDataPathOptionTypeDef = TypedDict(
@@ -11092,14 +8919,23 @@
 )
 
 class PivotTableDataPathOptionTypeDef(
     _RequiredPivotTableDataPathOptionTypeDef, _OptionalPivotTableDataPathOptionTypeDef
 ):
     pass
 
+PivotTableFieldCollapseStateTargetOutputTypeDef = TypedDict(
+    "PivotTableFieldCollapseStateTargetOutputTypeDef",
+    {
+        "FieldId": str,
+        "FieldDataPathValues": List[DataPathValueTypeDef],
+    },
+    total=False,
+)
+
 PivotTableFieldCollapseStateTargetTypeDef = TypedDict(
     "PivotTableFieldCollapseStateTargetTypeDef",
     {
         "FieldId": str,
         "FieldDataPathValues": Sequence[DataPathValueTypeDef],
     },
     total=False,
@@ -11122,30 +8958,14 @@
 )
 
 class SearchDataSetsRequestRequestTypeDef(
     _RequiredSearchDataSetsRequestRequestTypeDef, _OptionalSearchDataSetsRequestRequestTypeDef
 ):
     pass
 
-DataSetSummaryTypeDef = TypedDict(
-    "DataSetSummaryTypeDef",
-    {
-        "Arn": str,
-        "DataSetId": str,
-        "Name": str,
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "ImportMode": DataSetImportModeType,
-        "RowLevelPermissionDataSet": RowLevelPermissionDataSetOutputTypeDef,
-        "RowLevelPermissionTagConfigurationApplied": bool,
-        "ColumnLevelPermissionRulesApplied": bool,
-    },
-    total=False,
-)
-
 _RequiredSearchDataSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchDataSourcesRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "Filters": Sequence[DataSourceSearchFilterTypeDef],
     },
 )
@@ -11218,15 +9038,15 @@
 ):
     pass
 
 TimeRangeFilterValueOutputTypeDef = TypedDict(
     "TimeRangeFilterValueOutputTypeDef",
     {
         "StaticValue": datetime,
-        "RollingDate": RollingDateConfigurationOutputTypeDef,
+        "RollingDate": RollingDateConfigurationTypeDef,
         "Parameter": str,
     },
     total=False,
 )
 
 TimeRangeFilterValueTypeDef = TypedDict(
     "TimeRangeFilterValueTypeDef",
@@ -11536,33 +9356,14 @@
         "User": UserTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisplayFormatOptionsOutputTypeDef = TypedDict(
-    "DisplayFormatOptionsOutputTypeDef",
-    {
-        "UseBlankCellFormat": bool,
-        "BlankCellFormat": str,
-        "DateFormat": str,
-        "DecimalSeparator": TopicNumericSeparatorSymbolType,
-        "GroupingSeparator": str,
-        "UseGrouping": bool,
-        "FractionDigits": int,
-        "Prefix": str,
-        "Suffix": str,
-        "UnitScaler": NumberScaleType,
-        "NegativeFormat": NegativeFormatOutputTypeDef,
-        "CurrencySymbol": str,
-    },
-    total=False,
-)
-
 DisplayFormatOptionsTypeDef = TypedDict(
     "DisplayFormatOptionsTypeDef",
     {
         "UseBlankCellFormat": bool,
         "BlankCellFormat": str,
         "DateFormat": str,
         "DecimalSeparator": TopicNumericSeparatorSymbolType,
@@ -11574,59 +9375,23 @@
         "UnitScaler": NumberScaleType,
         "NegativeFormat": NegativeFormatTypeDef,
         "CurrencySymbol": str,
     },
     total=False,
 )
 
-DonutOptionsOutputTypeDef = TypedDict(
-    "DonutOptionsOutputTypeDef",
-    {
-        "ArcOptions": ArcOptionsOutputTypeDef,
-        "DonutCenterOptions": DonutCenterOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 DonutOptionsTypeDef = TypedDict(
     "DonutOptionsTypeDef",
     {
         "ArcOptions": ArcOptionsTypeDef,
         "DonutCenterOptions": DonutCenterOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredRelativeDatesFilterOutputTypeDef = TypedDict(
-    "_RequiredRelativeDatesFilterOutputTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-        "AnchorDateConfiguration": AnchorDateConfigurationOutputTypeDef,
-        "TimeGranularity": TimeGranularityType,
-        "RelativeDateType": RelativeDateTypeType,
-        "NullOption": FilterNullOptionType,
-    },
-)
-_OptionalRelativeDatesFilterOutputTypeDef = TypedDict(
-    "_OptionalRelativeDatesFilterOutputTypeDef",
-    {
-        "MinimumGranularity": TimeGranularityType,
-        "RelativeDateValue": int,
-        "ParameterName": str,
-        "ExcludePeriodConfiguration": ExcludePeriodConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class RelativeDatesFilterOutputTypeDef(
-    _RequiredRelativeDatesFilterOutputTypeDef, _OptionalRelativeDatesFilterOutputTypeDef
-):
-    pass
-
 _RequiredRelativeDatesFilterTypeDef = TypedDict(
     "_RequiredRelativeDatesFilterTypeDef",
     {
         "FilterId": str,
         "Column": ColumnIdentifierTypeDef,
         "AnchorDateConfiguration": AnchorDateConfigurationTypeDef,
         "TimeGranularity": TimeGranularityType,
@@ -11705,26 +9470,14 @@
         "FolderSummaryList": List[FolderSummaryTypeDef],
         "NextToken": str,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FontConfigurationOutputTypeDef = TypedDict(
-    "FontConfigurationOutputTypeDef",
-    {
-        "FontSize": FontSizeOutputTypeDef,
-        "FontDecoration": FontDecorationType,
-        "FontColor": str,
-        "FontWeight": FontWeightOutputTypeDef,
-        "FontStyle": FontStyleType,
-    },
-    total=False,
-)
-
 FontConfigurationTypeDef = TypedDict(
     "FontConfigurationTypeDef",
     {
         "FontSize": FontSizeTypeDef,
         "FontDecoration": FontDecorationType,
         "FontColor": str,
         "FontWeight": FontWeightTypeDef,
@@ -11732,15 +9485,15 @@
     },
     total=False,
 )
 
 TypographyOutputTypeDef = TypedDict(
     "TypographyOutputTypeDef",
     {
-        "FontFamilies": List[FontOutputTypeDef],
+        "FontFamilies": List[FontTypeDef],
     },
     total=False,
 )
 
 TypographyTypeDef = TypedDict(
     "TypographyTypeDef",
     {
@@ -11763,22 +9516,14 @@
     {
         "WhatIfPointScenario": WhatIfPointScenarioTypeDef,
         "WhatIfRangeScenario": WhatIfRangeScenarioTypeDef,
     },
     total=False,
 )
 
-FreeFormLayoutCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "FreeFormLayoutCanvasSizeOptionsOutputTypeDef",
-    {
-        "ScreenCanvasSizeOptions": FreeFormLayoutScreenCanvasSizeOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 FreeFormLayoutCanvasSizeOptionsTypeDef = TypedDict(
     "FreeFormLayoutCanvasSizeOptionsTypeDef",
     {
         "ScreenCanvasSizeOptions": FreeFormLayoutScreenCanvasSizeOptionsTypeDef,
     },
     total=False,
 )
@@ -11787,61 +9532,39 @@
     "SnapshotAnonymousUserTypeDef",
     {
         "RowLevelPermissionTags": Sequence[SessionTagTypeDef],
     },
     total=False,
 )
 
-GeospatialWindowOptionsOutputTypeDef = TypedDict(
-    "GeospatialWindowOptionsOutputTypeDef",
-    {
-        "Bounds": GeospatialCoordinateBoundsOutputTypeDef,
-        "MapZoomMode": MapZoomModeType,
-    },
-    total=False,
-)
-
 GeospatialWindowOptionsTypeDef = TypedDict(
     "GeospatialWindowOptionsTypeDef",
     {
         "Bounds": GeospatialCoordinateBoundsTypeDef,
         "MapZoomMode": MapZoomModeType,
     },
     total=False,
 )
 
 GeospatialHeatmapColorScaleOutputTypeDef = TypedDict(
     "GeospatialHeatmapColorScaleOutputTypeDef",
     {
-        "Colors": List[GeospatialHeatmapDataColorOutputTypeDef],
+        "Colors": List[GeospatialHeatmapDataColorTypeDef],
     },
     total=False,
 )
 
 GeospatialHeatmapColorScaleTypeDef = TypedDict(
     "GeospatialHeatmapColorScaleTypeDef",
     {
         "Colors": Sequence[GeospatialHeatmapDataColorTypeDef],
     },
     total=False,
 )
 
-TableSideBorderOptionsOutputTypeDef = TypedDict(
-    "TableSideBorderOptionsOutputTypeDef",
-    {
-        "InnerVertical": TableBorderOptionsOutputTypeDef,
-        "InnerHorizontal": TableBorderOptionsOutputTypeDef,
-        "Left": TableBorderOptionsOutputTypeDef,
-        "Right": TableBorderOptionsOutputTypeDef,
-        "Top": TableBorderOptionsOutputTypeDef,
-        "Bottom": TableBorderOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 TableSideBorderOptionsTypeDef = TypedDict(
     "TableSideBorderOptionsTypeDef",
     {
         "InnerVertical": TableBorderOptionsTypeDef,
         "InnerHorizontal": TableBorderOptionsTypeDef,
         "Left": TableBorderOptionsTypeDef,
         "Right": TableBorderOptionsTypeDef,
@@ -11850,35 +9573,27 @@
     },
     total=False,
 )
 
 GradientColorOutputTypeDef = TypedDict(
     "GradientColorOutputTypeDef",
     {
-        "Stops": List[GradientStopOutputTypeDef],
+        "Stops": List[GradientStopTypeDef],
     },
     total=False,
 )
 
 GradientColorTypeDef = TypedDict(
     "GradientColorTypeDef",
     {
         "Stops": Sequence[GradientStopTypeDef],
     },
     total=False,
 )
 
-GridLayoutCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "GridLayoutCanvasSizeOptionsOutputTypeDef",
-    {
-        "ScreenCanvasSizeOptions": GridLayoutScreenCanvasSizeOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 GridLayoutCanvasSizeOptionsTypeDef = TypedDict(
     "GridLayoutCanvasSizeOptionsTypeDef",
     {
         "ScreenCanvasSizeOptions": GridLayoutScreenCanvasSizeOptionsTypeDef,
     },
     total=False,
 )
@@ -11912,21 +9627,14 @@
         "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IncrementalRefreshOutputTypeDef = TypedDict(
-    "IncrementalRefreshOutputTypeDef",
-    {
-        "LookbackWindow": LookbackWindowOutputTypeDef,
-    },
-)
-
 IncrementalRefreshTypeDef = TypedDict(
     "IncrementalRefreshTypeDef",
     {
         "LookbackWindow": LookbackWindowTypeDef,
     },
 )
 
@@ -11994,37 +9702,14 @@
 )
 
 class IntegerDatasetParameterTypeDef(
     _RequiredIntegerDatasetParameterTypeDef, _OptionalIntegerDatasetParameterTypeDef
 ):
     pass
 
-_RequiredJoinInstructionOutputTypeDef = TypedDict(
-    "_RequiredJoinInstructionOutputTypeDef",
-    {
-        "LeftOperand": str,
-        "RightOperand": str,
-        "Type": JoinTypeType,
-        "OnClause": str,
-    },
-)
-_OptionalJoinInstructionOutputTypeDef = TypedDict(
-    "_OptionalJoinInstructionOutputTypeDef",
-    {
-        "LeftJoinKeyProperties": JoinKeyPropertiesOutputTypeDef,
-        "RightJoinKeyProperties": JoinKeyPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
-class JoinInstructionOutputTypeDef(
-    _RequiredJoinInstructionOutputTypeDef, _OptionalJoinInstructionOutputTypeDef
-):
-    pass
-
 _RequiredJoinInstructionTypeDef = TypedDict(
     "_RequiredJoinInstructionTypeDef",
     {
         "LeftOperand": str,
         "RightOperand": str,
         "Type": JoinTypeType,
         "OnClause": str,
@@ -12038,33 +9723,14 @@
     },
     total=False,
 )
 
 class JoinInstructionTypeDef(_RequiredJoinInstructionTypeDef, _OptionalJoinInstructionTypeDef):
     pass
 
-LineChartDefaultSeriesSettingsOutputTypeDef = TypedDict(
-    "LineChartDefaultSeriesSettingsOutputTypeDef",
-    {
-        "AxisBinding": AxisBindingType,
-        "LineStyleSettings": LineChartLineStyleSettingsOutputTypeDef,
-        "MarkerStyleSettings": LineChartMarkerStyleSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-LineChartSeriesSettingsOutputTypeDef = TypedDict(
-    "LineChartSeriesSettingsOutputTypeDef",
-    {
-        "LineStyleSettings": LineChartLineStyleSettingsOutputTypeDef,
-        "MarkerStyleSettings": LineChartMarkerStyleSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 LineChartDefaultSeriesSettingsTypeDef = TypedDict(
     "LineChartDefaultSeriesSettingsTypeDef",
     {
         "AxisBinding": AxisBindingType,
         "LineStyleSettings": LineChartLineStyleSettingsTypeDef,
         "MarkerStyleSettings": LineChartMarkerStyleSettingsTypeDef,
     },
@@ -12609,24 +10275,14 @@
         "FolderMemberList": List[MemberIdArnPairTypeDef],
         "NextToken": str,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTemplateVersionsResponseTypeDef = TypedDict(
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionSummaryList": List[TemplateVersionSummaryTypeDef],
         "NextToken": str,
         "Status": int,
         "RequestId": str,
@@ -12674,51 +10330,23 @@
         "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VisualSubtitleLabelOptionsOutputTypeDef = TypedDict(
-    "VisualSubtitleLabelOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "FormatText": LongFormatTextOutputTypeDef,
-    },
-    total=False,
-)
-
 VisualSubtitleLabelOptionsTypeDef = TypedDict(
     "VisualSubtitleLabelOptionsTypeDef",
     {
         "Visibility": VisibilityType,
         "FormatText": LongFormatTextTypeDef,
     },
     total=False,
 )
 
-_RequiredS3ParametersOutputTypeDef = TypedDict(
-    "_RequiredS3ParametersOutputTypeDef",
-    {
-        "ManifestFileLocation": ManifestFileLocationOutputTypeDef,
-    },
-)
-_OptionalS3ParametersOutputTypeDef = TypedDict(
-    "_OptionalS3ParametersOutputTypeDef",
-    {
-        "RoleArn": str,
-    },
-    total=False,
-)
-
-class S3ParametersOutputTypeDef(
-    _RequiredS3ParametersOutputTypeDef, _OptionalS3ParametersOutputTypeDef
-):
-    pass
-
 _RequiredS3ParametersTypeDef = TypedDict(
     "_RequiredS3ParametersTypeDef",
     {
         "ManifestFileLocation": ManifestFileLocationTypeDef,
     },
 )
 _OptionalS3ParametersTypeDef = TypedDict(
@@ -12728,23 +10356,14 @@
     },
     total=False,
 )
 
 class S3ParametersTypeDef(_RequiredS3ParametersTypeDef, _OptionalS3ParametersTypeDef):
     pass
 
-TileLayoutStyleOutputTypeDef = TypedDict(
-    "TileLayoutStyleOutputTypeDef",
-    {
-        "Gutter": GutterStyleOutputTypeDef,
-        "Margin": MarginStyleOutputTypeDef,
-    },
-    total=False,
-)
-
 TileLayoutStyleTypeDef = TypedDict(
     "TileLayoutStyleTypeDef",
     {
         "Gutter": GutterStyleTypeDef,
         "Margin": MarginStyleTypeDef,
     },
     total=False,
@@ -12863,41 +10482,23 @@
 
 class OverrideDatasetParameterOperationTypeDef(
     _RequiredOverrideDatasetParameterOperationTypeDef,
     _OptionalOverrideDatasetParameterOperationTypeDef,
 ):
     pass
 
-NumericSeparatorConfigurationOutputTypeDef = TypedDict(
-    "NumericSeparatorConfigurationOutputTypeDef",
-    {
-        "DecimalSeparator": NumericSeparatorSymbolType,
-        "ThousandsSeparator": ThousandSeparatorOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 NumericSeparatorConfigurationTypeDef = TypedDict(
     "NumericSeparatorConfigurationTypeDef",
     {
         "DecimalSeparator": NumericSeparatorSymbolType,
         "ThousandsSeparator": ThousandSeparatorOptionsTypeDef,
     },
     total=False,
 )
 
-NumericalAggregationFunctionOutputTypeDef = TypedDict(
-    "NumericalAggregationFunctionOutputTypeDef",
-    {
-        "SimpleNumericalAggregation": SimpleNumericalAggregationFunctionType,
-        "PercentileAggregation": PercentileAggregationOutputTypeDef,
-    },
-    total=False,
-)
-
 NumericalAggregationFunctionTypeDef = TypedDict(
     "NumericalAggregationFunctionTypeDef",
     {
         "SimpleNumericalAggregation": SimpleNumericalAggregationFunctionType,
         "PercentileAggregation": PercentileAggregationTypeDef,
     },
     total=False,
@@ -12921,85 +10522,39 @@
         "IntegerParameters": Sequence[IntegerParameterTypeDef],
         "DecimalParameters": Sequence[DecimalParameterTypeDef],
         "DateTimeParameters": Sequence[DateTimeParameterTypeDef],
     },
     total=False,
 )
 
-VisibleRangeOptionsOutputTypeDef = TypedDict(
-    "VisibleRangeOptionsOutputTypeDef",
-    {
-        "PercentRange": PercentVisibleRangeOutputTypeDef,
-    },
-    total=False,
-)
-
 VisibleRangeOptionsTypeDef = TypedDict(
     "VisibleRangeOptionsTypeDef",
     {
         "PercentRange": PercentVisibleRangeTypeDef,
     },
     total=False,
 )
 
-RadarChartSeriesSettingsOutputTypeDef = TypedDict(
-    "RadarChartSeriesSettingsOutputTypeDef",
-    {
-        "AreaStyleSettings": RadarChartAreaStyleSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 RadarChartSeriesSettingsTypeDef = TypedDict(
     "RadarChartSeriesSettingsTypeDef",
     {
         "AreaStyleSettings": RadarChartAreaStyleSettingsTypeDef,
     },
     total=False,
 )
 
-TopicRangeFilterConstantOutputTypeDef = TypedDict(
-    "TopicRangeFilterConstantOutputTypeDef",
-    {
-        "ConstantType": ConstantTypeType,
-        "RangeConstant": RangeConstantOutputTypeDef,
-    },
-    total=False,
-)
-
 TopicRangeFilterConstantTypeDef = TypedDict(
     "TopicRangeFilterConstantTypeDef",
     {
         "ConstantType": ConstantTypeType,
         "RangeConstant": RangeConstantTypeDef,
     },
     total=False,
 )
 
-_RequiredRefreshFrequencyOutputTypeDef = TypedDict(
-    "_RequiredRefreshFrequencyOutputTypeDef",
-    {
-        "Interval": RefreshIntervalType,
-    },
-)
-_OptionalRefreshFrequencyOutputTypeDef = TypedDict(
-    "_OptionalRefreshFrequencyOutputTypeDef",
-    {
-        "RefreshOnDay": ScheduleRefreshOnEntityOutputTypeDef,
-        "Timezone": str,
-        "TimeOfTheDay": str,
-    },
-    total=False,
-)
-
-class RefreshFrequencyOutputTypeDef(
-    _RequiredRefreshFrequencyOutputTypeDef, _OptionalRefreshFrequencyOutputTypeDef
-):
-    pass
-
 _RequiredRefreshFrequencyTypeDef = TypedDict(
     "_RequiredRefreshFrequencyTypeDef",
     {
         "Interval": RefreshIntervalType,
     },
 )
 _OptionalRefreshFrequencyTypeDef = TypedDict(
@@ -13031,15 +10586,15 @@
     },
     total=False,
 )
 
 _RequiredRowLevelPermissionTagConfigurationOutputTypeDef = TypedDict(
     "_RequiredRowLevelPermissionTagConfigurationOutputTypeDef",
     {
-        "TagRules": List[RowLevelPermissionTagRuleOutputTypeDef],
+        "TagRules": List[RowLevelPermissionTagRuleTypeDef],
     },
 )
 _OptionalRowLevelPermissionTagConfigurationOutputTypeDef = TypedDict(
     "_OptionalRowLevelPermissionTagConfigurationOutputTypeDef",
     {
         "Status": StatusType,
         "TagRuleConfigurations": List[List[str]],
@@ -13070,41 +10625,33 @@
 
 class RowLevelPermissionTagConfigurationTypeDef(
     _RequiredRowLevelPermissionTagConfigurationTypeDef,
     _OptionalRowLevelPermissionTagConfigurationTypeDef,
 ):
     pass
 
-SnapshotS3DestinationConfigurationOutputTypeDef = TypedDict(
-    "SnapshotS3DestinationConfigurationOutputTypeDef",
-    {
-        "BucketConfiguration": S3BucketConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 SnapshotS3DestinationConfigurationTypeDef = TypedDict(
     "SnapshotS3DestinationConfigurationTypeDef",
     {
         "BucketConfiguration": S3BucketConfigurationTypeDef,
     },
     total=False,
 )
 
 _RequiredS3SourceOutputTypeDef = TypedDict(
     "_RequiredS3SourceOutputTypeDef",
     {
         "DataSourceArn": str,
-        "InputColumns": List[InputColumnOutputTypeDef],
+        "InputColumns": List[InputColumnTypeDef],
     },
 )
 _OptionalS3SourceOutputTypeDef = TypedDict(
     "_OptionalS3SourceOutputTypeDef",
     {
-        "UploadSettings": UploadSettingsOutputTypeDef,
+        "UploadSettings": UploadSettingsTypeDef,
     },
     total=False,
 )
 
 class S3SourceOutputTypeDef(_RequiredS3SourceOutputTypeDef, _OptionalS3SourceOutputTypeDef):
     pass
 
@@ -13122,49 +10669,22 @@
     },
     total=False,
 )
 
 class S3SourceTypeDef(_RequiredS3SourceTypeDef, _OptionalS3SourceTypeDef):
     pass
 
-SectionPageBreakConfigurationOutputTypeDef = TypedDict(
-    "SectionPageBreakConfigurationOutputTypeDef",
-    {
-        "After": SectionAfterPageBreakOutputTypeDef,
-    },
-    total=False,
-)
-
 SectionPageBreakConfigurationTypeDef = TypedDict(
     "SectionPageBreakConfigurationTypeDef",
     {
         "After": SectionAfterPageBreakTypeDef,
     },
     total=False,
 )
 
-SectionBasedLayoutPaperCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "SectionBasedLayoutPaperCanvasSizeOptionsOutputTypeDef",
-    {
-        "PaperSize": PaperSizeType,
-        "PaperOrientation": PaperOrientationType,
-        "PaperMargin": SpacingOutputTypeDef,
-    },
-    total=False,
-)
-
-SectionStyleOutputTypeDef = TypedDict(
-    "SectionStyleOutputTypeDef",
-    {
-        "Height": str,
-        "Padding": SpacingOutputTypeDef,
-    },
-    total=False,
-)
-
 SectionBasedLayoutPaperCanvasSizeOptionsTypeDef = TypedDict(
     "SectionBasedLayoutPaperCanvasSizeOptionsTypeDef",
     {
         "PaperSize": PaperSizeType,
         "PaperOrientation": PaperOrientationType,
         "PaperMargin": SpacingTypeDef,
     },
@@ -13192,39 +10712,22 @@
     "SelectedSheetsFilterScopeConfigurationTypeDef",
     {
         "SheetVisualScopingConfigurations": Sequence[SheetVisualScopingConfigurationTypeDef],
     },
     total=False,
 )
 
-SheetElementRenderingRuleOutputTypeDef = TypedDict(
-    "SheetElementRenderingRuleOutputTypeDef",
-    {
-        "Expression": str,
-        "ConfigurationOverrides": SheetElementConfigurationOverridesOutputTypeDef,
-    },
-)
-
 SheetElementRenderingRuleTypeDef = TypedDict(
     "SheetElementRenderingRuleTypeDef",
     {
         "Expression": str,
         "ConfigurationOverrides": SheetElementConfigurationOverridesTypeDef,
     },
 )
 
-VisualTitleLabelOptionsOutputTypeDef = TypedDict(
-    "VisualTitleLabelOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "FormatText": ShortFormatTextOutputTypeDef,
-    },
-    total=False,
-)
-
 VisualTitleLabelOptionsTypeDef = TypedDict(
     "VisualTitleLabelOptionsTypeDef",
     {
         "Visibility": VisibilityType,
         "FormatText": ShortFormatTextTypeDef,
     },
     total=False,
@@ -13292,49 +10795,22 @@
 )
 
 class StringDatasetParameterTypeDef(
     _RequiredStringDatasetParameterTypeDef, _OptionalStringDatasetParameterTypeDef
 ):
     pass
 
-TableFieldImageConfigurationOutputTypeDef = TypedDict(
-    "TableFieldImageConfigurationOutputTypeDef",
-    {
-        "SizingOptions": TableCellImageSizingConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 TableFieldImageConfigurationTypeDef = TypedDict(
     "TableFieldImageConfigurationTypeDef",
     {
         "SizingOptions": TableCellImageSizingConfigurationTypeDef,
     },
     total=False,
 )
 
-TopicNumericEqualityFilterOutputTypeDef = TypedDict(
-    "TopicNumericEqualityFilterOutputTypeDef",
-    {
-        "Constant": TopicSingularFilterConstantOutputTypeDef,
-        "Aggregation": NamedFilterAggTypeType,
-    },
-    total=False,
-)
-
-TopicRelativeDateFilterOutputTypeDef = TypedDict(
-    "TopicRelativeDateFilterOutputTypeDef",
-    {
-        "TimeGranularity": TopicTimeGranularityType,
-        "RelativeDateFilterFunction": TopicRelativeDateFilterFunctionType,
-        "Constant": TopicSingularFilterConstantOutputTypeDef,
-    },
-    total=False,
-)
-
 TopicNumericEqualityFilterTypeDef = TypedDict(
     "TopicNumericEqualityFilterTypeDef",
     {
         "Constant": TopicSingularFilterConstantTypeDef,
         "Aggregation": NamedFilterAggTypeType,
     },
     total=False,
@@ -13349,107 +10825,107 @@
     },
     total=False,
 )
 
 CascadingControlConfigurationOutputTypeDef = TypedDict(
     "CascadingControlConfigurationOutputTypeDef",
     {
-        "SourceControls": List[CascadingControlSourceOutputTypeDef],
+        "SourceControls": List[CascadingControlSourceTypeDef],
     },
     total=False,
 )
 
-DateTimeDefaultValuesOutputTypeDef = TypedDict(
-    "DateTimeDefaultValuesOutputTypeDef",
+CascadingControlConfigurationTypeDef = TypedDict(
+    "CascadingControlConfigurationTypeDef",
     {
-        "DynamicValue": DynamicDefaultValueOutputTypeDef,
-        "StaticValues": List[datetime],
-        "RollingDate": RollingDateConfigurationOutputTypeDef,
+        "SourceControls": Sequence[CascadingControlSourceTypeDef],
     },
     total=False,
 )
 
-DecimalDefaultValuesOutputTypeDef = TypedDict(
-    "DecimalDefaultValuesOutputTypeDef",
+DateTimeDefaultValuesOutputTypeDef = TypedDict(
+    "DateTimeDefaultValuesOutputTypeDef",
     {
-        "DynamicValue": DynamicDefaultValueOutputTypeDef,
-        "StaticValues": List[float],
+        "DynamicValue": DynamicDefaultValueTypeDef,
+        "StaticValues": List[datetime],
+        "RollingDate": RollingDateConfigurationTypeDef,
     },
     total=False,
 )
 
-IntegerDefaultValuesOutputTypeDef = TypedDict(
-    "IntegerDefaultValuesOutputTypeDef",
+DateTimeDefaultValuesTypeDef = TypedDict(
+    "DateTimeDefaultValuesTypeDef",
     {
-        "DynamicValue": DynamicDefaultValueOutputTypeDef,
-        "StaticValues": List[int],
+        "DynamicValue": DynamicDefaultValueTypeDef,
+        "StaticValues": Sequence[Union[datetime, str]],
+        "RollingDate": RollingDateConfigurationTypeDef,
     },
     total=False,
 )
 
-StringDefaultValuesOutputTypeDef = TypedDict(
-    "StringDefaultValuesOutputTypeDef",
+DecimalDefaultValuesOutputTypeDef = TypedDict(
+    "DecimalDefaultValuesOutputTypeDef",
     {
-        "DynamicValue": DynamicDefaultValueOutputTypeDef,
-        "StaticValues": List[str],
+        "DynamicValue": DynamicDefaultValueTypeDef,
+        "StaticValues": List[float],
     },
     total=False,
 )
 
-DrillDownFilterOutputTypeDef = TypedDict(
-    "DrillDownFilterOutputTypeDef",
+DecimalDefaultValuesTypeDef = TypedDict(
+    "DecimalDefaultValuesTypeDef",
     {
-        "NumericEqualityFilter": NumericEqualityDrillDownFilterOutputTypeDef,
-        "CategoryFilter": CategoryDrillDownFilterOutputTypeDef,
-        "TimeRangeFilter": TimeRangeDrillDownFilterOutputTypeDef,
+        "DynamicValue": DynamicDefaultValueTypeDef,
+        "StaticValues": Sequence[float],
     },
     total=False,
 )
 
-CascadingControlConfigurationTypeDef = TypedDict(
-    "CascadingControlConfigurationTypeDef",
+IntegerDefaultValuesOutputTypeDef = TypedDict(
+    "IntegerDefaultValuesOutputTypeDef",
     {
-        "SourceControls": Sequence[CascadingControlSourceTypeDef],
+        "DynamicValue": DynamicDefaultValueTypeDef,
+        "StaticValues": List[int],
     },
     total=False,
 )
 
-DateTimeDefaultValuesTypeDef = TypedDict(
-    "DateTimeDefaultValuesTypeDef",
+IntegerDefaultValuesTypeDef = TypedDict(
+    "IntegerDefaultValuesTypeDef",
     {
         "DynamicValue": DynamicDefaultValueTypeDef,
-        "StaticValues": Sequence[Union[datetime, str]],
-        "RollingDate": RollingDateConfigurationTypeDef,
+        "StaticValues": Sequence[int],
     },
     total=False,
 )
 
-DecimalDefaultValuesTypeDef = TypedDict(
-    "DecimalDefaultValuesTypeDef",
+StringDefaultValuesOutputTypeDef = TypedDict(
+    "StringDefaultValuesOutputTypeDef",
     {
         "DynamicValue": DynamicDefaultValueTypeDef,
-        "StaticValues": Sequence[float],
+        "StaticValues": List[str],
     },
     total=False,
 )
 
-IntegerDefaultValuesTypeDef = TypedDict(
-    "IntegerDefaultValuesTypeDef",
+StringDefaultValuesTypeDef = TypedDict(
+    "StringDefaultValuesTypeDef",
     {
         "DynamicValue": DynamicDefaultValueTypeDef,
-        "StaticValues": Sequence[int],
+        "StaticValues": Sequence[str],
     },
     total=False,
 )
 
-StringDefaultValuesTypeDef = TypedDict(
-    "StringDefaultValuesTypeDef",
+DrillDownFilterOutputTypeDef = TypedDict(
+    "DrillDownFilterOutputTypeDef",
     {
-        "DynamicValue": DynamicDefaultValueTypeDef,
-        "StaticValues": Sequence[str],
+        "NumericEqualityFilter": NumericEqualityDrillDownFilterTypeDef,
+        "CategoryFilter": CategoryDrillDownFilterOutputTypeDef,
+        "TimeRangeFilter": TimeRangeDrillDownFilterOutputTypeDef,
     },
     total=False,
 )
 
 DrillDownFilterTypeDef = TypedDict(
     "DrillDownFilterTypeDef",
     {
@@ -13576,15 +11052,15 @@
     _OptionalStartAssetBundleExportJobRequestRequestTypeDef,
 ):
     pass
 
 NumericAxisOptionsOutputTypeDef = TypedDict(
     "NumericAxisOptionsOutputTypeDef",
     {
-        "Scale": AxisScaleOutputTypeDef,
+        "Scale": AxisScaleTypeDef,
         "Range": AxisDisplayRangeOutputTypeDef,
     },
     total=False,
 )
 
 NumericAxisOptionsTypeDef = TypedDict(
     "NumericAxisOptionsTypeDef",
@@ -13595,36 +11071,28 @@
     total=False,
 )
 
 CategoryFilterOutputTypeDef = TypedDict(
     "CategoryFilterOutputTypeDef",
     {
         "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
+        "Column": ColumnIdentifierTypeDef,
         "Configuration": CategoryFilterConfigurationOutputTypeDef,
     },
 )
 
 CategoryFilterTypeDef = TypedDict(
     "CategoryFilterTypeDef",
     {
         "FilterId": str,
         "Column": ColumnIdentifierTypeDef,
         "Configuration": CategoryFilterConfigurationTypeDef,
     },
 )
 
-ClusterMarkerConfigurationOutputTypeDef = TypedDict(
-    "ClusterMarkerConfigurationOutputTypeDef",
-    {
-        "ClusterMarker": ClusterMarkerOutputTypeDef,
-    },
-    total=False,
-)
-
 ClusterMarkerConfigurationTypeDef = TypedDict(
     "ClusterMarkerConfigurationTypeDef",
     {
         "ClusterMarker": ClusterMarkerTypeDef,
     },
     total=False,
 )
@@ -13651,15 +11119,15 @@
     total=False,
 )
 
 TagColumnOperationOutputTypeDef = TypedDict(
     "TagColumnOperationOutputTypeDef",
     {
         "ColumnName": str,
-        "Tags": List[ColumnTagOutputTypeDef],
+        "Tags": List[ColumnTagTypeDef],
     },
 )
 
 TagColumnOperationTypeDef = TypedDict(
     "TagColumnOperationTypeDef",
     {
         "ColumnName": str,
@@ -13683,40 +11151,53 @@
         "Placeholder": str,
         "DataSetSchema": DataSetSchemaTypeDef,
         "ColumnGroupSchemaList": Sequence[ColumnGroupSchemaTypeDef],
     },
     total=False,
 )
 
-ConditionalFormattingIconOutputTypeDef = TypedDict(
-    "ConditionalFormattingIconOutputTypeDef",
-    {
-        "IconSet": ConditionalFormattingIconSetOutputTypeDef,
-        "CustomCondition": ConditionalFormattingCustomIconConditionOutputTypeDef,
-    },
-    total=False,
-)
-
 ConditionalFormattingIconTypeDef = TypedDict(
     "ConditionalFormattingIconTypeDef",
     {
         "IconSet": ConditionalFormattingIconSetTypeDef,
         "CustomCondition": ConditionalFormattingCustomIconConditionTypeDef,
     },
     total=False,
 )
 
+ListDataSetsResponseTypeDef = TypedDict(
+    "ListDataSetsResponseTypeDef",
+    {
+        "DataSetSummaries": List[DataSetSummaryTypeDef],
+        "NextToken": str,
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchDataSetsResponseTypeDef = TypedDict(
+    "SearchDataSetsResponseTypeDef",
+    {
+        "DataSetSummaries": List[DataSetSummaryTypeDef],
+        "NextToken": str,
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DestinationParameterValueConfigurationOutputTypeDef = TypedDict(
     "DestinationParameterValueConfigurationOutputTypeDef",
     {
         "CustomValuesConfiguration": CustomValuesConfigurationOutputTypeDef,
         "SelectAllValueOptions": Literal["ALL_VALUES"],
         "SourceParameterName": str,
         "SourceField": str,
-        "SourceColumn": ColumnIdentifierOutputTypeDef,
+        "SourceColumn": ColumnIdentifierTypeDef,
     },
     total=False,
 )
 
 DestinationParameterValueConfigurationTypeDef = TypedDict(
     "DestinationParameterValueConfigurationTypeDef",
     {
@@ -13725,32 +11206,14 @@
         "SourceParameterName": str,
         "SourceField": str,
         "SourceColumn": ColumnIdentifierTypeDef,
     },
     total=False,
 )
 
-DashboardPublishOptionsOutputTypeDef = TypedDict(
-    "DashboardPublishOptionsOutputTypeDef",
-    {
-        "AdHocFilteringOption": AdHocFilteringOptionOutputTypeDef,
-        "ExportToCSVOption": ExportToCSVOptionOutputTypeDef,
-        "SheetControlsOption": SheetControlsOptionOutputTypeDef,
-        "VisualPublishOptions": DashboardVisualPublishOptionsOutputTypeDef,
-        "SheetLayoutElementMaximizationOption": SheetLayoutElementMaximizationOptionOutputTypeDef,
-        "VisualMenuOption": VisualMenuOptionOutputTypeDef,
-        "VisualAxisSortOption": VisualAxisSortOptionOutputTypeDef,
-        "ExportWithHiddenFieldsOption": ExportWithHiddenFieldsOptionOutputTypeDef,
-        "DataPointDrillUpDownOption": DataPointDrillUpDownOptionOutputTypeDef,
-        "DataPointMenuLabelOption": DataPointMenuLabelOptionOutputTypeDef,
-        "DataPointTooltipOption": DataPointTooltipOptionOutputTypeDef,
-    },
-    total=False,
-)
-
 DashboardPublishOptionsTypeDef = TypedDict(
     "DashboardPublishOptionsTypeDef",
     {
         "AdHocFilteringOption": AdHocFilteringOptionTypeDef,
         "ExportToCSVOption": ExportToCSVOptionTypeDef,
         "SheetControlsOption": SheetControlsOptionTypeDef,
         "VisualPublishOptions": DashboardVisualPublishOptionsTypeDef,
@@ -13765,15 +11228,24 @@
     total=False,
 )
 
 VisualPaletteOutputTypeDef = TypedDict(
     "VisualPaletteOutputTypeDef",
     {
         "ChartColor": str,
-        "ColorMap": List[DataPathColorOutputTypeDef],
+        "ColorMap": List[DataPathColorTypeDef],
+    },
+    total=False,
+)
+
+VisualPaletteTypeDef = TypedDict(
+    "VisualPaletteTypeDef",
+    {
+        "ChartColor": str,
+        "ColorMap": Sequence[DataPathColorTypeDef],
     },
     total=False,
 )
 
 _RequiredPivotTableFieldCollapseStateOptionOutputTypeDef = TypedDict(
     "_RequiredPivotTableFieldCollapseStateOptionOutputTypeDef",
     {
@@ -13790,23 +11262,14 @@
 
 class PivotTableFieldCollapseStateOptionOutputTypeDef(
     _RequiredPivotTableFieldCollapseStateOptionOutputTypeDef,
     _OptionalPivotTableFieldCollapseStateOptionOutputTypeDef,
 ):
     pass
 
-VisualPaletteTypeDef = TypedDict(
-    "VisualPaletteTypeDef",
-    {
-        "ChartColor": str,
-        "ColorMap": Sequence[DataPathColorTypeDef],
-    },
-    total=False,
-)
-
 _RequiredPivotTableFieldCollapseStateOptionTypeDef = TypedDict(
     "_RequiredPivotTableFieldCollapseStateOptionTypeDef",
     {
         "Target": PivotTableFieldCollapseStateTargetTypeDef,
     },
 )
 _OptionalPivotTableFieldCollapseStateOptionTypeDef = TypedDict(
@@ -13819,52 +11282,30 @@
 
 class PivotTableFieldCollapseStateOptionTypeDef(
     _RequiredPivotTableFieldCollapseStateOptionTypeDef,
     _OptionalPivotTableFieldCollapseStateOptionTypeDef,
 ):
     pass
 
-ListDataSetsResponseTypeDef = TypedDict(
-    "ListDataSetsResponseTypeDef",
-    {
-        "DataSetSummaries": List[DataSetSummaryTypeDef],
-        "NextToken": str,
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SearchDataSetsResponseTypeDef = TypedDict(
-    "SearchDataSetsResponseTypeDef",
-    {
-        "DataSetSummaries": List[DataSetSummaryTypeDef],
-        "NextToken": str,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredTimeRangeFilterOutputTypeDef = TypedDict(
     "_RequiredTimeRangeFilterOutputTypeDef",
     {
         "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
+        "Column": ColumnIdentifierTypeDef,
         "NullOption": FilterNullOptionType,
     },
 )
 _OptionalTimeRangeFilterOutputTypeDef = TypedDict(
     "_OptionalTimeRangeFilterOutputTypeDef",
     {
         "IncludeMinimum": bool,
         "IncludeMaximum": bool,
         "RangeMinimumValue": TimeRangeFilterValueOutputTypeDef,
         "RangeMaximumValue": TimeRangeFilterValueOutputTypeDef,
-        "ExcludePeriodConfiguration": ExcludePeriodConfigurationOutputTypeDef,
+        "ExcludePeriodConfiguration": ExcludePeriodConfigurationTypeDef,
         "TimeGranularity": TimeGranularityType,
     },
     total=False,
 )
 
 class TimeRangeFilterOutputTypeDef(
     _RequiredTimeRangeFilterOutputTypeDef, _OptionalTimeRangeFilterOutputTypeDef
@@ -13929,23 +11370,14 @@
         "RefreshSchedules": List[TopicRefreshScheduleSummaryTypeDef],
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DefaultFormattingOutputTypeDef = TypedDict(
-    "DefaultFormattingOutputTypeDef",
-    {
-        "DisplayFormat": DisplayFormatType,
-        "DisplayFormatOptions": DisplayFormatOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 DefaultFormattingTypeDef = TypedDict(
     "DefaultFormattingTypeDef",
     {
         "DisplayFormat": DisplayFormatType,
         "DisplayFormatOptions": DisplayFormatOptionsTypeDef,
     },
     total=False,
@@ -13963,105 +11395,41 @@
     "CustomActionFilterOperationTypeDef",
     {
         "SelectedFieldsConfiguration": FilterOperationSelectedFieldsConfigurationTypeDef,
         "TargetVisualsConfiguration": FilterOperationTargetVisualsConfigurationTypeDef,
     },
 )
 
-AxisLabelOptionsOutputTypeDef = TypedDict(
-    "AxisLabelOptionsOutputTypeDef",
+AxisLabelOptionsTypeDef = TypedDict(
+    "AxisLabelOptionsTypeDef",
     {
-        "FontConfiguration": FontConfigurationOutputTypeDef,
+        "FontConfiguration": FontConfigurationTypeDef,
         "CustomLabel": str,
-        "ApplyTo": AxisLabelReferenceOptionsOutputTypeDef,
+        "ApplyTo": AxisLabelReferenceOptionsTypeDef,
     },
     total=False,
 )
 
 DataLabelOptionsOutputTypeDef = TypedDict(
     "DataLabelOptionsOutputTypeDef",
     {
         "Visibility": VisibilityType,
         "CategoryLabelVisibility": VisibilityType,
         "MeasureLabelVisibility": VisibilityType,
-        "DataLabelTypes": List[DataLabelTypeOutputTypeDef],
+        "DataLabelTypes": List[DataLabelTypeTypeDef],
         "Position": DataLabelPositionType,
         "LabelContent": DataLabelContentType,
-        "LabelFontConfiguration": FontConfigurationOutputTypeDef,
+        "LabelFontConfiguration": FontConfigurationTypeDef,
         "LabelColor": str,
         "Overlap": DataLabelOverlapType,
         "TotalsVisibility": VisibilityType,
     },
     total=False,
 )
 
-FunnelChartDataLabelOptionsOutputTypeDef = TypedDict(
-    "FunnelChartDataLabelOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "CategoryLabelVisibility": VisibilityType,
-        "MeasureLabelVisibility": VisibilityType,
-        "Position": DataLabelPositionType,
-        "LabelFontConfiguration": FontConfigurationOutputTypeDef,
-        "LabelColor": str,
-        "MeasureDataLabelStyle": FunnelChartMeasureDataLabelStyleType,
-    },
-    total=False,
-)
-
-LabelOptionsOutputTypeDef = TypedDict(
-    "LabelOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "FontConfiguration": FontConfigurationOutputTypeDef,
-        "CustomLabel": str,
-    },
-    total=False,
-)
-
-PanelTitleOptionsOutputTypeDef = TypedDict(
-    "PanelTitleOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "FontConfiguration": FontConfigurationOutputTypeDef,
-        "HorizontalTextAlignment": HorizontalTextAlignmentType,
-    },
-    total=False,
-)
-
-_RequiredTableFieldCustomTextContentOutputTypeDef = TypedDict(
-    "_RequiredTableFieldCustomTextContentOutputTypeDef",
-    {
-        "FontConfiguration": FontConfigurationOutputTypeDef,
-    },
-)
-_OptionalTableFieldCustomTextContentOutputTypeDef = TypedDict(
-    "_OptionalTableFieldCustomTextContentOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-class TableFieldCustomTextContentOutputTypeDef(
-    _RequiredTableFieldCustomTextContentOutputTypeDef,
-    _OptionalTableFieldCustomTextContentOutputTypeDef,
-):
-    pass
-
-AxisLabelOptionsTypeDef = TypedDict(
-    "AxisLabelOptionsTypeDef",
-    {
-        "FontConfiguration": FontConfigurationTypeDef,
-        "CustomLabel": str,
-        "ApplyTo": AxisLabelReferenceOptionsTypeDef,
-    },
-    total=False,
-)
-
 DataLabelOptionsTypeDef = TypedDict(
     "DataLabelOptionsTypeDef",
     {
         "Visibility": VisibilityType,
         "CategoryLabelVisibility": VisibilityType,
         "MeasureLabelVisibility": VisibilityType,
         "DataLabelTypes": Sequence[DataLabelTypeTypeDef],
@@ -14127,36 +11495,29 @@
     _RequiredTableFieldCustomTextContentTypeDef, _OptionalTableFieldCustomTextContentTypeDef
 ):
     pass
 
 ForecastConfigurationOutputTypeDef = TypedDict(
     "ForecastConfigurationOutputTypeDef",
     {
-        "ForecastProperties": TimeBasedForecastPropertiesOutputTypeDef,
+        "ForecastProperties": TimeBasedForecastPropertiesTypeDef,
         "Scenario": ForecastScenarioOutputTypeDef,
     },
     total=False,
 )
 
 ForecastConfigurationTypeDef = TypedDict(
     "ForecastConfigurationTypeDef",
     {
         "ForecastProperties": TimeBasedForecastPropertiesTypeDef,
         "Scenario": ForecastScenarioTypeDef,
     },
     total=False,
 )
 
-DefaultFreeFormLayoutConfigurationOutputTypeDef = TypedDict(
-    "DefaultFreeFormLayoutConfigurationOutputTypeDef",
-    {
-        "CanvasSizeOptions": FreeFormLayoutCanvasSizeOptionsOutputTypeDef,
-    },
-)
-
 DefaultFreeFormLayoutConfigurationTypeDef = TypedDict(
     "DefaultFreeFormLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": FreeFormLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
@@ -14180,23 +11541,14 @@
     "GeospatialHeatmapConfigurationTypeDef",
     {
         "HeatmapColor": GeospatialHeatmapColorScaleTypeDef,
     },
     total=False,
 )
 
-GlobalTableBorderOptionsOutputTypeDef = TypedDict(
-    "GlobalTableBorderOptionsOutputTypeDef",
-    {
-        "UniformBorder": TableBorderOptionsOutputTypeDef,
-        "SideSpecificBorder": TableSideBorderOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 GlobalTableBorderOptionsTypeDef = TypedDict(
     "GlobalTableBorderOptionsTypeDef",
     {
         "UniformBorder": TableBorderOptionsTypeDef,
         "SideSpecificBorder": TableSideBorderOptionsTypeDef,
     },
     total=False,
@@ -14214,47 +11566,40 @@
     "ConditionalFormattingGradientColorTypeDef",
     {
         "Expression": str,
         "Color": GradientColorTypeDef,
     },
 )
 
-DefaultGridLayoutConfigurationOutputTypeDef = TypedDict(
-    "DefaultGridLayoutConfigurationOutputTypeDef",
+DefaultGridLayoutConfigurationTypeDef = TypedDict(
+    "DefaultGridLayoutConfigurationTypeDef",
     {
-        "CanvasSizeOptions": GridLayoutCanvasSizeOptionsOutputTypeDef,
+        "CanvasSizeOptions": GridLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
 _RequiredGridLayoutConfigurationOutputTypeDef = TypedDict(
     "_RequiredGridLayoutConfigurationOutputTypeDef",
     {
-        "Elements": List[GridLayoutElementOutputTypeDef],
+        "Elements": List[GridLayoutElementTypeDef],
     },
 )
 _OptionalGridLayoutConfigurationOutputTypeDef = TypedDict(
     "_OptionalGridLayoutConfigurationOutputTypeDef",
     {
-        "CanvasSizeOptions": GridLayoutCanvasSizeOptionsOutputTypeDef,
+        "CanvasSizeOptions": GridLayoutCanvasSizeOptionsTypeDef,
     },
     total=False,
 )
 
 class GridLayoutConfigurationOutputTypeDef(
     _RequiredGridLayoutConfigurationOutputTypeDef, _OptionalGridLayoutConfigurationOutputTypeDef
 ):
     pass
 
-DefaultGridLayoutConfigurationTypeDef = TypedDict(
-    "DefaultGridLayoutConfigurationTypeDef",
-    {
-        "CanvasSizeOptions": GridLayoutCanvasSizeOptionsTypeDef,
-    },
-)
-
 _RequiredGridLayoutConfigurationTypeDef = TypedDict(
     "_RequiredGridLayoutConfigurationTypeDef",
     {
         "Elements": Sequence[GridLayoutElementTypeDef],
     },
 )
 _OptionalGridLayoutConfigurationTypeDef = TypedDict(
@@ -14266,21 +11611,14 @@
 )
 
 class GridLayoutConfigurationTypeDef(
     _RequiredGridLayoutConfigurationTypeDef, _OptionalGridLayoutConfigurationTypeDef
 ):
     pass
 
-RefreshConfigurationOutputTypeDef = TypedDict(
-    "RefreshConfigurationOutputTypeDef",
-    {
-        "IncrementalRefresh": IncrementalRefreshOutputTypeDef,
-    },
-)
-
 RefreshConfigurationTypeDef = TypedDict(
     "RefreshConfigurationTypeDef",
     {
         "IncrementalRefresh": IncrementalRefreshTypeDef,
     },
 )
 
@@ -14301,75 +11639,24 @@
         "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LogicalTableSourceOutputTypeDef = TypedDict(
-    "LogicalTableSourceOutputTypeDef",
-    {
-        "JoinInstruction": JoinInstructionOutputTypeDef,
-        "PhysicalTableId": str,
-        "DataSetArn": str,
-    },
-    total=False,
-)
-
 LogicalTableSourceTypeDef = TypedDict(
     "LogicalTableSourceTypeDef",
     {
         "JoinInstruction": JoinInstructionTypeDef,
         "PhysicalTableId": str,
         "DataSetArn": str,
     },
     total=False,
 )
 
-_RequiredDataFieldSeriesItemOutputTypeDef = TypedDict(
-    "_RequiredDataFieldSeriesItemOutputTypeDef",
-    {
-        "FieldId": str,
-        "AxisBinding": AxisBindingType,
-    },
-)
-_OptionalDataFieldSeriesItemOutputTypeDef = TypedDict(
-    "_OptionalDataFieldSeriesItemOutputTypeDef",
-    {
-        "FieldValue": str,
-        "Settings": LineChartSeriesSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-class DataFieldSeriesItemOutputTypeDef(
-    _RequiredDataFieldSeriesItemOutputTypeDef, _OptionalDataFieldSeriesItemOutputTypeDef
-):
-    pass
-
-_RequiredFieldSeriesItemOutputTypeDef = TypedDict(
-    "_RequiredFieldSeriesItemOutputTypeDef",
-    {
-        "FieldId": str,
-        "AxisBinding": AxisBindingType,
-    },
-)
-_OptionalFieldSeriesItemOutputTypeDef = TypedDict(
-    "_OptionalFieldSeriesItemOutputTypeDef",
-    {
-        "Settings": LineChartSeriesSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-class FieldSeriesItemOutputTypeDef(
-    _RequiredFieldSeriesItemOutputTypeDef, _OptionalFieldSeriesItemOutputTypeDef
-):
-    pass
-
 _RequiredDataFieldSeriesItemTypeDef = TypedDict(
     "_RequiredDataFieldSeriesItemTypeDef",
     {
         "FieldId": str,
         "AxisBinding": AxisBindingType,
     },
 )
@@ -14401,44 +11688,14 @@
     },
     total=False,
 )
 
 class FieldSeriesItemTypeDef(_RequiredFieldSeriesItemTypeDef, _OptionalFieldSeriesItemTypeDef):
     pass
 
-DataSourceParametersOutputTypeDef = TypedDict(
-    "DataSourceParametersOutputTypeDef",
-    {
-        "AmazonElasticsearchParameters": AmazonElasticsearchParametersOutputTypeDef,
-        "AthenaParameters": AthenaParametersOutputTypeDef,
-        "AuroraParameters": AuroraParametersOutputTypeDef,
-        "AuroraPostgreSqlParameters": AuroraPostgreSqlParametersOutputTypeDef,
-        "AwsIotAnalyticsParameters": AwsIotAnalyticsParametersOutputTypeDef,
-        "JiraParameters": JiraParametersOutputTypeDef,
-        "MariaDbParameters": MariaDbParametersOutputTypeDef,
-        "MySqlParameters": MySqlParametersOutputTypeDef,
-        "OracleParameters": OracleParametersOutputTypeDef,
-        "PostgreSqlParameters": PostgreSqlParametersOutputTypeDef,
-        "PrestoParameters": PrestoParametersOutputTypeDef,
-        "RdsParameters": RdsParametersOutputTypeDef,
-        "RedshiftParameters": RedshiftParametersOutputTypeDef,
-        "S3Parameters": S3ParametersOutputTypeDef,
-        "ServiceNowParameters": ServiceNowParametersOutputTypeDef,
-        "SnowflakeParameters": SnowflakeParametersOutputTypeDef,
-        "SparkParameters": SparkParametersOutputTypeDef,
-        "SqlServerParameters": SqlServerParametersOutputTypeDef,
-        "TeradataParameters": TeradataParametersOutputTypeDef,
-        "TwitterParameters": TwitterParametersOutputTypeDef,
-        "AmazonOpenSearchParameters": AmazonOpenSearchParametersOutputTypeDef,
-        "ExasolParameters": ExasolParametersOutputTypeDef,
-        "DatabricksParameters": DatabricksParametersOutputTypeDef,
-    },
-    total=False,
-)
-
 DataSourceParametersTypeDef = TypedDict(
     "DataSourceParametersTypeDef",
     {
         "AmazonElasticsearchParameters": AmazonElasticsearchParametersTypeDef,
         "AthenaParameters": AthenaParametersTypeDef,
         "AuroraParameters": AuroraParametersTypeDef,
         "AuroraPostgreSqlParameters": AuroraPostgreSqlParametersTypeDef,
@@ -14461,23 +11718,14 @@
         "AmazonOpenSearchParameters": AmazonOpenSearchParametersTypeDef,
         "ExasolParameters": ExasolParametersTypeDef,
         "DatabricksParameters": DatabricksParametersTypeDef,
     },
     total=False,
 )
 
-SheetStyleOutputTypeDef = TypedDict(
-    "SheetStyleOutputTypeDef",
-    {
-        "Tile": TileStyleOutputTypeDef,
-        "TileLayout": TileLayoutStyleOutputTypeDef,
-    },
-    total=False,
-)
-
 SheetStyleTypeDef = TypedDict(
     "SheetStyleTypeDef",
     {
         "Tile": TileStyleTypeDef,
         "TileLayout": TileLayoutStyleTypeDef,
     },
     total=False,
@@ -14563,56 +11811,14 @@
         "VPCConnection": VPCConnectionTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CurrencyDisplayFormatConfigurationOutputTypeDef = TypedDict(
-    "CurrencyDisplayFormatConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-        "Suffix": str,
-        "SeparatorConfiguration": NumericSeparatorConfigurationOutputTypeDef,
-        "Symbol": str,
-        "DecimalPlacesConfiguration": DecimalPlacesConfigurationOutputTypeDef,
-        "NumberScale": NumberScaleType,
-        "NegativeValueConfiguration": NegativeValueConfigurationOutputTypeDef,
-        "NullValueFormatConfiguration": NullValueFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-NumberDisplayFormatConfigurationOutputTypeDef = TypedDict(
-    "NumberDisplayFormatConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-        "Suffix": str,
-        "SeparatorConfiguration": NumericSeparatorConfigurationOutputTypeDef,
-        "DecimalPlacesConfiguration": DecimalPlacesConfigurationOutputTypeDef,
-        "NumberScale": NumberScaleType,
-        "NegativeValueConfiguration": NegativeValueConfigurationOutputTypeDef,
-        "NullValueFormatConfiguration": NullValueFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-PercentageDisplayFormatConfigurationOutputTypeDef = TypedDict(
-    "PercentageDisplayFormatConfigurationOutputTypeDef",
-    {
-        "Prefix": str,
-        "Suffix": str,
-        "SeparatorConfiguration": NumericSeparatorConfigurationOutputTypeDef,
-        "DecimalPlacesConfiguration": DecimalPlacesConfigurationOutputTypeDef,
-        "NegativeValueConfiguration": NegativeValueConfigurationOutputTypeDef,
-        "NullValueFormatConfiguration": NullValueFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 CurrencyDisplayFormatConfigurationTypeDef = TypedDict(
     "CurrencyDisplayFormatConfigurationTypeDef",
     {
         "Prefix": str,
         "Suffix": str,
         "SeparatorConfiguration": NumericSeparatorConfigurationTypeDef,
         "Symbol": str,
@@ -14647,73 +11853,34 @@
         "DecimalPlacesConfiguration": DecimalPlacesConfigurationTypeDef,
         "NegativeValueConfiguration": NegativeValueConfigurationTypeDef,
         "NullValueFormatConfiguration": NullValueFormatConfigurationTypeDef,
     },
     total=False,
 )
 
-AggregationFunctionOutputTypeDef = TypedDict(
-    "AggregationFunctionOutputTypeDef",
-    {
-        "NumericalAggregationFunction": NumericalAggregationFunctionOutputTypeDef,
-        "CategoricalAggregationFunction": CategoricalAggregationFunctionType,
-        "DateAggregationFunction": DateAggregationFunctionType,
-        "AttributeAggregationFunction": AttributeAggregationFunctionOutputTypeDef,
-    },
-    total=False,
-)
-
 AggregationFunctionTypeDef = TypedDict(
     "AggregationFunctionTypeDef",
     {
         "NumericalAggregationFunction": NumericalAggregationFunctionTypeDef,
         "CategoricalAggregationFunction": CategoricalAggregationFunctionType,
         "DateAggregationFunction": DateAggregationFunctionType,
         "AttributeAggregationFunction": AttributeAggregationFunctionTypeDef,
     },
     total=False,
 )
 
-ScrollBarOptionsOutputTypeDef = TypedDict(
-    "ScrollBarOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "VisibleRange": VisibleRangeOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 ScrollBarOptionsTypeDef = TypedDict(
     "ScrollBarOptionsTypeDef",
     {
         "Visibility": VisibilityType,
         "VisibleRange": VisibleRangeOptionsTypeDef,
     },
     total=False,
 )
 
-TopicDateRangeFilterOutputTypeDef = TypedDict(
-    "TopicDateRangeFilterOutputTypeDef",
-    {
-        "Inclusive": bool,
-        "Constant": TopicRangeFilterConstantOutputTypeDef,
-    },
-    total=False,
-)
-
-TopicNumericRangeFilterOutputTypeDef = TypedDict(
-    "TopicNumericRangeFilterOutputTypeDef",
-    {
-        "Inclusive": bool,
-        "Constant": TopicRangeFilterConstantOutputTypeDef,
-        "Aggregation": NamedFilterAggTypeType,
-    },
-    total=False,
-)
-
 TopicDateRangeFilterTypeDef = TypedDict(
     "TopicDateRangeFilterTypeDef",
     {
         "Inclusive": bool,
         "Constant": TopicRangeFilterConstantTypeDef,
     },
     total=False,
@@ -14729,15 +11896,15 @@
     total=False,
 )
 
 _RequiredRefreshScheduleOutputTypeDef = TypedDict(
     "_RequiredRefreshScheduleOutputTypeDef",
     {
         "ScheduleId": str,
-        "ScheduleFrequency": RefreshFrequencyOutputTypeDef,
+        "ScheduleFrequency": RefreshFrequencyTypeDef,
         "RefreshType": IngestionTypeType,
     },
 )
 _OptionalRefreshScheduleOutputTypeDef = TypedDict(
     "_OptionalRefreshScheduleOutputTypeDef",
     {
         "StartAfterDateTime": datetime,
@@ -14799,33 +11966,33 @@
     _OptionalRegisteredUserDashboardEmbeddingConfigurationTypeDef,
 ):
     pass
 
 SnapshotDestinationConfigurationOutputTypeDef = TypedDict(
     "SnapshotDestinationConfigurationOutputTypeDef",
     {
-        "S3Destinations": List[SnapshotS3DestinationConfigurationOutputTypeDef],
+        "S3Destinations": List[SnapshotS3DestinationConfigurationTypeDef],
     },
     total=False,
 )
 
-SnapshotJobS3ResultTypeDef = TypedDict(
-    "SnapshotJobS3ResultTypeDef",
+SnapshotDestinationConfigurationTypeDef = TypedDict(
+    "SnapshotDestinationConfigurationTypeDef",
     {
-        "S3DestinationConfiguration": SnapshotS3DestinationConfigurationOutputTypeDef,
-        "S3Uri": str,
-        "ErrorInfo": List[SnapshotJobResultErrorInfoTypeDef],
+        "S3Destinations": Sequence[SnapshotS3DestinationConfigurationTypeDef],
     },
     total=False,
 )
 
-SnapshotDestinationConfigurationTypeDef = TypedDict(
-    "SnapshotDestinationConfigurationTypeDef",
+SnapshotJobS3ResultTypeDef = TypedDict(
+    "SnapshotJobS3ResultTypeDef",
     {
-        "S3Destinations": Sequence[SnapshotS3DestinationConfigurationTypeDef],
+        "S3DestinationConfiguration": SnapshotS3DestinationConfigurationTypeDef,
+        "S3Uri": str,
+        "ErrorInfo": List[SnapshotJobResultErrorInfoTypeDef],
     },
     total=False,
 )
 
 PhysicalTableOutputTypeDef = TypedDict(
     "PhysicalTableOutputTypeDef",
     {
@@ -14842,22 +12009,14 @@
         "RelationalTable": RelationalTableTypeDef,
         "CustomSql": CustomSqlTypeDef,
         "S3Source": S3SourceTypeDef,
     },
     total=False,
 )
 
-SectionBasedLayoutCanvasSizeOptionsOutputTypeDef = TypedDict(
-    "SectionBasedLayoutCanvasSizeOptionsOutputTypeDef",
-    {
-        "PaperCanvasSizeOptions": SectionBasedLayoutPaperCanvasSizeOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 SectionBasedLayoutCanvasSizeOptionsTypeDef = TypedDict(
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
     {
         "PaperCanvasSizeOptions": SectionBasedLayoutPaperCanvasSizeOptionsTypeDef,
     },
     total=False,
 )
@@ -14889,19 +12048,19 @@
         "Height": str,
     },
 )
 _OptionalFreeFormLayoutElementOutputTypeDef = TypedDict(
     "_OptionalFreeFormLayoutElementOutputTypeDef",
     {
         "Visibility": VisibilityType,
-        "RenderingRules": List[SheetElementRenderingRuleOutputTypeDef],
-        "BorderStyle": FreeFormLayoutElementBorderStyleOutputTypeDef,
-        "SelectedBorderStyle": FreeFormLayoutElementBorderStyleOutputTypeDef,
-        "BackgroundStyle": FreeFormLayoutElementBackgroundStyleOutputTypeDef,
-        "LoadingAnimation": LoadingAnimationOutputTypeDef,
+        "RenderingRules": List[SheetElementRenderingRuleTypeDef],
+        "BorderStyle": FreeFormLayoutElementBorderStyleTypeDef,
+        "SelectedBorderStyle": FreeFormLayoutElementBorderStyleTypeDef,
+        "BackgroundStyle": FreeFormLayoutElementBackgroundStyleTypeDef,
+        "LoadingAnimation": LoadingAnimationTypeDef,
     },
     total=False,
 )
 
 class FreeFormLayoutElementOutputTypeDef(
     _RequiredFreeFormLayoutElementOutputTypeDef, _OptionalFreeFormLayoutElementOutputTypeDef
 ):
@@ -14982,94 +12141,182 @@
 )
 _OptionalDateTimeParameterDeclarationOutputTypeDef = TypedDict(
     "_OptionalDateTimeParameterDeclarationOutputTypeDef",
     {
         "DefaultValues": DateTimeDefaultValuesOutputTypeDef,
         "TimeGranularity": TimeGranularityType,
         "ValueWhenUnset": DateTimeValueWhenUnsetConfigurationOutputTypeDef,
-        "MappedDataSetParameters": List[MappedDataSetParameterOutputTypeDef],
+        "MappedDataSetParameters": List[MappedDataSetParameterTypeDef],
     },
     total=False,
 )
 
 class DateTimeParameterDeclarationOutputTypeDef(
     _RequiredDateTimeParameterDeclarationOutputTypeDef,
     _OptionalDateTimeParameterDeclarationOutputTypeDef,
 ):
     pass
 
+_RequiredDateTimeParameterDeclarationTypeDef = TypedDict(
+    "_RequiredDateTimeParameterDeclarationTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalDateTimeParameterDeclarationTypeDef = TypedDict(
+    "_OptionalDateTimeParameterDeclarationTypeDef",
+    {
+        "DefaultValues": DateTimeDefaultValuesTypeDef,
+        "TimeGranularity": TimeGranularityType,
+        "ValueWhenUnset": DateTimeValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
+    },
+    total=False,
+)
+
+class DateTimeParameterDeclarationTypeDef(
+    _RequiredDateTimeParameterDeclarationTypeDef, _OptionalDateTimeParameterDeclarationTypeDef
+):
+    pass
+
 _RequiredDecimalParameterDeclarationOutputTypeDef = TypedDict(
     "_RequiredDecimalParameterDeclarationOutputTypeDef",
     {
         "ParameterValueType": ParameterValueTypeType,
         "Name": str,
     },
 )
 _OptionalDecimalParameterDeclarationOutputTypeDef = TypedDict(
     "_OptionalDecimalParameterDeclarationOutputTypeDef",
     {
         "DefaultValues": DecimalDefaultValuesOutputTypeDef,
-        "ValueWhenUnset": DecimalValueWhenUnsetConfigurationOutputTypeDef,
-        "MappedDataSetParameters": List[MappedDataSetParameterOutputTypeDef],
+        "ValueWhenUnset": DecimalValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": List[MappedDataSetParameterTypeDef],
     },
     total=False,
 )
 
 class DecimalParameterDeclarationOutputTypeDef(
     _RequiredDecimalParameterDeclarationOutputTypeDef,
     _OptionalDecimalParameterDeclarationOutputTypeDef,
 ):
     pass
 
+_RequiredDecimalParameterDeclarationTypeDef = TypedDict(
+    "_RequiredDecimalParameterDeclarationTypeDef",
+    {
+        "ParameterValueType": ParameterValueTypeType,
+        "Name": str,
+    },
+)
+_OptionalDecimalParameterDeclarationTypeDef = TypedDict(
+    "_OptionalDecimalParameterDeclarationTypeDef",
+    {
+        "DefaultValues": DecimalDefaultValuesTypeDef,
+        "ValueWhenUnset": DecimalValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
+    },
+    total=False,
+)
+
+class DecimalParameterDeclarationTypeDef(
+    _RequiredDecimalParameterDeclarationTypeDef, _OptionalDecimalParameterDeclarationTypeDef
+):
+    pass
+
 _RequiredIntegerParameterDeclarationOutputTypeDef = TypedDict(
     "_RequiredIntegerParameterDeclarationOutputTypeDef",
     {
         "ParameterValueType": ParameterValueTypeType,
         "Name": str,
     },
 )
 _OptionalIntegerParameterDeclarationOutputTypeDef = TypedDict(
     "_OptionalIntegerParameterDeclarationOutputTypeDef",
     {
         "DefaultValues": IntegerDefaultValuesOutputTypeDef,
-        "ValueWhenUnset": IntegerValueWhenUnsetConfigurationOutputTypeDef,
-        "MappedDataSetParameters": List[MappedDataSetParameterOutputTypeDef],
+        "ValueWhenUnset": IntegerValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": List[MappedDataSetParameterTypeDef],
     },
     total=False,
 )
 
 class IntegerParameterDeclarationOutputTypeDef(
     _RequiredIntegerParameterDeclarationOutputTypeDef,
     _OptionalIntegerParameterDeclarationOutputTypeDef,
 ):
     pass
 
+_RequiredIntegerParameterDeclarationTypeDef = TypedDict(
+    "_RequiredIntegerParameterDeclarationTypeDef",
+    {
+        "ParameterValueType": ParameterValueTypeType,
+        "Name": str,
+    },
+)
+_OptionalIntegerParameterDeclarationTypeDef = TypedDict(
+    "_OptionalIntegerParameterDeclarationTypeDef",
+    {
+        "DefaultValues": IntegerDefaultValuesTypeDef,
+        "ValueWhenUnset": IntegerValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
+    },
+    total=False,
+)
+
+class IntegerParameterDeclarationTypeDef(
+    _RequiredIntegerParameterDeclarationTypeDef, _OptionalIntegerParameterDeclarationTypeDef
+):
+    pass
+
 _RequiredStringParameterDeclarationOutputTypeDef = TypedDict(
     "_RequiredStringParameterDeclarationOutputTypeDef",
     {
         "ParameterValueType": ParameterValueTypeType,
         "Name": str,
     },
 )
 _OptionalStringParameterDeclarationOutputTypeDef = TypedDict(
     "_OptionalStringParameterDeclarationOutputTypeDef",
     {
         "DefaultValues": StringDefaultValuesOutputTypeDef,
-        "ValueWhenUnset": StringValueWhenUnsetConfigurationOutputTypeDef,
-        "MappedDataSetParameters": List[MappedDataSetParameterOutputTypeDef],
+        "ValueWhenUnset": StringValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": List[MappedDataSetParameterTypeDef],
     },
     total=False,
 )
 
 class StringParameterDeclarationOutputTypeDef(
     _RequiredStringParameterDeclarationOutputTypeDef,
     _OptionalStringParameterDeclarationOutputTypeDef,
 ):
     pass
 
+_RequiredStringParameterDeclarationTypeDef = TypedDict(
+    "_RequiredStringParameterDeclarationTypeDef",
+    {
+        "ParameterValueType": ParameterValueTypeType,
+        "Name": str,
+    },
+)
+_OptionalStringParameterDeclarationTypeDef = TypedDict(
+    "_OptionalStringParameterDeclarationTypeDef",
+    {
+        "DefaultValues": StringDefaultValuesTypeDef,
+        "ValueWhenUnset": StringValueWhenUnsetConfigurationTypeDef,
+        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
+    },
+    total=False,
+)
+
+class StringParameterDeclarationTypeDef(
+    _RequiredStringParameterDeclarationTypeDef, _OptionalStringParameterDeclarationTypeDef
+):
+    pass
+
 _RequiredDateTimeHierarchyOutputTypeDef = TypedDict(
     "_RequiredDateTimeHierarchyOutputTypeDef",
     {
         "HierarchyId": str,
     },
 )
 _OptionalDateTimeHierarchyOutputTypeDef = TypedDict(
@@ -15085,15 +12332,15 @@
 ):
     pass
 
 _RequiredExplicitHierarchyOutputTypeDef = TypedDict(
     "_RequiredExplicitHierarchyOutputTypeDef",
     {
         "HierarchyId": str,
-        "Columns": List[ColumnIdentifierOutputTypeDef],
+        "Columns": List[ColumnIdentifierTypeDef],
     },
 )
 _OptionalExplicitHierarchyOutputTypeDef = TypedDict(
     "_OptionalExplicitHierarchyOutputTypeDef",
     {
         "DrillDownFilters": List[DrillDownFilterOutputTypeDef],
     },
@@ -15105,15 +12352,15 @@
 ):
     pass
 
 _RequiredPredefinedHierarchyOutputTypeDef = TypedDict(
     "_RequiredPredefinedHierarchyOutputTypeDef",
     {
         "HierarchyId": str,
-        "Columns": List[ColumnIdentifierOutputTypeDef],
+        "Columns": List[ColumnIdentifierTypeDef],
     },
 )
 _OptionalPredefinedHierarchyOutputTypeDef = TypedDict(
     "_OptionalPredefinedHierarchyOutputTypeDef",
     {
         "DrillDownFilters": List[DrillDownFilterOutputTypeDef],
     },
@@ -15121,102 +12368,14 @@
 )
 
 class PredefinedHierarchyOutputTypeDef(
     _RequiredPredefinedHierarchyOutputTypeDef, _OptionalPredefinedHierarchyOutputTypeDef
 ):
     pass
 
-_RequiredDateTimeParameterDeclarationTypeDef = TypedDict(
-    "_RequiredDateTimeParameterDeclarationTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalDateTimeParameterDeclarationTypeDef = TypedDict(
-    "_OptionalDateTimeParameterDeclarationTypeDef",
-    {
-        "DefaultValues": DateTimeDefaultValuesTypeDef,
-        "TimeGranularity": TimeGranularityType,
-        "ValueWhenUnset": DateTimeValueWhenUnsetConfigurationTypeDef,
-        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
-    },
-    total=False,
-)
-
-class DateTimeParameterDeclarationTypeDef(
-    _RequiredDateTimeParameterDeclarationTypeDef, _OptionalDateTimeParameterDeclarationTypeDef
-):
-    pass
-
-_RequiredDecimalParameterDeclarationTypeDef = TypedDict(
-    "_RequiredDecimalParameterDeclarationTypeDef",
-    {
-        "ParameterValueType": ParameterValueTypeType,
-        "Name": str,
-    },
-)
-_OptionalDecimalParameterDeclarationTypeDef = TypedDict(
-    "_OptionalDecimalParameterDeclarationTypeDef",
-    {
-        "DefaultValues": DecimalDefaultValuesTypeDef,
-        "ValueWhenUnset": DecimalValueWhenUnsetConfigurationTypeDef,
-        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
-    },
-    total=False,
-)
-
-class DecimalParameterDeclarationTypeDef(
-    _RequiredDecimalParameterDeclarationTypeDef, _OptionalDecimalParameterDeclarationTypeDef
-):
-    pass
-
-_RequiredIntegerParameterDeclarationTypeDef = TypedDict(
-    "_RequiredIntegerParameterDeclarationTypeDef",
-    {
-        "ParameterValueType": ParameterValueTypeType,
-        "Name": str,
-    },
-)
-_OptionalIntegerParameterDeclarationTypeDef = TypedDict(
-    "_OptionalIntegerParameterDeclarationTypeDef",
-    {
-        "DefaultValues": IntegerDefaultValuesTypeDef,
-        "ValueWhenUnset": IntegerValueWhenUnsetConfigurationTypeDef,
-        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
-    },
-    total=False,
-)
-
-class IntegerParameterDeclarationTypeDef(
-    _RequiredIntegerParameterDeclarationTypeDef, _OptionalIntegerParameterDeclarationTypeDef
-):
-    pass
-
-_RequiredStringParameterDeclarationTypeDef = TypedDict(
-    "_RequiredStringParameterDeclarationTypeDef",
-    {
-        "ParameterValueType": ParameterValueTypeType,
-        "Name": str,
-    },
-)
-_OptionalStringParameterDeclarationTypeDef = TypedDict(
-    "_OptionalStringParameterDeclarationTypeDef",
-    {
-        "DefaultValues": StringDefaultValuesTypeDef,
-        "ValueWhenUnset": StringValueWhenUnsetConfigurationTypeDef,
-        "MappedDataSetParameters": Sequence[MappedDataSetParameterTypeDef],
-    },
-    total=False,
-)
-
-class StringParameterDeclarationTypeDef(
-    _RequiredStringParameterDeclarationTypeDef, _OptionalStringParameterDeclarationTypeDef
-):
-    pass
-
 _RequiredDateTimeHierarchyTypeDef = TypedDict(
     "_RequiredDateTimeHierarchyTypeDef",
     {
         "HierarchyId": str,
     },
 )
 _OptionalDateTimeHierarchyTypeDef = TypedDict(
@@ -15321,15 +12480,15 @@
 ):
     pass
 
 AxisDataOptionsOutputTypeDef = TypedDict(
     "AxisDataOptionsOutputTypeDef",
     {
         "NumericAxisOptions": NumericAxisOptionsOutputTypeDef,
-        "DateAxisOptions": DateAxisOptionsOutputTypeDef,
+        "DateAxisOptions": DateAxisOptionsTypeDef,
     },
     total=False,
 )
 
 AxisDataOptionsTypeDef = TypedDict(
     "AxisDataOptionsTypeDef",
     {
@@ -15339,18 +12498,18 @@
     total=False,
 )
 
 TransformOperationOutputTypeDef = TypedDict(
     "TransformOperationOutputTypeDef",
     {
         "ProjectOperation": ProjectOperationOutputTypeDef,
-        "FilterOperation": FilterOperationOutputTypeDef,
+        "FilterOperation": FilterOperationTypeDef,
         "CreateColumnsOperation": CreateColumnsOperationOutputTypeDef,
-        "RenameColumnOperation": RenameColumnOperationOutputTypeDef,
-        "CastColumnTypeOperation": CastColumnTypeOperationOutputTypeDef,
+        "RenameColumnOperation": RenameColumnOperationTypeDef,
+        "CastColumnTypeOperation": CastColumnTypeOperationTypeDef,
         "TagColumnOperation": TagColumnOperationOutputTypeDef,
         "UntagColumnOperation": UntagColumnOperationOutputTypeDef,
         "OverrideDatasetParameterOperation": OverrideDatasetParameterOperationOutputTypeDef,
     },
     total=False,
 )
 
@@ -15400,15 +12559,15 @@
         "Value": DestinationParameterValueConfigurationTypeDef,
     },
 )
 
 PivotTableFieldOptionsOutputTypeDef = TypedDict(
     "PivotTableFieldOptionsOutputTypeDef",
     {
-        "SelectedFieldOptions": List[PivotTableFieldOptionOutputTypeDef],
+        "SelectedFieldOptions": List[PivotTableFieldOptionTypeDef],
         "DataPathOptions": List[PivotTableDataPathOptionOutputTypeDef],
         "CollapseStateOptions": List[PivotTableFieldCollapseStateOptionOutputTypeDef],
     },
     total=False,
 )
 
 PivotTableFieldOptionsTypeDef = TypedDict(
@@ -15433,15 +12592,15 @@
     {
         "CalculatedFieldDescription": str,
         "CalculatedFieldSynonyms": List[str],
         "IsIncludedInTopic": bool,
         "DisableIndexing": bool,
         "ColumnDataRole": ColumnDataRoleType,
         "TimeGranularity": TopicTimeGranularityType,
-        "DefaultFormatting": DefaultFormattingOutputTypeDef,
+        "DefaultFormatting": DefaultFormattingTypeDef,
         "Aggregation": DefaultAggregationType,
         "ComparativeOrder": ComparativeOrderOutputTypeDef,
         "SemanticType": SemanticTypeOutputTypeDef,
         "AllowedAggregations": List[AuthorSpecifiedAggregationType],
         "NotAllowedAggregations": List[AuthorSpecifiedAggregationType],
         "NeverAggregateInFilter": bool,
         "CellValueSynonyms": List[CellValueSynonymOutputTypeDef],
@@ -15450,47 +12609,14 @@
 )
 
 class TopicCalculatedFieldOutputTypeDef(
     _RequiredTopicCalculatedFieldOutputTypeDef, _OptionalTopicCalculatedFieldOutputTypeDef
 ):
     pass
 
-_RequiredTopicColumnOutputTypeDef = TypedDict(
-    "_RequiredTopicColumnOutputTypeDef",
-    {
-        "ColumnName": str,
-    },
-)
-_OptionalTopicColumnOutputTypeDef = TypedDict(
-    "_OptionalTopicColumnOutputTypeDef",
-    {
-        "ColumnFriendlyName": str,
-        "ColumnDescription": str,
-        "ColumnSynonyms": List[str],
-        "ColumnDataRole": ColumnDataRoleType,
-        "Aggregation": DefaultAggregationType,
-        "IsIncludedInTopic": bool,
-        "DisableIndexing": bool,
-        "ComparativeOrder": ComparativeOrderOutputTypeDef,
-        "SemanticType": SemanticTypeOutputTypeDef,
-        "TimeGranularity": TopicTimeGranularityType,
-        "AllowedAggregations": List[AuthorSpecifiedAggregationType],
-        "NotAllowedAggregations": List[AuthorSpecifiedAggregationType],
-        "DefaultFormatting": DefaultFormattingOutputTypeDef,
-        "NeverAggregateInFilter": bool,
-        "CellValueSynonyms": List[CellValueSynonymOutputTypeDef],
-    },
-    total=False,
-)
-
-class TopicColumnOutputTypeDef(
-    _RequiredTopicColumnOutputTypeDef, _OptionalTopicColumnOutputTypeDef
-):
-    pass
-
 _RequiredTopicCalculatedFieldTypeDef = TypedDict(
     "_RequiredTopicCalculatedFieldTypeDef",
     {
         "CalculatedFieldName": str,
         "Expression": str,
     },
 )
@@ -15516,14 +12642,47 @@
 )
 
 class TopicCalculatedFieldTypeDef(
     _RequiredTopicCalculatedFieldTypeDef, _OptionalTopicCalculatedFieldTypeDef
 ):
     pass
 
+_RequiredTopicColumnOutputTypeDef = TypedDict(
+    "_RequiredTopicColumnOutputTypeDef",
+    {
+        "ColumnName": str,
+    },
+)
+_OptionalTopicColumnOutputTypeDef = TypedDict(
+    "_OptionalTopicColumnOutputTypeDef",
+    {
+        "ColumnFriendlyName": str,
+        "ColumnDescription": str,
+        "ColumnSynonyms": List[str],
+        "ColumnDataRole": ColumnDataRoleType,
+        "Aggregation": DefaultAggregationType,
+        "IsIncludedInTopic": bool,
+        "DisableIndexing": bool,
+        "ComparativeOrder": ComparativeOrderOutputTypeDef,
+        "SemanticType": SemanticTypeOutputTypeDef,
+        "TimeGranularity": TopicTimeGranularityType,
+        "AllowedAggregations": List[AuthorSpecifiedAggregationType],
+        "NotAllowedAggregations": List[AuthorSpecifiedAggregationType],
+        "DefaultFormatting": DefaultFormattingTypeDef,
+        "NeverAggregateInFilter": bool,
+        "CellValueSynonyms": List[CellValueSynonymOutputTypeDef],
+    },
+    total=False,
+)
+
+class TopicColumnOutputTypeDef(
+    _RequiredTopicColumnOutputTypeDef, _OptionalTopicColumnOutputTypeDef
+):
+    pass
+
 _RequiredTopicColumnTypeDef = TypedDict(
     "_RequiredTopicColumnTypeDef",
     {
         "ColumnName": str,
     },
 )
 _OptionalTopicColumnTypeDef = TypedDict(
@@ -15552,131 +12711,15 @@
     pass
 
 ChartAxisLabelOptionsOutputTypeDef = TypedDict(
     "ChartAxisLabelOptionsOutputTypeDef",
     {
         "Visibility": VisibilityType,
         "SortIconVisibility": VisibilityType,
-        "AxisLabelOptions": List[AxisLabelOptionsOutputTypeDef],
-    },
-    total=False,
-)
-
-AxisTickLabelOptionsOutputTypeDef = TypedDict(
-    "AxisTickLabelOptionsOutputTypeDef",
-    {
-        "LabelOptions": LabelOptionsOutputTypeDef,
-        "RotationAngle": float,
-    },
-    total=False,
-)
-
-DateTimePickerControlDisplayOptionsOutputTypeDef = TypedDict(
-    "DateTimePickerControlDisplayOptionsOutputTypeDef",
-    {
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "DateTimeFormat": str,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-DropDownControlDisplayOptionsOutputTypeDef = TypedDict(
-    "DropDownControlDisplayOptionsOutputTypeDef",
-    {
-        "SelectAllOptions": ListControlSelectAllOptionsOutputTypeDef,
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-LegendOptionsOutputTypeDef = TypedDict(
-    "LegendOptionsOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "Title": LabelOptionsOutputTypeDef,
-        "Position": LegendPositionType,
-        "Width": str,
-        "Height": str,
-    },
-    total=False,
-)
-
-ListControlDisplayOptionsOutputTypeDef = TypedDict(
-    "ListControlDisplayOptionsOutputTypeDef",
-    {
-        "SearchOptions": ListControlSearchOptionsOutputTypeDef,
-        "SelectAllOptions": ListControlSelectAllOptionsOutputTypeDef,
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-RelativeDateTimeControlDisplayOptionsOutputTypeDef = TypedDict(
-    "RelativeDateTimeControlDisplayOptionsOutputTypeDef",
-    {
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "DateTimeFormat": str,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-SliderControlDisplayOptionsOutputTypeDef = TypedDict(
-    "SliderControlDisplayOptionsOutputTypeDef",
-    {
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-TextAreaControlDisplayOptionsOutputTypeDef = TypedDict(
-    "TextAreaControlDisplayOptionsOutputTypeDef",
-    {
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "PlaceholderOptions": TextControlPlaceholderOptionsOutputTypeDef,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-TextFieldControlDisplayOptionsOutputTypeDef = TypedDict(
-    "TextFieldControlDisplayOptionsOutputTypeDef",
-    {
-        "TitleOptions": LabelOptionsOutputTypeDef,
-        "PlaceholderOptions": TextControlPlaceholderOptionsOutputTypeDef,
-        "InfoIconLabelOptions": SheetControlInfoIconLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-PanelConfigurationOutputTypeDef = TypedDict(
-    "PanelConfigurationOutputTypeDef",
-    {
-        "Title": PanelTitleOptionsOutputTypeDef,
-        "BorderVisibility": VisibilityType,
-        "BorderThickness": str,
-        "BorderStyle": PanelBorderStyleType,
-        "BorderColor": str,
-        "GutterVisibility": VisibilityType,
-        "GutterSpacing": str,
-        "BackgroundVisibility": VisibilityType,
-        "BackgroundColor": str,
-    },
-    total=False,
-)
-
-TableFieldLinkContentConfigurationOutputTypeDef = TypedDict(
-    "TableFieldLinkContentConfigurationOutputTypeDef",
-    {
-        "CustomTextContent": TableFieldCustomTextContentOutputTypeDef,
-        "CustomIconContent": TableFieldCustomIconContentOutputTypeDef,
+        "AxisLabelOptions": List[AxisLabelOptionsTypeDef],
     },
     total=False,
 )
 
 ChartAxisLabelOptionsTypeDef = TypedDict(
     "ChartAxisLabelOptionsTypeDef",
     {
@@ -15803,15 +12846,15 @@
     total=False,
 )
 
 GeospatialPointStyleOptionsOutputTypeDef = TypedDict(
     "GeospatialPointStyleOptionsOutputTypeDef",
     {
         "SelectedPointStyle": GeospatialSelectedPointStyleType,
-        "ClusterMarkerConfiguration": ClusterMarkerConfigurationOutputTypeDef,
+        "ClusterMarkerConfiguration": ClusterMarkerConfigurationTypeDef,
         "HeatmapConfiguration": GeospatialHeatmapConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 GeospatialPointStyleOptionsTypeDef = TypedDict(
     "GeospatialPointStyleOptionsTypeDef",
@@ -15819,29 +12862,14 @@
         "SelectedPointStyle": GeospatialSelectedPointStyleType,
         "ClusterMarkerConfiguration": ClusterMarkerConfigurationTypeDef,
         "HeatmapConfiguration": GeospatialHeatmapConfigurationTypeDef,
     },
     total=False,
 )
 
-TableCellStyleOutputTypeDef = TypedDict(
-    "TableCellStyleOutputTypeDef",
-    {
-        "Visibility": VisibilityType,
-        "FontConfiguration": FontConfigurationOutputTypeDef,
-        "TextWrap": TextWrapType,
-        "HorizontalTextAlignment": HorizontalTextAlignmentType,
-        "VerticalTextAlignment": VerticalTextAlignmentType,
-        "BackgroundColor": str,
-        "Height": int,
-        "Border": GlobalTableBorderOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 TableCellStyleTypeDef = TypedDict(
     "TableCellStyleTypeDef",
     {
         "Visibility": VisibilityType,
         "FontConfiguration": FontConfigurationTypeDef,
         "TextWrap": TextWrapType,
         "HorizontalTextAlignment": HorizontalTextAlignmentType,
@@ -15852,139 +12880,70 @@
     },
     total=False,
 )
 
 ConditionalFormattingColorOutputTypeDef = TypedDict(
     "ConditionalFormattingColorOutputTypeDef",
     {
-        "Solid": ConditionalFormattingSolidColorOutputTypeDef,
+        "Solid": ConditionalFormattingSolidColorTypeDef,
         "Gradient": ConditionalFormattingGradientColorOutputTypeDef,
     },
     total=False,
 )
 
 ConditionalFormattingColorTypeDef = TypedDict(
     "ConditionalFormattingColorTypeDef",
     {
         "Solid": ConditionalFormattingSolidColorTypeDef,
         "Gradient": ConditionalFormattingGradientColorTypeDef,
     },
     total=False,
 )
 
-DefaultInteractiveLayoutConfigurationOutputTypeDef = TypedDict(
-    "DefaultInteractiveLayoutConfigurationOutputTypeDef",
+DefaultInteractiveLayoutConfigurationTypeDef = TypedDict(
+    "DefaultInteractiveLayoutConfigurationTypeDef",
     {
-        "Grid": DefaultGridLayoutConfigurationOutputTypeDef,
-        "FreeForm": DefaultFreeFormLayoutConfigurationOutputTypeDef,
+        "Grid": DefaultGridLayoutConfigurationTypeDef,
+        "FreeForm": DefaultFreeFormLayoutConfigurationTypeDef,
     },
     total=False,
 )
 
 SheetControlLayoutConfigurationOutputTypeDef = TypedDict(
     "SheetControlLayoutConfigurationOutputTypeDef",
     {
         "GridLayout": GridLayoutConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-DefaultInteractiveLayoutConfigurationTypeDef = TypedDict(
-    "DefaultInteractiveLayoutConfigurationTypeDef",
-    {
-        "Grid": DefaultGridLayoutConfigurationTypeDef,
-        "FreeForm": DefaultFreeFormLayoutConfigurationTypeDef,
-    },
-    total=False,
-)
-
 SheetControlLayoutConfigurationTypeDef = TypedDict(
     "SheetControlLayoutConfigurationTypeDef",
     {
         "GridLayout": GridLayoutConfigurationTypeDef,
     },
     total=False,
 )
 
-DataSetRefreshPropertiesOutputTypeDef = TypedDict(
-    "DataSetRefreshPropertiesOutputTypeDef",
-    {
-        "RefreshConfiguration": RefreshConfigurationOutputTypeDef,
-    },
-)
-
 DataSetRefreshPropertiesTypeDef = TypedDict(
     "DataSetRefreshPropertiesTypeDef",
     {
         "RefreshConfiguration": RefreshConfigurationTypeDef,
     },
 )
 
-SeriesItemOutputTypeDef = TypedDict(
-    "SeriesItemOutputTypeDef",
-    {
-        "FieldSeriesItem": FieldSeriesItemOutputTypeDef,
-        "DataFieldSeriesItem": DataFieldSeriesItemOutputTypeDef,
-    },
-    total=False,
-)
-
 SeriesItemTypeDef = TypedDict(
     "SeriesItemTypeDef",
     {
         "FieldSeriesItem": FieldSeriesItemTypeDef,
         "DataFieldSeriesItem": DataFieldSeriesItemTypeDef,
     },
     total=False,
 )
 
-_RequiredAssetBundleImportJobDataSourceOverrideParametersOutputTypeDef = TypedDict(
-    "_RequiredAssetBundleImportJobDataSourceOverrideParametersOutputTypeDef",
-    {
-        "DataSourceId": str,
-    },
-)
-_OptionalAssetBundleImportJobDataSourceOverrideParametersOutputTypeDef = TypedDict(
-    "_OptionalAssetBundleImportJobDataSourceOverrideParametersOutputTypeDef",
-    {
-        "Name": str,
-        "DataSourceParameters": DataSourceParametersOutputTypeDef,
-        "VpcConnectionProperties": VpcConnectionPropertiesOutputTypeDef,
-        "SslProperties": SslPropertiesOutputTypeDef,
-        "Credentials": AssetBundleImportJobDataSourceCredentialsOutputTypeDef,
-    },
-    total=False,
-)
-
-class AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef(
-    _RequiredAssetBundleImportJobDataSourceOverrideParametersOutputTypeDef,
-    _OptionalAssetBundleImportJobDataSourceOverrideParametersOutputTypeDef,
-):
-    pass
-
-DataSourceTypeDef = TypedDict(
-    "DataSourceTypeDef",
-    {
-        "Arn": str,
-        "DataSourceId": str,
-        "Name": str,
-        "Type": DataSourceTypeType,
-        "Status": ResourceStatusType,
-        "CreatedTime": datetime,
-        "LastUpdatedTime": datetime,
-        "DataSourceParameters": DataSourceParametersOutputTypeDef,
-        "AlternateDataSourceParameters": List[DataSourceParametersOutputTypeDef],
-        "VpcConnectionProperties": VpcConnectionPropertiesOutputTypeDef,
-        "SslProperties": SslPropertiesOutputTypeDef,
-        "ErrorInfo": DataSourceErrorInfoTypeDef,
-        "SecretArn": str,
-    },
-    total=False,
-)
-
 _RequiredAssetBundleImportJobDataSourceOverrideParametersTypeDef = TypedDict(
     "_RequiredAssetBundleImportJobDataSourceOverrideParametersTypeDef",
     {
         "DataSourceId": str,
     },
 )
 _OptionalAssetBundleImportJobDataSourceOverrideParametersTypeDef = TypedDict(
@@ -16019,20 +12978,40 @@
     },
     total=False,
 )
 
 class CredentialPairTypeDef(_RequiredCredentialPairTypeDef, _OptionalCredentialPairTypeDef):
     pass
 
+DataSourceTypeDef = TypedDict(
+    "DataSourceTypeDef",
+    {
+        "Arn": str,
+        "DataSourceId": str,
+        "Name": str,
+        "Type": DataSourceTypeType,
+        "Status": ResourceStatusType,
+        "CreatedTime": datetime,
+        "LastUpdatedTime": datetime,
+        "DataSourceParameters": DataSourceParametersTypeDef,
+        "AlternateDataSourceParameters": List[DataSourceParametersTypeDef],
+        "VpcConnectionProperties": VpcConnectionPropertiesTypeDef,
+        "SslProperties": SslPropertiesTypeDef,
+        "ErrorInfo": DataSourceErrorInfoTypeDef,
+        "SecretArn": str,
+    },
+    total=False,
+)
+
 ThemeConfigurationOutputTypeDef = TypedDict(
     "ThemeConfigurationOutputTypeDef",
     {
         "DataColorPalette": DataColorPaletteOutputTypeDef,
-        "UIColorPalette": UIColorPaletteOutputTypeDef,
-        "Sheet": SheetStyleOutputTypeDef,
+        "UIColorPalette": UIColorPaletteTypeDef,
+        "Sheet": SheetStyleTypeDef,
         "Typography": TypographyOutputTypeDef,
     },
     total=False,
 )
 
 ThemeConfigurationTypeDef = TypedDict(
     "ThemeConfigurationTypeDef",
@@ -16041,33 +13020,14 @@
         "UIColorPalette": UIColorPaletteTypeDef,
         "Sheet": SheetStyleTypeDef,
         "Typography": TypographyTypeDef,
     },
     total=False,
 )
 
-ComparisonFormatConfigurationOutputTypeDef = TypedDict(
-    "ComparisonFormatConfigurationOutputTypeDef",
-    {
-        "NumberDisplayFormatConfiguration": NumberDisplayFormatConfigurationOutputTypeDef,
-        "PercentageDisplayFormatConfiguration": PercentageDisplayFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-NumericFormatConfigurationOutputTypeDef = TypedDict(
-    "NumericFormatConfigurationOutputTypeDef",
-    {
-        "NumberDisplayFormatConfiguration": NumberDisplayFormatConfigurationOutputTypeDef,
-        "CurrencyDisplayFormatConfiguration": CurrencyDisplayFormatConfigurationOutputTypeDef,
-        "PercentageDisplayFormatConfiguration": PercentageDisplayFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ComparisonFormatConfigurationTypeDef = TypedDict(
     "ComparisonFormatConfigurationTypeDef",
     {
         "NumberDisplayFormatConfiguration": NumberDisplayFormatConfigurationTypeDef,
         "PercentageDisplayFormatConfiguration": PercentageDisplayFormatConfigurationTypeDef,
     },
     total=False,
@@ -16079,146 +13039,14 @@
         "NumberDisplayFormatConfiguration": NumberDisplayFormatConfigurationTypeDef,
         "CurrencyDisplayFormatConfiguration": CurrencyDisplayFormatConfigurationTypeDef,
         "PercentageDisplayFormatConfiguration": PercentageDisplayFormatConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredAggregationSortConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAggregationSortConfigurationOutputTypeDef",
-    {
-        "Column": ColumnIdentifierOutputTypeDef,
-        "SortDirection": SortDirectionType,
-    },
-)
-_OptionalAggregationSortConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAggregationSortConfigurationOutputTypeDef",
-    {
-        "AggregationFunction": AggregationFunctionOutputTypeDef,
-    },
-    total=False,
-)
-
-class AggregationSortConfigurationOutputTypeDef(
-    _RequiredAggregationSortConfigurationOutputTypeDef,
-    _OptionalAggregationSortConfigurationOutputTypeDef,
-):
-    pass
-
-_RequiredColumnSortOutputTypeDef = TypedDict(
-    "_RequiredColumnSortOutputTypeDef",
-    {
-        "SortBy": ColumnIdentifierOutputTypeDef,
-        "Direction": SortDirectionType,
-    },
-)
-_OptionalColumnSortOutputTypeDef = TypedDict(
-    "_OptionalColumnSortOutputTypeDef",
-    {
-        "AggregationFunction": AggregationFunctionOutputTypeDef,
-    },
-    total=False,
-)
-
-class ColumnSortOutputTypeDef(_RequiredColumnSortOutputTypeDef, _OptionalColumnSortOutputTypeDef):
-    pass
-
-_RequiredColumnTooltipItemOutputTypeDef = TypedDict(
-    "_RequiredColumnTooltipItemOutputTypeDef",
-    {
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalColumnTooltipItemOutputTypeDef = TypedDict(
-    "_OptionalColumnTooltipItemOutputTypeDef",
-    {
-        "Label": str,
-        "Visibility": VisibilityType,
-        "Aggregation": AggregationFunctionOutputTypeDef,
-    },
-    total=False,
-)
-
-class ColumnTooltipItemOutputTypeDef(
-    _RequiredColumnTooltipItemOutputTypeDef, _OptionalColumnTooltipItemOutputTypeDef
-):
-    pass
-
-_RequiredNumericEqualityFilterOutputTypeDef = TypedDict(
-    "_RequiredNumericEqualityFilterOutputTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-        "MatchOperator": NumericEqualityMatchOperatorType,
-        "NullOption": FilterNullOptionType,
-    },
-)
-_OptionalNumericEqualityFilterOutputTypeDef = TypedDict(
-    "_OptionalNumericEqualityFilterOutputTypeDef",
-    {
-        "Value": float,
-        "SelectAllOptions": Literal["FILTER_ALL_VALUES"],
-        "AggregationFunction": AggregationFunctionOutputTypeDef,
-        "ParameterName": str,
-    },
-    total=False,
-)
-
-class NumericEqualityFilterOutputTypeDef(
-    _RequiredNumericEqualityFilterOutputTypeDef, _OptionalNumericEqualityFilterOutputTypeDef
-):
-    pass
-
-_RequiredNumericRangeFilterOutputTypeDef = TypedDict(
-    "_RequiredNumericRangeFilterOutputTypeDef",
-    {
-        "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-        "NullOption": FilterNullOptionType,
-    },
-)
-_OptionalNumericRangeFilterOutputTypeDef = TypedDict(
-    "_OptionalNumericRangeFilterOutputTypeDef",
-    {
-        "IncludeMinimum": bool,
-        "IncludeMaximum": bool,
-        "RangeMinimum": NumericRangeFilterValueOutputTypeDef,
-        "RangeMaximum": NumericRangeFilterValueOutputTypeDef,
-        "SelectAllOptions": Literal["FILTER_ALL_VALUES"],
-        "AggregationFunction": AggregationFunctionOutputTypeDef,
-    },
-    total=False,
-)
-
-class NumericRangeFilterOutputTypeDef(
-    _RequiredNumericRangeFilterOutputTypeDef, _OptionalNumericRangeFilterOutputTypeDef
-):
-    pass
-
-_RequiredReferenceLineDynamicDataConfigurationOutputTypeDef = TypedDict(
-    "_RequiredReferenceLineDynamicDataConfigurationOutputTypeDef",
-    {
-        "Column": ColumnIdentifierOutputTypeDef,
-        "Calculation": NumericalAggregationFunctionOutputTypeDef,
-    },
-)
-_OptionalReferenceLineDynamicDataConfigurationOutputTypeDef = TypedDict(
-    "_OptionalReferenceLineDynamicDataConfigurationOutputTypeDef",
-    {
-        "MeasureAggregationFunction": AggregationFunctionOutputTypeDef,
-    },
-    total=False,
-)
-
-class ReferenceLineDynamicDataConfigurationOutputTypeDef(
-    _RequiredReferenceLineDynamicDataConfigurationOutputTypeDef,
-    _OptionalReferenceLineDynamicDataConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredAggregationSortConfigurationTypeDef = TypedDict(
     "_RequiredAggregationSortConfigurationTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "SortDirection": SortDirectionType,
     },
 )
@@ -16357,18 +13185,18 @@
     "_OptionalTopicFilterOutputTypeDef",
     {
         "FilterDescription": str,
         "FilterClass": FilterClassType,
         "FilterSynonyms": List[str],
         "FilterType": NamedFilterTypeType,
         "CategoryFilter": TopicCategoryFilterOutputTypeDef,
-        "NumericEqualityFilter": TopicNumericEqualityFilterOutputTypeDef,
-        "NumericRangeFilter": TopicNumericRangeFilterOutputTypeDef,
-        "DateRangeFilter": TopicDateRangeFilterOutputTypeDef,
-        "RelativeDateFilter": TopicRelativeDateFilterOutputTypeDef,
+        "NumericEqualityFilter": TopicNumericEqualityFilterTypeDef,
+        "NumericRangeFilter": TopicNumericRangeFilterTypeDef,
+        "DateRangeFilter": TopicDateRangeFilterTypeDef,
+        "RelativeDateFilter": TopicRelativeDateFilterTypeDef,
     },
     total=False,
 )
 
 class TopicFilterOutputTypeDef(
     _RequiredTopicFilterOutputTypeDef, _OptionalTopicFilterOutputTypeDef
 ):
@@ -16455,21 +13283,14 @@
     {
         "Files": List[SnapshotFileOutputTypeDef],
         "S3Results": List[SnapshotJobS3ResultTypeDef],
     },
     total=False,
 )
 
-DefaultSectionBasedLayoutConfigurationOutputTypeDef = TypedDict(
-    "DefaultSectionBasedLayoutConfigurationOutputTypeDef",
-    {
-        "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsOutputTypeDef,
-    },
-)
-
 DefaultSectionBasedLayoutConfigurationTypeDef = TypedDict(
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
@@ -16478,15 +13299,15 @@
     {
         "Elements": List[FreeFormLayoutElementOutputTypeDef],
     },
 )
 _OptionalFreeFormLayoutConfigurationOutputTypeDef = TypedDict(
     "_OptionalFreeFormLayoutConfigurationOutputTypeDef",
     {
-        "CanvasSizeOptions": FreeFormLayoutCanvasSizeOptionsOutputTypeDef,
+        "CanvasSizeOptions": FreeFormLayoutCanvasSizeOptionsTypeDef,
     },
     total=False,
 )
 
 class FreeFormLayoutConfigurationOutputTypeDef(
     _RequiredFreeFormLayoutConfigurationOutputTypeDef,
     _OptionalFreeFormLayoutConfigurationOutputTypeDef,
@@ -16573,35 +13394,35 @@
         "DecimalParameterDeclaration": DecimalParameterDeclarationOutputTypeDef,
         "IntegerParameterDeclaration": IntegerParameterDeclarationOutputTypeDef,
         "DateTimeParameterDeclaration": DateTimeParameterDeclarationOutputTypeDef,
     },
     total=False,
 )
 
-ColumnHierarchyOutputTypeDef = TypedDict(
-    "ColumnHierarchyOutputTypeDef",
-    {
-        "ExplicitHierarchy": ExplicitHierarchyOutputTypeDef,
-        "DateTimeHierarchy": DateTimeHierarchyOutputTypeDef,
-        "PredefinedHierarchy": PredefinedHierarchyOutputTypeDef,
-    },
-    total=False,
-)
-
 ParameterDeclarationTypeDef = TypedDict(
     "ParameterDeclarationTypeDef",
     {
         "StringParameterDeclaration": StringParameterDeclarationTypeDef,
         "DecimalParameterDeclaration": DecimalParameterDeclarationTypeDef,
         "IntegerParameterDeclaration": IntegerParameterDeclarationTypeDef,
         "DateTimeParameterDeclaration": DateTimeParameterDeclarationTypeDef,
     },
     total=False,
 )
 
+ColumnHierarchyOutputTypeDef = TypedDict(
+    "ColumnHierarchyOutputTypeDef",
+    {
+        "ExplicitHierarchy": ExplicitHierarchyOutputTypeDef,
+        "DateTimeHierarchy": DateTimeHierarchyOutputTypeDef,
+        "PredefinedHierarchy": PredefinedHierarchyOutputTypeDef,
+    },
+    total=False,
+)
+
 ColumnHierarchyTypeDef = TypedDict(
     "ColumnHierarchyTypeDef",
     {
         "ExplicitHierarchy": ExplicitHierarchyTypeDef,
         "DateTimeHierarchy": DateTimeHierarchyTypeDef,
         "PredefinedHierarchy": PredefinedHierarchyTypeDef,
     },
@@ -16618,15 +13439,15 @@
     },
 )
 
 _RequiredLogicalTableOutputTypeDef = TypedDict(
     "_RequiredLogicalTableOutputTypeDef",
     {
         "Alias": str,
-        "Source": LogicalTableSourceOutputTypeDef,
+        "Source": LogicalTableSourceTypeDef,
     },
 )
 _OptionalLogicalTableOutputTypeDef = TypedDict(
     "_OptionalLogicalTableOutputTypeDef",
     {
         "DataTransforms": List[TransformOperationOutputTypeDef],
     },
@@ -16682,467 +13503,245 @@
         "ParameterValueConfigurations": Sequence[SetParameterValueConfigurationTypeDef],
     },
 )
 
 AxisDisplayOptionsOutputTypeDef = TypedDict(
     "AxisDisplayOptionsOutputTypeDef",
     {
-        "TickLabelOptions": AxisTickLabelOptionsOutputTypeDef,
+        "TickLabelOptions": AxisTickLabelOptionsTypeDef,
         "AxisLineVisibility": VisibilityType,
         "GridLineVisibility": VisibilityType,
         "DataOptions": AxisDataOptionsOutputTypeDef,
-        "ScrollbarOptions": ScrollBarOptionsOutputTypeDef,
+        "ScrollbarOptions": ScrollBarOptionsTypeDef,
+        "AxisOffset": str,
+    },
+    total=False,
+)
+
+AxisDisplayOptionsTypeDef = TypedDict(
+    "AxisDisplayOptionsTypeDef",
+    {
+        "TickLabelOptions": AxisTickLabelOptionsTypeDef,
+        "AxisLineVisibility": VisibilityType,
+        "GridLineVisibility": VisibilityType,
+        "DataOptions": AxisDataOptionsTypeDef,
+        "ScrollbarOptions": ScrollBarOptionsTypeDef,
         "AxisOffset": str,
     },
     total=False,
 )
 
-_RequiredFilterDateTimePickerControlOutputTypeDef = TypedDict(
-    "_RequiredFilterDateTimePickerControlOutputTypeDef",
+_RequiredFilterDateTimePickerControlTypeDef = TypedDict(
+    "_RequiredFilterDateTimePickerControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
     },
 )
-_OptionalFilterDateTimePickerControlOutputTypeDef = TypedDict(
-    "_OptionalFilterDateTimePickerControlOutputTypeDef",
+_OptionalFilterDateTimePickerControlTypeDef = TypedDict(
+    "_OptionalFilterDateTimePickerControlTypeDef",
     {
-        "DisplayOptions": DateTimePickerControlDisplayOptionsOutputTypeDef,
+        "DisplayOptions": DateTimePickerControlDisplayOptionsTypeDef,
         "Type": SheetControlDateTimePickerTypeType,
     },
     total=False,
 )
 
-class FilterDateTimePickerControlOutputTypeDef(
-    _RequiredFilterDateTimePickerControlOutputTypeDef,
-    _OptionalFilterDateTimePickerControlOutputTypeDef,
+class FilterDateTimePickerControlTypeDef(
+    _RequiredFilterDateTimePickerControlTypeDef, _OptionalFilterDateTimePickerControlTypeDef
 ):
     pass
 
-_RequiredParameterDateTimePickerControlOutputTypeDef = TypedDict(
-    "_RequiredParameterDateTimePickerControlOutputTypeDef",
+_RequiredParameterDateTimePickerControlTypeDef = TypedDict(
+    "_RequiredParameterDateTimePickerControlTypeDef",
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
     },
 )
-_OptionalParameterDateTimePickerControlOutputTypeDef = TypedDict(
-    "_OptionalParameterDateTimePickerControlOutputTypeDef",
+_OptionalParameterDateTimePickerControlTypeDef = TypedDict(
+    "_OptionalParameterDateTimePickerControlTypeDef",
     {
-        "DisplayOptions": DateTimePickerControlDisplayOptionsOutputTypeDef,
+        "DisplayOptions": DateTimePickerControlDisplayOptionsTypeDef,
     },
     total=False,
 )
 
-class ParameterDateTimePickerControlOutputTypeDef(
-    _RequiredParameterDateTimePickerControlOutputTypeDef,
-    _OptionalParameterDateTimePickerControlOutputTypeDef,
+class ParameterDateTimePickerControlTypeDef(
+    _RequiredParameterDateTimePickerControlTypeDef, _OptionalParameterDateTimePickerControlTypeDef
 ):
     pass
 
 _RequiredFilterDropDownControlOutputTypeDef = TypedDict(
     "_RequiredFilterDropDownControlOutputTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
     },
 )
 _OptionalFilterDropDownControlOutputTypeDef = TypedDict(
     "_OptionalFilterDropDownControlOutputTypeDef",
     {
-        "DisplayOptions": DropDownControlDisplayOptionsOutputTypeDef,
+        "DisplayOptions": DropDownControlDisplayOptionsTypeDef,
         "Type": SheetControlListTypeType,
         "SelectableValues": FilterSelectableValuesOutputTypeDef,
         "CascadingControlConfiguration": CascadingControlConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 class FilterDropDownControlOutputTypeDef(
     _RequiredFilterDropDownControlOutputTypeDef, _OptionalFilterDropDownControlOutputTypeDef
 ):
     pass
 
-_RequiredParameterDropDownControlOutputTypeDef = TypedDict(
-    "_RequiredParameterDropDownControlOutputTypeDef",
-    {
-        "ParameterControlId": str,
-        "Title": str,
-        "SourceParameterName": str,
-    },
-)
-_OptionalParameterDropDownControlOutputTypeDef = TypedDict(
-    "_OptionalParameterDropDownControlOutputTypeDef",
-    {
-        "DisplayOptions": DropDownControlDisplayOptionsOutputTypeDef,
-        "Type": SheetControlListTypeType,
-        "SelectableValues": ParameterSelectableValuesOutputTypeDef,
-        "CascadingControlConfiguration": CascadingControlConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class ParameterDropDownControlOutputTypeDef(
-    _RequiredParameterDropDownControlOutputTypeDef, _OptionalParameterDropDownControlOutputTypeDef
-):
-    pass
-
-_RequiredFilterListControlOutputTypeDef = TypedDict(
-    "_RequiredFilterListControlOutputTypeDef",
+_RequiredFilterDropDownControlTypeDef = TypedDict(
+    "_RequiredFilterDropDownControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
     },
 )
-_OptionalFilterListControlOutputTypeDef = TypedDict(
-    "_OptionalFilterListControlOutputTypeDef",
+_OptionalFilterDropDownControlTypeDef = TypedDict(
+    "_OptionalFilterDropDownControlTypeDef",
     {
-        "DisplayOptions": ListControlDisplayOptionsOutputTypeDef,
+        "DisplayOptions": DropDownControlDisplayOptionsTypeDef,
         "Type": SheetControlListTypeType,
-        "SelectableValues": FilterSelectableValuesOutputTypeDef,
-        "CascadingControlConfiguration": CascadingControlConfigurationOutputTypeDef,
+        "SelectableValues": FilterSelectableValuesTypeDef,
+        "CascadingControlConfiguration": CascadingControlConfigurationTypeDef,
     },
     total=False,
 )
 
-class FilterListControlOutputTypeDef(
-    _RequiredFilterListControlOutputTypeDef, _OptionalFilterListControlOutputTypeDef
+class FilterDropDownControlTypeDef(
+    _RequiredFilterDropDownControlTypeDef, _OptionalFilterDropDownControlTypeDef
 ):
     pass
 
-_RequiredParameterListControlOutputTypeDef = TypedDict(
-    "_RequiredParameterListControlOutputTypeDef",
+_RequiredParameterDropDownControlOutputTypeDef = TypedDict(
+    "_RequiredParameterDropDownControlOutputTypeDef",
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
     },
 )
-_OptionalParameterListControlOutputTypeDef = TypedDict(
-    "_OptionalParameterListControlOutputTypeDef",
+_OptionalParameterDropDownControlOutputTypeDef = TypedDict(
+    "_OptionalParameterDropDownControlOutputTypeDef",
     {
-        "DisplayOptions": ListControlDisplayOptionsOutputTypeDef,
+        "DisplayOptions": DropDownControlDisplayOptionsTypeDef,
         "Type": SheetControlListTypeType,
         "SelectableValues": ParameterSelectableValuesOutputTypeDef,
         "CascadingControlConfiguration": CascadingControlConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-class ParameterListControlOutputTypeDef(
-    _RequiredParameterListControlOutputTypeDef, _OptionalParameterListControlOutputTypeDef
-):
-    pass
-
-_RequiredFilterRelativeDateTimeControlOutputTypeDef = TypedDict(
-    "_RequiredFilterRelativeDateTimeControlOutputTypeDef",
-    {
-        "FilterControlId": str,
-        "Title": str,
-        "SourceFilterId": str,
-    },
-)
-_OptionalFilterRelativeDateTimeControlOutputTypeDef = TypedDict(
-    "_OptionalFilterRelativeDateTimeControlOutputTypeDef",
-    {
-        "DisplayOptions": RelativeDateTimeControlDisplayOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-class FilterRelativeDateTimeControlOutputTypeDef(
-    _RequiredFilterRelativeDateTimeControlOutputTypeDef,
-    _OptionalFilterRelativeDateTimeControlOutputTypeDef,
-):
-    pass
-
-_RequiredFilterSliderControlOutputTypeDef = TypedDict(
-    "_RequiredFilterSliderControlOutputTypeDef",
-    {
-        "FilterControlId": str,
-        "Title": str,
-        "SourceFilterId": str,
-        "MaximumValue": float,
-        "MinimumValue": float,
-        "StepSize": float,
-    },
-)
-_OptionalFilterSliderControlOutputTypeDef = TypedDict(
-    "_OptionalFilterSliderControlOutputTypeDef",
-    {
-        "DisplayOptions": SliderControlDisplayOptionsOutputTypeDef,
-        "Type": SheetControlSliderTypeType,
-    },
-    total=False,
-)
-
-class FilterSliderControlOutputTypeDef(
-    _RequiredFilterSliderControlOutputTypeDef, _OptionalFilterSliderControlOutputTypeDef
-):
-    pass
-
-_RequiredParameterSliderControlOutputTypeDef = TypedDict(
-    "_RequiredParameterSliderControlOutputTypeDef",
-    {
-        "ParameterControlId": str,
-        "Title": str,
-        "SourceParameterName": str,
-        "MaximumValue": float,
-        "MinimumValue": float,
-        "StepSize": float,
-    },
-)
-_OptionalParameterSliderControlOutputTypeDef = TypedDict(
-    "_OptionalParameterSliderControlOutputTypeDef",
-    {
-        "DisplayOptions": SliderControlDisplayOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-class ParameterSliderControlOutputTypeDef(
-    _RequiredParameterSliderControlOutputTypeDef, _OptionalParameterSliderControlOutputTypeDef
-):
-    pass
-
-_RequiredFilterTextAreaControlOutputTypeDef = TypedDict(
-    "_RequiredFilterTextAreaControlOutputTypeDef",
-    {
-        "FilterControlId": str,
-        "Title": str,
-        "SourceFilterId": str,
-    },
-)
-_OptionalFilterTextAreaControlOutputTypeDef = TypedDict(
-    "_OptionalFilterTextAreaControlOutputTypeDef",
-    {
-        "Delimiter": str,
-        "DisplayOptions": TextAreaControlDisplayOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-class FilterTextAreaControlOutputTypeDef(
-    _RequiredFilterTextAreaControlOutputTypeDef, _OptionalFilterTextAreaControlOutputTypeDef
-):
-    pass
-
-_RequiredParameterTextAreaControlOutputTypeDef = TypedDict(
-    "_RequiredParameterTextAreaControlOutputTypeDef",
-    {
-        "ParameterControlId": str,
-        "Title": str,
-        "SourceParameterName": str,
-    },
-)
-_OptionalParameterTextAreaControlOutputTypeDef = TypedDict(
-    "_OptionalParameterTextAreaControlOutputTypeDef",
-    {
-        "Delimiter": str,
-        "DisplayOptions": TextAreaControlDisplayOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-class ParameterTextAreaControlOutputTypeDef(
-    _RequiredParameterTextAreaControlOutputTypeDef, _OptionalParameterTextAreaControlOutputTypeDef
-):
-    pass
-
-_RequiredFilterTextFieldControlOutputTypeDef = TypedDict(
-    "_RequiredFilterTextFieldControlOutputTypeDef",
-    {
-        "FilterControlId": str,
-        "Title": str,
-        "SourceFilterId": str,
-    },
-)
-_OptionalFilterTextFieldControlOutputTypeDef = TypedDict(
-    "_OptionalFilterTextFieldControlOutputTypeDef",
-    {
-        "DisplayOptions": TextFieldControlDisplayOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-class FilterTextFieldControlOutputTypeDef(
-    _RequiredFilterTextFieldControlOutputTypeDef, _OptionalFilterTextFieldControlOutputTypeDef
+class ParameterDropDownControlOutputTypeDef(
+    _RequiredParameterDropDownControlOutputTypeDef, _OptionalParameterDropDownControlOutputTypeDef
 ):
     pass
 
-_RequiredParameterTextFieldControlOutputTypeDef = TypedDict(
-    "_RequiredParameterTextFieldControlOutputTypeDef",
+_RequiredParameterDropDownControlTypeDef = TypedDict(
+    "_RequiredParameterDropDownControlTypeDef",
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
     },
 )
-_OptionalParameterTextFieldControlOutputTypeDef = TypedDict(
-    "_OptionalParameterTextFieldControlOutputTypeDef",
+_OptionalParameterDropDownControlTypeDef = TypedDict(
+    "_OptionalParameterDropDownControlTypeDef",
     {
-        "DisplayOptions": TextFieldControlDisplayOptionsOutputTypeDef,
+        "DisplayOptions": DropDownControlDisplayOptionsTypeDef,
+        "Type": SheetControlListTypeType,
+        "SelectableValues": ParameterSelectableValuesTypeDef,
+        "CascadingControlConfiguration": CascadingControlConfigurationTypeDef,
     },
     total=False,
 )
 
-class ParameterTextFieldControlOutputTypeDef(
-    _RequiredParameterTextFieldControlOutputTypeDef, _OptionalParameterTextFieldControlOutputTypeDef
+class ParameterDropDownControlTypeDef(
+    _RequiredParameterDropDownControlTypeDef, _OptionalParameterDropDownControlTypeDef
 ):
     pass
 
-SmallMultiplesOptionsOutputTypeDef = TypedDict(
-    "SmallMultiplesOptionsOutputTypeDef",
-    {
-        "MaxVisibleRows": int,
-        "MaxVisibleColumns": int,
-        "PanelConfiguration": PanelConfigurationOutputTypeDef,
-        "XAxis": SmallMultiplesAxisPropertiesOutputTypeDef,
-        "YAxis": SmallMultiplesAxisPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
-TableFieldLinkConfigurationOutputTypeDef = TypedDict(
-    "TableFieldLinkConfigurationOutputTypeDef",
-    {
-        "Target": URLTargetConfigurationType,
-        "Content": TableFieldLinkContentConfigurationOutputTypeDef,
-    },
-)
-
-AxisDisplayOptionsTypeDef = TypedDict(
-    "AxisDisplayOptionsTypeDef",
-    {
-        "TickLabelOptions": AxisTickLabelOptionsTypeDef,
-        "AxisLineVisibility": VisibilityType,
-        "GridLineVisibility": VisibilityType,
-        "DataOptions": AxisDataOptionsTypeDef,
-        "ScrollbarOptions": ScrollBarOptionsTypeDef,
-        "AxisOffset": str,
-    },
-    total=False,
-)
-
-_RequiredFilterDateTimePickerControlTypeDef = TypedDict(
-    "_RequiredFilterDateTimePickerControlTypeDef",
+_RequiredFilterListControlOutputTypeDef = TypedDict(
+    "_RequiredFilterListControlOutputTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
     },
 )
-_OptionalFilterDateTimePickerControlTypeDef = TypedDict(
-    "_OptionalFilterDateTimePickerControlTypeDef",
-    {
-        "DisplayOptions": DateTimePickerControlDisplayOptionsTypeDef,
-        "Type": SheetControlDateTimePickerTypeType,
-    },
-    total=False,
-)
-
-class FilterDateTimePickerControlTypeDef(
-    _RequiredFilterDateTimePickerControlTypeDef, _OptionalFilterDateTimePickerControlTypeDef
-):
-    pass
-
-_RequiredParameterDateTimePickerControlTypeDef = TypedDict(
-    "_RequiredParameterDateTimePickerControlTypeDef",
-    {
-        "ParameterControlId": str,
-        "Title": str,
-        "SourceParameterName": str,
-    },
-)
-_OptionalParameterDateTimePickerControlTypeDef = TypedDict(
-    "_OptionalParameterDateTimePickerControlTypeDef",
+_OptionalFilterListControlOutputTypeDef = TypedDict(
+    "_OptionalFilterListControlOutputTypeDef",
     {
-        "DisplayOptions": DateTimePickerControlDisplayOptionsTypeDef,
+        "DisplayOptions": ListControlDisplayOptionsTypeDef,
+        "Type": SheetControlListTypeType,
+        "SelectableValues": FilterSelectableValuesOutputTypeDef,
+        "CascadingControlConfiguration": CascadingControlConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-class ParameterDateTimePickerControlTypeDef(
-    _RequiredParameterDateTimePickerControlTypeDef, _OptionalParameterDateTimePickerControlTypeDef
+class FilterListControlOutputTypeDef(
+    _RequiredFilterListControlOutputTypeDef, _OptionalFilterListControlOutputTypeDef
 ):
     pass
 
-_RequiredFilterDropDownControlTypeDef = TypedDict(
-    "_RequiredFilterDropDownControlTypeDef",
+_RequiredFilterListControlTypeDef = TypedDict(
+    "_RequiredFilterListControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
     },
 )
-_OptionalFilterDropDownControlTypeDef = TypedDict(
-    "_OptionalFilterDropDownControlTypeDef",
+_OptionalFilterListControlTypeDef = TypedDict(
+    "_OptionalFilterListControlTypeDef",
     {
-        "DisplayOptions": DropDownControlDisplayOptionsTypeDef,
+        "DisplayOptions": ListControlDisplayOptionsTypeDef,
         "Type": SheetControlListTypeType,
         "SelectableValues": FilterSelectableValuesTypeDef,
         "CascadingControlConfiguration": CascadingControlConfigurationTypeDef,
     },
     total=False,
 )
 
-class FilterDropDownControlTypeDef(
-    _RequiredFilterDropDownControlTypeDef, _OptionalFilterDropDownControlTypeDef
+class FilterListControlTypeDef(
+    _RequiredFilterListControlTypeDef, _OptionalFilterListControlTypeDef
 ):
     pass
 
-_RequiredParameterDropDownControlTypeDef = TypedDict(
-    "_RequiredParameterDropDownControlTypeDef",
+_RequiredParameterListControlOutputTypeDef = TypedDict(
+    "_RequiredParameterListControlOutputTypeDef",
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
     },
 )
-_OptionalParameterDropDownControlTypeDef = TypedDict(
-    "_OptionalParameterDropDownControlTypeDef",
-    {
-        "DisplayOptions": DropDownControlDisplayOptionsTypeDef,
-        "Type": SheetControlListTypeType,
-        "SelectableValues": ParameterSelectableValuesTypeDef,
-        "CascadingControlConfiguration": CascadingControlConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class ParameterDropDownControlTypeDef(
-    _RequiredParameterDropDownControlTypeDef, _OptionalParameterDropDownControlTypeDef
-):
-    pass
-
-_RequiredFilterListControlTypeDef = TypedDict(
-    "_RequiredFilterListControlTypeDef",
-    {
-        "FilterControlId": str,
-        "Title": str,
-        "SourceFilterId": str,
-    },
-)
-_OptionalFilterListControlTypeDef = TypedDict(
-    "_OptionalFilterListControlTypeDef",
+_OptionalParameterListControlOutputTypeDef = TypedDict(
+    "_OptionalParameterListControlOutputTypeDef",
     {
         "DisplayOptions": ListControlDisplayOptionsTypeDef,
         "Type": SheetControlListTypeType,
-        "SelectableValues": FilterSelectableValuesTypeDef,
-        "CascadingControlConfiguration": CascadingControlConfigurationTypeDef,
+        "SelectableValues": ParameterSelectableValuesOutputTypeDef,
+        "CascadingControlConfiguration": CascadingControlConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-class FilterListControlTypeDef(
-    _RequiredFilterListControlTypeDef, _OptionalFilterListControlTypeDef
+class ParameterListControlOutputTypeDef(
+    _RequiredParameterListControlOutputTypeDef, _OptionalParameterListControlOutputTypeDef
 ):
     pass
 
 _RequiredParameterListControlTypeDef = TypedDict(
     "_RequiredParameterListControlTypeDef",
     {
         "ParameterControlId": str,
@@ -17345,75 +13944,24 @@
 PivotTableOptionsOutputTypeDef = TypedDict(
     "PivotTableOptionsOutputTypeDef",
     {
         "MetricPlacement": PivotTableMetricPlacementType,
         "SingleMetricVisibility": VisibilityType,
         "ColumnNamesVisibility": VisibilityType,
         "ToggleButtonsVisibility": VisibilityType,
-        "ColumnHeaderStyle": TableCellStyleOutputTypeDef,
-        "RowHeaderStyle": TableCellStyleOutputTypeDef,
-        "CellStyle": TableCellStyleOutputTypeDef,
-        "RowFieldNamesStyle": TableCellStyleOutputTypeDef,
+        "ColumnHeaderStyle": TableCellStyleTypeDef,
+        "RowHeaderStyle": TableCellStyleTypeDef,
+        "CellStyle": TableCellStyleTypeDef,
+        "RowFieldNamesStyle": TableCellStyleTypeDef,
         "RowAlternateColorOptions": RowAlternateColorOptionsOutputTypeDef,
         "CollapsedRowDimensionsVisibility": VisibilityType,
     },
     total=False,
 )
 
-PivotTotalOptionsOutputTypeDef = TypedDict(
-    "PivotTotalOptionsOutputTypeDef",
-    {
-        "TotalsVisibility": VisibilityType,
-        "Placement": TableTotalsPlacementType,
-        "ScrollStatus": TableTotalsScrollStatusType,
-        "CustomLabel": str,
-        "TotalCellStyle": TableCellStyleOutputTypeDef,
-        "ValueCellStyle": TableCellStyleOutputTypeDef,
-        "MetricHeaderCellStyle": TableCellStyleOutputTypeDef,
-    },
-    total=False,
-)
-
-SubtotalOptionsOutputTypeDef = TypedDict(
-    "SubtotalOptionsOutputTypeDef",
-    {
-        "TotalsVisibility": VisibilityType,
-        "CustomLabel": str,
-        "FieldLevel": PivotTableSubtotalLevelType,
-        "FieldLevelOptions": List[PivotTableFieldSubtotalOptionsOutputTypeDef],
-        "TotalCellStyle": TableCellStyleOutputTypeDef,
-        "ValueCellStyle": TableCellStyleOutputTypeDef,
-        "MetricHeaderCellStyle": TableCellStyleOutputTypeDef,
-    },
-    total=False,
-)
-
-TableOptionsOutputTypeDef = TypedDict(
-    "TableOptionsOutputTypeDef",
-    {
-        "Orientation": TableOrientationType,
-        "HeaderStyle": TableCellStyleOutputTypeDef,
-        "CellStyle": TableCellStyleOutputTypeDef,
-        "RowAlternateColorOptions": RowAlternateColorOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-TotalOptionsOutputTypeDef = TypedDict(
-    "TotalOptionsOutputTypeDef",
-    {
-        "TotalsVisibility": VisibilityType,
-        "Placement": TableTotalsPlacementType,
-        "ScrollStatus": TableTotalsScrollStatusType,
-        "CustomLabel": str,
-        "TotalCellStyle": TableCellStyleOutputTypeDef,
-    },
-    total=False,
-)
-
 PivotTableOptionsTypeDef = TypedDict(
     "PivotTableOptionsTypeDef",
     {
         "MetricPlacement": PivotTableMetricPlacementType,
         "SingleMetricVisibility": VisibilityType,
         "ColumnNamesVisibility": VisibilityType,
         "ToggleButtonsVisibility": VisibilityType,
@@ -17437,28 +13985,53 @@
         "TotalCellStyle": TableCellStyleTypeDef,
         "ValueCellStyle": TableCellStyleTypeDef,
         "MetricHeaderCellStyle": TableCellStyleTypeDef,
     },
     total=False,
 )
 
+SubtotalOptionsOutputTypeDef = TypedDict(
+    "SubtotalOptionsOutputTypeDef",
+    {
+        "TotalsVisibility": VisibilityType,
+        "CustomLabel": str,
+        "FieldLevel": PivotTableSubtotalLevelType,
+        "FieldLevelOptions": List[PivotTableFieldSubtotalOptionsTypeDef],
+        "TotalCellStyle": TableCellStyleTypeDef,
+        "ValueCellStyle": TableCellStyleTypeDef,
+        "MetricHeaderCellStyle": TableCellStyleTypeDef,
+    },
+    total=False,
+)
+
 SubtotalOptionsTypeDef = TypedDict(
     "SubtotalOptionsTypeDef",
     {
         "TotalsVisibility": VisibilityType,
         "CustomLabel": str,
         "FieldLevel": PivotTableSubtotalLevelType,
         "FieldLevelOptions": Sequence[PivotTableFieldSubtotalOptionsTypeDef],
         "TotalCellStyle": TableCellStyleTypeDef,
         "ValueCellStyle": TableCellStyleTypeDef,
         "MetricHeaderCellStyle": TableCellStyleTypeDef,
     },
     total=False,
 )
 
+TableOptionsOutputTypeDef = TypedDict(
+    "TableOptionsOutputTypeDef",
+    {
+        "Orientation": TableOrientationType,
+        "HeaderStyle": TableCellStyleTypeDef,
+        "CellStyle": TableCellStyleTypeDef,
+        "RowAlternateColorOptions": RowAlternateColorOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 TableOptionsTypeDef = TypedDict(
     "TableOptionsTypeDef",
     {
         "Orientation": TableOrientationType,
         "HeaderStyle": TableCellStyleTypeDef,
         "CellStyle": TableCellStyleTypeDef,
         "RowAlternateColorOptions": RowAlternateColorOptionsTypeDef,
@@ -17486,24 +14059,24 @@
     total=False,
 )
 
 GaugeChartPrimaryValueConditionalFormattingOutputTypeDef = TypedDict(
     "GaugeChartPrimaryValueConditionalFormattingOutputTypeDef",
     {
         "TextColor": ConditionalFormattingColorOutputTypeDef,
-        "Icon": ConditionalFormattingIconOutputTypeDef,
+        "Icon": ConditionalFormattingIconTypeDef,
     },
     total=False,
 )
 
 KPIPrimaryValueConditionalFormattingOutputTypeDef = TypedDict(
     "KPIPrimaryValueConditionalFormattingOutputTypeDef",
     {
         "TextColor": ConditionalFormattingColorOutputTypeDef,
-        "Icon": ConditionalFormattingIconOutputTypeDef,
+        "Icon": ConditionalFormattingIconTypeDef,
     },
     total=False,
 )
 
 KPIProgressBarConditionalFormattingOutputTypeDef = TypedDict(
     "KPIProgressBarConditionalFormattingOutputTypeDef",
     {
@@ -17529,15 +14102,15 @@
 )
 
 TextConditionalFormatOutputTypeDef = TypedDict(
     "TextConditionalFormatOutputTypeDef",
     {
         "BackgroundColor": ConditionalFormattingColorOutputTypeDef,
         "TextColor": ConditionalFormattingColorOutputTypeDef,
-        "Icon": ConditionalFormattingIconOutputTypeDef,
+        "Icon": ConditionalFormattingIconTypeDef,
     },
     total=False,
 )
 
 GaugeChartArcConditionalFormattingTypeDef = TypedDict(
     "GaugeChartArcConditionalFormattingTypeDef",
     {
@@ -17613,15 +14186,15 @@
 )
 
 DescribeDataSetRefreshPropertiesResponseTypeDef = TypedDict(
     "DescribeDataSetRefreshPropertiesResponseTypeDef",
     {
         "RequestId": str,
         "Status": int,
-        "DataSetRefreshProperties": DataSetRefreshPropertiesOutputTypeDef,
+        "DataSetRefreshProperties": DataSetRefreshPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDataSetRefreshPropertiesRequestRequestTypeDef = TypedDict(
     "PutDataSetRefreshPropertiesRequestRequestTypeDef",
     {
@@ -17631,50 +14204,29 @@
     },
 )
 
 AssetBundleImportJobOverrideParametersOutputTypeDef = TypedDict(
     "AssetBundleImportJobOverrideParametersOutputTypeDef",
     {
         "ResourceIdOverrideConfiguration": (
-            AssetBundleImportJobResourceIdOverrideConfigurationOutputTypeDef
+            AssetBundleImportJobResourceIdOverrideConfigurationTypeDef
         ),
         "VPCConnections": List[AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef],
         "RefreshSchedules": List[
             AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef
         ],
-        "DataSources": List[AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef],
-        "DataSets": List[AssetBundleImportJobDataSetOverrideParametersOutputTypeDef],
-        "Themes": List[AssetBundleImportJobThemeOverrideParametersOutputTypeDef],
-        "Analyses": List[AssetBundleImportJobAnalysisOverrideParametersOutputTypeDef],
-        "Dashboards": List[AssetBundleImportJobDashboardOverrideParametersOutputTypeDef],
+        "DataSources": List[AssetBundleImportJobDataSourceOverrideParametersTypeDef],
+        "DataSets": List[AssetBundleImportJobDataSetOverrideParametersTypeDef],
+        "Themes": List[AssetBundleImportJobThemeOverrideParametersTypeDef],
+        "Analyses": List[AssetBundleImportJobAnalysisOverrideParametersTypeDef],
+        "Dashboards": List[AssetBundleImportJobDashboardOverrideParametersTypeDef],
     },
     total=False,
 )
 
-DescribeDataSourceResponseTypeDef = TypedDict(
-    "DescribeDataSourceResponseTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataSourcesResponseTypeDef = TypedDict(
-    "ListDataSourcesResponseTypeDef",
-    {
-        "DataSources": List[DataSourceTypeDef],
-        "NextToken": str,
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AssetBundleImportJobOverrideParametersTypeDef = TypedDict(
     "AssetBundleImportJobOverrideParametersTypeDef",
     {
         "ResourceIdOverrideConfiguration": (
             AssetBundleImportJobResourceIdOverrideConfigurationTypeDef
         ),
         "VPCConnections": Sequence[AssetBundleImportJobVPCConnectionOverrideParametersTypeDef],
@@ -17694,14 +14246,35 @@
         "CredentialPair": CredentialPairTypeDef,
         "CopySourceArn": str,
         "SecretArn": str,
     },
     total=False,
 )
 
+DescribeDataSourceResponseTypeDef = TypedDict(
+    "DescribeDataSourceResponseTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDataSourcesResponseTypeDef = TypedDict(
+    "ListDataSourcesResponseTypeDef",
+    {
+        "DataSources": List[DataSourceTypeDef],
+        "NextToken": str,
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ThemeVersionTypeDef = TypedDict(
     "ThemeVersionTypeDef",
     {
         "VersionNumber": int,
         "Arn": str,
         "Description": str,
         "BaseThemeId": str,
@@ -17757,59 +14330,14 @@
 )
 
 class UpdateThemeRequestRequestTypeDef(
     _RequiredUpdateThemeRequestRequestTypeDef, _OptionalUpdateThemeRequestRequestTypeDef
 ):
     pass
 
-ComparisonConfigurationOutputTypeDef = TypedDict(
-    "ComparisonConfigurationOutputTypeDef",
-    {
-        "ComparisonMethod": ComparisonMethodType,
-        "ComparisonFormat": ComparisonFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-DateTimeFormatConfigurationOutputTypeDef = TypedDict(
-    "DateTimeFormatConfigurationOutputTypeDef",
-    {
-        "DateTimeFormat": str,
-        "NullValueFormatConfiguration": NullValueFormatConfigurationOutputTypeDef,
-        "NumericFormatConfiguration": NumericFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-NumberFormatConfigurationOutputTypeDef = TypedDict(
-    "NumberFormatConfigurationOutputTypeDef",
-    {
-        "FormatConfiguration": NumericFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-ReferenceLineValueLabelConfigurationOutputTypeDef = TypedDict(
-    "ReferenceLineValueLabelConfigurationOutputTypeDef",
-    {
-        "RelativePosition": ReferenceLineValueLabelRelativePositionType,
-        "FormatConfiguration": NumericFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-StringFormatConfigurationOutputTypeDef = TypedDict(
-    "StringFormatConfigurationOutputTypeDef",
-    {
-        "NullValueFormatConfiguration": NullValueFormatConfigurationOutputTypeDef,
-        "NumericFormatConfiguration": NumericFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ComparisonConfigurationTypeDef = TypedDict(
     "ComparisonConfigurationTypeDef",
     {
         "ComparisonMethod": ComparisonMethodType,
         "ComparisonFormat": ComparisonFormatConfigurationTypeDef,
     },
     total=False,
@@ -17851,16 +14379,16 @@
     total=False,
 )
 
 _RequiredTopBottomFilterOutputTypeDef = TypedDict(
     "_RequiredTopBottomFilterOutputTypeDef",
     {
         "FilterId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-        "AggregationSortConfigurations": List[AggregationSortConfigurationOutputTypeDef],
+        "Column": ColumnIdentifierTypeDef,
+        "AggregationSortConfigurations": List[AggregationSortConfigurationTypeDef],
     },
 )
 _OptionalTopBottomFilterOutputTypeDef = TypedDict(
     "_OptionalTopBottomFilterOutputTypeDef",
     {
         "Limit": int,
         "TimeGranularity": TimeGranularityType,
@@ -17870,52 +14398,14 @@
 )
 
 class TopBottomFilterOutputTypeDef(
     _RequiredTopBottomFilterOutputTypeDef, _OptionalTopBottomFilterOutputTypeDef
 ):
     pass
 
-FieldSortOptionsOutputTypeDef = TypedDict(
-    "FieldSortOptionsOutputTypeDef",
-    {
-        "FieldSort": FieldSortOutputTypeDef,
-        "ColumnSort": ColumnSortOutputTypeDef,
-    },
-    total=False,
-)
-
-PivotTableSortByOutputTypeDef = TypedDict(
-    "PivotTableSortByOutputTypeDef",
-    {
-        "Field": FieldSortOutputTypeDef,
-        "Column": ColumnSortOutputTypeDef,
-        "DataPath": DataPathSortOutputTypeDef,
-    },
-    total=False,
-)
-
-TooltipItemOutputTypeDef = TypedDict(
-    "TooltipItemOutputTypeDef",
-    {
-        "FieldTooltipItem": FieldTooltipItemOutputTypeDef,
-        "ColumnTooltipItem": ColumnTooltipItemOutputTypeDef,
-    },
-    total=False,
-)
-
-ReferenceLineDataConfigurationOutputTypeDef = TypedDict(
-    "ReferenceLineDataConfigurationOutputTypeDef",
-    {
-        "StaticConfiguration": ReferenceLineStaticDataConfigurationOutputTypeDef,
-        "DynamicConfiguration": ReferenceLineDynamicDataConfigurationOutputTypeDef,
-        "AxisBinding": AxisBindingType,
-    },
-    total=False,
-)
-
 _RequiredTopBottomFilterTypeDef = TypedDict(
     "_RequiredTopBottomFilterTypeDef",
     {
         "FilterId": str,
         "Column": ColumnIdentifierTypeDef,
         "AggregationSortConfigurations": Sequence[AggregationSortConfigurationTypeDef],
     },
@@ -17938,14 +14428,24 @@
     {
         "FieldSort": FieldSortTypeDef,
         "ColumnSort": ColumnSortTypeDef,
     },
     total=False,
 )
 
+PivotTableSortByOutputTypeDef = TypedDict(
+    "PivotTableSortByOutputTypeDef",
+    {
+        "Field": FieldSortTypeDef,
+        "Column": ColumnSortTypeDef,
+        "DataPath": DataPathSortOutputTypeDef,
+    },
+    total=False,
+)
+
 PivotTableSortByTypeDef = TypedDict(
     "PivotTableSortByTypeDef",
     {
         "Field": FieldSortTypeDef,
         "Column": ColumnSortTypeDef,
         "DataPath": DataPathSortTypeDef,
     },
@@ -17978,15 +14478,15 @@
     },
 )
 _OptionalDatasetMetadataOutputTypeDef = TypedDict(
     "_OptionalDatasetMetadataOutputTypeDef",
     {
         "DatasetName": str,
         "DatasetDescription": str,
-        "DataAggregation": DataAggregationOutputTypeDef,
+        "DataAggregation": DataAggregationTypeDef,
         "Filters": List[TopicFilterOutputTypeDef],
         "Columns": List[TopicColumnOutputTypeDef],
         "CalculatedFields": List[TopicCalculatedFieldOutputTypeDef],
         "NamedEntities": List[TopicNamedEntityOutputTypeDef],
     },
     total=False,
 )
@@ -18046,22 +14546,14 @@
     "AnonymousUserSnapshotJobResultTypeDef",
     {
         "FileGroups": List[SnapshotJobResultFileGroupTypeDef],
     },
     total=False,
 )
 
-DefaultPaginatedLayoutConfigurationOutputTypeDef = TypedDict(
-    "DefaultPaginatedLayoutConfigurationOutputTypeDef",
-    {
-        "SectionBased": DefaultSectionBasedLayoutConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 DefaultPaginatedLayoutConfigurationTypeDef = TypedDict(
     "DefaultPaginatedLayoutConfigurationTypeDef",
     {
         "SectionBased": DefaultSectionBasedLayoutConfigurationTypeDef,
     },
     total=False,
 )
@@ -18120,18 +14612,18 @@
         "PhysicalTableMap": Dict[str, PhysicalTableOutputTypeDef],
         "LogicalTableMap": Dict[str, LogicalTableOutputTypeDef],
         "OutputColumns": List[OutputColumnTypeDef],
         "ImportMode": DataSetImportModeType,
         "ConsumedSpiceCapacityInBytes": int,
         "ColumnGroups": List[ColumnGroupOutputTypeDef],
         "FieldFolders": Dict[str, FieldFolderOutputTypeDef],
-        "RowLevelPermissionDataSet": RowLevelPermissionDataSetOutputTypeDef,
+        "RowLevelPermissionDataSet": RowLevelPermissionDataSetTypeDef,
         "RowLevelPermissionTagConfiguration": RowLevelPermissionTagConfigurationOutputTypeDef,
         "ColumnLevelPermissionRules": List[ColumnLevelPermissionRuleOutputTypeDef],
-        "DataSetUsageConfiguration": DataSetUsageConfigurationOutputTypeDef,
+        "DataSetUsageConfiguration": DataSetUsageConfigurationTypeDef,
         "DatasetParameters": List[DatasetParameterOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateDataSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSetRequestRequestTypeDef",
@@ -18205,16 +14697,16 @@
     },
 )
 
 VisualCustomActionOperationOutputTypeDef = TypedDict(
     "VisualCustomActionOperationOutputTypeDef",
     {
         "FilterOperation": CustomActionFilterOperationOutputTypeDef,
-        "NavigationOperation": CustomActionNavigationOperationOutputTypeDef,
-        "URLOperation": CustomActionURLOperationOutputTypeDef,
+        "NavigationOperation": CustomActionNavigationOperationTypeDef,
+        "URLOperation": CustomActionURLOperationTypeDef,
         "SetParametersOperation": CustomActionSetParametersOperationOutputTypeDef,
     },
     total=False,
 )
 
 VisualCustomActionOperationTypeDef = TypedDict(
     "VisualCustomActionOperationTypeDef",
@@ -18227,60 +14719,38 @@
     total=False,
 )
 
 LineSeriesAxisDisplayOptionsOutputTypeDef = TypedDict(
     "LineSeriesAxisDisplayOptionsOutputTypeDef",
     {
         "AxisOptions": AxisDisplayOptionsOutputTypeDef,
-        "MissingDataConfigurations": List[MissingDataConfigurationOutputTypeDef],
-    },
-    total=False,
-)
-
-FilterControlOutputTypeDef = TypedDict(
-    "FilterControlOutputTypeDef",
-    {
-        "DateTimePicker": FilterDateTimePickerControlOutputTypeDef,
-        "List": FilterListControlOutputTypeDef,
-        "Dropdown": FilterDropDownControlOutputTypeDef,
-        "TextField": FilterTextFieldControlOutputTypeDef,
-        "TextArea": FilterTextAreaControlOutputTypeDef,
-        "Slider": FilterSliderControlOutputTypeDef,
-        "RelativeDateTime": FilterRelativeDateTimeControlOutputTypeDef,
+        "MissingDataConfigurations": List[MissingDataConfigurationTypeDef],
     },
     total=False,
 )
 
-ParameterControlOutputTypeDef = TypedDict(
-    "ParameterControlOutputTypeDef",
-    {
-        "DateTimePicker": ParameterDateTimePickerControlOutputTypeDef,
-        "List": ParameterListControlOutputTypeDef,
-        "Dropdown": ParameterDropDownControlOutputTypeDef,
-        "TextField": ParameterTextFieldControlOutputTypeDef,
-        "TextArea": ParameterTextAreaControlOutputTypeDef,
-        "Slider": ParameterSliderControlOutputTypeDef,
-    },
-    total=False,
-)
-
-TableFieldURLConfigurationOutputTypeDef = TypedDict(
-    "TableFieldURLConfigurationOutputTypeDef",
+LineSeriesAxisDisplayOptionsTypeDef = TypedDict(
+    "LineSeriesAxisDisplayOptionsTypeDef",
     {
-        "LinkConfiguration": TableFieldLinkConfigurationOutputTypeDef,
-        "ImageConfiguration": TableFieldImageConfigurationOutputTypeDef,
+        "AxisOptions": AxisDisplayOptionsTypeDef,
+        "MissingDataConfigurations": Sequence[MissingDataConfigurationTypeDef],
     },
     total=False,
 )
 
-LineSeriesAxisDisplayOptionsTypeDef = TypedDict(
-    "LineSeriesAxisDisplayOptionsTypeDef",
+FilterControlOutputTypeDef = TypedDict(
+    "FilterControlOutputTypeDef",
     {
-        "AxisOptions": AxisDisplayOptionsTypeDef,
-        "MissingDataConfigurations": Sequence[MissingDataConfigurationTypeDef],
+        "DateTimePicker": FilterDateTimePickerControlTypeDef,
+        "List": FilterListControlOutputTypeDef,
+        "Dropdown": FilterDropDownControlOutputTypeDef,
+        "TextField": FilterTextFieldControlTypeDef,
+        "TextArea": FilterTextAreaControlTypeDef,
+        "Slider": FilterSliderControlTypeDef,
+        "RelativeDateTime": FilterRelativeDateTimeControlTypeDef,
     },
     total=False,
 )
 
 FilterControlTypeDef = TypedDict(
     "FilterControlTypeDef",
     {
@@ -18291,14 +14761,27 @@
         "TextArea": FilterTextAreaControlTypeDef,
         "Slider": FilterSliderControlTypeDef,
         "RelativeDateTime": FilterRelativeDateTimeControlTypeDef,
     },
     total=False,
 )
 
+ParameterControlOutputTypeDef = TypedDict(
+    "ParameterControlOutputTypeDef",
+    {
+        "DateTimePicker": ParameterDateTimePickerControlTypeDef,
+        "List": ParameterListControlOutputTypeDef,
+        "Dropdown": ParameterDropDownControlOutputTypeDef,
+        "TextField": ParameterTextFieldControlTypeDef,
+        "TextArea": ParameterTextAreaControlTypeDef,
+        "Slider": ParameterSliderControlTypeDef,
+    },
+    total=False,
+)
+
 ParameterControlTypeDef = TypedDict(
     "ParameterControlTypeDef",
     {
         "DateTimePicker": ParameterDateTimePickerControlTypeDef,
         "List": ParameterListControlTypeDef,
         "Dropdown": ParameterDropDownControlTypeDef,
         "TextField": ParameterTextFieldControlTypeDef,
@@ -18318,16 +14801,16 @@
 )
 
 PivotTableTotalOptionsOutputTypeDef = TypedDict(
     "PivotTableTotalOptionsOutputTypeDef",
     {
         "RowSubtotalOptions": SubtotalOptionsOutputTypeDef,
         "ColumnSubtotalOptions": SubtotalOptionsOutputTypeDef,
-        "RowTotalOptions": PivotTotalOptionsOutputTypeDef,
-        "ColumnTotalOptions": PivotTotalOptionsOutputTypeDef,
+        "RowTotalOptions": PivotTotalOptionsTypeDef,
+        "ColumnTotalOptions": PivotTotalOptionsTypeDef,
     },
     total=False,
 )
 
 PivotTableTotalOptionsTypeDef = TypedDict(
     "PivotTableTotalOptionsTypeDef",
     {
@@ -18383,16 +14866,16 @@
         "FieldId": str,
     },
 )
 _OptionalPivotTableCellConditionalFormattingOutputTypeDef = TypedDict(
     "_OptionalPivotTableCellConditionalFormattingOutputTypeDef",
     {
         "TextFormat": TextConditionalFormatOutputTypeDef,
-        "Scope": PivotTableConditionalFormattingScopeOutputTypeDef,
-        "Scopes": List[PivotTableConditionalFormattingScopeOutputTypeDef],
+        "Scope": PivotTableConditionalFormattingScopeTypeDef,
+        "Scopes": List[PivotTableConditionalFormattingScopeTypeDef],
     },
     total=False,
 )
 
 class PivotTableCellConditionalFormattingOutputTypeDef(
     _RequiredPivotTableCellConditionalFormattingOutputTypeDef,
     _OptionalPivotTableCellConditionalFormattingOutputTypeDef,
@@ -18601,190 +15084,14 @@
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
         "Type": ThemeTypeType,
     },
     total=False,
 )
 
-GaugeChartOptionsOutputTypeDef = TypedDict(
-    "GaugeChartOptionsOutputTypeDef",
-    {
-        "PrimaryValueDisplayType": PrimaryValueDisplayTypeType,
-        "Comparison": ComparisonConfigurationOutputTypeDef,
-        "ArcAxis": ArcAxisConfigurationOutputTypeDef,
-        "Arc": ArcConfigurationOutputTypeDef,
-        "PrimaryValueFontConfiguration": FontConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-KPIOptionsOutputTypeDef = TypedDict(
-    "KPIOptionsOutputTypeDef",
-    {
-        "ProgressBar": ProgressBarOptionsOutputTypeDef,
-        "TrendArrows": TrendArrowOptionsOutputTypeDef,
-        "SecondaryValue": SecondaryValueOptionsOutputTypeDef,
-        "Comparison": ComparisonConfigurationOutputTypeDef,
-        "PrimaryValueDisplayType": PrimaryValueDisplayTypeType,
-        "PrimaryValueFontConfiguration": FontConfigurationOutputTypeDef,
-        "SecondaryValueFontConfiguration": FontConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDateDimensionFieldOutputTypeDef = TypedDict(
-    "_RequiredDateDimensionFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalDateDimensionFieldOutputTypeDef = TypedDict(
-    "_OptionalDateDimensionFieldOutputTypeDef",
-    {
-        "DateGranularity": TimeGranularityType,
-        "HierarchyId": str,
-        "FormatConfiguration": DateTimeFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class DateDimensionFieldOutputTypeDef(
-    _RequiredDateDimensionFieldOutputTypeDef, _OptionalDateDimensionFieldOutputTypeDef
-):
-    pass
-
-_RequiredDateMeasureFieldOutputTypeDef = TypedDict(
-    "_RequiredDateMeasureFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalDateMeasureFieldOutputTypeDef = TypedDict(
-    "_OptionalDateMeasureFieldOutputTypeDef",
-    {
-        "AggregationFunction": DateAggregationFunctionType,
-        "FormatConfiguration": DateTimeFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class DateMeasureFieldOutputTypeDef(
-    _RequiredDateMeasureFieldOutputTypeDef, _OptionalDateMeasureFieldOutputTypeDef
-):
-    pass
-
-_RequiredNumericalDimensionFieldOutputTypeDef = TypedDict(
-    "_RequiredNumericalDimensionFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalNumericalDimensionFieldOutputTypeDef = TypedDict(
-    "_OptionalNumericalDimensionFieldOutputTypeDef",
-    {
-        "HierarchyId": str,
-        "FormatConfiguration": NumberFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class NumericalDimensionFieldOutputTypeDef(
-    _RequiredNumericalDimensionFieldOutputTypeDef, _OptionalNumericalDimensionFieldOutputTypeDef
-):
-    pass
-
-_RequiredNumericalMeasureFieldOutputTypeDef = TypedDict(
-    "_RequiredNumericalMeasureFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalNumericalMeasureFieldOutputTypeDef = TypedDict(
-    "_OptionalNumericalMeasureFieldOutputTypeDef",
-    {
-        "AggregationFunction": NumericalAggregationFunctionOutputTypeDef,
-        "FormatConfiguration": NumberFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class NumericalMeasureFieldOutputTypeDef(
-    _RequiredNumericalMeasureFieldOutputTypeDef, _OptionalNumericalMeasureFieldOutputTypeDef
-):
-    pass
-
-ReferenceLineLabelConfigurationOutputTypeDef = TypedDict(
-    "ReferenceLineLabelConfigurationOutputTypeDef",
-    {
-        "ValueLabelConfiguration": ReferenceLineValueLabelConfigurationOutputTypeDef,
-        "CustomLabelConfiguration": ReferenceLineCustomLabelConfigurationOutputTypeDef,
-        "FontConfiguration": FontConfigurationOutputTypeDef,
-        "FontColor": str,
-        "HorizontalPosition": ReferenceLineLabelHorizontalPositionType,
-        "VerticalPosition": ReferenceLineLabelVerticalPositionType,
-    },
-    total=False,
-)
-
-_RequiredCategoricalDimensionFieldOutputTypeDef = TypedDict(
-    "_RequiredCategoricalDimensionFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalCategoricalDimensionFieldOutputTypeDef = TypedDict(
-    "_OptionalCategoricalDimensionFieldOutputTypeDef",
-    {
-        "HierarchyId": str,
-        "FormatConfiguration": StringFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class CategoricalDimensionFieldOutputTypeDef(
-    _RequiredCategoricalDimensionFieldOutputTypeDef, _OptionalCategoricalDimensionFieldOutputTypeDef
-):
-    pass
-
-_RequiredCategoricalMeasureFieldOutputTypeDef = TypedDict(
-    "_RequiredCategoricalMeasureFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalCategoricalMeasureFieldOutputTypeDef = TypedDict(
-    "_OptionalCategoricalMeasureFieldOutputTypeDef",
-    {
-        "AggregationFunction": CategoricalAggregationFunctionType,
-        "FormatConfiguration": StringFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class CategoricalMeasureFieldOutputTypeDef(
-    _RequiredCategoricalMeasureFieldOutputTypeDef, _OptionalCategoricalMeasureFieldOutputTypeDef
-):
-    pass
-
-FormatConfigurationOutputTypeDef = TypedDict(
-    "FormatConfigurationOutputTypeDef",
-    {
-        "StringFormatConfiguration": StringFormatConfigurationOutputTypeDef,
-        "NumberFormatConfiguration": NumberFormatConfigurationOutputTypeDef,
-        "DateTimeFormatConfiguration": DateTimeFormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 GaugeChartOptionsTypeDef = TypedDict(
     "GaugeChartOptionsTypeDef",
     {
         "PrimaryValueDisplayType": PrimaryValueDisplayTypeType,
         "Comparison": ComparisonConfigurationTypeDef,
         "ArcAxis": ArcAxisConfigurationTypeDef,
         "Arc": ArcConfigurationTypeDef,
@@ -18955,362 +15262,362 @@
     total=False,
 )
 
 FilterOutputTypeDef = TypedDict(
     "FilterOutputTypeDef",
     {
         "CategoryFilter": CategoryFilterOutputTypeDef,
-        "NumericRangeFilter": NumericRangeFilterOutputTypeDef,
-        "NumericEqualityFilter": NumericEqualityFilterOutputTypeDef,
+        "NumericRangeFilter": NumericRangeFilterTypeDef,
+        "NumericEqualityFilter": NumericEqualityFilterTypeDef,
         "TimeEqualityFilter": TimeEqualityFilterOutputTypeDef,
         "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
-        "RelativeDatesFilter": RelativeDatesFilterOutputTypeDef,
+        "RelativeDatesFilter": RelativeDatesFilterTypeDef,
         "TopBottomFilter": TopBottomFilterOutputTypeDef,
     },
     total=False,
 )
 
-BarChartSortConfigurationOutputTypeDef = TypedDict(
-    "BarChartSortConfigurationOutputTypeDef",
+FilterTypeDef = TypedDict(
+    "FilterTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "ColorSort": List[FieldSortOptionsOutputTypeDef],
-        "ColorItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "SmallMultiplesSort": List[FieldSortOptionsOutputTypeDef],
-        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
+        "CategoryFilter": CategoryFilterTypeDef,
+        "NumericRangeFilter": NumericRangeFilterTypeDef,
+        "NumericEqualityFilter": NumericEqualityFilterTypeDef,
+        "TimeEqualityFilter": TimeEqualityFilterTypeDef,
+        "TimeRangeFilter": TimeRangeFilterTypeDef,
+        "RelativeDatesFilter": RelativeDatesFilterTypeDef,
+        "TopBottomFilter": TopBottomFilterTypeDef,
     },
     total=False,
 )
 
-BoxPlotSortConfigurationOutputTypeDef = TypedDict(
-    "BoxPlotSortConfigurationOutputTypeDef",
+BarChartSortConfigurationOutputTypeDef = TypedDict(
+    "BarChartSortConfigurationOutputTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "PaginationConfiguration": PaginationConfigurationOutputTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "ColorSort": List[FieldSortOptionsTypeDef],
+        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
+        "SmallMultiplesSort": List[FieldSortOptionsTypeDef],
+        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-ComboChartSortConfigurationOutputTypeDef = TypedDict(
-    "ComboChartSortConfigurationOutputTypeDef",
+BarChartSortConfigurationTypeDef = TypedDict(
+    "BarChartSortConfigurationTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "ColorSort": List[FieldSortOptionsOutputTypeDef],
-        "ColorItemsLimit": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "ColorSort": Sequence[FieldSortOptionsTypeDef],
+        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
+        "SmallMultiplesSort": Sequence[FieldSortOptionsTypeDef],
+        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-FilledMapSortConfigurationOutputTypeDef = TypedDict(
-    "FilledMapSortConfigurationOutputTypeDef",
+BoxPlotSortConfigurationOutputTypeDef = TypedDict(
+    "BoxPlotSortConfigurationOutputTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "PaginationConfiguration": PaginationConfigurationTypeDef,
     },
     total=False,
 )
 
-FunnelChartSortConfigurationOutputTypeDef = TypedDict(
-    "FunnelChartSortConfigurationOutputTypeDef",
+BoxPlotSortConfigurationTypeDef = TypedDict(
+    "BoxPlotSortConfigurationTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "PaginationConfiguration": PaginationConfigurationTypeDef,
     },
     total=False,
 )
 
-HeatMapSortConfigurationOutputTypeDef = TypedDict(
-    "HeatMapSortConfigurationOutputTypeDef",
+ComboChartSortConfigurationOutputTypeDef = TypedDict(
+    "ComboChartSortConfigurationOutputTypeDef",
     {
-        "HeatMapRowSort": List[FieldSortOptionsOutputTypeDef],
-        "HeatMapColumnSort": List[FieldSortOptionsOutputTypeDef],
-        "HeatMapRowItemsLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
-        "HeatMapColumnItemsLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "ColorSort": List[FieldSortOptionsTypeDef],
+        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-KPISortConfigurationOutputTypeDef = TypedDict(
-    "KPISortConfigurationOutputTypeDef",
+ComboChartSortConfigurationTypeDef = TypedDict(
+    "ComboChartSortConfigurationTypeDef",
     {
-        "TrendGroupSort": List[FieldSortOptionsOutputTypeDef],
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "ColorSort": Sequence[FieldSortOptionsTypeDef],
+        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-LineChartSortConfigurationOutputTypeDef = TypedDict(
-    "LineChartSortConfigurationOutputTypeDef",
+FilledMapSortConfigurationOutputTypeDef = TypedDict(
+    "FilledMapSortConfigurationOutputTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "CategoryItemsLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
-        "ColorItemsLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
-        "SmallMultiplesSort": List[FieldSortOptionsOutputTypeDef],
-        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
     },
     total=False,
 )
 
-PieChartSortConfigurationOutputTypeDef = TypedDict(
-    "PieChartSortConfigurationOutputTypeDef",
+FilledMapSortConfigurationTypeDef = TypedDict(
+    "FilledMapSortConfigurationTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "SmallMultiplesSort": List[FieldSortOptionsOutputTypeDef],
-        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
     },
     total=False,
 )
 
-RadarChartSortConfigurationOutputTypeDef = TypedDict(
-    "RadarChartSortConfigurationOutputTypeDef",
+FunnelChartSortConfigurationOutputTypeDef = TypedDict(
+    "FunnelChartSortConfigurationOutputTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "ColorSort": List[FieldSortOptionsOutputTypeDef],
-        "ColorItemsLimit": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-SankeyDiagramSortConfigurationOutputTypeDef = TypedDict(
-    "SankeyDiagramSortConfigurationOutputTypeDef",
+FunnelChartSortConfigurationTypeDef = TypedDict(
+    "FunnelChartSortConfigurationTypeDef",
     {
-        "WeightSort": List[FieldSortOptionsOutputTypeDef],
-        "SourceItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "DestinationItemsLimit": ItemsLimitConfigurationOutputTypeDef,
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-TableSortConfigurationOutputTypeDef = TypedDict(
-    "TableSortConfigurationOutputTypeDef",
+HeatMapSortConfigurationOutputTypeDef = TypedDict(
+    "HeatMapSortConfigurationOutputTypeDef",
     {
-        "RowSort": List[FieldSortOptionsOutputTypeDef],
-        "PaginationConfiguration": PaginationConfigurationOutputTypeDef,
+        "HeatMapRowSort": List[FieldSortOptionsTypeDef],
+        "HeatMapColumnSort": List[FieldSortOptionsTypeDef],
+        "HeatMapRowItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "HeatMapColumnItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-TreeMapSortConfigurationOutputTypeDef = TypedDict(
-    "TreeMapSortConfigurationOutputTypeDef",
+HeatMapSortConfigurationTypeDef = TypedDict(
+    "HeatMapSortConfigurationTypeDef",
     {
-        "TreeMapSort": List[FieldSortOptionsOutputTypeDef],
-        "TreeMapGroupItemsLimitConfiguration": ItemsLimitConfigurationOutputTypeDef,
+        "HeatMapRowSort": Sequence[FieldSortOptionsTypeDef],
+        "HeatMapColumnSort": Sequence[FieldSortOptionsTypeDef],
+        "HeatMapRowItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "HeatMapColumnItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-WaterfallChartSortConfigurationOutputTypeDef = TypedDict(
-    "WaterfallChartSortConfigurationOutputTypeDef",
+KPISortConfigurationOutputTypeDef = TypedDict(
+    "KPISortConfigurationOutputTypeDef",
     {
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
-        "BreakdownItemsLimit": ItemsLimitConfigurationOutputTypeDef,
+        "TrendGroupSort": List[FieldSortOptionsTypeDef],
     },
     total=False,
 )
 
-WordCloudSortConfigurationOutputTypeDef = TypedDict(
-    "WordCloudSortConfigurationOutputTypeDef",
+KPISortConfigurationTypeDef = TypedDict(
+    "KPISortConfigurationTypeDef",
     {
-        "CategoryItemsLimit": ItemsLimitConfigurationOutputTypeDef,
-        "CategorySort": List[FieldSortOptionsOutputTypeDef],
+        "TrendGroupSort": Sequence[FieldSortOptionsTypeDef],
     },
     total=False,
 )
 
-PivotFieldSortOptionsOutputTypeDef = TypedDict(
-    "PivotFieldSortOptionsOutputTypeDef",
+LineChartSortConfigurationOutputTypeDef = TypedDict(
+    "LineChartSortConfigurationOutputTypeDef",
     {
-        "FieldId": str,
-        "SortBy": PivotTableSortByOutputTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "CategoryItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "ColorItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "SmallMultiplesSort": List[FieldSortOptionsTypeDef],
+        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
+    total=False,
 )
 
-FieldBasedTooltipOutputTypeDef = TypedDict(
-    "FieldBasedTooltipOutputTypeDef",
+LineChartSortConfigurationTypeDef = TypedDict(
+    "LineChartSortConfigurationTypeDef",
     {
-        "AggregationVisibility": VisibilityType,
-        "TooltipTitleType": TooltipTitleTypeType,
-        "TooltipFields": List[TooltipItemOutputTypeDef],
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "CategoryItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "ColorItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "SmallMultiplesSort": Sequence[FieldSortOptionsTypeDef],
+        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-FilterTypeDef = TypedDict(
-    "FilterTypeDef",
+PieChartSortConfigurationOutputTypeDef = TypedDict(
+    "PieChartSortConfigurationOutputTypeDef",
     {
-        "CategoryFilter": CategoryFilterTypeDef,
-        "NumericRangeFilter": NumericRangeFilterTypeDef,
-        "NumericEqualityFilter": NumericEqualityFilterTypeDef,
-        "TimeEqualityFilter": TimeEqualityFilterTypeDef,
-        "TimeRangeFilter": TimeRangeFilterTypeDef,
-        "RelativeDatesFilter": RelativeDatesFilterTypeDef,
-        "TopBottomFilter": TopBottomFilterTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "SmallMultiplesSort": List[FieldSortOptionsTypeDef],
+        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-BarChartSortConfigurationTypeDef = TypedDict(
-    "BarChartSortConfigurationTypeDef",
+PieChartSortConfigurationTypeDef = TypedDict(
+    "PieChartSortConfigurationTypeDef",
     {
         "CategorySort": Sequence[FieldSortOptionsTypeDef],
         "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
-        "ColorSort": Sequence[FieldSortOptionsTypeDef],
-        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
         "SmallMultiplesSort": Sequence[FieldSortOptionsTypeDef],
         "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-BoxPlotSortConfigurationTypeDef = TypedDict(
-    "BoxPlotSortConfigurationTypeDef",
+RadarChartSortConfigurationOutputTypeDef = TypedDict(
+    "RadarChartSortConfigurationOutputTypeDef",
     {
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
-        "PaginationConfiguration": PaginationConfigurationTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "ColorSort": List[FieldSortOptionsTypeDef],
+        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-ComboChartSortConfigurationTypeDef = TypedDict(
-    "ComboChartSortConfigurationTypeDef",
+RadarChartSortConfigurationTypeDef = TypedDict(
+    "RadarChartSortConfigurationTypeDef",
     {
         "CategorySort": Sequence[FieldSortOptionsTypeDef],
         "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
         "ColorSort": Sequence[FieldSortOptionsTypeDef],
         "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-FilledMapSortConfigurationTypeDef = TypedDict(
-    "FilledMapSortConfigurationTypeDef",
-    {
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
-    },
-    total=False,
-)
-
-FunnelChartSortConfigurationTypeDef = TypedDict(
-    "FunnelChartSortConfigurationTypeDef",
+SankeyDiagramSortConfigurationOutputTypeDef = TypedDict(
+    "SankeyDiagramSortConfigurationOutputTypeDef",
     {
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "WeightSort": List[FieldSortOptionsTypeDef],
+        "SourceItemsLimit": ItemsLimitConfigurationTypeDef,
+        "DestinationItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-HeatMapSortConfigurationTypeDef = TypedDict(
-    "HeatMapSortConfigurationTypeDef",
+SankeyDiagramSortConfigurationTypeDef = TypedDict(
+    "SankeyDiagramSortConfigurationTypeDef",
     {
-        "HeatMapRowSort": Sequence[FieldSortOptionsTypeDef],
-        "HeatMapColumnSort": Sequence[FieldSortOptionsTypeDef],
-        "HeatMapRowItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
-        "HeatMapColumnItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "WeightSort": Sequence[FieldSortOptionsTypeDef],
+        "SourceItemsLimit": ItemsLimitConfigurationTypeDef,
+        "DestinationItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-KPISortConfigurationTypeDef = TypedDict(
-    "KPISortConfigurationTypeDef",
+TableSortConfigurationOutputTypeDef = TypedDict(
+    "TableSortConfigurationOutputTypeDef",
     {
-        "TrendGroupSort": Sequence[FieldSortOptionsTypeDef],
+        "RowSort": List[FieldSortOptionsTypeDef],
+        "PaginationConfiguration": PaginationConfigurationTypeDef,
     },
     total=False,
 )
 
-LineChartSortConfigurationTypeDef = TypedDict(
-    "LineChartSortConfigurationTypeDef",
+TableSortConfigurationTypeDef = TypedDict(
+    "TableSortConfigurationTypeDef",
     {
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
-        "CategoryItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
-        "ColorItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
-        "SmallMultiplesSort": Sequence[FieldSortOptionsTypeDef],
-        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "RowSort": Sequence[FieldSortOptionsTypeDef],
+        "PaginationConfiguration": PaginationConfigurationTypeDef,
     },
     total=False,
 )
 
-PieChartSortConfigurationTypeDef = TypedDict(
-    "PieChartSortConfigurationTypeDef",
+TreeMapSortConfigurationOutputTypeDef = TypedDict(
+    "TreeMapSortConfigurationOutputTypeDef",
     {
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
-        "SmallMultiplesSort": Sequence[FieldSortOptionsTypeDef],
-        "SmallMultiplesLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "TreeMapSort": List[FieldSortOptionsTypeDef],
+        "TreeMapGroupItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-RadarChartSortConfigurationTypeDef = TypedDict(
-    "RadarChartSortConfigurationTypeDef",
+TreeMapSortConfigurationTypeDef = TypedDict(
+    "TreeMapSortConfigurationTypeDef",
     {
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
-        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
-        "ColorSort": Sequence[FieldSortOptionsTypeDef],
-        "ColorItemsLimit": ItemsLimitConfigurationTypeDef,
+        "TreeMapSort": Sequence[FieldSortOptionsTypeDef],
+        "TreeMapGroupItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-SankeyDiagramSortConfigurationTypeDef = TypedDict(
-    "SankeyDiagramSortConfigurationTypeDef",
+WaterfallChartSortConfigurationOutputTypeDef = TypedDict(
+    "WaterfallChartSortConfigurationOutputTypeDef",
     {
-        "WeightSort": Sequence[FieldSortOptionsTypeDef],
-        "SourceItemsLimit": ItemsLimitConfigurationTypeDef,
-        "DestinationItemsLimit": ItemsLimitConfigurationTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
+        "BreakdownItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-TableSortConfigurationTypeDef = TypedDict(
-    "TableSortConfigurationTypeDef",
+WaterfallChartSortConfigurationTypeDef = TypedDict(
+    "WaterfallChartSortConfigurationTypeDef",
     {
-        "RowSort": Sequence[FieldSortOptionsTypeDef],
-        "PaginationConfiguration": PaginationConfigurationTypeDef,
+        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "BreakdownItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-TreeMapSortConfigurationTypeDef = TypedDict(
-    "TreeMapSortConfigurationTypeDef",
+WordCloudSortConfigurationOutputTypeDef = TypedDict(
+    "WordCloudSortConfigurationOutputTypeDef",
     {
-        "TreeMapSort": Sequence[FieldSortOptionsTypeDef],
-        "TreeMapGroupItemsLimitConfiguration": ItemsLimitConfigurationTypeDef,
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
+        "CategorySort": List[FieldSortOptionsTypeDef],
     },
     total=False,
 )
 
-WaterfallChartSortConfigurationTypeDef = TypedDict(
-    "WaterfallChartSortConfigurationTypeDef",
+WordCloudSortConfigurationTypeDef = TypedDict(
+    "WordCloudSortConfigurationTypeDef",
     {
+        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
         "CategorySort": Sequence[FieldSortOptionsTypeDef],
-        "BreakdownItemsLimit": ItemsLimitConfigurationTypeDef,
     },
     total=False,
 )
 
-WordCloudSortConfigurationTypeDef = TypedDict(
-    "WordCloudSortConfigurationTypeDef",
+PivotFieldSortOptionsOutputTypeDef = TypedDict(
+    "PivotFieldSortOptionsOutputTypeDef",
     {
-        "CategoryItemsLimit": ItemsLimitConfigurationTypeDef,
-        "CategorySort": Sequence[FieldSortOptionsTypeDef],
+        "FieldId": str,
+        "SortBy": PivotTableSortByOutputTypeDef,
     },
-    total=False,
 )
 
 PivotFieldSortOptionsTypeDef = TypedDict(
     "PivotFieldSortOptionsTypeDef",
     {
         "FieldId": str,
         "SortBy": PivotTableSortByTypeDef,
     },
 )
 
+FieldBasedTooltipOutputTypeDef = TypedDict(
+    "FieldBasedTooltipOutputTypeDef",
+    {
+        "AggregationVisibility": VisibilityType,
+        "TooltipTitleType": TooltipTitleTypeType,
+        "TooltipFields": List[TooltipItemTypeDef],
+    },
+    total=False,
+)
+
 FieldBasedTooltipTypeDef = TypedDict(
     "FieldBasedTooltipTypeDef",
     {
         "AggregationVisibility": VisibilityType,
         "TooltipTitleType": TooltipTitleTypeType,
         "TooltipFields": Sequence[TooltipItemTypeDef],
     },
@@ -19341,24 +15648,14 @@
     "SnapshotJobResultTypeDef",
     {
         "AnonymousUsers": List[AnonymousUserSnapshotJobResultTypeDef],
     },
     total=False,
 )
 
-DefaultNewSheetConfigurationOutputTypeDef = TypedDict(
-    "DefaultNewSheetConfigurationOutputTypeDef",
-    {
-        "InteractiveLayoutConfiguration": DefaultInteractiveLayoutConfigurationOutputTypeDef,
-        "PaginatedLayoutConfiguration": DefaultPaginatedLayoutConfigurationOutputTypeDef,
-        "SheetContentType": SheetContentTypeType,
-    },
-    total=False,
-)
-
 DefaultNewSheetConfigurationTypeDef = TypedDict(
     "DefaultNewSheetConfigurationTypeDef",
     {
         "InteractiveLayoutConfiguration": DefaultInteractiveLayoutConfigurationTypeDef,
         "PaginatedLayoutConfiguration": DefaultPaginatedLayoutConfigurationTypeDef,
         "SheetContentType": SheetContentTypeType,
     },
@@ -19379,15 +15676,15 @@
         "SectionId": str,
         "Layout": SectionLayoutConfigurationOutputTypeDef,
     },
 )
 _OptionalHeaderFooterSectionConfigurationOutputTypeDef = TypedDict(
     "_OptionalHeaderFooterSectionConfigurationOutputTypeDef",
     {
-        "Style": SectionStyleOutputTypeDef,
+        "Style": SectionStyleTypeDef,
     },
     total=False,
 )
 
 class HeaderFooterSectionConfigurationOutputTypeDef(
     _RequiredHeaderFooterSectionConfigurationOutputTypeDef,
     _OptionalHeaderFooterSectionConfigurationOutputTypeDef,
@@ -19473,36 +15770,14 @@
 )
 
 class VisualCustomActionTypeDef(
     _RequiredVisualCustomActionTypeDef, _OptionalVisualCustomActionTypeDef
 ):
     pass
 
-_RequiredTableFieldOptionOutputTypeDef = TypedDict(
-    "_RequiredTableFieldOptionOutputTypeDef",
-    {
-        "FieldId": str,
-    },
-)
-_OptionalTableFieldOptionOutputTypeDef = TypedDict(
-    "_OptionalTableFieldOptionOutputTypeDef",
-    {
-        "Width": str,
-        "CustomLabel": str,
-        "Visibility": VisibilityType,
-        "URLStyling": TableFieldURLConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class TableFieldOptionOutputTypeDef(
-    _RequiredTableFieldOptionOutputTypeDef, _OptionalTableFieldOptionOutputTypeDef
-):
-    pass
-
 _RequiredTableFieldOptionTypeDef = TypedDict(
     "_RequiredTableFieldOptionTypeDef",
     {
         "FieldId": str,
     },
 )
 _OptionalTableFieldOptionTypeDef = TypedDict(
@@ -19605,97 +15880,14 @@
         "Theme": ThemeTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredReferenceLineOutputTypeDef = TypedDict(
-    "_RequiredReferenceLineOutputTypeDef",
-    {
-        "DataConfiguration": ReferenceLineDataConfigurationOutputTypeDef,
-    },
-)
-_OptionalReferenceLineOutputTypeDef = TypedDict(
-    "_OptionalReferenceLineOutputTypeDef",
-    {
-        "Status": WidgetStatusType,
-        "StyleConfiguration": ReferenceLineStyleConfigurationOutputTypeDef,
-        "LabelConfiguration": ReferenceLineLabelConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class ReferenceLineOutputTypeDef(
-    _RequiredReferenceLineOutputTypeDef, _OptionalReferenceLineOutputTypeDef
-):
-    pass
-
-DimensionFieldOutputTypeDef = TypedDict(
-    "DimensionFieldOutputTypeDef",
-    {
-        "NumericalDimensionField": NumericalDimensionFieldOutputTypeDef,
-        "CategoricalDimensionField": CategoricalDimensionFieldOutputTypeDef,
-        "DateDimensionField": DateDimensionFieldOutputTypeDef,
-    },
-    total=False,
-)
-
-MeasureFieldOutputTypeDef = TypedDict(
-    "MeasureFieldOutputTypeDef",
-    {
-        "NumericalMeasureField": NumericalMeasureFieldOutputTypeDef,
-        "CategoricalMeasureField": CategoricalMeasureFieldOutputTypeDef,
-        "DateMeasureField": DateMeasureFieldOutputTypeDef,
-        "CalculatedMeasureField": CalculatedMeasureFieldOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredColumnConfigurationOutputTypeDef = TypedDict(
-    "_RequiredColumnConfigurationOutputTypeDef",
-    {
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalColumnConfigurationOutputTypeDef = TypedDict(
-    "_OptionalColumnConfigurationOutputTypeDef",
-    {
-        "FormatConfiguration": FormatConfigurationOutputTypeDef,
-        "Role": ColumnRoleType,
-        "ColorsConfiguration": ColorsConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class ColumnConfigurationOutputTypeDef(
-    _RequiredColumnConfigurationOutputTypeDef, _OptionalColumnConfigurationOutputTypeDef
-):
-    pass
-
-_RequiredUnaggregatedFieldOutputTypeDef = TypedDict(
-    "_RequiredUnaggregatedFieldOutputTypeDef",
-    {
-        "FieldId": str,
-        "Column": ColumnIdentifierOutputTypeDef,
-    },
-)
-_OptionalUnaggregatedFieldOutputTypeDef = TypedDict(
-    "_OptionalUnaggregatedFieldOutputTypeDef",
-    {
-        "FormatConfiguration": FormatConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class UnaggregatedFieldOutputTypeDef(
-    _RequiredUnaggregatedFieldOutputTypeDef, _OptionalUnaggregatedFieldOutputTypeDef
-):
-    pass
-
 _RequiredReferenceLineTypeDef = TypedDict(
     "_RequiredReferenceLineTypeDef",
     {
         "DataConfiguration": ReferenceLineDataConfigurationTypeDef,
     },
 )
 _OptionalReferenceLineTypeDef = TypedDict(
@@ -19728,14 +15920,35 @@
         "CategoricalMeasureField": CategoricalMeasureFieldTypeDef,
         "DateMeasureField": DateMeasureFieldTypeDef,
         "CalculatedMeasureField": CalculatedMeasureFieldTypeDef,
     },
     total=False,
 )
 
+_RequiredColumnConfigurationOutputTypeDef = TypedDict(
+    "_RequiredColumnConfigurationOutputTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+    },
+)
+_OptionalColumnConfigurationOutputTypeDef = TypedDict(
+    "_OptionalColumnConfigurationOutputTypeDef",
+    {
+        "FormatConfiguration": FormatConfigurationTypeDef,
+        "Role": ColumnRoleType,
+        "ColorsConfiguration": ColorsConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class ColumnConfigurationOutputTypeDef(
+    _RequiredColumnConfigurationOutputTypeDef, _OptionalColumnConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredColumnConfigurationTypeDef = TypedDict(
     "_RequiredColumnConfigurationTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
     },
 )
 _OptionalColumnConfigurationTypeDef = TypedDict(
@@ -19791,32 +16004,14 @@
 )
 
 class FilterGroupOutputTypeDef(
     _RequiredFilterGroupOutputTypeDef, _OptionalFilterGroupOutputTypeDef
 ):
     pass
 
-PivotTableSortConfigurationOutputTypeDef = TypedDict(
-    "PivotTableSortConfigurationOutputTypeDef",
-    {
-        "FieldSortOptions": List[PivotFieldSortOptionsOutputTypeDef],
-    },
-    total=False,
-)
-
-TooltipOptionsOutputTypeDef = TypedDict(
-    "TooltipOptionsOutputTypeDef",
-    {
-        "TooltipVisibility": VisibilityType,
-        "SelectedTooltipType": SelectedTooltipTypeType,
-        "FieldBasedTooltip": FieldBasedTooltipOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredFilterGroupTypeDef = TypedDict(
     "_RequiredFilterGroupTypeDef",
     {
         "FilterGroupId": str,
         "Filters": Sequence[FilterTypeDef],
         "ScopeConfiguration": FilterScopeConfigurationTypeDef,
         "CrossDataset": CrossDatasetTypesType,
@@ -19829,22 +16024,40 @@
     },
     total=False,
 )
 
 class FilterGroupTypeDef(_RequiredFilterGroupTypeDef, _OptionalFilterGroupTypeDef):
     pass
 
+PivotTableSortConfigurationOutputTypeDef = TypedDict(
+    "PivotTableSortConfigurationOutputTypeDef",
+    {
+        "FieldSortOptions": List[PivotFieldSortOptionsOutputTypeDef],
+    },
+    total=False,
+)
+
 PivotTableSortConfigurationTypeDef = TypedDict(
     "PivotTableSortConfigurationTypeDef",
     {
         "FieldSortOptions": Sequence[PivotFieldSortOptionsTypeDef],
     },
     total=False,
 )
 
+TooltipOptionsOutputTypeDef = TypedDict(
+    "TooltipOptionsOutputTypeDef",
+    {
+        "TooltipVisibility": VisibilityType,
+        "SelectedTooltipType": SelectedTooltipTypeType,
+        "FieldBasedTooltip": FieldBasedTooltipOutputTypeDef,
+    },
+    total=False,
+)
+
 TooltipOptionsTypeDef = TypedDict(
     "TooltipOptionsTypeDef",
     {
         "TooltipVisibility": VisibilityType,
         "SelectedTooltipType": SelectedTooltipTypeType,
         "FieldBasedTooltip": FieldBasedTooltipTypeDef,
     },
@@ -19904,21 +16117,14 @@
         "ErrorInfo": SnapshotJobErrorInfoTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AnalysisDefaultsOutputTypeDef = TypedDict(
-    "AnalysisDefaultsOutputTypeDef",
-    {
-        "DefaultNewSheetConfiguration": DefaultNewSheetConfigurationOutputTypeDef,
-    },
-)
-
 AnalysisDefaultsTypeDef = TypedDict(
     "AnalysisDefaultsTypeDef",
     {
         "DefaultNewSheetConfiguration": DefaultNewSheetConfigurationTypeDef,
     },
 )
 
@@ -19928,16 +16134,16 @@
         "SectionId": str,
         "Content": BodySectionContentOutputTypeDef,
     },
 )
 _OptionalBodySectionConfigurationOutputTypeDef = TypedDict(
     "_OptionalBodySectionConfigurationOutputTypeDef",
     {
-        "Style": SectionStyleOutputTypeDef,
-        "PageBreakConfiguration": SectionPageBreakConfigurationOutputTypeDef,
+        "Style": SectionStyleTypeDef,
+        "PageBreakConfiguration": SectionPageBreakConfigurationTypeDef,
     },
     total=False,
 )
 
 class BodySectionConfigurationOutputTypeDef(
     _RequiredBodySectionConfigurationOutputTypeDef, _OptionalBodySectionConfigurationOutputTypeDef
 ):
@@ -19970,17 +16176,17 @@
         "VisualId": str,
         "DataSetIdentifier": str,
     },
 )
 _OptionalCustomContentVisualOutputTypeDef = TypedDict(
     "_OptionalCustomContentVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": CustomContentConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": CustomContentConfigurationTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
 class CustomContentVisualOutputTypeDef(
     _RequiredCustomContentVisualOutputTypeDef, _OptionalCustomContentVisualOutputTypeDef
@@ -20047,15 +16253,15 @@
 
 class EmptyVisualTypeDef(_RequiredEmptyVisualTypeDef, _OptionalEmptyVisualTypeDef):
     pass
 
 TableFieldOptionsOutputTypeDef = TypedDict(
     "TableFieldOptionsOutputTypeDef",
     {
-        "SelectedFieldOptions": List[TableFieldOptionOutputTypeDef],
+        "SelectedFieldOptions": List[TableFieldOptionTypeDef],
         "Order": List[str],
     },
     total=False,
 )
 
 TableFieldOptionsTypeDef = TypedDict(
     "TableFieldOptionsTypeDef",
@@ -20108,497 +16314,81 @@
     "TableConditionalFormattingTypeDef",
     {
         "ConditionalFormattingOptions": Sequence[TableConditionalFormattingOptionTypeDef],
     },
     total=False,
 )
 
-_RequiredUniqueValuesComputationOutputTypeDef = TypedDict(
-    "_RequiredUniqueValuesComputationOutputTypeDef",
+_RequiredUniqueValuesComputationTypeDef = TypedDict(
+    "_RequiredUniqueValuesComputationTypeDef",
     {
         "ComputationId": str,
-        "Category": DimensionFieldOutputTypeDef,
+        "Category": DimensionFieldTypeDef,
     },
 )
-_OptionalUniqueValuesComputationOutputTypeDef = TypedDict(
-    "_OptionalUniqueValuesComputationOutputTypeDef",
+_OptionalUniqueValuesComputationTypeDef = TypedDict(
+    "_OptionalUniqueValuesComputationTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-class UniqueValuesComputationOutputTypeDef(
-    _RequiredUniqueValuesComputationOutputTypeDef, _OptionalUniqueValuesComputationOutputTypeDef
+class UniqueValuesComputationTypeDef(
+    _RequiredUniqueValuesComputationTypeDef, _OptionalUniqueValuesComputationTypeDef
 ):
     pass
 
 BarChartAggregatedFieldWellsOutputTypeDef = TypedDict(
     "BarChartAggregatedFieldWellsOutputTypeDef",
     {
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-        "Colors": List[DimensionFieldOutputTypeDef],
-        "SmallMultiples": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-BoxPlotAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "BoxPlotAggregatedFieldWellsOutputTypeDef",
-    {
-        "GroupBy": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-ComboChartAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "ComboChartAggregatedFieldWellsOutputTypeDef",
-    {
-        "Category": List[DimensionFieldOutputTypeDef],
-        "BarValues": List[MeasureFieldOutputTypeDef],
-        "Colors": List[DimensionFieldOutputTypeDef],
-        "LineValues": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-FilledMapAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "FilledMapAggregatedFieldWellsOutputTypeDef",
-    {
-        "Geospatial": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-_RequiredForecastComputationOutputTypeDef = TypedDict(
-    "_RequiredForecastComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-    },
-)
-_OptionalForecastComputationOutputTypeDef = TypedDict(
-    "_OptionalForecastComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-        "PeriodsForward": int,
-        "PeriodsBackward": int,
-        "UpperBoundary": float,
-        "LowerBoundary": float,
-        "PredictionInterval": int,
-        "Seasonality": ForecastComputationSeasonalityType,
-        "CustomSeasonalityValue": int,
-    },
-    total=False,
-)
-
-class ForecastComputationOutputTypeDef(
-    _RequiredForecastComputationOutputTypeDef, _OptionalForecastComputationOutputTypeDef
-):
-    pass
-
-FunnelChartAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "FunnelChartAggregatedFieldWellsOutputTypeDef",
-    {
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-GaugeChartFieldWellsOutputTypeDef = TypedDict(
-    "GaugeChartFieldWellsOutputTypeDef",
-    {
-        "Values": List[MeasureFieldOutputTypeDef],
-        "TargetValues": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-GeospatialMapAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "GeospatialMapAggregatedFieldWellsOutputTypeDef",
-    {
-        "Geospatial": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-        "Colors": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-_RequiredGrowthRateComputationOutputTypeDef = TypedDict(
-    "_RequiredGrowthRateComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-    },
-)
-_OptionalGrowthRateComputationOutputTypeDef = TypedDict(
-    "_OptionalGrowthRateComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-        "PeriodSize": int,
-    },
-    total=False,
-)
-
-class GrowthRateComputationOutputTypeDef(
-    _RequiredGrowthRateComputationOutputTypeDef, _OptionalGrowthRateComputationOutputTypeDef
-):
-    pass
-
-HeatMapAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "HeatMapAggregatedFieldWellsOutputTypeDef",
-    {
-        "Rows": List[DimensionFieldOutputTypeDef],
-        "Columns": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-HistogramAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "HistogramAggregatedFieldWellsOutputTypeDef",
-    {
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-KPIFieldWellsOutputTypeDef = TypedDict(
-    "KPIFieldWellsOutputTypeDef",
-    {
-        "Values": List[MeasureFieldOutputTypeDef],
-        "TargetValues": List[MeasureFieldOutputTypeDef],
-        "TrendGroups": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-LineChartAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "LineChartAggregatedFieldWellsOutputTypeDef",
-    {
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-        "Colors": List[DimensionFieldOutputTypeDef],
-        "SmallMultiples": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-_RequiredMaximumMinimumComputationOutputTypeDef = TypedDict(
-    "_RequiredMaximumMinimumComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-        "Type": MaximumMinimumComputationTypeType,
-    },
-)
-_OptionalMaximumMinimumComputationOutputTypeDef = TypedDict(
-    "_OptionalMaximumMinimumComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-    },
-    total=False,
-)
-
-class MaximumMinimumComputationOutputTypeDef(
-    _RequiredMaximumMinimumComputationOutputTypeDef, _OptionalMaximumMinimumComputationOutputTypeDef
-):
-    pass
-
-_RequiredMetricComparisonComputationOutputTypeDef = TypedDict(
-    "_RequiredMetricComparisonComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-        "FromValue": MeasureFieldOutputTypeDef,
-        "TargetValue": MeasureFieldOutputTypeDef,
-    },
-)
-_OptionalMetricComparisonComputationOutputTypeDef = TypedDict(
-    "_OptionalMetricComparisonComputationOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-class MetricComparisonComputationOutputTypeDef(
-    _RequiredMetricComparisonComputationOutputTypeDef,
-    _OptionalMetricComparisonComputationOutputTypeDef,
-):
-    pass
-
-_RequiredPeriodOverPeriodComputationOutputTypeDef = TypedDict(
-    "_RequiredPeriodOverPeriodComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-    },
-)
-_OptionalPeriodOverPeriodComputationOutputTypeDef = TypedDict(
-    "_OptionalPeriodOverPeriodComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-    },
-    total=False,
-)
-
-class PeriodOverPeriodComputationOutputTypeDef(
-    _RequiredPeriodOverPeriodComputationOutputTypeDef,
-    _OptionalPeriodOverPeriodComputationOutputTypeDef,
-):
-    pass
-
-_RequiredPeriodToDateComputationOutputTypeDef = TypedDict(
-    "_RequiredPeriodToDateComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-    },
-)
-_OptionalPeriodToDateComputationOutputTypeDef = TypedDict(
-    "_OptionalPeriodToDateComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-        "PeriodTimeGranularity": TimeGranularityType,
-    },
-    total=False,
-)
-
-class PeriodToDateComputationOutputTypeDef(
-    _RequiredPeriodToDateComputationOutputTypeDef, _OptionalPeriodToDateComputationOutputTypeDef
-):
-    pass
-
-PieChartAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "PieChartAggregatedFieldWellsOutputTypeDef",
-    {
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-        "SmallMultiples": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-PivotTableAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "PivotTableAggregatedFieldWellsOutputTypeDef",
-    {
-        "Rows": List[DimensionFieldOutputTypeDef],
-        "Columns": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-RadarChartAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "RadarChartAggregatedFieldWellsOutputTypeDef",
-    {
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Color": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-SankeyDiagramAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "SankeyDiagramAggregatedFieldWellsOutputTypeDef",
-    {
-        "Source": List[DimensionFieldOutputTypeDef],
-        "Destination": List[DimensionFieldOutputTypeDef],
-        "Weight": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef",
-    {
-        "XAxis": List[MeasureFieldOutputTypeDef],
-        "YAxis": List[MeasureFieldOutputTypeDef],
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Size": List[MeasureFieldOutputTypeDef],
-        "Label": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-ScatterPlotUnaggregatedFieldWellsOutputTypeDef = TypedDict(
-    "ScatterPlotUnaggregatedFieldWellsOutputTypeDef",
-    {
-        "XAxis": List[DimensionFieldOutputTypeDef],
-        "YAxis": List[DimensionFieldOutputTypeDef],
-        "Size": List[MeasureFieldOutputTypeDef],
-        "Category": List[DimensionFieldOutputTypeDef],
-        "Label": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-TableAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "TableAggregatedFieldWellsOutputTypeDef",
-    {
-        "GroupBy": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
+        "Category": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+        "Colors": List[DimensionFieldTypeDef],
+        "SmallMultiples": List[DimensionFieldTypeDef],
     },
     total=False,
 )
 
-_RequiredTopBottomMoversComputationOutputTypeDef = TypedDict(
-    "_RequiredTopBottomMoversComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Time": DimensionFieldOutputTypeDef,
-        "Category": DimensionFieldOutputTypeDef,
-        "Type": TopBottomComputationTypeType,
-    },
-)
-_OptionalTopBottomMoversComputationOutputTypeDef = TypedDict(
-    "_OptionalTopBottomMoversComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-        "MoverSize": int,
-        "SortOrder": TopBottomSortOrderType,
-    },
-    total=False,
-)
-
-class TopBottomMoversComputationOutputTypeDef(
-    _RequiredTopBottomMoversComputationOutputTypeDef,
-    _OptionalTopBottomMoversComputationOutputTypeDef,
-):
-    pass
-
-_RequiredTopBottomRankedComputationOutputTypeDef = TypedDict(
-    "_RequiredTopBottomRankedComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Category": DimensionFieldOutputTypeDef,
-        "Type": TopBottomComputationTypeType,
-    },
-)
-_OptionalTopBottomRankedComputationOutputTypeDef = TypedDict(
-    "_OptionalTopBottomRankedComputationOutputTypeDef",
-    {
-        "Name": str,
-        "Value": MeasureFieldOutputTypeDef,
-        "ResultSize": int,
-    },
-    total=False,
-)
-
-class TopBottomRankedComputationOutputTypeDef(
-    _RequiredTopBottomRankedComputationOutputTypeDef,
-    _OptionalTopBottomRankedComputationOutputTypeDef,
-):
-    pass
-
-_RequiredTotalAggregationComputationOutputTypeDef = TypedDict(
-    "_RequiredTotalAggregationComputationOutputTypeDef",
-    {
-        "ComputationId": str,
-        "Value": MeasureFieldOutputTypeDef,
-    },
-)
-_OptionalTotalAggregationComputationOutputTypeDef = TypedDict(
-    "_OptionalTotalAggregationComputationOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-class TotalAggregationComputationOutputTypeDef(
-    _RequiredTotalAggregationComputationOutputTypeDef,
-    _OptionalTotalAggregationComputationOutputTypeDef,
-):
-    pass
-
-TreeMapAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "TreeMapAggregatedFieldWellsOutputTypeDef",
-    {
-        "Groups": List[DimensionFieldOutputTypeDef],
-        "Sizes": List[MeasureFieldOutputTypeDef],
-        "Colors": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-WaterfallChartAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "WaterfallChartAggregatedFieldWellsOutputTypeDef",
-    {
-        "Categories": List[DimensionFieldOutputTypeDef],
-        "Values": List[MeasureFieldOutputTypeDef],
-        "Breakdowns": List[DimensionFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-WordCloudAggregatedFieldWellsOutputTypeDef = TypedDict(
-    "WordCloudAggregatedFieldWellsOutputTypeDef",
-    {
-        "GroupBy": List[DimensionFieldOutputTypeDef],
-        "Size": List[MeasureFieldOutputTypeDef],
-    },
-    total=False,
-)
-
-TableUnaggregatedFieldWellsOutputTypeDef = TypedDict(
-    "TableUnaggregatedFieldWellsOutputTypeDef",
+BarChartAggregatedFieldWellsTypeDef = TypedDict(
+    "BarChartAggregatedFieldWellsTypeDef",
     {
-        "Values": List[UnaggregatedFieldOutputTypeDef],
+        "Category": Sequence[DimensionFieldTypeDef],
+        "Values": Sequence[MeasureFieldTypeDef],
+        "Colors": Sequence[DimensionFieldTypeDef],
+        "SmallMultiples": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
-_RequiredUniqueValuesComputationTypeDef = TypedDict(
-    "_RequiredUniqueValuesComputationTypeDef",
-    {
-        "ComputationId": str,
-        "Category": DimensionFieldTypeDef,
-    },
-)
-_OptionalUniqueValuesComputationTypeDef = TypedDict(
-    "_OptionalUniqueValuesComputationTypeDef",
+BoxPlotAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "BoxPlotAggregatedFieldWellsOutputTypeDef",
     {
-        "Name": str,
+        "GroupBy": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
     },
     total=False,
 )
 
-class UniqueValuesComputationTypeDef(
-    _RequiredUniqueValuesComputationTypeDef, _OptionalUniqueValuesComputationTypeDef
-):
-    pass
-
-BarChartAggregatedFieldWellsTypeDef = TypedDict(
-    "BarChartAggregatedFieldWellsTypeDef",
+BoxPlotAggregatedFieldWellsTypeDef = TypedDict(
+    "BoxPlotAggregatedFieldWellsTypeDef",
     {
-        "Category": Sequence[DimensionFieldTypeDef],
+        "GroupBy": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
-        "Colors": Sequence[DimensionFieldTypeDef],
-        "SmallMultiples": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
-BoxPlotAggregatedFieldWellsTypeDef = TypedDict(
-    "BoxPlotAggregatedFieldWellsTypeDef",
+ComboChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "ComboChartAggregatedFieldWellsOutputTypeDef",
     {
-        "GroupBy": Sequence[DimensionFieldTypeDef],
-        "Values": Sequence[MeasureFieldTypeDef],
+        "Category": List[DimensionFieldTypeDef],
+        "BarValues": List[MeasureFieldTypeDef],
+        "Colors": List[DimensionFieldTypeDef],
+        "LineValues": List[MeasureFieldTypeDef],
     },
     total=False,
 )
 
 ComboChartAggregatedFieldWellsTypeDef = TypedDict(
     "ComboChartAggregatedFieldWellsTypeDef",
     {
@@ -20606,14 +16396,23 @@
         "BarValues": Sequence[MeasureFieldTypeDef],
         "Colors": Sequence[DimensionFieldTypeDef],
         "LineValues": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+FilledMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "FilledMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Geospatial": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 FilledMapAggregatedFieldWellsTypeDef = TypedDict(
     "FilledMapAggregatedFieldWellsTypeDef",
     {
         "Geospatial": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
@@ -20643,32 +16442,60 @@
 )
 
 class ForecastComputationTypeDef(
     _RequiredForecastComputationTypeDef, _OptionalForecastComputationTypeDef
 ):
     pass
 
+FunnelChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "FunnelChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 FunnelChartAggregatedFieldWellsTypeDef = TypedDict(
     "FunnelChartAggregatedFieldWellsTypeDef",
     {
         "Category": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+GaugeChartFieldWellsOutputTypeDef = TypedDict(
+    "GaugeChartFieldWellsOutputTypeDef",
+    {
+        "Values": List[MeasureFieldTypeDef],
+        "TargetValues": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 GaugeChartFieldWellsTypeDef = TypedDict(
     "GaugeChartFieldWellsTypeDef",
     {
         "Values": Sequence[MeasureFieldTypeDef],
         "TargetValues": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+GeospatialMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "GeospatialMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Geospatial": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+        "Colors": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 GeospatialMapAggregatedFieldWellsTypeDef = TypedDict(
     "GeospatialMapAggregatedFieldWellsTypeDef",
     {
         "Geospatial": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
         "Colors": Sequence[DimensionFieldTypeDef],
     },
@@ -20693,42 +16520,81 @@
 )
 
 class GrowthRateComputationTypeDef(
     _RequiredGrowthRateComputationTypeDef, _OptionalGrowthRateComputationTypeDef
 ):
     pass
 
+HeatMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "HeatMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Rows": List[DimensionFieldTypeDef],
+        "Columns": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 HeatMapAggregatedFieldWellsTypeDef = TypedDict(
     "HeatMapAggregatedFieldWellsTypeDef",
     {
         "Rows": Sequence[DimensionFieldTypeDef],
         "Columns": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+HistogramAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "HistogramAggregatedFieldWellsOutputTypeDef",
+    {
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 HistogramAggregatedFieldWellsTypeDef = TypedDict(
     "HistogramAggregatedFieldWellsTypeDef",
     {
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+KPIFieldWellsOutputTypeDef = TypedDict(
+    "KPIFieldWellsOutputTypeDef",
+    {
+        "Values": List[MeasureFieldTypeDef],
+        "TargetValues": List[MeasureFieldTypeDef],
+        "TrendGroups": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 KPIFieldWellsTypeDef = TypedDict(
     "KPIFieldWellsTypeDef",
     {
         "Values": Sequence[MeasureFieldTypeDef],
         "TargetValues": Sequence[MeasureFieldTypeDef],
         "TrendGroups": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
+LineChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "LineChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+        "Colors": List[DimensionFieldTypeDef],
+        "SmallMultiples": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 LineChartAggregatedFieldWellsTypeDef = TypedDict(
     "LineChartAggregatedFieldWellsTypeDef",
     {
         "Category": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
         "Colors": Sequence[DimensionFieldTypeDef],
         "SmallMultiples": Sequence[DimensionFieldTypeDef],
@@ -20819,78 +16685,151 @@
 )
 
 class PeriodToDateComputationTypeDef(
     _RequiredPeriodToDateComputationTypeDef, _OptionalPeriodToDateComputationTypeDef
 ):
     pass
 
+PieChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "PieChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+        "SmallMultiples": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 PieChartAggregatedFieldWellsTypeDef = TypedDict(
     "PieChartAggregatedFieldWellsTypeDef",
     {
         "Category": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
         "SmallMultiples": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
+PivotTableAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "PivotTableAggregatedFieldWellsOutputTypeDef",
+    {
+        "Rows": List[DimensionFieldTypeDef],
+        "Columns": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 PivotTableAggregatedFieldWellsTypeDef = TypedDict(
     "PivotTableAggregatedFieldWellsTypeDef",
     {
         "Rows": Sequence[DimensionFieldTypeDef],
         "Columns": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+RadarChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "RadarChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": List[DimensionFieldTypeDef],
+        "Color": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 RadarChartAggregatedFieldWellsTypeDef = TypedDict(
     "RadarChartAggregatedFieldWellsTypeDef",
     {
         "Category": Sequence[DimensionFieldTypeDef],
         "Color": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+SankeyDiagramAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "SankeyDiagramAggregatedFieldWellsOutputTypeDef",
+    {
+        "Source": List[DimensionFieldTypeDef],
+        "Destination": List[DimensionFieldTypeDef],
+        "Weight": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 SankeyDiagramAggregatedFieldWellsTypeDef = TypedDict(
     "SankeyDiagramAggregatedFieldWellsTypeDef",
     {
         "Source": Sequence[DimensionFieldTypeDef],
         "Destination": Sequence[DimensionFieldTypeDef],
         "Weight": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef",
+    {
+        "XAxis": List[MeasureFieldTypeDef],
+        "YAxis": List[MeasureFieldTypeDef],
+        "Category": List[DimensionFieldTypeDef],
+        "Size": List[MeasureFieldTypeDef],
+        "Label": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 ScatterPlotCategoricallyAggregatedFieldWellsTypeDef = TypedDict(
     "ScatterPlotCategoricallyAggregatedFieldWellsTypeDef",
     {
         "XAxis": Sequence[MeasureFieldTypeDef],
         "YAxis": Sequence[MeasureFieldTypeDef],
         "Category": Sequence[DimensionFieldTypeDef],
         "Size": Sequence[MeasureFieldTypeDef],
         "Label": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
+ScatterPlotUnaggregatedFieldWellsOutputTypeDef = TypedDict(
+    "ScatterPlotUnaggregatedFieldWellsOutputTypeDef",
+    {
+        "XAxis": List[DimensionFieldTypeDef],
+        "YAxis": List[DimensionFieldTypeDef],
+        "Size": List[MeasureFieldTypeDef],
+        "Category": List[DimensionFieldTypeDef],
+        "Label": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 ScatterPlotUnaggregatedFieldWellsTypeDef = TypedDict(
     "ScatterPlotUnaggregatedFieldWellsTypeDef",
     {
         "XAxis": Sequence[DimensionFieldTypeDef],
         "YAxis": Sequence[DimensionFieldTypeDef],
         "Size": Sequence[MeasureFieldTypeDef],
         "Category": Sequence[DimensionFieldTypeDef],
         "Label": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
+TableAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "TableAggregatedFieldWellsOutputTypeDef",
+    {
+        "GroupBy": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 TableAggregatedFieldWellsTypeDef = TypedDict(
     "TableAggregatedFieldWellsTypeDef",
     {
         "GroupBy": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
     },
     total=False,
@@ -20960,58 +16899,95 @@
 )
 
 class TotalAggregationComputationTypeDef(
     _RequiredTotalAggregationComputationTypeDef, _OptionalTotalAggregationComputationTypeDef
 ):
     pass
 
+TreeMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "TreeMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Groups": List[DimensionFieldTypeDef],
+        "Sizes": List[MeasureFieldTypeDef],
+        "Colors": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 TreeMapAggregatedFieldWellsTypeDef = TypedDict(
     "TreeMapAggregatedFieldWellsTypeDef",
     {
         "Groups": Sequence[DimensionFieldTypeDef],
         "Sizes": Sequence[MeasureFieldTypeDef],
         "Colors": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+WaterfallChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "WaterfallChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Categories": List[DimensionFieldTypeDef],
+        "Values": List[MeasureFieldTypeDef],
+        "Breakdowns": List[DimensionFieldTypeDef],
+    },
+    total=False,
+)
+
 WaterfallChartAggregatedFieldWellsTypeDef = TypedDict(
     "WaterfallChartAggregatedFieldWellsTypeDef",
     {
         "Categories": Sequence[DimensionFieldTypeDef],
         "Values": Sequence[MeasureFieldTypeDef],
         "Breakdowns": Sequence[DimensionFieldTypeDef],
     },
     total=False,
 )
 
+WordCloudAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "WordCloudAggregatedFieldWellsOutputTypeDef",
+    {
+        "GroupBy": List[DimensionFieldTypeDef],
+        "Size": List[MeasureFieldTypeDef],
+    },
+    total=False,
+)
+
 WordCloudAggregatedFieldWellsTypeDef = TypedDict(
     "WordCloudAggregatedFieldWellsTypeDef",
     {
         "GroupBy": Sequence[DimensionFieldTypeDef],
         "Size": Sequence[MeasureFieldTypeDef],
     },
     total=False,
 )
 
+TableUnaggregatedFieldWellsOutputTypeDef = TypedDict(
+    "TableUnaggregatedFieldWellsOutputTypeDef",
+    {
+        "Values": List[UnaggregatedFieldTypeDef],
+    },
+    total=False,
+)
+
 TableUnaggregatedFieldWellsTypeDef = TypedDict(
     "TableUnaggregatedFieldWellsTypeDef",
     {
         "Values": Sequence[UnaggregatedFieldTypeDef],
     },
     total=False,
 )
 
 SectionBasedLayoutConfigurationOutputTypeDef = TypedDict(
     "SectionBasedLayoutConfigurationOutputTypeDef",
     {
         "HeaderSections": List[HeaderFooterSectionConfigurationOutputTypeDef],
         "BodySections": List[BodySectionConfigurationOutputTypeDef],
         "FooterSections": List[HeaderFooterSectionConfigurationOutputTypeDef],
-        "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsOutputTypeDef,
+        "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
     },
 )
 
 SectionBasedLayoutConfigurationTypeDef = TypedDict(
     "SectionBasedLayoutConfigurationTypeDef",
     {
         "HeaderSections": Sequence[HeaderFooterSectionConfigurationTypeDef],
@@ -21025,315 +17001,265 @@
     "BarChartFieldWellsOutputTypeDef",
     {
         "BarChartAggregatedFieldWells": BarChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-BoxPlotFieldWellsOutputTypeDef = TypedDict(
-    "BoxPlotFieldWellsOutputTypeDef",
-    {
-        "BoxPlotAggregatedFieldWells": BoxPlotAggregatedFieldWellsOutputTypeDef,
-    },
-    total=False,
-)
-
-ComboChartFieldWellsOutputTypeDef = TypedDict(
-    "ComboChartFieldWellsOutputTypeDef",
-    {
-        "ComboChartAggregatedFieldWells": ComboChartAggregatedFieldWellsOutputTypeDef,
-    },
-    total=False,
-)
-
-FilledMapFieldWellsOutputTypeDef = TypedDict(
-    "FilledMapFieldWellsOutputTypeDef",
-    {
-        "FilledMapAggregatedFieldWells": FilledMapAggregatedFieldWellsOutputTypeDef,
-    },
-    total=False,
-)
-
-FunnelChartFieldWellsOutputTypeDef = TypedDict(
-    "FunnelChartFieldWellsOutputTypeDef",
-    {
-        "FunnelChartAggregatedFieldWells": FunnelChartAggregatedFieldWellsOutputTypeDef,
-    },
-    total=False,
-)
-
-GaugeChartConfigurationOutputTypeDef = TypedDict(
-    "GaugeChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": GaugeChartFieldWellsOutputTypeDef,
-        "GaugeChartOptions": GaugeChartOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "TooltipOptions": TooltipOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-GeospatialMapFieldWellsOutputTypeDef = TypedDict(
-    "GeospatialMapFieldWellsOutputTypeDef",
+BarChartFieldWellsTypeDef = TypedDict(
+    "BarChartFieldWellsTypeDef",
     {
-        "GeospatialMapAggregatedFieldWells": GeospatialMapAggregatedFieldWellsOutputTypeDef,
+        "BarChartAggregatedFieldWells": BarChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-HeatMapFieldWellsOutputTypeDef = TypedDict(
-    "HeatMapFieldWellsOutputTypeDef",
+BoxPlotFieldWellsOutputTypeDef = TypedDict(
+    "BoxPlotFieldWellsOutputTypeDef",
     {
-        "HeatMapAggregatedFieldWells": HeatMapAggregatedFieldWellsOutputTypeDef,
+        "BoxPlotAggregatedFieldWells": BoxPlotAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-HistogramFieldWellsOutputTypeDef = TypedDict(
-    "HistogramFieldWellsOutputTypeDef",
+BoxPlotFieldWellsTypeDef = TypedDict(
+    "BoxPlotFieldWellsTypeDef",
     {
-        "HistogramAggregatedFieldWells": HistogramAggregatedFieldWellsOutputTypeDef,
+        "BoxPlotAggregatedFieldWells": BoxPlotAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-KPIConfigurationOutputTypeDef = TypedDict(
-    "KPIConfigurationOutputTypeDef",
+ComboChartFieldWellsOutputTypeDef = TypedDict(
+    "ComboChartFieldWellsOutputTypeDef",
     {
-        "FieldWells": KPIFieldWellsOutputTypeDef,
-        "SortConfiguration": KPISortConfigurationOutputTypeDef,
-        "KPIOptions": KPIOptionsOutputTypeDef,
+        "ComboChartAggregatedFieldWells": ComboChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-LineChartFieldWellsOutputTypeDef = TypedDict(
-    "LineChartFieldWellsOutputTypeDef",
+ComboChartFieldWellsTypeDef = TypedDict(
+    "ComboChartFieldWellsTypeDef",
     {
-        "LineChartAggregatedFieldWells": LineChartAggregatedFieldWellsOutputTypeDef,
+        "ComboChartAggregatedFieldWells": ComboChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-PieChartFieldWellsOutputTypeDef = TypedDict(
-    "PieChartFieldWellsOutputTypeDef",
+FilledMapFieldWellsOutputTypeDef = TypedDict(
+    "FilledMapFieldWellsOutputTypeDef",
     {
-        "PieChartAggregatedFieldWells": PieChartAggregatedFieldWellsOutputTypeDef,
+        "FilledMapAggregatedFieldWells": FilledMapAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-PivotTableFieldWellsOutputTypeDef = TypedDict(
-    "PivotTableFieldWellsOutputTypeDef",
+FilledMapFieldWellsTypeDef = TypedDict(
+    "FilledMapFieldWellsTypeDef",
     {
-        "PivotTableAggregatedFieldWells": PivotTableAggregatedFieldWellsOutputTypeDef,
+        "FilledMapAggregatedFieldWells": FilledMapAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-RadarChartFieldWellsOutputTypeDef = TypedDict(
-    "RadarChartFieldWellsOutputTypeDef",
+FunnelChartFieldWellsOutputTypeDef = TypedDict(
+    "FunnelChartFieldWellsOutputTypeDef",
     {
-        "RadarChartAggregatedFieldWells": RadarChartAggregatedFieldWellsOutputTypeDef,
+        "FunnelChartAggregatedFieldWells": FunnelChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-SankeyDiagramFieldWellsOutputTypeDef = TypedDict(
-    "SankeyDiagramFieldWellsOutputTypeDef",
+FunnelChartFieldWellsTypeDef = TypedDict(
+    "FunnelChartFieldWellsTypeDef",
     {
-        "SankeyDiagramAggregatedFieldWells": SankeyDiagramAggregatedFieldWellsOutputTypeDef,
+        "FunnelChartAggregatedFieldWells": FunnelChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-ScatterPlotFieldWellsOutputTypeDef = TypedDict(
-    "ScatterPlotFieldWellsOutputTypeDef",
+GaugeChartConfigurationOutputTypeDef = TypedDict(
+    "GaugeChartConfigurationOutputTypeDef",
     {
-        "ScatterPlotCategoricallyAggregatedFieldWells": (
-            ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef
-        ),
-        "ScatterPlotUnaggregatedFieldWells": ScatterPlotUnaggregatedFieldWellsOutputTypeDef,
+        "FieldWells": GaugeChartFieldWellsOutputTypeDef,
+        "GaugeChartOptions": GaugeChartOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "TooltipOptions": TooltipOptionsOutputTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
     },
     total=False,
 )
 
-ComputationOutputTypeDef = TypedDict(
-    "ComputationOutputTypeDef",
+GaugeChartConfigurationTypeDef = TypedDict(
+    "GaugeChartConfigurationTypeDef",
     {
-        "TopBottomRanked": TopBottomRankedComputationOutputTypeDef,
-        "TopBottomMovers": TopBottomMoversComputationOutputTypeDef,
-        "TotalAggregation": TotalAggregationComputationOutputTypeDef,
-        "MaximumMinimum": MaximumMinimumComputationOutputTypeDef,
-        "MetricComparison": MetricComparisonComputationOutputTypeDef,
-        "PeriodOverPeriod": PeriodOverPeriodComputationOutputTypeDef,
-        "PeriodToDate": PeriodToDateComputationOutputTypeDef,
-        "GrowthRate": GrowthRateComputationOutputTypeDef,
-        "UniqueValues": UniqueValuesComputationOutputTypeDef,
-        "Forecast": ForecastComputationOutputTypeDef,
+        "FieldWells": GaugeChartFieldWellsTypeDef,
+        "GaugeChartOptions": GaugeChartOptionsTypeDef,
+        "DataLabels": DataLabelOptionsTypeDef,
+        "TooltipOptions": TooltipOptionsTypeDef,
+        "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
-TreeMapFieldWellsOutputTypeDef = TypedDict(
-    "TreeMapFieldWellsOutputTypeDef",
+GeospatialMapFieldWellsOutputTypeDef = TypedDict(
+    "GeospatialMapFieldWellsOutputTypeDef",
     {
-        "TreeMapAggregatedFieldWells": TreeMapAggregatedFieldWellsOutputTypeDef,
+        "GeospatialMapAggregatedFieldWells": GeospatialMapAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-WaterfallChartFieldWellsOutputTypeDef = TypedDict(
-    "WaterfallChartFieldWellsOutputTypeDef",
+GeospatialMapFieldWellsTypeDef = TypedDict(
+    "GeospatialMapFieldWellsTypeDef",
     {
-        "WaterfallChartAggregatedFieldWells": WaterfallChartAggregatedFieldWellsOutputTypeDef,
+        "GeospatialMapAggregatedFieldWells": GeospatialMapAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-WordCloudFieldWellsOutputTypeDef = TypedDict(
-    "WordCloudFieldWellsOutputTypeDef",
+HeatMapFieldWellsOutputTypeDef = TypedDict(
+    "HeatMapFieldWellsOutputTypeDef",
     {
-        "WordCloudAggregatedFieldWells": WordCloudAggregatedFieldWellsOutputTypeDef,
+        "HeatMapAggregatedFieldWells": HeatMapAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-TableFieldWellsOutputTypeDef = TypedDict(
-    "TableFieldWellsOutputTypeDef",
+HeatMapFieldWellsTypeDef = TypedDict(
+    "HeatMapFieldWellsTypeDef",
     {
-        "TableAggregatedFieldWells": TableAggregatedFieldWellsOutputTypeDef,
-        "TableUnaggregatedFieldWells": TableUnaggregatedFieldWellsOutputTypeDef,
+        "HeatMapAggregatedFieldWells": HeatMapAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-BarChartFieldWellsTypeDef = TypedDict(
-    "BarChartFieldWellsTypeDef",
+HistogramFieldWellsOutputTypeDef = TypedDict(
+    "HistogramFieldWellsOutputTypeDef",
     {
-        "BarChartAggregatedFieldWells": BarChartAggregatedFieldWellsTypeDef,
+        "HistogramAggregatedFieldWells": HistogramAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-BoxPlotFieldWellsTypeDef = TypedDict(
-    "BoxPlotFieldWellsTypeDef",
+HistogramFieldWellsTypeDef = TypedDict(
+    "HistogramFieldWellsTypeDef",
     {
-        "BoxPlotAggregatedFieldWells": BoxPlotAggregatedFieldWellsTypeDef,
+        "HistogramAggregatedFieldWells": HistogramAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-ComboChartFieldWellsTypeDef = TypedDict(
-    "ComboChartFieldWellsTypeDef",
+KPIConfigurationOutputTypeDef = TypedDict(
+    "KPIConfigurationOutputTypeDef",
     {
-        "ComboChartAggregatedFieldWells": ComboChartAggregatedFieldWellsTypeDef,
+        "FieldWells": KPIFieldWellsOutputTypeDef,
+        "SortConfiguration": KPISortConfigurationOutputTypeDef,
+        "KPIOptions": KPIOptionsTypeDef,
     },
     total=False,
 )
 
-FilledMapFieldWellsTypeDef = TypedDict(
-    "FilledMapFieldWellsTypeDef",
+KPIConfigurationTypeDef = TypedDict(
+    "KPIConfigurationTypeDef",
     {
-        "FilledMapAggregatedFieldWells": FilledMapAggregatedFieldWellsTypeDef,
+        "FieldWells": KPIFieldWellsTypeDef,
+        "SortConfiguration": KPISortConfigurationTypeDef,
+        "KPIOptions": KPIOptionsTypeDef,
     },
     total=False,
 )
 
-FunnelChartFieldWellsTypeDef = TypedDict(
-    "FunnelChartFieldWellsTypeDef",
+LineChartFieldWellsOutputTypeDef = TypedDict(
+    "LineChartFieldWellsOutputTypeDef",
     {
-        "FunnelChartAggregatedFieldWells": FunnelChartAggregatedFieldWellsTypeDef,
+        "LineChartAggregatedFieldWells": LineChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-GaugeChartConfigurationTypeDef = TypedDict(
-    "GaugeChartConfigurationTypeDef",
+LineChartFieldWellsTypeDef = TypedDict(
+    "LineChartFieldWellsTypeDef",
     {
-        "FieldWells": GaugeChartFieldWellsTypeDef,
-        "GaugeChartOptions": GaugeChartOptionsTypeDef,
-        "DataLabels": DataLabelOptionsTypeDef,
-        "TooltipOptions": TooltipOptionsTypeDef,
-        "VisualPalette": VisualPaletteTypeDef,
+        "LineChartAggregatedFieldWells": LineChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-GeospatialMapFieldWellsTypeDef = TypedDict(
-    "GeospatialMapFieldWellsTypeDef",
+PieChartFieldWellsOutputTypeDef = TypedDict(
+    "PieChartFieldWellsOutputTypeDef",
     {
-        "GeospatialMapAggregatedFieldWells": GeospatialMapAggregatedFieldWellsTypeDef,
+        "PieChartAggregatedFieldWells": PieChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-HeatMapFieldWellsTypeDef = TypedDict(
-    "HeatMapFieldWellsTypeDef",
+PieChartFieldWellsTypeDef = TypedDict(
+    "PieChartFieldWellsTypeDef",
     {
-        "HeatMapAggregatedFieldWells": HeatMapAggregatedFieldWellsTypeDef,
+        "PieChartAggregatedFieldWells": PieChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-HistogramFieldWellsTypeDef = TypedDict(
-    "HistogramFieldWellsTypeDef",
+PivotTableFieldWellsOutputTypeDef = TypedDict(
+    "PivotTableFieldWellsOutputTypeDef",
     {
-        "HistogramAggregatedFieldWells": HistogramAggregatedFieldWellsTypeDef,
+        "PivotTableAggregatedFieldWells": PivotTableAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-KPIConfigurationTypeDef = TypedDict(
-    "KPIConfigurationTypeDef",
+PivotTableFieldWellsTypeDef = TypedDict(
+    "PivotTableFieldWellsTypeDef",
     {
-        "FieldWells": KPIFieldWellsTypeDef,
-        "SortConfiguration": KPISortConfigurationTypeDef,
-        "KPIOptions": KPIOptionsTypeDef,
+        "PivotTableAggregatedFieldWells": PivotTableAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-LineChartFieldWellsTypeDef = TypedDict(
-    "LineChartFieldWellsTypeDef",
+RadarChartFieldWellsOutputTypeDef = TypedDict(
+    "RadarChartFieldWellsOutputTypeDef",
     {
-        "LineChartAggregatedFieldWells": LineChartAggregatedFieldWellsTypeDef,
+        "RadarChartAggregatedFieldWells": RadarChartAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-PieChartFieldWellsTypeDef = TypedDict(
-    "PieChartFieldWellsTypeDef",
+RadarChartFieldWellsTypeDef = TypedDict(
+    "RadarChartFieldWellsTypeDef",
     {
-        "PieChartAggregatedFieldWells": PieChartAggregatedFieldWellsTypeDef,
+        "RadarChartAggregatedFieldWells": RadarChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-PivotTableFieldWellsTypeDef = TypedDict(
-    "PivotTableFieldWellsTypeDef",
+SankeyDiagramFieldWellsOutputTypeDef = TypedDict(
+    "SankeyDiagramFieldWellsOutputTypeDef",
     {
-        "PivotTableAggregatedFieldWells": PivotTableAggregatedFieldWellsTypeDef,
+        "SankeyDiagramAggregatedFieldWells": SankeyDiagramAggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
-RadarChartFieldWellsTypeDef = TypedDict(
-    "RadarChartFieldWellsTypeDef",
+SankeyDiagramFieldWellsTypeDef = TypedDict(
+    "SankeyDiagramFieldWellsTypeDef",
     {
-        "RadarChartAggregatedFieldWells": RadarChartAggregatedFieldWellsTypeDef,
+        "SankeyDiagramAggregatedFieldWells": SankeyDiagramAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
-SankeyDiagramFieldWellsTypeDef = TypedDict(
-    "SankeyDiagramFieldWellsTypeDef",
+ScatterPlotFieldWellsOutputTypeDef = TypedDict(
+    "ScatterPlotFieldWellsOutputTypeDef",
     {
-        "SankeyDiagramAggregatedFieldWells": SankeyDiagramAggregatedFieldWellsTypeDef,
+        "ScatterPlotCategoricallyAggregatedFieldWells": (
+            ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef
+        ),
+        "ScatterPlotUnaggregatedFieldWells": ScatterPlotUnaggregatedFieldWellsOutputTypeDef,
     },
     total=False,
 )
 
 ScatterPlotFieldWellsTypeDef = TypedDict(
     "ScatterPlotFieldWellsTypeDef",
     {
@@ -21358,38 +17284,71 @@
         "GrowthRate": GrowthRateComputationTypeDef,
         "UniqueValues": UniqueValuesComputationTypeDef,
         "Forecast": ForecastComputationTypeDef,
     },
     total=False,
 )
 
+TreeMapFieldWellsOutputTypeDef = TypedDict(
+    "TreeMapFieldWellsOutputTypeDef",
+    {
+        "TreeMapAggregatedFieldWells": TreeMapAggregatedFieldWellsOutputTypeDef,
+    },
+    total=False,
+)
+
 TreeMapFieldWellsTypeDef = TypedDict(
     "TreeMapFieldWellsTypeDef",
     {
         "TreeMapAggregatedFieldWells": TreeMapAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
+WaterfallChartFieldWellsOutputTypeDef = TypedDict(
+    "WaterfallChartFieldWellsOutputTypeDef",
+    {
+        "WaterfallChartAggregatedFieldWells": WaterfallChartAggregatedFieldWellsOutputTypeDef,
+    },
+    total=False,
+)
+
 WaterfallChartFieldWellsTypeDef = TypedDict(
     "WaterfallChartFieldWellsTypeDef",
     {
         "WaterfallChartAggregatedFieldWells": WaterfallChartAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
+WordCloudFieldWellsOutputTypeDef = TypedDict(
+    "WordCloudFieldWellsOutputTypeDef",
+    {
+        "WordCloudAggregatedFieldWells": WordCloudAggregatedFieldWellsOutputTypeDef,
+    },
+    total=False,
+)
+
 WordCloudFieldWellsTypeDef = TypedDict(
     "WordCloudFieldWellsTypeDef",
     {
         "WordCloudAggregatedFieldWells": WordCloudAggregatedFieldWellsTypeDef,
     },
     total=False,
 )
 
+TableFieldWellsOutputTypeDef = TypedDict(
+    "TableFieldWellsOutputTypeDef",
+    {
+        "TableAggregatedFieldWells": TableAggregatedFieldWellsOutputTypeDef,
+        "TableUnaggregatedFieldWells": TableUnaggregatedFieldWellsOutputTypeDef,
+    },
+    total=False,
+)
+
 TableFieldWellsTypeDef = TypedDict(
     "TableFieldWellsTypeDef",
     {
         "TableAggregatedFieldWells": TableAggregatedFieldWellsTypeDef,
         "TableUnaggregatedFieldWells": TableUnaggregatedFieldWellsTypeDef,
     },
     total=False,
@@ -21419,358 +17378,29 @@
     "BarChartConfigurationOutputTypeDef",
     {
         "FieldWells": BarChartFieldWellsOutputTypeDef,
         "SortConfiguration": BarChartSortConfigurationOutputTypeDef,
         "Orientation": BarChartOrientationType,
         "BarsArrangement": BarsArrangementType,
         "VisualPalette": VisualPaletteOutputTypeDef,
-        "SmallMultiplesOptions": SmallMultiplesOptionsOutputTypeDef,
+        "SmallMultiplesOptions": SmallMultiplesOptionsTypeDef,
         "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
         "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
         "ValueAxis": AxisDisplayOptionsOutputTypeDef,
         "ValueLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
         "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "ReferenceLines": List[ReferenceLineOutputTypeDef],
-        "ContributionAnalysisDefaults": List[ContributionAnalysisDefaultOutputTypeDef],
-    },
-    total=False,
-)
-
-BoxPlotChartConfigurationOutputTypeDef = TypedDict(
-    "BoxPlotChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": BoxPlotFieldWellsOutputTypeDef,
-        "SortConfiguration": BoxPlotSortConfigurationOutputTypeDef,
-        "BoxPlotOptions": BoxPlotOptionsOutputTypeDef,
-        "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
-        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "PrimaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "ReferenceLines": List[ReferenceLineOutputTypeDef],
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-ComboChartConfigurationOutputTypeDef = TypedDict(
-    "ComboChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": ComboChartFieldWellsOutputTypeDef,
-        "SortConfiguration": ComboChartSortConfigurationOutputTypeDef,
-        "BarsArrangement": BarsArrangementType,
-        "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
-        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "PrimaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "SecondaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "SecondaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "BarDataLabels": DataLabelOptionsOutputTypeDef,
-        "LineDataLabels": DataLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "ReferenceLines": List[ReferenceLineOutputTypeDef],
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-FilledMapConfigurationOutputTypeDef = TypedDict(
-    "FilledMapConfigurationOutputTypeDef",
-    {
-        "FieldWells": FilledMapFieldWellsOutputTypeDef,
-        "SortConfiguration": FilledMapSortConfigurationOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "WindowOptions": GeospatialWindowOptionsOutputTypeDef,
-        "MapStyleOptions": GeospatialMapStyleOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-FunnelChartConfigurationOutputTypeDef = TypedDict(
-    "FunnelChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": FunnelChartFieldWellsOutputTypeDef,
-        "SortConfiguration": FunnelChartSortConfigurationOutputTypeDef,
-        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ValueLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "DataLabelOptions": FunnelChartDataLabelOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredGaugeChartVisualOutputTypeDef = TypedDict(
-    "_RequiredGaugeChartVisualOutputTypeDef",
-    {
-        "VisualId": str,
-    },
-)
-_OptionalGaugeChartVisualOutputTypeDef = TypedDict(
-    "_OptionalGaugeChartVisualOutputTypeDef",
-    {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": GaugeChartConfigurationOutputTypeDef,
-        "ConditionalFormatting": GaugeChartConditionalFormattingOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-    },
-    total=False,
-)
-
-class GaugeChartVisualOutputTypeDef(
-    _RequiredGaugeChartVisualOutputTypeDef, _OptionalGaugeChartVisualOutputTypeDef
-):
-    pass
-
-GeospatialMapConfigurationOutputTypeDef = TypedDict(
-    "GeospatialMapConfigurationOutputTypeDef",
-    {
-        "FieldWells": GeospatialMapFieldWellsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "WindowOptions": GeospatialWindowOptionsOutputTypeDef,
-        "MapStyleOptions": GeospatialMapStyleOptionsOutputTypeDef,
-        "PointStyleOptions": GeospatialPointStyleOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-HeatMapConfigurationOutputTypeDef = TypedDict(
-    "HeatMapConfigurationOutputTypeDef",
-    {
-        "FieldWells": HeatMapFieldWellsOutputTypeDef,
-        "SortConfiguration": HeatMapSortConfigurationOutputTypeDef,
-        "RowLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ColumnLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ColorScale": ColorScaleOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-HistogramConfigurationOutputTypeDef = TypedDict(
-    "HistogramConfigurationOutputTypeDef",
-    {
-        "FieldWells": HistogramFieldWellsOutputTypeDef,
-        "XAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "XAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "YAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "BinOptions": HistogramBinOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredKPIVisualOutputTypeDef = TypedDict(
-    "_RequiredKPIVisualOutputTypeDef",
-    {
-        "VisualId": str,
-    },
-)
-_OptionalKPIVisualOutputTypeDef = TypedDict(
-    "_OptionalKPIVisualOutputTypeDef",
-    {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": KPIConfigurationOutputTypeDef,
-        "ConditionalFormatting": KPIConditionalFormattingOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
-    },
-    total=False,
-)
-
-class KPIVisualOutputTypeDef(_RequiredKPIVisualOutputTypeDef, _OptionalKPIVisualOutputTypeDef):
-    pass
-
-LineChartConfigurationOutputTypeDef = TypedDict(
-    "LineChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": LineChartFieldWellsOutputTypeDef,
-        "SortConfiguration": LineChartSortConfigurationOutputTypeDef,
-        "ForecastConfigurations": List[ForecastConfigurationOutputTypeDef],
-        "Type": LineChartTypeType,
-        "SmallMultiplesOptions": SmallMultiplesOptionsOutputTypeDef,
-        "XAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "XAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "PrimaryYAxisDisplayOptions": LineSeriesAxisDisplayOptionsOutputTypeDef,
-        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "SecondaryYAxisDisplayOptions": LineSeriesAxisDisplayOptionsOutputTypeDef,
-        "SecondaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "DefaultSeriesSettings": LineChartDefaultSeriesSettingsOutputTypeDef,
-        "Series": List[SeriesItemOutputTypeDef],
-        "Legend": LegendOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "ReferenceLines": List[ReferenceLineOutputTypeDef],
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "ContributionAnalysisDefaults": List[ContributionAnalysisDefaultOutputTypeDef],
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-PieChartConfigurationOutputTypeDef = TypedDict(
-    "PieChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": PieChartFieldWellsOutputTypeDef,
-        "SortConfiguration": PieChartSortConfigurationOutputTypeDef,
-        "DonutOptions": DonutOptionsOutputTypeDef,
-        "SmallMultiplesOptions": SmallMultiplesOptionsOutputTypeDef,
-        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ValueLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
         "DataLabels": DataLabelOptionsOutputTypeDef,
         "Tooltip": TooltipOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
+        "ReferenceLines": List[ReferenceLineTypeDef],
         "ContributionAnalysisDefaults": List[ContributionAnalysisDefaultOutputTypeDef],
     },
     total=False,
 )
 
-PivotTableConfigurationOutputTypeDef = TypedDict(
-    "PivotTableConfigurationOutputTypeDef",
-    {
-        "FieldWells": PivotTableFieldWellsOutputTypeDef,
-        "SortConfiguration": PivotTableSortConfigurationOutputTypeDef,
-        "TableOptions": PivotTableOptionsOutputTypeDef,
-        "TotalOptions": PivotTableTotalOptionsOutputTypeDef,
-        "FieldOptions": PivotTableFieldOptionsOutputTypeDef,
-        "PaginatedReportOptions": PivotTablePaginatedReportOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-RadarChartConfigurationOutputTypeDef = TypedDict(
-    "RadarChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": RadarChartFieldWellsOutputTypeDef,
-        "SortConfiguration": RadarChartSortConfigurationOutputTypeDef,
-        "Shape": RadarChartShapeType,
-        "BaseSeriesSettings": RadarChartSeriesSettingsOutputTypeDef,
-        "StartAngle": float,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-        "AlternateBandColorsVisibility": VisibilityType,
-        "AlternateBandEvenColor": str,
-        "AlternateBandOddColor": str,
-        "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
-        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ColorAxis": AxisDisplayOptionsOutputTypeDef,
-        "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "AxesRangeScale": RadarChartAxesRangeScaleType,
-    },
-    total=False,
-)
-
-SankeyDiagramChartConfigurationOutputTypeDef = TypedDict(
-    "SankeyDiagramChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": SankeyDiagramFieldWellsOutputTypeDef,
-        "SortConfiguration": SankeyDiagramSortConfigurationOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-ScatterPlotConfigurationOutputTypeDef = TypedDict(
-    "ScatterPlotConfigurationOutputTypeDef",
-    {
-        "FieldWells": ScatterPlotFieldWellsOutputTypeDef,
-        "XAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "XAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "YAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "YAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-InsightConfigurationOutputTypeDef = TypedDict(
-    "InsightConfigurationOutputTypeDef",
-    {
-        "Computations": List[ComputationOutputTypeDef],
-        "CustomNarrative": CustomNarrativeOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-TreeMapConfigurationOutputTypeDef = TypedDict(
-    "TreeMapConfigurationOutputTypeDef",
-    {
-        "FieldWells": TreeMapFieldWellsOutputTypeDef,
-        "SortConfiguration": TreeMapSortConfigurationOutputTypeDef,
-        "GroupLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "SizeLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "ColorScale": ColorScaleOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "Tooltip": TooltipOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-WaterfallChartConfigurationOutputTypeDef = TypedDict(
-    "WaterfallChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": WaterfallChartFieldWellsOutputTypeDef,
-        "SortConfiguration": WaterfallChartSortConfigurationOutputTypeDef,
-        "WaterfallChartOptions": WaterfallChartOptionsOutputTypeDef,
-        "CategoryAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "CategoryAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "PrimaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
-        "Legend": LegendOptionsOutputTypeDef,
-        "DataLabels": DataLabelOptionsOutputTypeDef,
-        "VisualPalette": VisualPaletteOutputTypeDef,
-    },
-    total=False,
-)
-
-WordCloudChartConfigurationOutputTypeDef = TypedDict(
-    "WordCloudChartConfigurationOutputTypeDef",
-    {
-        "FieldWells": WordCloudFieldWellsOutputTypeDef,
-        "SortConfiguration": WordCloudSortConfigurationOutputTypeDef,
-        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
-        "WordCloudOptions": WordCloudOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-TableConfigurationOutputTypeDef = TypedDict(
-    "TableConfigurationOutputTypeDef",
-    {
-        "FieldWells": TableFieldWellsOutputTypeDef,
-        "SortConfiguration": TableSortConfigurationOutputTypeDef,
-        "TableOptions": TableOptionsOutputTypeDef,
-        "TotalOptions": TotalOptionsOutputTypeDef,
-        "FieldOptions": TableFieldOptionsOutputTypeDef,
-        "PaginatedReportOptions": TablePaginatedReportOptionsOutputTypeDef,
-        "TableInlineVisualizations": List[TableInlineVisualizationOutputTypeDef],
-    },
-    total=False,
-)
-
 BarChartConfigurationTypeDef = TypedDict(
     "BarChartConfigurationTypeDef",
     {
         "FieldWells": BarChartFieldWellsTypeDef,
         "SortConfiguration": BarChartSortConfigurationTypeDef,
         "Orientation": BarChartOrientationType,
         "BarsArrangement": BarsArrangementType,
@@ -21786,14 +17416,32 @@
         "Tooltip": TooltipOptionsTypeDef,
         "ReferenceLines": Sequence[ReferenceLineTypeDef],
         "ContributionAnalysisDefaults": Sequence[ContributionAnalysisDefaultTypeDef],
     },
     total=False,
 )
 
+BoxPlotChartConfigurationOutputTypeDef = TypedDict(
+    "BoxPlotChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": BoxPlotFieldWellsOutputTypeDef,
+        "SortConfiguration": BoxPlotSortConfigurationOutputTypeDef,
+        "BoxPlotOptions": BoxPlotOptionsTypeDef,
+        "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
+        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "PrimaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "ReferenceLines": List[ReferenceLineTypeDef],
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 BoxPlotChartConfigurationTypeDef = TypedDict(
     "BoxPlotChartConfigurationTypeDef",
     {
         "FieldWells": BoxPlotFieldWellsTypeDef,
         "SortConfiguration": BoxPlotSortConfigurationTypeDef,
         "BoxPlotOptions": BoxPlotOptionsTypeDef,
         "CategoryAxis": AxisDisplayOptionsTypeDef,
@@ -21804,14 +17452,37 @@
         "Tooltip": TooltipOptionsTypeDef,
         "ReferenceLines": Sequence[ReferenceLineTypeDef],
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+ComboChartConfigurationOutputTypeDef = TypedDict(
+    "ComboChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": ComboChartFieldWellsOutputTypeDef,
+        "SortConfiguration": ComboChartSortConfigurationOutputTypeDef,
+        "BarsArrangement": BarsArrangementType,
+        "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
+        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "PrimaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "SecondaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "SecondaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "BarDataLabels": DataLabelOptionsOutputTypeDef,
+        "LineDataLabels": DataLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "ReferenceLines": List[ReferenceLineTypeDef],
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 ComboChartConfigurationTypeDef = TypedDict(
     "ComboChartConfigurationTypeDef",
     {
         "FieldWells": ComboChartFieldWellsTypeDef,
         "SortConfiguration": ComboChartSortConfigurationTypeDef,
         "BarsArrangement": BarsArrangementType,
         "CategoryAxis": AxisDisplayOptionsTypeDef,
@@ -21827,41 +17498,91 @@
         "Tooltip": TooltipOptionsTypeDef,
         "ReferenceLines": Sequence[ReferenceLineTypeDef],
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+FilledMapConfigurationOutputTypeDef = TypedDict(
+    "FilledMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": FilledMapFieldWellsOutputTypeDef,
+        "SortConfiguration": FilledMapSortConfigurationOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "WindowOptions": GeospatialWindowOptionsTypeDef,
+        "MapStyleOptions": GeospatialMapStyleOptionsTypeDef,
+    },
+    total=False,
+)
+
 FilledMapConfigurationTypeDef = TypedDict(
     "FilledMapConfigurationTypeDef",
     {
         "FieldWells": FilledMapFieldWellsTypeDef,
         "SortConfiguration": FilledMapSortConfigurationTypeDef,
         "Legend": LegendOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
         "WindowOptions": GeospatialWindowOptionsTypeDef,
         "MapStyleOptions": GeospatialMapStyleOptionsTypeDef,
     },
     total=False,
 )
 
+FunnelChartConfigurationOutputTypeDef = TypedDict(
+    "FunnelChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": FunnelChartFieldWellsOutputTypeDef,
+        "SortConfiguration": FunnelChartSortConfigurationOutputTypeDef,
+        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ValueLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "DataLabelOptions": FunnelChartDataLabelOptionsTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 FunnelChartConfigurationTypeDef = TypedDict(
     "FunnelChartConfigurationTypeDef",
     {
         "FieldWells": FunnelChartFieldWellsTypeDef,
         "SortConfiguration": FunnelChartSortConfigurationTypeDef,
         "CategoryLabelOptions": ChartAxisLabelOptionsTypeDef,
         "ValueLabelOptions": ChartAxisLabelOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
         "DataLabelOptions": FunnelChartDataLabelOptionsTypeDef,
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+_RequiredGaugeChartVisualOutputTypeDef = TypedDict(
+    "_RequiredGaugeChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+    },
+)
+_OptionalGaugeChartVisualOutputTypeDef = TypedDict(
+    "_OptionalGaugeChartVisualOutputTypeDef",
+    {
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": GaugeChartConfigurationOutputTypeDef,
+        "ConditionalFormatting": GaugeChartConditionalFormattingOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+    },
+    total=False,
+)
+
+class GaugeChartVisualOutputTypeDef(
+    _RequiredGaugeChartVisualOutputTypeDef, _OptionalGaugeChartVisualOutputTypeDef
+):
+    pass
+
 _RequiredGaugeChartVisualTypeDef = TypedDict(
     "_RequiredGaugeChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
 _OptionalGaugeChartVisualTypeDef = TypedDict(
@@ -21875,28 +17596,57 @@
     },
     total=False,
 )
 
 class GaugeChartVisualTypeDef(_RequiredGaugeChartVisualTypeDef, _OptionalGaugeChartVisualTypeDef):
     pass
 
+GeospatialMapConfigurationOutputTypeDef = TypedDict(
+    "GeospatialMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": GeospatialMapFieldWellsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "WindowOptions": GeospatialWindowOptionsTypeDef,
+        "MapStyleOptions": GeospatialMapStyleOptionsTypeDef,
+        "PointStyleOptions": GeospatialPointStyleOptionsOutputTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 GeospatialMapConfigurationTypeDef = TypedDict(
     "GeospatialMapConfigurationTypeDef",
     {
         "FieldWells": GeospatialMapFieldWellsTypeDef,
         "Legend": LegendOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
         "WindowOptions": GeospatialWindowOptionsTypeDef,
         "MapStyleOptions": GeospatialMapStyleOptionsTypeDef,
         "PointStyleOptions": GeospatialPointStyleOptionsTypeDef,
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+HeatMapConfigurationOutputTypeDef = TypedDict(
+    "HeatMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": HeatMapFieldWellsOutputTypeDef,
+        "SortConfiguration": HeatMapSortConfigurationOutputTypeDef,
+        "RowLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ColumnLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ColorScale": ColorScaleOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 HeatMapConfigurationTypeDef = TypedDict(
     "HeatMapConfigurationTypeDef",
     {
         "FieldWells": HeatMapFieldWellsTypeDef,
         "SortConfiguration": HeatMapSortConfigurationTypeDef,
         "RowLabelOptions": ChartAxisLabelOptionsTypeDef,
         "ColumnLabelOptions": ChartAxisLabelOptionsTypeDef,
@@ -21904,14 +17654,29 @@
         "Legend": LegendOptionsTypeDef,
         "DataLabels": DataLabelOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
     },
     total=False,
 )
 
+HistogramConfigurationOutputTypeDef = TypedDict(
+    "HistogramConfigurationOutputTypeDef",
+    {
+        "FieldWells": HistogramFieldWellsOutputTypeDef,
+        "XAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "XAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "YAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "BinOptions": HistogramBinOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 HistogramConfigurationTypeDef = TypedDict(
     "HistogramConfigurationTypeDef",
     {
         "FieldWells": HistogramFieldWellsTypeDef,
         "XAxisDisplayOptions": AxisDisplayOptionsTypeDef,
         "XAxisLabelOptions": ChartAxisLabelOptionsTypeDef,
         "YAxisDisplayOptions": AxisDisplayOptionsTypeDef,
@@ -21919,14 +17684,36 @@
         "DataLabels": DataLabelOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+_RequiredKPIVisualOutputTypeDef = TypedDict(
+    "_RequiredKPIVisualOutputTypeDef",
+    {
+        "VisualId": str,
+    },
+)
+_OptionalKPIVisualOutputTypeDef = TypedDict(
+    "_OptionalKPIVisualOutputTypeDef",
+    {
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": KPIConfigurationOutputTypeDef,
+        "ConditionalFormatting": KPIConditionalFormattingOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+    },
+    total=False,
+)
+
+class KPIVisualOutputTypeDef(_RequiredKPIVisualOutputTypeDef, _OptionalKPIVisualOutputTypeDef):
+    pass
+
 _RequiredKPIVisualTypeDef = TypedDict(
     "_RequiredKPIVisualTypeDef",
     {
         "VisualId": str,
     },
 )
 _OptionalKPIVisualTypeDef = TypedDict(
@@ -21941,14 +17728,40 @@
     },
     total=False,
 )
 
 class KPIVisualTypeDef(_RequiredKPIVisualTypeDef, _OptionalKPIVisualTypeDef):
     pass
 
+LineChartConfigurationOutputTypeDef = TypedDict(
+    "LineChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": LineChartFieldWellsOutputTypeDef,
+        "SortConfiguration": LineChartSortConfigurationOutputTypeDef,
+        "ForecastConfigurations": List[ForecastConfigurationOutputTypeDef],
+        "Type": LineChartTypeType,
+        "SmallMultiplesOptions": SmallMultiplesOptionsTypeDef,
+        "XAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "XAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "PrimaryYAxisDisplayOptions": LineSeriesAxisDisplayOptionsOutputTypeDef,
+        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "SecondaryYAxisDisplayOptions": LineSeriesAxisDisplayOptionsOutputTypeDef,
+        "SecondaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "DefaultSeriesSettings": LineChartDefaultSeriesSettingsTypeDef,
+        "Series": List[SeriesItemTypeDef],
+        "Legend": LegendOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "ReferenceLines": List[ReferenceLineTypeDef],
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "ContributionAnalysisDefaults": List[ContributionAnalysisDefaultOutputTypeDef],
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 LineChartConfigurationTypeDef = TypedDict(
     "LineChartConfigurationTypeDef",
     {
         "FieldWells": LineChartFieldWellsTypeDef,
         "SortConfiguration": LineChartSortConfigurationTypeDef,
         "ForecastConfigurations": Sequence[ForecastConfigurationTypeDef],
         "Type": LineChartTypeType,
@@ -21967,14 +17780,32 @@
         "Tooltip": TooltipOptionsTypeDef,
         "ContributionAnalysisDefaults": Sequence[ContributionAnalysisDefaultTypeDef],
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+PieChartConfigurationOutputTypeDef = TypedDict(
+    "PieChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": PieChartFieldWellsOutputTypeDef,
+        "SortConfiguration": PieChartSortConfigurationOutputTypeDef,
+        "DonutOptions": DonutOptionsTypeDef,
+        "SmallMultiplesOptions": SmallMultiplesOptionsTypeDef,
+        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ValueLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+        "ContributionAnalysisDefaults": List[ContributionAnalysisDefaultOutputTypeDef],
+    },
+    total=False,
+)
+
 PieChartConfigurationTypeDef = TypedDict(
     "PieChartConfigurationTypeDef",
     {
         "FieldWells": PieChartFieldWellsTypeDef,
         "SortConfiguration": PieChartSortConfigurationTypeDef,
         "DonutOptions": DonutOptionsTypeDef,
         "SmallMultiplesOptions": SmallMultiplesOptionsTypeDef,
@@ -21985,27 +17816,62 @@
         "Tooltip": TooltipOptionsTypeDef,
         "VisualPalette": VisualPaletteTypeDef,
         "ContributionAnalysisDefaults": Sequence[ContributionAnalysisDefaultTypeDef],
     },
     total=False,
 )
 
+PivotTableConfigurationOutputTypeDef = TypedDict(
+    "PivotTableConfigurationOutputTypeDef",
+    {
+        "FieldWells": PivotTableFieldWellsOutputTypeDef,
+        "SortConfiguration": PivotTableSortConfigurationOutputTypeDef,
+        "TableOptions": PivotTableOptionsOutputTypeDef,
+        "TotalOptions": PivotTableTotalOptionsOutputTypeDef,
+        "FieldOptions": PivotTableFieldOptionsOutputTypeDef,
+        "PaginatedReportOptions": PivotTablePaginatedReportOptionsTypeDef,
+    },
+    total=False,
+)
+
 PivotTableConfigurationTypeDef = TypedDict(
     "PivotTableConfigurationTypeDef",
     {
         "FieldWells": PivotTableFieldWellsTypeDef,
         "SortConfiguration": PivotTableSortConfigurationTypeDef,
         "TableOptions": PivotTableOptionsTypeDef,
         "TotalOptions": PivotTableTotalOptionsTypeDef,
         "FieldOptions": PivotTableFieldOptionsTypeDef,
         "PaginatedReportOptions": PivotTablePaginatedReportOptionsTypeDef,
     },
     total=False,
 )
 
+RadarChartConfigurationOutputTypeDef = TypedDict(
+    "RadarChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": RadarChartFieldWellsOutputTypeDef,
+        "SortConfiguration": RadarChartSortConfigurationOutputTypeDef,
+        "Shape": RadarChartShapeType,
+        "BaseSeriesSettings": RadarChartSeriesSettingsTypeDef,
+        "StartAngle": float,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+        "AlternateBandColorsVisibility": VisibilityType,
+        "AlternateBandEvenColor": str,
+        "AlternateBandOddColor": str,
+        "CategoryAxis": AxisDisplayOptionsOutputTypeDef,
+        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ColorAxis": AxisDisplayOptionsOutputTypeDef,
+        "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "AxesRangeScale": RadarChartAxesRangeScaleType,
+    },
+    total=False,
+)
+
 RadarChartConfigurationTypeDef = TypedDict(
     "RadarChartConfigurationTypeDef",
     {
         "FieldWells": RadarChartFieldWellsTypeDef,
         "SortConfiguration": RadarChartSortConfigurationTypeDef,
         "Shape": RadarChartShapeType,
         "BaseSeriesSettings": RadarChartSeriesSettingsTypeDef,
@@ -22020,24 +17886,50 @@
         "ColorLabelOptions": ChartAxisLabelOptionsTypeDef,
         "Legend": LegendOptionsTypeDef,
         "AxesRangeScale": RadarChartAxesRangeScaleType,
     },
     total=False,
 )
 
+SankeyDiagramChartConfigurationOutputTypeDef = TypedDict(
+    "SankeyDiagramChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": SankeyDiagramFieldWellsOutputTypeDef,
+        "SortConfiguration": SankeyDiagramSortConfigurationOutputTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 SankeyDiagramChartConfigurationTypeDef = TypedDict(
     "SankeyDiagramChartConfigurationTypeDef",
     {
         "FieldWells": SankeyDiagramFieldWellsTypeDef,
         "SortConfiguration": SankeyDiagramSortConfigurationTypeDef,
         "DataLabels": DataLabelOptionsTypeDef,
     },
     total=False,
 )
 
+ScatterPlotConfigurationOutputTypeDef = TypedDict(
+    "ScatterPlotConfigurationOutputTypeDef",
+    {
+        "FieldWells": ScatterPlotFieldWellsOutputTypeDef,
+        "XAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "XAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "YAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "YAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 ScatterPlotConfigurationTypeDef = TypedDict(
     "ScatterPlotConfigurationTypeDef",
     {
         "FieldWells": ScatterPlotFieldWellsTypeDef,
         "XAxisLabelOptions": ChartAxisLabelOptionsTypeDef,
         "XAxisDisplayOptions": AxisDisplayOptionsTypeDef,
         "YAxisLabelOptions": ChartAxisLabelOptionsTypeDef,
@@ -22046,23 +17938,48 @@
         "DataLabels": DataLabelOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+InsightConfigurationOutputTypeDef = TypedDict(
+    "InsightConfigurationOutputTypeDef",
+    {
+        "Computations": List[ComputationTypeDef],
+        "CustomNarrative": CustomNarrativeOptionsTypeDef,
+    },
+    total=False,
+)
+
 InsightConfigurationTypeDef = TypedDict(
     "InsightConfigurationTypeDef",
     {
         "Computations": Sequence[ComputationTypeDef],
         "CustomNarrative": CustomNarrativeOptionsTypeDef,
     },
     total=False,
 )
 
+TreeMapConfigurationOutputTypeDef = TypedDict(
+    "TreeMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": TreeMapFieldWellsOutputTypeDef,
+        "SortConfiguration": TreeMapSortConfigurationOutputTypeDef,
+        "GroupLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "SizeLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ColorLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "ColorScale": ColorScaleOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "Tooltip": TooltipOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 TreeMapConfigurationTypeDef = TypedDict(
     "TreeMapConfigurationTypeDef",
     {
         "FieldWells": TreeMapFieldWellsTypeDef,
         "SortConfiguration": TreeMapSortConfigurationTypeDef,
         "GroupLabelOptions": ChartAxisLabelOptionsTypeDef,
         "SizeLabelOptions": ChartAxisLabelOptionsTypeDef,
@@ -22071,14 +17988,31 @@
         "Legend": LegendOptionsTypeDef,
         "DataLabels": DataLabelOptionsTypeDef,
         "Tooltip": TooltipOptionsTypeDef,
     },
     total=False,
 )
 
+WaterfallChartConfigurationOutputTypeDef = TypedDict(
+    "WaterfallChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": WaterfallChartFieldWellsOutputTypeDef,
+        "SortConfiguration": WaterfallChartSortConfigurationOutputTypeDef,
+        "WaterfallChartOptions": WaterfallChartOptionsTypeDef,
+        "CategoryAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "CategoryAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "PrimaryYAxisLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "PrimaryYAxisDisplayOptions": AxisDisplayOptionsOutputTypeDef,
+        "Legend": LegendOptionsTypeDef,
+        "DataLabels": DataLabelOptionsOutputTypeDef,
+        "VisualPalette": VisualPaletteOutputTypeDef,
+    },
+    total=False,
+)
+
 WaterfallChartConfigurationTypeDef = TypedDict(
     "WaterfallChartConfigurationTypeDef",
     {
         "FieldWells": WaterfallChartFieldWellsTypeDef,
         "SortConfiguration": WaterfallChartSortConfigurationTypeDef,
         "WaterfallChartOptions": WaterfallChartOptionsTypeDef,
         "CategoryAxisLabelOptions": ChartAxisLabelOptionsTypeDef,
@@ -22088,25 +18022,50 @@
         "Legend": LegendOptionsTypeDef,
         "DataLabels": DataLabelOptionsTypeDef,
         "VisualPalette": VisualPaletteTypeDef,
     },
     total=False,
 )
 
+WordCloudChartConfigurationOutputTypeDef = TypedDict(
+    "WordCloudChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": WordCloudFieldWellsOutputTypeDef,
+        "SortConfiguration": WordCloudSortConfigurationOutputTypeDef,
+        "CategoryLabelOptions": ChartAxisLabelOptionsOutputTypeDef,
+        "WordCloudOptions": WordCloudOptionsTypeDef,
+    },
+    total=False,
+)
+
 WordCloudChartConfigurationTypeDef = TypedDict(
     "WordCloudChartConfigurationTypeDef",
     {
         "FieldWells": WordCloudFieldWellsTypeDef,
         "SortConfiguration": WordCloudSortConfigurationTypeDef,
         "CategoryLabelOptions": ChartAxisLabelOptionsTypeDef,
         "WordCloudOptions": WordCloudOptionsTypeDef,
     },
     total=False,
 )
 
+TableConfigurationOutputTypeDef = TypedDict(
+    "TableConfigurationOutputTypeDef",
+    {
+        "FieldWells": TableFieldWellsOutputTypeDef,
+        "SortConfiguration": TableSortConfigurationOutputTypeDef,
+        "TableOptions": TableOptionsOutputTypeDef,
+        "TotalOptions": TotalOptionsTypeDef,
+        "FieldOptions": TableFieldOptionsOutputTypeDef,
+        "PaginatedReportOptions": TablePaginatedReportOptionsTypeDef,
+        "TableInlineVisualizations": List[TableInlineVisualizationTypeDef],
+    },
+    total=False,
+)
+
 TableConfigurationTypeDef = TypedDict(
     "TableConfigurationTypeDef",
     {
         "FieldWells": TableFieldWellsTypeDef,
         "SortConfiguration": TableSortConfigurationTypeDef,
         "TableOptions": TableOptionsTypeDef,
         "TotalOptions": TotalOptionsTypeDef,
@@ -22136,824 +18095,824 @@
     {
         "VisualId": str,
     },
 )
 _OptionalBarChartVisualOutputTypeDef = TypedDict(
     "_OptionalBarChartVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
         "ChartConfiguration": BarChartConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
         "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
 class BarChartVisualOutputTypeDef(
     _RequiredBarChartVisualOutputTypeDef, _OptionalBarChartVisualOutputTypeDef
 ):
     pass
 
-_RequiredBoxPlotVisualOutputTypeDef = TypedDict(
-    "_RequiredBoxPlotVisualOutputTypeDef",
+_RequiredBarChartVisualTypeDef = TypedDict(
+    "_RequiredBarChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalBoxPlotVisualOutputTypeDef = TypedDict(
-    "_OptionalBoxPlotVisualOutputTypeDef",
+_OptionalBarChartVisualTypeDef = TypedDict(
+    "_OptionalBarChartVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": BoxPlotChartConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": BarChartConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
-class BoxPlotVisualOutputTypeDef(
-    _RequiredBoxPlotVisualOutputTypeDef, _OptionalBoxPlotVisualOutputTypeDef
-):
+class BarChartVisualTypeDef(_RequiredBarChartVisualTypeDef, _OptionalBarChartVisualTypeDef):
     pass
 
-_RequiredComboChartVisualOutputTypeDef = TypedDict(
-    "_RequiredComboChartVisualOutputTypeDef",
+_RequiredBoxPlotVisualOutputTypeDef = TypedDict(
+    "_RequiredBoxPlotVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalComboChartVisualOutputTypeDef = TypedDict(
-    "_OptionalComboChartVisualOutputTypeDef",
+_OptionalBoxPlotVisualOutputTypeDef = TypedDict(
+    "_OptionalBoxPlotVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": ComboChartConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": BoxPlotChartConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
         "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
-class ComboChartVisualOutputTypeDef(
-    _RequiredComboChartVisualOutputTypeDef, _OptionalComboChartVisualOutputTypeDef
+class BoxPlotVisualOutputTypeDef(
+    _RequiredBoxPlotVisualOutputTypeDef, _OptionalBoxPlotVisualOutputTypeDef
 ):
     pass
 
-_RequiredFilledMapVisualOutputTypeDef = TypedDict(
-    "_RequiredFilledMapVisualOutputTypeDef",
+_RequiredBoxPlotVisualTypeDef = TypedDict(
+    "_RequiredBoxPlotVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalFilledMapVisualOutputTypeDef = TypedDict(
-    "_OptionalFilledMapVisualOutputTypeDef",
+_OptionalBoxPlotVisualTypeDef = TypedDict(
+    "_OptionalBoxPlotVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": FilledMapConfigurationOutputTypeDef,
-        "ConditionalFormatting": FilledMapConditionalFormattingOutputTypeDef,
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
-        "Actions": List[VisualCustomActionOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": BoxPlotChartConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
-class FilledMapVisualOutputTypeDef(
-    _RequiredFilledMapVisualOutputTypeDef, _OptionalFilledMapVisualOutputTypeDef
-):
+class BoxPlotVisualTypeDef(_RequiredBoxPlotVisualTypeDef, _OptionalBoxPlotVisualTypeDef):
     pass
 
-_RequiredFunnelChartVisualOutputTypeDef = TypedDict(
-    "_RequiredFunnelChartVisualOutputTypeDef",
+_RequiredComboChartVisualOutputTypeDef = TypedDict(
+    "_RequiredComboChartVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalFunnelChartVisualOutputTypeDef = TypedDict(
-    "_OptionalFunnelChartVisualOutputTypeDef",
+_OptionalComboChartVisualOutputTypeDef = TypedDict(
+    "_OptionalComboChartVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": FunnelChartConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": ComboChartConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
         "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
-class FunnelChartVisualOutputTypeDef(
-    _RequiredFunnelChartVisualOutputTypeDef, _OptionalFunnelChartVisualOutputTypeDef
+class ComboChartVisualOutputTypeDef(
+    _RequiredComboChartVisualOutputTypeDef, _OptionalComboChartVisualOutputTypeDef
 ):
     pass
 
-_RequiredGeospatialMapVisualOutputTypeDef = TypedDict(
-    "_RequiredGeospatialMapVisualOutputTypeDef",
+_RequiredComboChartVisualTypeDef = TypedDict(
+    "_RequiredComboChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalGeospatialMapVisualOutputTypeDef = TypedDict(
-    "_OptionalGeospatialMapVisualOutputTypeDef",
+_OptionalComboChartVisualTypeDef = TypedDict(
+    "_OptionalComboChartVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": GeospatialMapConfigurationOutputTypeDef,
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
-        "Actions": List[VisualCustomActionOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": ComboChartConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
-class GeospatialMapVisualOutputTypeDef(
-    _RequiredGeospatialMapVisualOutputTypeDef, _OptionalGeospatialMapVisualOutputTypeDef
-):
+class ComboChartVisualTypeDef(_RequiredComboChartVisualTypeDef, _OptionalComboChartVisualTypeDef):
     pass
 
-_RequiredHeatMapVisualOutputTypeDef = TypedDict(
-    "_RequiredHeatMapVisualOutputTypeDef",
+_RequiredFilledMapVisualOutputTypeDef = TypedDict(
+    "_RequiredFilledMapVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalHeatMapVisualOutputTypeDef = TypedDict(
-    "_OptionalHeatMapVisualOutputTypeDef",
+_OptionalFilledMapVisualOutputTypeDef = TypedDict(
+    "_OptionalFilledMapVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": HeatMapConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": FilledMapConfigurationOutputTypeDef,
+        "ConditionalFormatting": FilledMapConditionalFormattingOutputTypeDef,
         "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
         "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
-class HeatMapVisualOutputTypeDef(
-    _RequiredHeatMapVisualOutputTypeDef, _OptionalHeatMapVisualOutputTypeDef
+class FilledMapVisualOutputTypeDef(
+    _RequiredFilledMapVisualOutputTypeDef, _OptionalFilledMapVisualOutputTypeDef
 ):
     pass
 
-_RequiredHistogramVisualOutputTypeDef = TypedDict(
-    "_RequiredHistogramVisualOutputTypeDef",
+_RequiredFilledMapVisualTypeDef = TypedDict(
+    "_RequiredFilledMapVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalHistogramVisualOutputTypeDef = TypedDict(
-    "_OptionalHistogramVisualOutputTypeDef",
+_OptionalFilledMapVisualTypeDef = TypedDict(
+    "_OptionalFilledMapVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": HistogramConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": FilledMapConfigurationTypeDef,
+        "ConditionalFormatting": FilledMapConditionalFormattingTypeDef,
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "Actions": Sequence[VisualCustomActionTypeDef],
     },
     total=False,
 )
 
-class HistogramVisualOutputTypeDef(
-    _RequiredHistogramVisualOutputTypeDef, _OptionalHistogramVisualOutputTypeDef
-):
+class FilledMapVisualTypeDef(_RequiredFilledMapVisualTypeDef, _OptionalFilledMapVisualTypeDef):
     pass
 
-_RequiredLineChartVisualOutputTypeDef = TypedDict(
-    "_RequiredLineChartVisualOutputTypeDef",
+_RequiredFunnelChartVisualOutputTypeDef = TypedDict(
+    "_RequiredFunnelChartVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalLineChartVisualOutputTypeDef = TypedDict(
-    "_OptionalLineChartVisualOutputTypeDef",
+_OptionalFunnelChartVisualOutputTypeDef = TypedDict(
+    "_OptionalFunnelChartVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": LineChartConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": FunnelChartConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
         "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
-class LineChartVisualOutputTypeDef(
-    _RequiredLineChartVisualOutputTypeDef, _OptionalLineChartVisualOutputTypeDef
+class FunnelChartVisualOutputTypeDef(
+    _RequiredFunnelChartVisualOutputTypeDef, _OptionalFunnelChartVisualOutputTypeDef
 ):
     pass
 
-_RequiredPieChartVisualOutputTypeDef = TypedDict(
-    "_RequiredPieChartVisualOutputTypeDef",
+_RequiredFunnelChartVisualTypeDef = TypedDict(
+    "_RequiredFunnelChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalPieChartVisualOutputTypeDef = TypedDict(
-    "_OptionalPieChartVisualOutputTypeDef",
+_OptionalFunnelChartVisualTypeDef = TypedDict(
+    "_OptionalFunnelChartVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": PieChartConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": FunnelChartConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
-class PieChartVisualOutputTypeDef(
-    _RequiredPieChartVisualOutputTypeDef, _OptionalPieChartVisualOutputTypeDef
+class FunnelChartVisualTypeDef(
+    _RequiredFunnelChartVisualTypeDef, _OptionalFunnelChartVisualTypeDef
 ):
     pass
 
-_RequiredPivotTableVisualOutputTypeDef = TypedDict(
-    "_RequiredPivotTableVisualOutputTypeDef",
+_RequiredGeospatialMapVisualOutputTypeDef = TypedDict(
+    "_RequiredGeospatialMapVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalPivotTableVisualOutputTypeDef = TypedDict(
-    "_OptionalPivotTableVisualOutputTypeDef",
+_OptionalGeospatialMapVisualOutputTypeDef = TypedDict(
+    "_OptionalGeospatialMapVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": PivotTableConfigurationOutputTypeDef,
-        "ConditionalFormatting": PivotTableConditionalFormattingOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": GeospatialMapConfigurationOutputTypeDef,
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
         "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
-class PivotTableVisualOutputTypeDef(
-    _RequiredPivotTableVisualOutputTypeDef, _OptionalPivotTableVisualOutputTypeDef
+class GeospatialMapVisualOutputTypeDef(
+    _RequiredGeospatialMapVisualOutputTypeDef, _OptionalGeospatialMapVisualOutputTypeDef
 ):
     pass
 
-_RequiredRadarChartVisualOutputTypeDef = TypedDict(
-    "_RequiredRadarChartVisualOutputTypeDef",
+_RequiredGeospatialMapVisualTypeDef = TypedDict(
+    "_RequiredGeospatialMapVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalRadarChartVisualOutputTypeDef = TypedDict(
-    "_OptionalRadarChartVisualOutputTypeDef",
+_OptionalGeospatialMapVisualTypeDef = TypedDict(
+    "_OptionalGeospatialMapVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": RadarChartConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": GeospatialMapConfigurationTypeDef,
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "Actions": Sequence[VisualCustomActionTypeDef],
     },
     total=False,
 )
 
-class RadarChartVisualOutputTypeDef(
-    _RequiredRadarChartVisualOutputTypeDef, _OptionalRadarChartVisualOutputTypeDef
+class GeospatialMapVisualTypeDef(
+    _RequiredGeospatialMapVisualTypeDef, _OptionalGeospatialMapVisualTypeDef
 ):
     pass
 
-_RequiredSankeyDiagramVisualOutputTypeDef = TypedDict(
-    "_RequiredSankeyDiagramVisualOutputTypeDef",
+_RequiredHeatMapVisualOutputTypeDef = TypedDict(
+    "_RequiredHeatMapVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalSankeyDiagramVisualOutputTypeDef = TypedDict(
-    "_OptionalSankeyDiagramVisualOutputTypeDef",
+_OptionalHeatMapVisualOutputTypeDef = TypedDict(
+    "_OptionalHeatMapVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": SankeyDiagramChartConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": HeatMapConfigurationOutputTypeDef,
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
         "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
-class SankeyDiagramVisualOutputTypeDef(
-    _RequiredSankeyDiagramVisualOutputTypeDef, _OptionalSankeyDiagramVisualOutputTypeDef
+class HeatMapVisualOutputTypeDef(
+    _RequiredHeatMapVisualOutputTypeDef, _OptionalHeatMapVisualOutputTypeDef
 ):
     pass
 
-_RequiredScatterPlotVisualOutputTypeDef = TypedDict(
-    "_RequiredScatterPlotVisualOutputTypeDef",
+_RequiredHeatMapVisualTypeDef = TypedDict(
+    "_RequiredHeatMapVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalScatterPlotVisualOutputTypeDef = TypedDict(
-    "_OptionalScatterPlotVisualOutputTypeDef",
+_OptionalHeatMapVisualTypeDef = TypedDict(
+    "_OptionalHeatMapVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": ScatterPlotConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": HeatMapConfigurationTypeDef,
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "Actions": Sequence[VisualCustomActionTypeDef],
     },
     total=False,
 )
 
-class ScatterPlotVisualOutputTypeDef(
-    _RequiredScatterPlotVisualOutputTypeDef, _OptionalScatterPlotVisualOutputTypeDef
-):
+class HeatMapVisualTypeDef(_RequiredHeatMapVisualTypeDef, _OptionalHeatMapVisualTypeDef):
     pass
 
-_RequiredInsightVisualOutputTypeDef = TypedDict(
-    "_RequiredInsightVisualOutputTypeDef",
+_RequiredHistogramVisualOutputTypeDef = TypedDict(
+    "_RequiredHistogramVisualOutputTypeDef",
     {
         "VisualId": str,
-        "DataSetIdentifier": str,
     },
 )
-_OptionalInsightVisualOutputTypeDef = TypedDict(
-    "_OptionalInsightVisualOutputTypeDef",
+_OptionalHistogramVisualOutputTypeDef = TypedDict(
+    "_OptionalHistogramVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "InsightConfiguration": InsightConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": HistogramConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
-class InsightVisualOutputTypeDef(
-    _RequiredInsightVisualOutputTypeDef, _OptionalInsightVisualOutputTypeDef
+class HistogramVisualOutputTypeDef(
+    _RequiredHistogramVisualOutputTypeDef, _OptionalHistogramVisualOutputTypeDef
 ):
     pass
 
-_RequiredTreeMapVisualOutputTypeDef = TypedDict(
-    "_RequiredTreeMapVisualOutputTypeDef",
+_RequiredHistogramVisualTypeDef = TypedDict(
+    "_RequiredHistogramVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalTreeMapVisualOutputTypeDef = TypedDict(
-    "_OptionalTreeMapVisualOutputTypeDef",
+_OptionalHistogramVisualTypeDef = TypedDict(
+    "_OptionalHistogramVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": TreeMapConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": HistogramConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
     },
     total=False,
 )
 
-class TreeMapVisualOutputTypeDef(
-    _RequiredTreeMapVisualOutputTypeDef, _OptionalTreeMapVisualOutputTypeDef
-):
+class HistogramVisualTypeDef(_RequiredHistogramVisualTypeDef, _OptionalHistogramVisualTypeDef):
     pass
 
-_RequiredWaterfallVisualOutputTypeDef = TypedDict(
-    "_RequiredWaterfallVisualOutputTypeDef",
+_RequiredLineChartVisualOutputTypeDef = TypedDict(
+    "_RequiredLineChartVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalWaterfallVisualOutputTypeDef = TypedDict(
-    "_OptionalWaterfallVisualOutputTypeDef",
+_OptionalLineChartVisualOutputTypeDef = TypedDict(
+    "_OptionalLineChartVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": WaterfallChartConfigurationOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": LineChartConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
         "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
-class WaterfallVisualOutputTypeDef(
-    _RequiredWaterfallVisualOutputTypeDef, _OptionalWaterfallVisualOutputTypeDef
+class LineChartVisualOutputTypeDef(
+    _RequiredLineChartVisualOutputTypeDef, _OptionalLineChartVisualOutputTypeDef
 ):
     pass
 
-_RequiredWordCloudVisualOutputTypeDef = TypedDict(
-    "_RequiredWordCloudVisualOutputTypeDef",
+_RequiredLineChartVisualTypeDef = TypedDict(
+    "_RequiredLineChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalWordCloudVisualOutputTypeDef = TypedDict(
-    "_OptionalWordCloudVisualOutputTypeDef",
+_OptionalLineChartVisualTypeDef = TypedDict(
+    "_OptionalLineChartVisualTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": WordCloudChartConfigurationOutputTypeDef,
-        "Actions": List[VisualCustomActionOutputTypeDef],
-        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": LineChartConfigurationTypeDef,
+        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
-class WordCloudVisualOutputTypeDef(
-    _RequiredWordCloudVisualOutputTypeDef, _OptionalWordCloudVisualOutputTypeDef
-):
+class LineChartVisualTypeDef(_RequiredLineChartVisualTypeDef, _OptionalLineChartVisualTypeDef):
     pass
 
-_RequiredTableVisualOutputTypeDef = TypedDict(
-    "_RequiredTableVisualOutputTypeDef",
+_RequiredPieChartVisualOutputTypeDef = TypedDict(
+    "_RequiredPieChartVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalTableVisualOutputTypeDef = TypedDict(
-    "_OptionalTableVisualOutputTypeDef",
+_OptionalPieChartVisualOutputTypeDef = TypedDict(
+    "_OptionalPieChartVisualOutputTypeDef",
     {
-        "Title": VisualTitleLabelOptionsOutputTypeDef,
-        "Subtitle": VisualSubtitleLabelOptionsOutputTypeDef,
-        "ChartConfiguration": TableConfigurationOutputTypeDef,
-        "ConditionalFormatting": TableConditionalFormattingOutputTypeDef,
+        "Title": VisualTitleLabelOptionsTypeDef,
+        "Subtitle": VisualSubtitleLabelOptionsTypeDef,
+        "ChartConfiguration": PieChartConfigurationOutputTypeDef,
         "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
-class TableVisualOutputTypeDef(
-    _RequiredTableVisualOutputTypeDef, _OptionalTableVisualOutputTypeDef
+class PieChartVisualOutputTypeDef(
+    _RequiredPieChartVisualOutputTypeDef, _OptionalPieChartVisualOutputTypeDef
 ):
     pass
 
-_RequiredBarChartVisualTypeDef = TypedDict(
-    "_RequiredBarChartVisualTypeDef",
+_RequiredPieChartVisualTypeDef = TypedDict(
+    "_RequiredPieChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalBarChartVisualTypeDef = TypedDict(
-    "_OptionalBarChartVisualTypeDef",
+_OptionalPieChartVisualTypeDef = TypedDict(
+    "_OptionalPieChartVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": BarChartConfigurationTypeDef,
+        "ChartConfiguration": PieChartConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
         "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
-class BarChartVisualTypeDef(_RequiredBarChartVisualTypeDef, _OptionalBarChartVisualTypeDef):
+class PieChartVisualTypeDef(_RequiredPieChartVisualTypeDef, _OptionalPieChartVisualTypeDef):
     pass
 
-_RequiredBoxPlotVisualTypeDef = TypedDict(
-    "_RequiredBoxPlotVisualTypeDef",
+_RequiredPivotTableVisualOutputTypeDef = TypedDict(
+    "_RequiredPivotTableVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalBoxPlotVisualTypeDef = TypedDict(
-    "_OptionalBoxPlotVisualTypeDef",
+_OptionalPivotTableVisualOutputTypeDef = TypedDict(
+    "_OptionalPivotTableVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": BoxPlotChartConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "ChartConfiguration": PivotTableConfigurationOutputTypeDef,
+        "ConditionalFormatting": PivotTableConditionalFormattingOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
-class BoxPlotVisualTypeDef(_RequiredBoxPlotVisualTypeDef, _OptionalBoxPlotVisualTypeDef):
+class PivotTableVisualOutputTypeDef(
+    _RequiredPivotTableVisualOutputTypeDef, _OptionalPivotTableVisualOutputTypeDef
+):
     pass
 
-_RequiredComboChartVisualTypeDef = TypedDict(
-    "_RequiredComboChartVisualTypeDef",
+_RequiredPivotTableVisualTypeDef = TypedDict(
+    "_RequiredPivotTableVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalComboChartVisualTypeDef = TypedDict(
-    "_OptionalComboChartVisualTypeDef",
+_OptionalPivotTableVisualTypeDef = TypedDict(
+    "_OptionalPivotTableVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": ComboChartConfigurationTypeDef,
+        "ChartConfiguration": PivotTableConfigurationTypeDef,
+        "ConditionalFormatting": PivotTableConditionalFormattingTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
-class ComboChartVisualTypeDef(_RequiredComboChartVisualTypeDef, _OptionalComboChartVisualTypeDef):
+class PivotTableVisualTypeDef(_RequiredPivotTableVisualTypeDef, _OptionalPivotTableVisualTypeDef):
     pass
 
-_RequiredFilledMapVisualTypeDef = TypedDict(
-    "_RequiredFilledMapVisualTypeDef",
+_RequiredRadarChartVisualOutputTypeDef = TypedDict(
+    "_RequiredRadarChartVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalFilledMapVisualTypeDef = TypedDict(
-    "_OptionalFilledMapVisualTypeDef",
+_OptionalRadarChartVisualOutputTypeDef = TypedDict(
+    "_OptionalRadarChartVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": FilledMapConfigurationTypeDef,
-        "ConditionalFormatting": FilledMapConditionalFormattingTypeDef,
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
-        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ChartConfiguration": RadarChartConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
-class FilledMapVisualTypeDef(_RequiredFilledMapVisualTypeDef, _OptionalFilledMapVisualTypeDef):
+class RadarChartVisualOutputTypeDef(
+    _RequiredRadarChartVisualOutputTypeDef, _OptionalRadarChartVisualOutputTypeDef
+):
     pass
 
-_RequiredFunnelChartVisualTypeDef = TypedDict(
-    "_RequiredFunnelChartVisualTypeDef",
+_RequiredRadarChartVisualTypeDef = TypedDict(
+    "_RequiredRadarChartVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalFunnelChartVisualTypeDef = TypedDict(
-    "_OptionalFunnelChartVisualTypeDef",
+_OptionalRadarChartVisualTypeDef = TypedDict(
+    "_OptionalRadarChartVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": FunnelChartConfigurationTypeDef,
+        "ChartConfiguration": RadarChartConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
         "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
-class FunnelChartVisualTypeDef(
-    _RequiredFunnelChartVisualTypeDef, _OptionalFunnelChartVisualTypeDef
-):
+class RadarChartVisualTypeDef(_RequiredRadarChartVisualTypeDef, _OptionalRadarChartVisualTypeDef):
     pass
 
-_RequiredGeospatialMapVisualTypeDef = TypedDict(
-    "_RequiredGeospatialMapVisualTypeDef",
+_RequiredSankeyDiagramVisualOutputTypeDef = TypedDict(
+    "_RequiredSankeyDiagramVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalGeospatialMapVisualTypeDef = TypedDict(
-    "_OptionalGeospatialMapVisualTypeDef",
+_OptionalSankeyDiagramVisualOutputTypeDef = TypedDict(
+    "_OptionalSankeyDiagramVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": GeospatialMapConfigurationTypeDef,
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
-        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ChartConfiguration": SankeyDiagramChartConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
-class GeospatialMapVisualTypeDef(
-    _RequiredGeospatialMapVisualTypeDef, _OptionalGeospatialMapVisualTypeDef
+class SankeyDiagramVisualOutputTypeDef(
+    _RequiredSankeyDiagramVisualOutputTypeDef, _OptionalSankeyDiagramVisualOutputTypeDef
 ):
     pass
 
-_RequiredHeatMapVisualTypeDef = TypedDict(
-    "_RequiredHeatMapVisualTypeDef",
+_RequiredSankeyDiagramVisualTypeDef = TypedDict(
+    "_RequiredSankeyDiagramVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalHeatMapVisualTypeDef = TypedDict(
-    "_OptionalHeatMapVisualTypeDef",
+_OptionalSankeyDiagramVisualTypeDef = TypedDict(
+    "_OptionalSankeyDiagramVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": HeatMapConfigurationTypeDef,
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "ChartConfiguration": SankeyDiagramChartConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
     },
     total=False,
 )
 
-class HeatMapVisualTypeDef(_RequiredHeatMapVisualTypeDef, _OptionalHeatMapVisualTypeDef):
+class SankeyDiagramVisualTypeDef(
+    _RequiredSankeyDiagramVisualTypeDef, _OptionalSankeyDiagramVisualTypeDef
+):
     pass
 
-_RequiredHistogramVisualTypeDef = TypedDict(
-    "_RequiredHistogramVisualTypeDef",
+_RequiredScatterPlotVisualOutputTypeDef = TypedDict(
+    "_RequiredScatterPlotVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalHistogramVisualTypeDef = TypedDict(
-    "_OptionalHistogramVisualTypeDef",
+_OptionalScatterPlotVisualOutputTypeDef = TypedDict(
+    "_OptionalScatterPlotVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": HistogramConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
+        "ChartConfiguration": ScatterPlotConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
-class HistogramVisualTypeDef(_RequiredHistogramVisualTypeDef, _OptionalHistogramVisualTypeDef):
+class ScatterPlotVisualOutputTypeDef(
+    _RequiredScatterPlotVisualOutputTypeDef, _OptionalScatterPlotVisualOutputTypeDef
+):
     pass
 
-_RequiredLineChartVisualTypeDef = TypedDict(
-    "_RequiredLineChartVisualTypeDef",
+_RequiredScatterPlotVisualTypeDef = TypedDict(
+    "_RequiredScatterPlotVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalLineChartVisualTypeDef = TypedDict(
-    "_OptionalLineChartVisualTypeDef",
+_OptionalScatterPlotVisualTypeDef = TypedDict(
+    "_OptionalScatterPlotVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": LineChartConfigurationTypeDef,
+        "ChartConfiguration": ScatterPlotConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
         "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
-class LineChartVisualTypeDef(_RequiredLineChartVisualTypeDef, _OptionalLineChartVisualTypeDef):
+class ScatterPlotVisualTypeDef(
+    _RequiredScatterPlotVisualTypeDef, _OptionalScatterPlotVisualTypeDef
+):
     pass
 
-_RequiredPieChartVisualTypeDef = TypedDict(
-    "_RequiredPieChartVisualTypeDef",
+_RequiredInsightVisualOutputTypeDef = TypedDict(
+    "_RequiredInsightVisualOutputTypeDef",
     {
         "VisualId": str,
+        "DataSetIdentifier": str,
     },
 )
-_OptionalPieChartVisualTypeDef = TypedDict(
-    "_OptionalPieChartVisualTypeDef",
+_OptionalInsightVisualOutputTypeDef = TypedDict(
+    "_OptionalInsightVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": PieChartConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "InsightConfiguration": InsightConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
-class PieChartVisualTypeDef(_RequiredPieChartVisualTypeDef, _OptionalPieChartVisualTypeDef):
+class InsightVisualOutputTypeDef(
+    _RequiredInsightVisualOutputTypeDef, _OptionalInsightVisualOutputTypeDef
+):
     pass
 
-_RequiredPivotTableVisualTypeDef = TypedDict(
-    "_RequiredPivotTableVisualTypeDef",
+_RequiredInsightVisualTypeDef = TypedDict(
+    "_RequiredInsightVisualTypeDef",
     {
         "VisualId": str,
+        "DataSetIdentifier": str,
     },
 )
-_OptionalPivotTableVisualTypeDef = TypedDict(
-    "_OptionalPivotTableVisualTypeDef",
+_OptionalInsightVisualTypeDef = TypedDict(
+    "_OptionalInsightVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": PivotTableConfigurationTypeDef,
-        "ConditionalFormatting": PivotTableConditionalFormattingTypeDef,
+        "InsightConfiguration": InsightConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
     },
     total=False,
 )
 
-class PivotTableVisualTypeDef(_RequiredPivotTableVisualTypeDef, _OptionalPivotTableVisualTypeDef):
+class InsightVisualTypeDef(_RequiredInsightVisualTypeDef, _OptionalInsightVisualTypeDef):
     pass
 
-_RequiredRadarChartVisualTypeDef = TypedDict(
-    "_RequiredRadarChartVisualTypeDef",
+_RequiredTreeMapVisualOutputTypeDef = TypedDict(
+    "_RequiredTreeMapVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalRadarChartVisualTypeDef = TypedDict(
-    "_OptionalRadarChartVisualTypeDef",
+_OptionalTreeMapVisualOutputTypeDef = TypedDict(
+    "_OptionalTreeMapVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": RadarChartConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "ChartConfiguration": TreeMapConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
-class RadarChartVisualTypeDef(_RequiredRadarChartVisualTypeDef, _OptionalRadarChartVisualTypeDef):
+class TreeMapVisualOutputTypeDef(
+    _RequiredTreeMapVisualOutputTypeDef, _OptionalTreeMapVisualOutputTypeDef
+):
     pass
 
-_RequiredSankeyDiagramVisualTypeDef = TypedDict(
-    "_RequiredSankeyDiagramVisualTypeDef",
+_RequiredTreeMapVisualTypeDef = TypedDict(
+    "_RequiredTreeMapVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalSankeyDiagramVisualTypeDef = TypedDict(
-    "_OptionalSankeyDiagramVisualTypeDef",
+_OptionalTreeMapVisualTypeDef = TypedDict(
+    "_OptionalTreeMapVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": SankeyDiagramChartConfigurationTypeDef,
+        "ChartConfiguration": TreeMapConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
-class SankeyDiagramVisualTypeDef(
-    _RequiredSankeyDiagramVisualTypeDef, _OptionalSankeyDiagramVisualTypeDef
-):
+class TreeMapVisualTypeDef(_RequiredTreeMapVisualTypeDef, _OptionalTreeMapVisualTypeDef):
     pass
 
-_RequiredScatterPlotVisualTypeDef = TypedDict(
-    "_RequiredScatterPlotVisualTypeDef",
+_RequiredWaterfallVisualOutputTypeDef = TypedDict(
+    "_RequiredWaterfallVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalScatterPlotVisualTypeDef = TypedDict(
-    "_OptionalScatterPlotVisualTypeDef",
+_OptionalWaterfallVisualOutputTypeDef = TypedDict(
+    "_OptionalWaterfallVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": ScatterPlotConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "ChartConfiguration": WaterfallChartConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
-class ScatterPlotVisualTypeDef(
-    _RequiredScatterPlotVisualTypeDef, _OptionalScatterPlotVisualTypeDef
+class WaterfallVisualOutputTypeDef(
+    _RequiredWaterfallVisualOutputTypeDef, _OptionalWaterfallVisualOutputTypeDef
 ):
     pass
 
-_RequiredInsightVisualTypeDef = TypedDict(
-    "_RequiredInsightVisualTypeDef",
+_RequiredWaterfallVisualTypeDef = TypedDict(
+    "_RequiredWaterfallVisualTypeDef",
     {
         "VisualId": str,
-        "DataSetIdentifier": str,
     },
 )
-_OptionalInsightVisualTypeDef = TypedDict(
-    "_OptionalInsightVisualTypeDef",
+_OptionalWaterfallVisualTypeDef = TypedDict(
+    "_OptionalWaterfallVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "InsightConfiguration": InsightConfigurationTypeDef,
+        "ChartConfiguration": WaterfallChartConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
+        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
-class InsightVisualTypeDef(_RequiredInsightVisualTypeDef, _OptionalInsightVisualTypeDef):
+class WaterfallVisualTypeDef(_RequiredWaterfallVisualTypeDef, _OptionalWaterfallVisualTypeDef):
     pass
 
-_RequiredTreeMapVisualTypeDef = TypedDict(
-    "_RequiredTreeMapVisualTypeDef",
+_RequiredWordCloudVisualOutputTypeDef = TypedDict(
+    "_RequiredWordCloudVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalTreeMapVisualTypeDef = TypedDict(
-    "_OptionalTreeMapVisualTypeDef",
+_OptionalWordCloudVisualOutputTypeDef = TypedDict(
+    "_OptionalWordCloudVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": TreeMapConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "ChartConfiguration": WordCloudChartConfigurationOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
+        "ColumnHierarchies": List[ColumnHierarchyOutputTypeDef],
     },
     total=False,
 )
 
-class TreeMapVisualTypeDef(_RequiredTreeMapVisualTypeDef, _OptionalTreeMapVisualTypeDef):
+class WordCloudVisualOutputTypeDef(
+    _RequiredWordCloudVisualOutputTypeDef, _OptionalWordCloudVisualOutputTypeDef
+):
     pass
 
-_RequiredWaterfallVisualTypeDef = TypedDict(
-    "_RequiredWaterfallVisualTypeDef",
+_RequiredWordCloudVisualTypeDef = TypedDict(
+    "_RequiredWordCloudVisualTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalWaterfallVisualTypeDef = TypedDict(
-    "_OptionalWaterfallVisualTypeDef",
+_OptionalWordCloudVisualTypeDef = TypedDict(
+    "_OptionalWordCloudVisualTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": WaterfallChartConfigurationTypeDef,
+        "ChartConfiguration": WordCloudChartConfigurationTypeDef,
         "Actions": Sequence[VisualCustomActionTypeDef],
         "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
     },
     total=False,
 )
 
-class WaterfallVisualTypeDef(_RequiredWaterfallVisualTypeDef, _OptionalWaterfallVisualTypeDef):
+class WordCloudVisualTypeDef(_RequiredWordCloudVisualTypeDef, _OptionalWordCloudVisualTypeDef):
     pass
 
-_RequiredWordCloudVisualTypeDef = TypedDict(
-    "_RequiredWordCloudVisualTypeDef",
+_RequiredTableVisualOutputTypeDef = TypedDict(
+    "_RequiredTableVisualOutputTypeDef",
     {
         "VisualId": str,
     },
 )
-_OptionalWordCloudVisualTypeDef = TypedDict(
-    "_OptionalWordCloudVisualTypeDef",
+_OptionalTableVisualOutputTypeDef = TypedDict(
+    "_OptionalTableVisualOutputTypeDef",
     {
         "Title": VisualTitleLabelOptionsTypeDef,
         "Subtitle": VisualSubtitleLabelOptionsTypeDef,
-        "ChartConfiguration": WordCloudChartConfigurationTypeDef,
-        "Actions": Sequence[VisualCustomActionTypeDef],
-        "ColumnHierarchies": Sequence[ColumnHierarchyTypeDef],
+        "ChartConfiguration": TableConfigurationOutputTypeDef,
+        "ConditionalFormatting": TableConditionalFormattingOutputTypeDef,
+        "Actions": List[VisualCustomActionOutputTypeDef],
     },
     total=False,
 )
 
-class WordCloudVisualTypeDef(_RequiredWordCloudVisualTypeDef, _OptionalWordCloudVisualTypeDef):
+class TableVisualOutputTypeDef(
+    _RequiredTableVisualOutputTypeDef, _OptionalTableVisualOutputTypeDef
+):
     pass
 
 _RequiredTableVisualTypeDef = TypedDict(
     "_RequiredTableVisualTypeDef",
     {
         "VisualId": str,
     },
@@ -23044,15 +19003,15 @@
     {
         "Title": str,
         "Description": str,
         "Name": str,
         "ParameterControls": List[ParameterControlOutputTypeDef],
         "FilterControls": List[FilterControlOutputTypeDef],
         "Visuals": List[VisualOutputTypeDef],
-        "TextBoxes": List[SheetTextBoxOutputTypeDef],
+        "TextBoxes": List[SheetTextBoxTypeDef],
         "Layouts": List[LayoutOutputTypeDef],
         "SheetControlLayouts": List[SheetControlLayoutOutputTypeDef],
         "ContentType": SheetContentTypeType,
     },
     total=False,
 )
 
@@ -23086,50 +19045,50 @@
 
 class SheetDefinitionTypeDef(_RequiredSheetDefinitionTypeDef, _OptionalSheetDefinitionTypeDef):
     pass
 
 _RequiredAnalysisDefinitionOutputTypeDef = TypedDict(
     "_RequiredAnalysisDefinitionOutputTypeDef",
     {
-        "DataSetIdentifierDeclarations": List[DataSetIdentifierDeclarationOutputTypeDef],
+        "DataSetIdentifierDeclarations": List[DataSetIdentifierDeclarationTypeDef],
     },
 )
 _OptionalAnalysisDefinitionOutputTypeDef = TypedDict(
     "_OptionalAnalysisDefinitionOutputTypeDef",
     {
         "Sheets": List[SheetDefinitionOutputTypeDef],
-        "CalculatedFields": List[CalculatedFieldOutputTypeDef],
+        "CalculatedFields": List[CalculatedFieldTypeDef],
         "ParameterDeclarations": List[ParameterDeclarationOutputTypeDef],
         "FilterGroups": List[FilterGroupOutputTypeDef],
         "ColumnConfigurations": List[ColumnConfigurationOutputTypeDef],
-        "AnalysisDefaults": AnalysisDefaultsOutputTypeDef,
+        "AnalysisDefaults": AnalysisDefaultsTypeDef,
     },
     total=False,
 )
 
 class AnalysisDefinitionOutputTypeDef(
     _RequiredAnalysisDefinitionOutputTypeDef, _OptionalAnalysisDefinitionOutputTypeDef
 ):
     pass
 
 _RequiredDashboardVersionDefinitionOutputTypeDef = TypedDict(
     "_RequiredDashboardVersionDefinitionOutputTypeDef",
     {
-        "DataSetIdentifierDeclarations": List[DataSetIdentifierDeclarationOutputTypeDef],
+        "DataSetIdentifierDeclarations": List[DataSetIdentifierDeclarationTypeDef],
     },
 )
 _OptionalDashboardVersionDefinitionOutputTypeDef = TypedDict(
     "_OptionalDashboardVersionDefinitionOutputTypeDef",
     {
         "Sheets": List[SheetDefinitionOutputTypeDef],
-        "CalculatedFields": List[CalculatedFieldOutputTypeDef],
+        "CalculatedFields": List[CalculatedFieldTypeDef],
         "ParameterDeclarations": List[ParameterDeclarationOutputTypeDef],
         "FilterGroups": List[FilterGroupOutputTypeDef],
         "ColumnConfigurations": List[ColumnConfigurationOutputTypeDef],
-        "AnalysisDefaults": AnalysisDefaultsOutputTypeDef,
+        "AnalysisDefaults": AnalysisDefaultsTypeDef,
     },
     total=False,
 )
 
 class DashboardVersionDefinitionOutputTypeDef(
     _RequiredDashboardVersionDefinitionOutputTypeDef,
     _OptionalDashboardVersionDefinitionOutputTypeDef,
@@ -23142,19 +19101,19 @@
         "DataSetConfigurations": List[DataSetConfigurationOutputTypeDef],
     },
 )
 _OptionalTemplateVersionDefinitionOutputTypeDef = TypedDict(
     "_OptionalTemplateVersionDefinitionOutputTypeDef",
     {
         "Sheets": List[SheetDefinitionOutputTypeDef],
-        "CalculatedFields": List[CalculatedFieldOutputTypeDef],
+        "CalculatedFields": List[CalculatedFieldTypeDef],
         "ParameterDeclarations": List[ParameterDeclarationOutputTypeDef],
         "FilterGroups": List[FilterGroupOutputTypeDef],
         "ColumnConfigurations": List[ColumnConfigurationOutputTypeDef],
-        "AnalysisDefaults": AnalysisDefaultsOutputTypeDef,
+        "AnalysisDefaults": AnalysisDefaultsTypeDef,
     },
     total=False,
 )
 
 class TemplateVersionDefinitionOutputTypeDef(
     _RequiredTemplateVersionDefinitionOutputTypeDef, _OptionalTemplateVersionDefinitionOutputTypeDef
 ):
@@ -23254,15 +19213,15 @@
         "Errors": List[DashboardErrorTypeDef],
         "Name": str,
         "ResourceStatus": ResourceStatusType,
         "ThemeArn": str,
         "Definition": DashboardVersionDefinitionOutputTypeDef,
         "Status": int,
         "RequestId": str,
-        "DashboardPublishOptions": DashboardPublishOptionsOutputTypeDef,
+        "DashboardPublishOptions": DashboardPublishOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTemplateDefinitionResponseTypeDef = TypedDict(
     "DescribeTemplateDefinitionResponseTypeDef",
     {
```

### Comparing `mypy-boto3-quicksight-1.28.12/mypy_boto3_quicksight.egg-info/SOURCES.txt` & `mypy-boto3-quicksight-1.28.15/mypy_boto3_quicksight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-quicksight-1.28.12/setup.py` & `mypy-boto3-quicksight-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-quicksight",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_quicksight"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.QuickSight 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.QuickSight 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

