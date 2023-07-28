# Comparing `tmp/mypy-boto3-cleanrooms-1.28.12.tar.gz` & `tmp/mypy-boto3-cleanrooms-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cleanrooms-1.28.12.tar", last modified: Thu Jul 27 05:34:24 2023, max compression
+gzip compressed data, was "mypy-boto3-cleanrooms-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
```

## Comparing `mypy-boto3-cleanrooms-1.28.12.tar` & `mypy-boto3-cleanrooms-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.864563 mypy-boto3-cleanrooms-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19502 2023-07-27 05:34:24.864563 mypy-boto3-cleanrooms-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17996 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.864563 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29888 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29837 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46253 2023-07-27 05:18:25.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46192 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.864563 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19502 2023-07-27 05:34:24.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:24.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:24.000000 mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:24.864563 mypy-boto3-cleanrooms-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:18:23.000000 mypy-boto3-cleanrooms-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.356780 mypy-boto3-cleanrooms-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19147 2023-07-28 20:42:25.356780 mypy-boto3-cleanrooms-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.356780 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29888 2023-07-28 20:20:47.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29837 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-28 20:20:47.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-07-28 20:20:47.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-07-28 20:20:47.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-28 20:20:47.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43817 2023-07-28 20:20:48.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43758 2023-07-28 20:20:48.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.356780 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19147 2023-07-28 20:42:25.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:25.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:25.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:25.000000 mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.356780 mypy-boto3-cleanrooms-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:20:46.000000 mypy-boto3-cleanrooms-1.28.15/setup.py
```

### Comparing `mypy-boto3-cleanrooms-1.28.12/LICENSE` & `mypy-boto3-cleanrooms-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.12/PKG-INFO` & `mypy-boto3-cleanrooms-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanrooms
-Version: 1.28.12
-Summary: Type annotations for boto3.CleanRoomsService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CleanRoomsService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cleanrooms)](https://pepy.tech/project/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,27 +368,26 @@
 `mypy_boto3_cleanrooms.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cleanrooms.type_defs import (
     AggregateColumnOutputTypeDef,
     AggregateColumnTypeDef,
-    AggregationConstraintOutputTypeDef,
     AggregationConstraintTypeDef,
     AnalysisRuleListOutputTypeDef,
     AnalysisRuleListTypeDef,
     BatchGetSchemaErrorTypeDef,
     BatchGetSchemaInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     CollaborationSummaryTypeDef,
-    DataEncryptionMetadataOutputTypeDef,
+    DataEncryptionMetadataTypeDef,
     ColumnTypeDef,
     ConfiguredTableAssociationSummaryTypeDef,
     ConfiguredTableAssociationTypeDef,
     ConfiguredTableSummaryTypeDef,
-    DataEncryptionMetadataTypeDef,
     MemberSpecificationTypeDef,
     CreateConfiguredTableAssociationInputRequestTypeDef,
     CreateMembershipInputRequestTypeDef,
     MembershipTypeDef,
     DeleteCollaborationInputRequestTypeDef,
     DeleteConfiguredTableAnalysisRuleInputRequestTypeDef,
     DeleteConfiguredTableAssociationInputRequestTypeDef,
@@ -399,86 +398,79 @@
     GetConfiguredTableAnalysisRuleInputRequestTypeDef,
     GetConfiguredTableAssociationInputRequestTypeDef,
     GetConfiguredTableInputRequestTypeDef,
     GetMembershipInputRequestTypeDef,
     GetProtectedQueryInputRequestTypeDef,
     GetSchemaAnalysisRuleInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
-    GlueTableReferenceOutputTypeDef,
     GlueTableReferenceTypeDef,
-    ListCollaborationsInputListCollaborationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCollaborationsInputRequestTypeDef,
-    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
     ListConfiguredTableAssociationsInputRequestTypeDef,
-    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
     ListConfiguredTablesInputRequestTypeDef,
-    ListMembersInputListMembersPaginateTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
-    ListMembershipsInputListMembershipsPaginateTypeDef,
     ListMembershipsInputRequestTypeDef,
     MembershipSummaryTypeDef,
-    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
     ListProtectedQueriesInputRequestTypeDef,
     ProtectedQuerySummaryTypeDef,
-    ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
     ProtectedQueryErrorTypeDef,
-    ProtectedQueryS3OutputConfigurationOutputTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
-    ProtectedQuerySQLParametersOutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
     AnalysisRuleAggregationOutputTypeDef,
     AnalysisRuleAggregationTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     CreateCollaborationInputRequestTypeDef,
     CreateMembershipOutputTypeDef,
     GetMembershipOutputTypeDef,
     UpdateMembershipOutputTypeDef,
-    TableReferenceOutputTypeDef,
     TableReferenceTypeDef,
+    ListCollaborationsInputListCollaborationsPaginateTypeDef,
+    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
+    ListMembersInputListMembersPaginateTypeDef,
+    ListMembershipsInputListMembershipsPaginateTypeDef,
+    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+    ListSchemasInputListSchemasPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
-    ProtectedQueryOutputConfigurationOutputTypeDef,
     ProtectedQueryOutputConfigurationTypeDef,
     ProtectedQueryOutputTypeDef,
     AnalysisRulePolicyV1TypeDef,
     ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
     ConfiguredTableAnalysisRulePolicyV1TypeDef,
     CreateCollaborationOutputTypeDef,
     GetCollaborationOutputTypeDef,
     UpdateCollaborationOutputTypeDef,
     BatchGetSchemaOutputTypeDef,
     GetSchemaOutputTypeDef,
     ConfiguredTableTypeDef,
     CreateConfiguredTableInputRequestTypeDef,
-    ProtectedQueryResultConfigurationOutputTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQueryResultTypeDef,
     AnalysisRulePolicyTypeDef,
     ConfiguredTableAnalysisRulePolicyOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateConfiguredTableOutputTypeDef,
     GetConfiguredTableOutputTypeDef,
```

### Comparing `mypy-boto3-cleanrooms-1.28.12/README.md` & `mypy-boto3-cleanrooms-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cleanrooms)](https://pepy.tech/project/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,27 +336,26 @@
 `mypy_boto3_cleanrooms.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cleanrooms.type_defs import (
     AggregateColumnOutputTypeDef,
     AggregateColumnTypeDef,
-    AggregationConstraintOutputTypeDef,
     AggregationConstraintTypeDef,
     AnalysisRuleListOutputTypeDef,
     AnalysisRuleListTypeDef,
     BatchGetSchemaErrorTypeDef,
     BatchGetSchemaInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     CollaborationSummaryTypeDef,
-    DataEncryptionMetadataOutputTypeDef,
+    DataEncryptionMetadataTypeDef,
     ColumnTypeDef,
     ConfiguredTableAssociationSummaryTypeDef,
     ConfiguredTableAssociationTypeDef,
     ConfiguredTableSummaryTypeDef,
-    DataEncryptionMetadataTypeDef,
     MemberSpecificationTypeDef,
     CreateConfiguredTableAssociationInputRequestTypeDef,
     CreateMembershipInputRequestTypeDef,
     MembershipTypeDef,
     DeleteCollaborationInputRequestTypeDef,
     DeleteConfiguredTableAnalysisRuleInputRequestTypeDef,
     DeleteConfiguredTableAssociationInputRequestTypeDef,
@@ -367,86 +366,79 @@
     GetConfiguredTableAnalysisRuleInputRequestTypeDef,
     GetConfiguredTableAssociationInputRequestTypeDef,
     GetConfiguredTableInputRequestTypeDef,
     GetMembershipInputRequestTypeDef,
     GetProtectedQueryInputRequestTypeDef,
     GetSchemaAnalysisRuleInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
-    GlueTableReferenceOutputTypeDef,
     GlueTableReferenceTypeDef,
-    ListCollaborationsInputListCollaborationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCollaborationsInputRequestTypeDef,
-    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
     ListConfiguredTableAssociationsInputRequestTypeDef,
-    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
     ListConfiguredTablesInputRequestTypeDef,
-    ListMembersInputListMembersPaginateTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
-    ListMembershipsInputListMembershipsPaginateTypeDef,
     ListMembershipsInputRequestTypeDef,
     MembershipSummaryTypeDef,
-    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
     ListProtectedQueriesInputRequestTypeDef,
     ProtectedQuerySummaryTypeDef,
-    ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
     ProtectedQueryErrorTypeDef,
-    ProtectedQueryS3OutputConfigurationOutputTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
-    ProtectedQuerySQLParametersOutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
     AnalysisRuleAggregationOutputTypeDef,
     AnalysisRuleAggregationTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     CreateCollaborationInputRequestTypeDef,
     CreateMembershipOutputTypeDef,
     GetMembershipOutputTypeDef,
     UpdateMembershipOutputTypeDef,
-    TableReferenceOutputTypeDef,
     TableReferenceTypeDef,
+    ListCollaborationsInputListCollaborationsPaginateTypeDef,
+    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
+    ListMembersInputListMembersPaginateTypeDef,
+    ListMembershipsInputListMembershipsPaginateTypeDef,
+    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+    ListSchemasInputListSchemasPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
-    ProtectedQueryOutputConfigurationOutputTypeDef,
     ProtectedQueryOutputConfigurationTypeDef,
     ProtectedQueryOutputTypeDef,
     AnalysisRulePolicyV1TypeDef,
     ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
     ConfiguredTableAnalysisRulePolicyV1TypeDef,
     CreateCollaborationOutputTypeDef,
     GetCollaborationOutputTypeDef,
     UpdateCollaborationOutputTypeDef,
     BatchGetSchemaOutputTypeDef,
     GetSchemaOutputTypeDef,
     ConfiguredTableTypeDef,
     CreateConfiguredTableInputRequestTypeDef,
-    ProtectedQueryResultConfigurationOutputTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQueryResultTypeDef,
     AnalysisRulePolicyTypeDef,
     ConfiguredTableAnalysisRulePolicyOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateConfiguredTableOutputTypeDef,
     GetConfiguredTableOutputTypeDef,
```

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/__init__.py` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/__init__.pyi` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/__main__.py` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CleanRoomsService 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CleanRoomsService 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService\nOther"
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

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/client.py` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/client.pyi` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/literals.py` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/literals.pyi` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/paginator.py` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -49,146 +49,133 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListCollaborationsPaginator",
     "ListConfiguredTableAssociationsPaginator",
     "ListConfiguredTablesPaginator",
     "ListMembersPaginator",
     "ListMembershipsPaginator",
     "ListProtectedQueriesPaginator",
     "ListSchemasPaginator",
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
 class ListCollaborationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listcollaborationspaginator)
     """
 
     def paginate(
         self,
         *,
         memberStatus: FilterableMemberStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCollaborationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listcollaborationspaginator)
         """
 
-
 class ListConfiguredTableAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
     """
 
     def paginate(
-        self, *, membershipIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, membershipIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfiguredTableAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
         """
 
-
 class ListConfiguredTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfiguredTablesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtablespaginator)
         """
 
-
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, collaborationIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, collaborationIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmemberspaginator)
         """
 
-
 class ListMembershipsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmembershipspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        status: MembershipStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: MembershipStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembershipsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmembershipspaginator)
         """
 
-
 class ListProtectedQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listprotectedqueriespaginator)
     """
 
     def paginate(
         self,
         *,
         membershipIdentifier: str,
         status: ProtectedQueryStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProtectedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listprotectedqueriespaginator)
         """
 
-
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listschemaspaginator)
     """
 
     def paginate(
         self,
         *,
         collaborationIdentifier: str,
         schemaType: Literal["TABLE"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchemasOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listschemaspaginator)
         """
```

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/paginator.pyi` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,136 +49,143 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListCollaborationsPaginator",
     "ListConfiguredTableAssociationsPaginator",
     "ListConfiguredTablesPaginator",
     "ListMembersPaginator",
     "ListMembershipsPaginator",
     "ListProtectedQueriesPaginator",
     "ListSchemasPaginator",
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
 class ListCollaborationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listcollaborationspaginator)
     """
 
     def paginate(
         self,
         *,
         memberStatus: FilterableMemberStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCollaborationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listcollaborationspaginator)
         """
 
+
 class ListConfiguredTableAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
     """
 
     def paginate(
-        self, *, membershipIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, membershipIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfiguredTableAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
         """
 
+
 class ListConfiguredTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfiguredTablesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listconfiguredtablespaginator)
         """
 
+
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, collaborationIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, collaborationIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmemberspaginator)
         """
 
+
 class ListMembershipsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmembershipspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        status: MembershipStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: MembershipStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembershipsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listmembershipspaginator)
         """
 
+
 class ListProtectedQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listprotectedqueriespaginator)
     """
 
     def paginate(
         self,
         *,
         membershipIdentifier: str,
         status: ProtectedQueryStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProtectedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listprotectedqueriespaginator)
         """
 
+
 class ListSchemasPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listschemaspaginator)
     """
 
     def paginate(
         self,
         *,
         collaborationIdentifier: str,
         schemaType: Literal["TABLE"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchemasOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/paginators/#listschemaspaginator)
         """
```

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/type_defs.py` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,27 +40,26 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AggregateColumnOutputTypeDef",
     "AggregateColumnTypeDef",
-    "AggregationConstraintOutputTypeDef",
     "AggregationConstraintTypeDef",
     "AnalysisRuleListOutputTypeDef",
     "AnalysisRuleListTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CollaborationSummaryTypeDef",
-    "DataEncryptionMetadataOutputTypeDef",
+    "DataEncryptionMetadataTypeDef",
     "ColumnTypeDef",
     "ConfiguredTableAssociationSummaryTypeDef",
     "ConfiguredTableAssociationTypeDef",
     "ConfiguredTableSummaryTypeDef",
-    "DataEncryptionMetadataTypeDef",
     "MemberSpecificationTypeDef",
     "CreateConfiguredTableAssociationInputRequestTypeDef",
     "CreateMembershipInputRequestTypeDef",
     "MembershipTypeDef",
     "DeleteCollaborationInputRequestTypeDef",
     "DeleteConfiguredTableAnalysisRuleInputRequestTypeDef",
     "DeleteConfiguredTableAssociationInputRequestTypeDef",
@@ -71,86 +70,79 @@
     "GetConfiguredTableAnalysisRuleInputRequestTypeDef",
     "GetConfiguredTableAssociationInputRequestTypeDef",
     "GetConfiguredTableInputRequestTypeDef",
     "GetMembershipInputRequestTypeDef",
     "GetProtectedQueryInputRequestTypeDef",
     "GetSchemaAnalysisRuleInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
-    "GlueTableReferenceOutputTypeDef",
     "GlueTableReferenceTypeDef",
-    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListCollaborationsInputRequestTypeDef",
-    "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
     "ListConfiguredTableAssociationsInputRequestTypeDef",
-    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
     "ListConfiguredTablesInputRequestTypeDef",
-    "ListMembersInputListMembersPaginateTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
-    "ListMembershipsInputListMembershipsPaginateTypeDef",
     "ListMembershipsInputRequestTypeDef",
     "MembershipSummaryTypeDef",
-    "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
     "ListProtectedQueriesInputRequestTypeDef",
     "ProtectedQuerySummaryTypeDef",
-    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListSchemasInputRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ProtectedQueryErrorTypeDef",
-    "ProtectedQueryS3OutputConfigurationOutputTypeDef",
     "ProtectedQueryS3OutputConfigurationTypeDef",
     "ProtectedQueryS3OutputTypeDef",
-    "ProtectedQuerySQLParametersOutputTypeDef",
     "ProtectedQuerySQLParametersTypeDef",
     "ProtectedQueryStatisticsTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
     "AnalysisRuleAggregationOutputTypeDef",
     "AnalysisRuleAggregationTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
     "GetConfiguredTableAssociationOutputTypeDef",
     "UpdateConfiguredTableAssociationOutputTypeDef",
     "ListConfiguredTablesOutputTypeDef",
     "CreateCollaborationInputRequestTypeDef",
     "CreateMembershipOutputTypeDef",
     "GetMembershipOutputTypeDef",
     "UpdateMembershipOutputTypeDef",
-    "TableReferenceOutputTypeDef",
     "TableReferenceTypeDef",
+    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+    "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
+    "ListMembersInputListMembersPaginateTypeDef",
+    "ListMembershipsInputListMembershipsPaginateTypeDef",
+    "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListMembersOutputTypeDef",
     "ListMembershipsOutputTypeDef",
     "ListProtectedQueriesOutputTypeDef",
     "ListSchemasOutputTypeDef",
-    "ProtectedQueryOutputConfigurationOutputTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
     "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     "CreateCollaborationOutputTypeDef",
     "GetCollaborationOutputTypeDef",
     "UpdateCollaborationOutputTypeDef",
     "BatchGetSchemaOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "ConfiguredTableTypeDef",
     "CreateConfiguredTableInputRequestTypeDef",
-    "ProtectedQueryResultConfigurationOutputTypeDef",
     "ProtectedQueryResultConfigurationTypeDef",
     "ProtectedQueryResultTypeDef",
     "AnalysisRulePolicyTypeDef",
     "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     "CreateConfiguredTableOutputTypeDef",
     "GetConfiguredTableOutputTypeDef",
@@ -182,23 +174,14 @@
     "AggregateColumnTypeDef",
     {
         "columnNames": Sequence[str],
         "function": AggregateFunctionNameType,
     },
 )
 
-AggregationConstraintOutputTypeDef = TypedDict(
-    "AggregationConstraintOutputTypeDef",
-    {
-        "columnName": str,
-        "minimum": int,
-        "type": Literal["COUNT_DISTINCT"],
-    },
-)
-
 AggregationConstraintTypeDef = TypedDict(
     "AggregationConstraintTypeDef",
     {
         "columnName": str,
         "minimum": int,
         "type": Literal["COUNT_DISTINCT"],
     },
@@ -259,14 +242,25 @@
     "BatchGetSchemaInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "names": Sequence[str],
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
 _RequiredCollaborationSummaryTypeDef = TypedDict(
     "_RequiredCollaborationSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "creatorAccountId": str,
@@ -288,16 +282,16 @@
 
 class CollaborationSummaryTypeDef(
     _RequiredCollaborationSummaryTypeDef, _OptionalCollaborationSummaryTypeDef
 ):
     pass
 
 
-DataEncryptionMetadataOutputTypeDef = TypedDict(
-    "DataEncryptionMetadataOutputTypeDef",
+DataEncryptionMetadataTypeDef = TypedDict(
+    "DataEncryptionMetadataTypeDef",
     {
         "allowCleartext": bool,
         "allowDuplicates": bool,
         "allowJoinsOnColumnsWithDifferentNames": bool,
         "preserveNulls": bool,
     },
 )
@@ -363,24 +357,14 @@
         "createTime": datetime,
         "updateTime": datetime,
         "analysisRuleTypes": List[ConfiguredTableAnalysisRuleTypeType],
         "analysisMethod": Literal["DIRECT_QUERY"],
     },
 )
 
-DataEncryptionMetadataTypeDef = TypedDict(
-    "DataEncryptionMetadataTypeDef",
-    {
-        "allowCleartext": bool,
-        "allowDuplicates": bool,
-        "allowJoinsOnColumnsWithDifferentNames": bool,
-        "preserveNulls": bool,
-    },
-)
-
 MemberSpecificationTypeDef = TypedDict(
     "MemberSpecificationTypeDef",
     {
         "accountId": str,
         "memberAbilities": Sequence[MemberAbilityType],
         "displayName": str,
     },
@@ -555,71 +539,42 @@
     "GetSchemaInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "name": str,
     },
 )
 
-GlueTableReferenceOutputTypeDef = TypedDict(
-    "GlueTableReferenceOutputTypeDef",
-    {
-        "tableName": str,
-        "databaseName": str,
-    },
-)
-
 GlueTableReferenceTypeDef = TypedDict(
     "GlueTableReferenceTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
 
-ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
-    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "memberStatus": FilterableMemberStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListCollaborationsInputRequestTypeDef = TypedDict(
     "ListCollaborationsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "memberStatus": FilterableMemberStatusType,
     },
     total=False,
 )
 
-_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    {
-        "membershipIdentifier": str,
-    },
-)
-_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(
-    _RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-    _OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListConfiguredTableAssociationsInputRequestTypeDef = TypedDict(
     "_RequiredListConfiguredTableAssociationsInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalListConfiguredTableAssociationsInputRequestTypeDef = TypedDict(
@@ -635,53 +590,23 @@
 class ListConfiguredTableAssociationsInputRequestTypeDef(
     _RequiredListConfiguredTableAssociationsInputRequestTypeDef,
     _OptionalListConfiguredTableAssociationsInputRequestTypeDef,
 ):
     pass
 
 
-ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef = TypedDict(
-    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListConfiguredTablesInputRequestTypeDef = TypedDict(
     "ListConfiguredTablesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListMembersInputListMembersPaginateTypeDef = TypedDict(
-    "_RequiredListMembersInputListMembersPaginateTypeDef",
-    {
-        "collaborationIdentifier": str,
-    },
-)
-_OptionalListMembersInputListMembersPaginateTypeDef = TypedDict(
-    "_OptionalListMembersInputListMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMembersInputListMembersPaginateTypeDef(
-    _RequiredListMembersInputListMembersPaginateTypeDef,
-    _OptionalListMembersInputListMembersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMembersInputRequestTypeDef = TypedDict(
     "_RequiredListMembersInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalListMembersInputRequestTypeDef = TypedDict(
@@ -721,23 +646,14 @@
 )
 
 
 class MemberSummaryTypeDef(_RequiredMemberSummaryTypeDef, _OptionalMemberSummaryTypeDef):
     pass
 
 
-ListMembershipsInputListMembershipsPaginateTypeDef = TypedDict(
-    "ListMembershipsInputListMembershipsPaginateTypeDef",
-    {
-        "status": MembershipStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMembershipsInputRequestTypeDef = TypedDict(
     "ListMembershipsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": MembershipStatusType,
     },
@@ -757,37 +673,14 @@
         "createTime": datetime,
         "updateTime": datetime,
         "status": MembershipStatusType,
         "memberAbilities": List[MemberAbilityType],
     },
 )
 
-_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
-    "_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    {
-        "membershipIdentifier": str,
-    },
-)
-_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
-    "_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    {
-        "status": ProtectedQueryStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(
-    _RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-    _OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListProtectedQueriesInputRequestTypeDef = TypedDict(
     "_RequiredListProtectedQueriesInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalListProtectedQueriesInputRequestTypeDef = TypedDict(
@@ -815,37 +708,14 @@
         "membershipId": str,
         "membershipArn": str,
         "createTime": datetime,
         "status": ProtectedQueryStatusType,
     },
 )
 
-_RequiredListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "collaborationIdentifier": str,
-    },
-)
-_OptionalListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "schemaType": Literal["TABLE"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSchemasInputListSchemasPaginateTypeDef(
-    _RequiredListSchemasInputListSchemasPaginateTypeDef,
-    _OptionalListSchemasInputListSchemasPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSchemasInputRequestTypeDef = TypedDict(
     "_RequiredListSchemasInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalListSchemasInputRequestTypeDef = TypedDict(
@@ -894,63 +764,22 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": Dict[str, str],
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
 ProtectedQueryErrorTypeDef = TypedDict(
     "ProtectedQueryErrorTypeDef",
     {
         "message": str,
         "code": str,
     },
 )
 
-_RequiredProtectedQueryS3OutputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredProtectedQueryS3OutputConfigurationOutputTypeDef",
-    {
-        "resultFormat": ResultFormatType,
-        "bucket": str,
-    },
-)
-_OptionalProtectedQueryS3OutputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalProtectedQueryS3OutputConfigurationOutputTypeDef",
-    {
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-
-class ProtectedQueryS3OutputConfigurationOutputTypeDef(
-    _RequiredProtectedQueryS3OutputConfigurationOutputTypeDef,
-    _OptionalProtectedQueryS3OutputConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredProtectedQueryS3OutputConfigurationTypeDef = TypedDict(
     "_RequiredProtectedQueryS3OutputConfigurationTypeDef",
     {
         "resultFormat": ResultFormatType,
         "bucket": str,
     },
 )
@@ -973,22 +802,14 @@
 ProtectedQueryS3OutputTypeDef = TypedDict(
     "ProtectedQueryS3OutputTypeDef",
     {
         "location": str,
     },
 )
 
-ProtectedQuerySQLParametersOutputTypeDef = TypedDict(
-    "ProtectedQuerySQLParametersOutputTypeDef",
-    {
-        "queryString": str,
-    },
-    total=False,
-)
-
 ProtectedQuerySQLParametersTypeDef = TypedDict(
     "ProtectedQuerySQLParametersTypeDef",
     {
         "queryString": str,
     },
     total=False,
 )
@@ -997,25 +818,14 @@
     "ProtectedQueryStatisticsTypeDef",
     {
         "totalDurationInMillis": int,
     },
     total=False,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1130,15 +940,15 @@
 _RequiredAnalysisRuleAggregationOutputTypeDef = TypedDict(
     "_RequiredAnalysisRuleAggregationOutputTypeDef",
     {
         "aggregateColumns": List[AggregateColumnOutputTypeDef],
         "joinColumns": List[str],
         "dimensionColumns": List[str],
         "scalarFunctions": List[ScalarFunctionsType],
-        "outputConstraints": List[AggregationConstraintOutputTypeDef],
+        "outputConstraints": List[AggregationConstraintTypeDef],
     },
 )
 _OptionalAnalysisRuleAggregationOutputTypeDef = TypedDict(
     "_OptionalAnalysisRuleAggregationOutputTypeDef",
     {
         "joinRequired": Literal["QUERY_RUNNER"],
         "allowedJoinOperators": List[JoinOperatorType],
@@ -1175,20 +985,28 @@
 
 class AnalysisRuleAggregationTypeDef(
     _RequiredAnalysisRuleAggregationTypeDef, _OptionalAnalysisRuleAggregationTypeDef
 ):
     pass
 
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCollaborationsOutputTypeDef = TypedDict(
     "ListCollaborationsOutputTypeDef",
     {
         "nextToken": str,
         "collaborationList": List[CollaborationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCollaborationTypeDef = TypedDict(
     "_RequiredCollaborationTypeDef",
     {
         "id": str,
@@ -1204,15 +1022,15 @@
 )
 _OptionalCollaborationTypeDef = TypedDict(
     "_OptionalCollaborationTypeDef",
     {
         "description": str,
         "membershipId": str,
         "membershipArn": str,
-        "dataEncryptionMetadata": DataEncryptionMetadataOutputTypeDef,
+        "dataEncryptionMetadata": DataEncryptionMetadataTypeDef,
     },
     total=False,
 )
 
 
 class CollaborationTypeDef(_RequiredCollaborationTypeDef, _OptionalCollaborationTypeDef):
     pass
@@ -1248,48 +1066,48 @@
 
 
 ListConfiguredTableAssociationsOutputTypeDef = TypedDict(
     "ListConfiguredTableAssociationsOutputTypeDef",
     {
         "configuredTableAssociationSummaries": List[ConfiguredTableAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConfiguredTableAssociationOutputTypeDef = TypedDict(
     "CreateConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConfiguredTableAssociationOutputTypeDef = TypedDict(
     "GetConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfiguredTableAssociationOutputTypeDef = TypedDict(
     "UpdateConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfiguredTablesOutputTypeDef = TypedDict(
     "ListConfiguredTablesOutputTypeDef",
     {
         "configuredTableSummaries": List[ConfiguredTableSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCollaborationInputRequestTypeDef = TypedDict(
     "_RequiredCreateCollaborationInputRequestTypeDef",
     {
         "members": Sequence[MemberSpecificationTypeDef],
@@ -1316,94 +1134,194 @@
     pass
 
 
 CreateMembershipOutputTypeDef = TypedDict(
     "CreateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMembershipOutputTypeDef = TypedDict(
     "GetMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMembershipOutputTypeDef = TypedDict(
     "UpdateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TableReferenceOutputTypeDef = TypedDict(
-    "TableReferenceOutputTypeDef",
+TableReferenceTypeDef = TypedDict(
+    "TableReferenceTypeDef",
     {
-        "glue": GlueTableReferenceOutputTypeDef,
+        "glue": GlueTableReferenceTypeDef,
     },
     total=False,
 )
 
-TableReferenceTypeDef = TypedDict(
-    "TableReferenceTypeDef",
+ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
+    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
     {
-        "glue": GlueTableReferenceTypeDef,
+        "memberStatus": FilterableMemberStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(
+    _RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+    _OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+):
+    pass
+
+
+ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef = TypedDict(
+    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMembersInputListMembersPaginateTypeDef = TypedDict(
+    "_RequiredListMembersInputListMembersPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListMembersInputListMembersPaginateTypeDef = TypedDict(
+    "_OptionalListMembersInputListMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMembersInputListMembersPaginateTypeDef(
+    _RequiredListMembersInputListMembersPaginateTypeDef,
+    _OptionalListMembersInputListMembersPaginateTypeDef,
+):
+    pass
+
+
+ListMembershipsInputListMembershipsPaginateTypeDef = TypedDict(
+    "ListMembershipsInputListMembershipsPaginateTypeDef",
+    {
+        "status": MembershipStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
+    "_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
+    "_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    {
+        "status": ProtectedQueryStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(
+    _RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+    _OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "schemaType": Literal["TABLE"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSchemasInputListSchemasPaginateTypeDef(
+    _RequiredListSchemasInputListSchemasPaginateTypeDef,
+    _OptionalListSchemasInputListSchemasPaginateTypeDef,
+):
+    pass
+
+
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "nextToken": str,
         "memberSummaries": List[MemberSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembershipsOutputTypeDef = TypedDict(
     "ListMembershipsOutputTypeDef",
     {
         "nextToken": str,
         "membershipSummaries": List[MembershipSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtectedQueriesOutputTypeDef = TypedDict(
     "ListProtectedQueriesOutputTypeDef",
     {
         "nextToken": str,
         "protectedQueries": List[ProtectedQuerySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemasOutputTypeDef = TypedDict(
     "ListSchemasOutputTypeDef",
     {
         "schemaSummaries": List[SchemaSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProtectedQueryOutputConfigurationOutputTypeDef = TypedDict(
-    "ProtectedQueryOutputConfigurationOutputTypeDef",
-    {
-        "s3": ProtectedQueryS3OutputConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ProtectedQueryOutputConfigurationTypeDef = TypedDict(
     "ProtectedQueryOutputConfigurationTypeDef",
     {
         "s3": ProtectedQueryS3OutputConfigurationTypeDef,
     },
     total=False,
 )
@@ -1443,58 +1361,58 @@
     total=False,
 )
 
 CreateCollaborationOutputTypeDef = TypedDict(
     "CreateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCollaborationOutputTypeDef = TypedDict(
     "GetCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCollaborationOutputTypeDef = TypedDict(
     "UpdateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetSchemaOutputTypeDef = TypedDict(
     "BatchGetSchemaOutputTypeDef",
     {
         "schemas": List[SchemaTypeDef],
         "errors": List[BatchGetSchemaErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSchemaOutputTypeDef = TypedDict(
     "GetSchemaOutputTypeDef",
     {
         "schema": SchemaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConfiguredTableTypeDef = TypedDict(
     "_RequiredConfiguredTableTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
-        "tableReference": TableReferenceOutputTypeDef,
+        "tableReference": TableReferenceTypeDef,
         "createTime": datetime,
         "updateTime": datetime,
         "analysisRuleTypes": List[ConfiguredTableAnalysisRuleTypeType],
         "analysisMethod": Literal["DIRECT_QUERY"],
         "allowedColumns": List[str],
     },
 )
@@ -1533,21 +1451,14 @@
 class CreateConfiguredTableInputRequestTypeDef(
     _RequiredCreateConfiguredTableInputRequestTypeDef,
     _OptionalCreateConfiguredTableInputRequestTypeDef,
 ):
     pass
 
 
-ProtectedQueryResultConfigurationOutputTypeDef = TypedDict(
-    "ProtectedQueryResultConfigurationOutputTypeDef",
-    {
-        "outputConfiguration": ProtectedQueryOutputConfigurationOutputTypeDef,
-    },
-)
-
 ProtectedQueryResultConfigurationTypeDef = TypedDict(
     "ProtectedQueryResultConfigurationTypeDef",
     {
         "outputConfiguration": ProtectedQueryOutputConfigurationTypeDef,
     },
 )
 
@@ -1582,31 +1493,31 @@
     total=False,
 )
 
 CreateConfiguredTableOutputTypeDef = TypedDict(
     "CreateConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConfiguredTableOutputTypeDef = TypedDict(
     "GetConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfiguredTableOutputTypeDef = TypedDict(
     "UpdateConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartProtectedQueryInputRequestTypeDef = TypedDict(
     "StartProtectedQueryInputRequestTypeDef",
     {
         "type": Literal["SQL"],
@@ -1619,17 +1530,17 @@
 _RequiredProtectedQueryTypeDef = TypedDict(
     "_RequiredProtectedQueryTypeDef",
     {
         "id": str,
         "membershipId": str,
         "membershipArn": str,
         "createTime": datetime,
-        "sqlParameters": ProtectedQuerySQLParametersOutputTypeDef,
+        "sqlParameters": ProtectedQuerySQLParametersTypeDef,
         "status": ProtectedQueryStatusType,
-        "resultConfiguration": ProtectedQueryResultConfigurationOutputTypeDef,
+        "resultConfiguration": ProtectedQueryResultConfigurationTypeDef,
     },
 )
 _OptionalProtectedQueryTypeDef = TypedDict(
     "_OptionalProtectedQueryTypeDef",
     {
         "statistics": ProtectedQueryStatisticsTypeDef,
         "result": ProtectedQueryResultTypeDef,
@@ -1685,58 +1596,58 @@
     },
 )
 
 GetProtectedQueryOutputTypeDef = TypedDict(
     "GetProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartProtectedQueryOutputTypeDef = TypedDict(
     "StartProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProtectedQueryOutputTypeDef = TypedDict(
     "UpdateProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSchemaAnalysisRuleOutputTypeDef = TypedDict(
     "GetSchemaAnalysisRuleOutputTypeDef",
     {
         "analysisRule": AnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "CreateConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "GetConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "UpdateConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms/type_defs.pyi` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -39,27 +39,26 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AggregateColumnOutputTypeDef",
     "AggregateColumnTypeDef",
-    "AggregationConstraintOutputTypeDef",
     "AggregationConstraintTypeDef",
     "AnalysisRuleListOutputTypeDef",
     "AnalysisRuleListTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CollaborationSummaryTypeDef",
-    "DataEncryptionMetadataOutputTypeDef",
+    "DataEncryptionMetadataTypeDef",
     "ColumnTypeDef",
     "ConfiguredTableAssociationSummaryTypeDef",
     "ConfiguredTableAssociationTypeDef",
     "ConfiguredTableSummaryTypeDef",
-    "DataEncryptionMetadataTypeDef",
     "MemberSpecificationTypeDef",
     "CreateConfiguredTableAssociationInputRequestTypeDef",
     "CreateMembershipInputRequestTypeDef",
     "MembershipTypeDef",
     "DeleteCollaborationInputRequestTypeDef",
     "DeleteConfiguredTableAnalysisRuleInputRequestTypeDef",
     "DeleteConfiguredTableAssociationInputRequestTypeDef",
@@ -70,86 +69,79 @@
     "GetConfiguredTableAnalysisRuleInputRequestTypeDef",
     "GetConfiguredTableAssociationInputRequestTypeDef",
     "GetConfiguredTableInputRequestTypeDef",
     "GetMembershipInputRequestTypeDef",
     "GetProtectedQueryInputRequestTypeDef",
     "GetSchemaAnalysisRuleInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
-    "GlueTableReferenceOutputTypeDef",
     "GlueTableReferenceTypeDef",
-    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListCollaborationsInputRequestTypeDef",
-    "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
     "ListConfiguredTableAssociationsInputRequestTypeDef",
-    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
     "ListConfiguredTablesInputRequestTypeDef",
-    "ListMembersInputListMembersPaginateTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
-    "ListMembershipsInputListMembershipsPaginateTypeDef",
     "ListMembershipsInputRequestTypeDef",
     "MembershipSummaryTypeDef",
-    "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
     "ListProtectedQueriesInputRequestTypeDef",
     "ProtectedQuerySummaryTypeDef",
-    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListSchemasInputRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ProtectedQueryErrorTypeDef",
-    "ProtectedQueryS3OutputConfigurationOutputTypeDef",
     "ProtectedQueryS3OutputConfigurationTypeDef",
     "ProtectedQueryS3OutputTypeDef",
-    "ProtectedQuerySQLParametersOutputTypeDef",
     "ProtectedQuerySQLParametersTypeDef",
     "ProtectedQueryStatisticsTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
     "AnalysisRuleAggregationOutputTypeDef",
     "AnalysisRuleAggregationTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
     "GetConfiguredTableAssociationOutputTypeDef",
     "UpdateConfiguredTableAssociationOutputTypeDef",
     "ListConfiguredTablesOutputTypeDef",
     "CreateCollaborationInputRequestTypeDef",
     "CreateMembershipOutputTypeDef",
     "GetMembershipOutputTypeDef",
     "UpdateMembershipOutputTypeDef",
-    "TableReferenceOutputTypeDef",
     "TableReferenceTypeDef",
+    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+    "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
+    "ListMembersInputListMembersPaginateTypeDef",
+    "ListMembershipsInputListMembershipsPaginateTypeDef",
+    "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListMembersOutputTypeDef",
     "ListMembershipsOutputTypeDef",
     "ListProtectedQueriesOutputTypeDef",
     "ListSchemasOutputTypeDef",
-    "ProtectedQueryOutputConfigurationOutputTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
     "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     "CreateCollaborationOutputTypeDef",
     "GetCollaborationOutputTypeDef",
     "UpdateCollaborationOutputTypeDef",
     "BatchGetSchemaOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "ConfiguredTableTypeDef",
     "CreateConfiguredTableInputRequestTypeDef",
-    "ProtectedQueryResultConfigurationOutputTypeDef",
     "ProtectedQueryResultConfigurationTypeDef",
     "ProtectedQueryResultTypeDef",
     "AnalysisRulePolicyTypeDef",
     "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     "CreateConfiguredTableOutputTypeDef",
     "GetConfiguredTableOutputTypeDef",
@@ -181,23 +173,14 @@
     "AggregateColumnTypeDef",
     {
         "columnNames": Sequence[str],
         "function": AggregateFunctionNameType,
     },
 )
 
-AggregationConstraintOutputTypeDef = TypedDict(
-    "AggregationConstraintOutputTypeDef",
-    {
-        "columnName": str,
-        "minimum": int,
-        "type": Literal["COUNT_DISTINCT"],
-    },
-)
-
 AggregationConstraintTypeDef = TypedDict(
     "AggregationConstraintTypeDef",
     {
         "columnName": str,
         "minimum": int,
         "type": Literal["COUNT_DISTINCT"],
     },
@@ -254,14 +237,25 @@
     "BatchGetSchemaInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "names": Sequence[str],
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
 _RequiredCollaborationSummaryTypeDef = TypedDict(
     "_RequiredCollaborationSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "creatorAccountId": str,
@@ -281,16 +275,16 @@
 )
 
 class CollaborationSummaryTypeDef(
     _RequiredCollaborationSummaryTypeDef, _OptionalCollaborationSummaryTypeDef
 ):
     pass
 
-DataEncryptionMetadataOutputTypeDef = TypedDict(
-    "DataEncryptionMetadataOutputTypeDef",
+DataEncryptionMetadataTypeDef = TypedDict(
+    "DataEncryptionMetadataTypeDef",
     {
         "allowCleartext": bool,
         "allowDuplicates": bool,
         "allowJoinsOnColumnsWithDifferentNames": bool,
         "preserveNulls": bool,
     },
 )
@@ -354,24 +348,14 @@
         "createTime": datetime,
         "updateTime": datetime,
         "analysisRuleTypes": List[ConfiguredTableAnalysisRuleTypeType],
         "analysisMethod": Literal["DIRECT_QUERY"],
     },
 )
 
-DataEncryptionMetadataTypeDef = TypedDict(
-    "DataEncryptionMetadataTypeDef",
-    {
-        "allowCleartext": bool,
-        "allowDuplicates": bool,
-        "allowJoinsOnColumnsWithDifferentNames": bool,
-        "preserveNulls": bool,
-    },
-)
-
 MemberSpecificationTypeDef = TypedDict(
     "MemberSpecificationTypeDef",
     {
         "accountId": str,
         "memberAbilities": Sequence[MemberAbilityType],
         "displayName": str,
     },
@@ -542,69 +526,42 @@
     "GetSchemaInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "name": str,
     },
 )
 
-GlueTableReferenceOutputTypeDef = TypedDict(
-    "GlueTableReferenceOutputTypeDef",
-    {
-        "tableName": str,
-        "databaseName": str,
-    },
-)
-
 GlueTableReferenceTypeDef = TypedDict(
     "GlueTableReferenceTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
 
-ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
-    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "memberStatus": FilterableMemberStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListCollaborationsInputRequestTypeDef = TypedDict(
     "ListCollaborationsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "memberStatus": FilterableMemberStatusType,
     },
     total=False,
 )
 
-_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    {
-        "membershipIdentifier": str,
-    },
-)
-_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(
-    _RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-    _OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListConfiguredTableAssociationsInputRequestTypeDef = TypedDict(
     "_RequiredListConfiguredTableAssociationsInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalListConfiguredTableAssociationsInputRequestTypeDef = TypedDict(
@@ -618,51 +575,23 @@
 
 class ListConfiguredTableAssociationsInputRequestTypeDef(
     _RequiredListConfiguredTableAssociationsInputRequestTypeDef,
     _OptionalListConfiguredTableAssociationsInputRequestTypeDef,
 ):
     pass
 
-ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef = TypedDict(
-    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListConfiguredTablesInputRequestTypeDef = TypedDict(
     "ListConfiguredTablesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListMembersInputListMembersPaginateTypeDef = TypedDict(
-    "_RequiredListMembersInputListMembersPaginateTypeDef",
-    {
-        "collaborationIdentifier": str,
-    },
-)
-_OptionalListMembersInputListMembersPaginateTypeDef = TypedDict(
-    "_OptionalListMembersInputListMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMembersInputListMembersPaginateTypeDef(
-    _RequiredListMembersInputListMembersPaginateTypeDef,
-    _OptionalListMembersInputListMembersPaginateTypeDef,
-):
-    pass
-
 _RequiredListMembersInputRequestTypeDef = TypedDict(
     "_RequiredListMembersInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalListMembersInputRequestTypeDef = TypedDict(
@@ -698,23 +627,14 @@
     },
     total=False,
 )
 
 class MemberSummaryTypeDef(_RequiredMemberSummaryTypeDef, _OptionalMemberSummaryTypeDef):
     pass
 
-ListMembershipsInputListMembershipsPaginateTypeDef = TypedDict(
-    "ListMembershipsInputListMembershipsPaginateTypeDef",
-    {
-        "status": MembershipStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMembershipsInputRequestTypeDef = TypedDict(
     "ListMembershipsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": MembershipStatusType,
     },
@@ -734,35 +654,14 @@
         "createTime": datetime,
         "updateTime": datetime,
         "status": MembershipStatusType,
         "memberAbilities": List[MemberAbilityType],
     },
 )
 
-_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
-    "_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    {
-        "membershipIdentifier": str,
-    },
-)
-_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
-    "_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    {
-        "status": ProtectedQueryStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(
-    _RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-    _OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-):
-    pass
-
 _RequiredListProtectedQueriesInputRequestTypeDef = TypedDict(
     "_RequiredListProtectedQueriesInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalListProtectedQueriesInputRequestTypeDef = TypedDict(
@@ -788,35 +687,14 @@
         "membershipId": str,
         "membershipArn": str,
         "createTime": datetime,
         "status": ProtectedQueryStatusType,
     },
 )
 
-_RequiredListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "collaborationIdentifier": str,
-    },
-)
-_OptionalListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "schemaType": Literal["TABLE"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSchemasInputListSchemasPaginateTypeDef(
-    _RequiredListSchemasInputListSchemasPaginateTypeDef,
-    _OptionalListSchemasInputListSchemasPaginateTypeDef,
-):
-    pass
-
 _RequiredListSchemasInputRequestTypeDef = TypedDict(
     "_RequiredListSchemasInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalListSchemasInputRequestTypeDef = TypedDict(
@@ -861,61 +739,22 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": Dict[str, str],
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
 ProtectedQueryErrorTypeDef = TypedDict(
     "ProtectedQueryErrorTypeDef",
     {
         "message": str,
         "code": str,
     },
 )
 
-_RequiredProtectedQueryS3OutputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredProtectedQueryS3OutputConfigurationOutputTypeDef",
-    {
-        "resultFormat": ResultFormatType,
-        "bucket": str,
-    },
-)
-_OptionalProtectedQueryS3OutputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalProtectedQueryS3OutputConfigurationOutputTypeDef",
-    {
-        "keyPrefix": str,
-    },
-    total=False,
-)
-
-class ProtectedQueryS3OutputConfigurationOutputTypeDef(
-    _RequiredProtectedQueryS3OutputConfigurationOutputTypeDef,
-    _OptionalProtectedQueryS3OutputConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredProtectedQueryS3OutputConfigurationTypeDef = TypedDict(
     "_RequiredProtectedQueryS3OutputConfigurationTypeDef",
     {
         "resultFormat": ResultFormatType,
         "bucket": str,
     },
 )
@@ -936,22 +775,14 @@
 ProtectedQueryS3OutputTypeDef = TypedDict(
     "ProtectedQueryS3OutputTypeDef",
     {
         "location": str,
     },
 )
 
-ProtectedQuerySQLParametersOutputTypeDef = TypedDict(
-    "ProtectedQuerySQLParametersOutputTypeDef",
-    {
-        "queryString": str,
-    },
-    total=False,
-)
-
 ProtectedQuerySQLParametersTypeDef = TypedDict(
     "ProtectedQuerySQLParametersTypeDef",
     {
         "queryString": str,
     },
     total=False,
 )
@@ -960,25 +791,14 @@
     "ProtectedQueryStatisticsTypeDef",
     {
         "totalDurationInMillis": int,
     },
     total=False,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1085,15 +905,15 @@
 _RequiredAnalysisRuleAggregationOutputTypeDef = TypedDict(
     "_RequiredAnalysisRuleAggregationOutputTypeDef",
     {
         "aggregateColumns": List[AggregateColumnOutputTypeDef],
         "joinColumns": List[str],
         "dimensionColumns": List[str],
         "scalarFunctions": List[ScalarFunctionsType],
-        "outputConstraints": List[AggregationConstraintOutputTypeDef],
+        "outputConstraints": List[AggregationConstraintTypeDef],
     },
 )
 _OptionalAnalysisRuleAggregationOutputTypeDef = TypedDict(
     "_OptionalAnalysisRuleAggregationOutputTypeDef",
     {
         "joinRequired": Literal["QUERY_RUNNER"],
         "allowedJoinOperators": List[JoinOperatorType],
@@ -1126,20 +946,28 @@
 )
 
 class AnalysisRuleAggregationTypeDef(
     _RequiredAnalysisRuleAggregationTypeDef, _OptionalAnalysisRuleAggregationTypeDef
 ):
     pass
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCollaborationsOutputTypeDef = TypedDict(
     "ListCollaborationsOutputTypeDef",
     {
         "nextToken": str,
         "collaborationList": List[CollaborationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCollaborationTypeDef = TypedDict(
     "_RequiredCollaborationTypeDef",
     {
         "id": str,
@@ -1155,15 +983,15 @@
 )
 _OptionalCollaborationTypeDef = TypedDict(
     "_OptionalCollaborationTypeDef",
     {
         "description": str,
         "membershipId": str,
         "membershipArn": str,
-        "dataEncryptionMetadata": DataEncryptionMetadataOutputTypeDef,
+        "dataEncryptionMetadata": DataEncryptionMetadataTypeDef,
     },
     total=False,
 )
 
 class CollaborationTypeDef(_RequiredCollaborationTypeDef, _OptionalCollaborationTypeDef):
     pass
 
@@ -1195,48 +1023,48 @@
     pass
 
 ListConfiguredTableAssociationsOutputTypeDef = TypedDict(
     "ListConfiguredTableAssociationsOutputTypeDef",
     {
         "configuredTableAssociationSummaries": List[ConfiguredTableAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConfiguredTableAssociationOutputTypeDef = TypedDict(
     "CreateConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConfiguredTableAssociationOutputTypeDef = TypedDict(
     "GetConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfiguredTableAssociationOutputTypeDef = TypedDict(
     "UpdateConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfiguredTablesOutputTypeDef = TypedDict(
     "ListConfiguredTablesOutputTypeDef",
     {
         "configuredTableSummaries": List[ConfiguredTableSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCollaborationInputRequestTypeDef = TypedDict(
     "_RequiredCreateCollaborationInputRequestTypeDef",
     {
         "members": Sequence[MemberSpecificationTypeDef],
@@ -1261,92 +1089,184 @@
 ):
     pass
 
 CreateMembershipOutputTypeDef = TypedDict(
     "CreateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMembershipOutputTypeDef = TypedDict(
     "GetMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMembershipOutputTypeDef = TypedDict(
     "UpdateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TableReferenceOutputTypeDef = TypedDict(
-    "TableReferenceOutputTypeDef",
+TableReferenceTypeDef = TypedDict(
+    "TableReferenceTypeDef",
     {
-        "glue": GlueTableReferenceOutputTypeDef,
+        "glue": GlueTableReferenceTypeDef,
     },
     total=False,
 )
 
-TableReferenceTypeDef = TypedDict(
-    "TableReferenceTypeDef",
+ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
+    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
     {
-        "glue": GlueTableReferenceTypeDef,
+        "memberStatus": FilterableMemberStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(
+    _RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+    _OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+):
+    pass
+
+ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef = TypedDict(
+    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMembersInputListMembersPaginateTypeDef = TypedDict(
+    "_RequiredListMembersInputListMembersPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListMembersInputListMembersPaginateTypeDef = TypedDict(
+    "_OptionalListMembersInputListMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMembersInputListMembersPaginateTypeDef(
+    _RequiredListMembersInputListMembersPaginateTypeDef,
+    _OptionalListMembersInputListMembersPaginateTypeDef,
+):
+    pass
+
+ListMembershipsInputListMembershipsPaginateTypeDef = TypedDict(
+    "ListMembershipsInputListMembershipsPaginateTypeDef",
+    {
+        "status": MembershipStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
+    "_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
+    "_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    {
+        "status": ProtectedQueryStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(
+    _RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+    _OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+):
+    pass
+
+_RequiredListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "schemaType": Literal["TABLE"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSchemasInputListSchemasPaginateTypeDef(
+    _RequiredListSchemasInputListSchemasPaginateTypeDef,
+    _OptionalListSchemasInputListSchemasPaginateTypeDef,
+):
+    pass
+
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "nextToken": str,
         "memberSummaries": List[MemberSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembershipsOutputTypeDef = TypedDict(
     "ListMembershipsOutputTypeDef",
     {
         "nextToken": str,
         "membershipSummaries": List[MembershipSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtectedQueriesOutputTypeDef = TypedDict(
     "ListProtectedQueriesOutputTypeDef",
     {
         "nextToken": str,
         "protectedQueries": List[ProtectedQuerySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemasOutputTypeDef = TypedDict(
     "ListSchemasOutputTypeDef",
     {
         "schemaSummaries": List[SchemaSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ProtectedQueryOutputConfigurationOutputTypeDef = TypedDict(
-    "ProtectedQueryOutputConfigurationOutputTypeDef",
-    {
-        "s3": ProtectedQueryS3OutputConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ProtectedQueryOutputConfigurationTypeDef = TypedDict(
     "ProtectedQueryOutputConfigurationTypeDef",
     {
         "s3": ProtectedQueryS3OutputConfigurationTypeDef,
     },
@@ -1388,58 +1308,58 @@
     total=False,
 )
 
 CreateCollaborationOutputTypeDef = TypedDict(
     "CreateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCollaborationOutputTypeDef = TypedDict(
     "GetCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCollaborationOutputTypeDef = TypedDict(
     "UpdateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetSchemaOutputTypeDef = TypedDict(
     "BatchGetSchemaOutputTypeDef",
     {
         "schemas": List[SchemaTypeDef],
         "errors": List[BatchGetSchemaErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSchemaOutputTypeDef = TypedDict(
     "GetSchemaOutputTypeDef",
     {
         "schema": SchemaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConfiguredTableTypeDef = TypedDict(
     "_RequiredConfiguredTableTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
-        "tableReference": TableReferenceOutputTypeDef,
+        "tableReference": TableReferenceTypeDef,
         "createTime": datetime,
         "updateTime": datetime,
         "analysisRuleTypes": List[ConfiguredTableAnalysisRuleTypeType],
         "analysisMethod": Literal["DIRECT_QUERY"],
         "allowedColumns": List[str],
     },
 )
@@ -1474,21 +1394,14 @@
 
 class CreateConfiguredTableInputRequestTypeDef(
     _RequiredCreateConfiguredTableInputRequestTypeDef,
     _OptionalCreateConfiguredTableInputRequestTypeDef,
 ):
     pass
 
-ProtectedQueryResultConfigurationOutputTypeDef = TypedDict(
-    "ProtectedQueryResultConfigurationOutputTypeDef",
-    {
-        "outputConfiguration": ProtectedQueryOutputConfigurationOutputTypeDef,
-    },
-)
-
 ProtectedQueryResultConfigurationTypeDef = TypedDict(
     "ProtectedQueryResultConfigurationTypeDef",
     {
         "outputConfiguration": ProtectedQueryOutputConfigurationTypeDef,
     },
 )
 
@@ -1523,31 +1436,31 @@
     total=False,
 )
 
 CreateConfiguredTableOutputTypeDef = TypedDict(
     "CreateConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConfiguredTableOutputTypeDef = TypedDict(
     "GetConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfiguredTableOutputTypeDef = TypedDict(
     "UpdateConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartProtectedQueryInputRequestTypeDef = TypedDict(
     "StartProtectedQueryInputRequestTypeDef",
     {
         "type": Literal["SQL"],
@@ -1560,17 +1473,17 @@
 _RequiredProtectedQueryTypeDef = TypedDict(
     "_RequiredProtectedQueryTypeDef",
     {
         "id": str,
         "membershipId": str,
         "membershipArn": str,
         "createTime": datetime,
-        "sqlParameters": ProtectedQuerySQLParametersOutputTypeDef,
+        "sqlParameters": ProtectedQuerySQLParametersTypeDef,
         "status": ProtectedQueryStatusType,
-        "resultConfiguration": ProtectedQueryResultConfigurationOutputTypeDef,
+        "resultConfiguration": ProtectedQueryResultConfigurationTypeDef,
     },
 )
 _OptionalProtectedQueryTypeDef = TypedDict(
     "_OptionalProtectedQueryTypeDef",
     {
         "statistics": ProtectedQueryStatisticsTypeDef,
         "result": ProtectedQueryResultTypeDef,
@@ -1624,58 +1537,58 @@
     },
 )
 
 GetProtectedQueryOutputTypeDef = TypedDict(
     "GetProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartProtectedQueryOutputTypeDef = TypedDict(
     "StartProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProtectedQueryOutputTypeDef = TypedDict(
     "UpdateProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSchemaAnalysisRuleOutputTypeDef = TypedDict(
     "GetSchemaAnalysisRuleOutputTypeDef",
     {
         "analysisRule": AnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "CreateConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "GetConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "UpdateConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/PKG-INFO` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cleanrooms
-Version: 1.28.12
-Summary: Type annotations for boto3.CleanRoomsService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CleanRoomsService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cleanrooms.svg?color=blue)](https://pypi.org/project/mypy-boto3-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cleanrooms)](https://pepy.tech/project/mypy-boto3-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CleanRoomsService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[boto3.CleanRoomsService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [mypy-boto3-cleanrooms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,27 +368,26 @@
 `mypy_boto3_cleanrooms.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cleanrooms.type_defs import (
     AggregateColumnOutputTypeDef,
     AggregateColumnTypeDef,
-    AggregationConstraintOutputTypeDef,
     AggregationConstraintTypeDef,
     AnalysisRuleListOutputTypeDef,
     AnalysisRuleListTypeDef,
     BatchGetSchemaErrorTypeDef,
     BatchGetSchemaInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     CollaborationSummaryTypeDef,
-    DataEncryptionMetadataOutputTypeDef,
+    DataEncryptionMetadataTypeDef,
     ColumnTypeDef,
     ConfiguredTableAssociationSummaryTypeDef,
     ConfiguredTableAssociationTypeDef,
     ConfiguredTableSummaryTypeDef,
-    DataEncryptionMetadataTypeDef,
     MemberSpecificationTypeDef,
     CreateConfiguredTableAssociationInputRequestTypeDef,
     CreateMembershipInputRequestTypeDef,
     MembershipTypeDef,
     DeleteCollaborationInputRequestTypeDef,
     DeleteConfiguredTableAnalysisRuleInputRequestTypeDef,
     DeleteConfiguredTableAssociationInputRequestTypeDef,
@@ -399,86 +398,79 @@
     GetConfiguredTableAnalysisRuleInputRequestTypeDef,
     GetConfiguredTableAssociationInputRequestTypeDef,
     GetConfiguredTableInputRequestTypeDef,
     GetMembershipInputRequestTypeDef,
     GetProtectedQueryInputRequestTypeDef,
     GetSchemaAnalysisRuleInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
-    GlueTableReferenceOutputTypeDef,
     GlueTableReferenceTypeDef,
-    ListCollaborationsInputListCollaborationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCollaborationsInputRequestTypeDef,
-    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
     ListConfiguredTableAssociationsInputRequestTypeDef,
-    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
     ListConfiguredTablesInputRequestTypeDef,
-    ListMembersInputListMembersPaginateTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
-    ListMembershipsInputListMembershipsPaginateTypeDef,
     ListMembershipsInputRequestTypeDef,
     MembershipSummaryTypeDef,
-    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
     ListProtectedQueriesInputRequestTypeDef,
     ProtectedQuerySummaryTypeDef,
-    ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
     ProtectedQueryErrorTypeDef,
-    ProtectedQueryS3OutputConfigurationOutputTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
-    ProtectedQuerySQLParametersOutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
     AnalysisRuleAggregationOutputTypeDef,
     AnalysisRuleAggregationTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     CreateCollaborationInputRequestTypeDef,
     CreateMembershipOutputTypeDef,
     GetMembershipOutputTypeDef,
     UpdateMembershipOutputTypeDef,
-    TableReferenceOutputTypeDef,
     TableReferenceTypeDef,
+    ListCollaborationsInputListCollaborationsPaginateTypeDef,
+    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
+    ListMembersInputListMembersPaginateTypeDef,
+    ListMembershipsInputListMembershipsPaginateTypeDef,
+    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+    ListSchemasInputListSchemasPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
-    ProtectedQueryOutputConfigurationOutputTypeDef,
     ProtectedQueryOutputConfigurationTypeDef,
     ProtectedQueryOutputTypeDef,
     AnalysisRulePolicyV1TypeDef,
     ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
     ConfiguredTableAnalysisRulePolicyV1TypeDef,
     CreateCollaborationOutputTypeDef,
     GetCollaborationOutputTypeDef,
     UpdateCollaborationOutputTypeDef,
     BatchGetSchemaOutputTypeDef,
     GetSchemaOutputTypeDef,
     ConfiguredTableTypeDef,
     CreateConfiguredTableInputRequestTypeDef,
-    ProtectedQueryResultConfigurationOutputTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQueryResultTypeDef,
     AnalysisRulePolicyTypeDef,
     ConfiguredTableAnalysisRulePolicyOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateConfiguredTableOutputTypeDef,
     GetConfiguredTableOutputTypeDef,
```

### Comparing `mypy-boto3-cleanrooms-1.28.12/mypy_boto3_cleanrooms.egg-info/SOURCES.txt` & `mypy-boto3-cleanrooms-1.28.15/mypy_boto3_cleanrooms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cleanrooms-1.28.12/setup.py` & `mypy-boto3-cleanrooms-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cleanrooms",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cleanrooms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CleanRoomsService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CleanRoomsService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

