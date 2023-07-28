# Comparing `tmp/mypy-boto3-lex-models-1.28.12.tar.gz` & `tmp/mypy-boto3-lex-models-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lex-models-1.28.12.tar", last modified: Thu Jul 27 05:34:55 2023, max compression
+gzip compressed data, was "mypy-boto3-lex-models-1.28.15.tar", last modified: Fri Jul 28 20:43:08 2023, max compression
```

## Comparing `mypy-boto3-lex-models-1.28.12.tar` & `mypy-boto3-lex-models-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.716460 mypy-boto3-lex-models-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-07-27 05:34:55.716460 mypy-boto3-lex-models-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18272 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.716460 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35106 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35047 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11225 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51752 2023-07-27 05:25:00.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51686 2023-07-27 05:25:00.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.716460 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-07-27 05:34:55.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:55.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:55.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:55.000000 mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:55.716460 mypy-boto3-lex-models-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 05:24:59.000000 mypy-boto3-lex-models-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.621383 mypy-boto3-lex-models-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19425 2023-07-28 20:43:08.621383 mypy-boto3-lex-models-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.621383 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35106 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35047 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11225 2023-07-28 20:29:40.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-07-28 20:29:40.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48627 2023-07-28 20:29:43.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48567 2023-07-28 20:29:40.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.621383 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19425 2023-07-28 20:43:08.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:43:08.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:08.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:43:08.000000 mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:08.621383 mypy-boto3-lex-models-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 20:29:39.000000 mypy-boto3-lex-models-1.28.15/setup.py
```

### Comparing `mypy-boto3-lex-models-1.28.12/LICENSE` & `mypy-boto3-lex-models-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.12/PKG-INFO` & `mypy-boto3-lex-models-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-models
-Version: 1.28.12
-Summary: Type annotations for boto3.LexModelBuildingService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LexModelBuildingService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-models)](https://pepy.tech/project/mypy-boto3-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelBuildingService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[boto3.LexModelBuildingService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -386,121 +386,110 @@
 ```python
 from mypy_boto3_lex_models.type_defs import (
     BotChannelAssociationTypeDef,
     BotMetadataTypeDef,
     BuiltinIntentMetadataTypeDef,
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
-    CodeHookOutputTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
     LogSettingsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
-    IntentOutputTypeDef,
+    IntentTypeDef,
+    ResponseMetadataTypeDef,
     CreateIntentVersionRequestRequestTypeDef,
-    InputContextOutputTypeDef,
-    KendraConfigurationOutputTypeDef,
-    OutputContextOutputTypeDef,
+    InputContextTypeDef,
+    KendraConfigurationTypeDef,
+    OutputContextTypeDef,
     CreateSlotTypeVersionRequestRequestTypeDef,
     EnumerationValueOutputTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
     DeleteBotChannelAssociationRequestRequestTypeDef,
     DeleteBotRequestRequestTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteIntentVersionRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteSlotTypeVersionRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnumerationValueTypeDef,
     GetBotAliasRequestRequestTypeDef,
-    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetBotAliasesRequestRequestTypeDef,
     GetBotChannelAssociationRequestRequestTypeDef,
-    GetBotChannelAssociationResponseTypeDef,
-    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotChannelAssociationsRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
-    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     GetBotVersionsRequestRequestTypeDef,
-    GetBotsRequestGetBotsPaginateTypeDef,
     GetBotsRequestRequestTypeDef,
     GetBuiltinIntentRequestRequestTypeDef,
-    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
     GetBuiltinIntentsRequestRequestTypeDef,
-    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
     GetBuiltinSlotTypesRequestRequestTypeDef,
     GetExportRequestRequestTypeDef,
-    GetExportResponseTypeDef,
     GetImportRequestRequestTypeDef,
-    GetImportResponseTypeDef,
     GetIntentRequestRequestTypeDef,
-    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
     GetIntentVersionsRequestRequestTypeDef,
     IntentMetadataTypeDef,
-    GetIntentsRequestGetIntentsPaginateTypeDef,
     GetIntentsRequestRequestTypeDef,
     GetMigrationRequestRequestTypeDef,
     MigrationAlertTypeDef,
     GetMigrationsRequestRequestTypeDef,
     MigrationSummaryTypeDef,
     GetSlotTypeRequestRequestTypeDef,
-    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     GetSlotTypeVersionsRequestRequestTypeDef,
     SlotTypeMetadataTypeDef,
-    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetSlotTypesRequestRequestTypeDef,
     GetUtterancesViewRequestRequestTypeDef,
-    InputContextTypeDef,
-    IntentTypeDef,
-    KendraConfigurationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    MessageOutputTypeDef,
-    MessageTypeDef,
-    OutputContextTypeDef,
-    PaginatorConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
-    SlotDefaultValueOutputTypeDef,
+    MessageTypeDef,
     SlotDefaultValueTypeDef,
-    SlotTypeRegexConfigurationOutputTypeDef,
     SlotTypeRegexConfigurationTypeDef,
     StartMigrationRequestRequestTypeDef,
-    StartMigrationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UtteranceDataTypeDef,
+    FulfillmentActivityTypeDef,
+    ConversationLogsRequestTypeDef,
+    ConversationLogsResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotVersionsResponseTypeDef,
     GetBotsResponseTypeDef,
-    GetBuiltinIntentsResponseTypeDef,
     GetBuiltinIntentResponseTypeDef,
+    GetBuiltinIntentsResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
-    FulfillmentActivityOutputTypeDef,
-    FulfillmentActivityTypeDef,
-    ConversationLogsRequestTypeDef,
-    ConversationLogsResponseTypeDef,
+    GetExportResponseTypeDef,
+    GetImportResponseTypeDef,
+    StartMigrationResponseTypeDef,
+    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+    GetBotsRequestGetBotsPaginateTypeDef,
+    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
+    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
+    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+    GetIntentsRequestGetIntentsPaginateTypeDef,
+    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetIntentVersionsResponseTypeDef,
     GetIntentsResponseTypeDef,
     GetMigrationResponseTypeDef,
     GetMigrationsResponseTypeDef,
     GetSlotTypeVersionsResponseTypeDef,
     GetSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     PromptOutputTypeDef,
-    StatementOutputTypeDef,
     PromptTypeDef,
+    StatementOutputTypeDef,
     StatementTypeDef,
-    StartImportRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     SlotDefaultValueSpecOutputTypeDef,
     SlotDefaultValueSpecTypeDef,
-    SlotTypeConfigurationOutputTypeDef,
     SlotTypeConfigurationTypeDef,
     UtteranceListTypeDef,
     PutBotAliasRequestRequestTypeDef,
     BotAliasMetadataTypeDef,
     GetBotAliasResponseTypeDef,
     PutBotAliasResponseTypeDef,
     CreateBotVersionResponseTypeDef,
@@ -509,16 +498,16 @@
     PutBotResponseTypeDef,
     FollowUpPromptTypeDef,
     PutBotRequestRequestTypeDef,
     SlotOutputTypeDef,
     SlotTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     GetSlotTypeResponseTypeDef,
-    PutSlotTypeResponseTypeDef,
     PutSlotTypeRequestRequestTypeDef,
+    PutSlotTypeResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     GetBotAliasesResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     GetIntentResponseTypeDef,
     PutIntentResponseTypeDef,
     PutIntentRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-lex-models-1.28.12/README.md` & `mypy-boto3-lex-models-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-models)](https://pepy.tech/project/mypy-boto3-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelBuildingService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[boto3.LexModelBuildingService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,121 +354,110 @@
 ```python
 from mypy_boto3_lex_models.type_defs import (
     BotChannelAssociationTypeDef,
     BotMetadataTypeDef,
     BuiltinIntentMetadataTypeDef,
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
-    CodeHookOutputTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
     LogSettingsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
-    IntentOutputTypeDef,
+    IntentTypeDef,
+    ResponseMetadataTypeDef,
     CreateIntentVersionRequestRequestTypeDef,
-    InputContextOutputTypeDef,
-    KendraConfigurationOutputTypeDef,
-    OutputContextOutputTypeDef,
+    InputContextTypeDef,
+    KendraConfigurationTypeDef,
+    OutputContextTypeDef,
     CreateSlotTypeVersionRequestRequestTypeDef,
     EnumerationValueOutputTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
     DeleteBotChannelAssociationRequestRequestTypeDef,
     DeleteBotRequestRequestTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteIntentVersionRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteSlotTypeVersionRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnumerationValueTypeDef,
     GetBotAliasRequestRequestTypeDef,
-    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetBotAliasesRequestRequestTypeDef,
     GetBotChannelAssociationRequestRequestTypeDef,
-    GetBotChannelAssociationResponseTypeDef,
-    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotChannelAssociationsRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
-    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     GetBotVersionsRequestRequestTypeDef,
-    GetBotsRequestGetBotsPaginateTypeDef,
     GetBotsRequestRequestTypeDef,
     GetBuiltinIntentRequestRequestTypeDef,
-    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
     GetBuiltinIntentsRequestRequestTypeDef,
-    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
     GetBuiltinSlotTypesRequestRequestTypeDef,
     GetExportRequestRequestTypeDef,
-    GetExportResponseTypeDef,
     GetImportRequestRequestTypeDef,
-    GetImportResponseTypeDef,
     GetIntentRequestRequestTypeDef,
-    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
     GetIntentVersionsRequestRequestTypeDef,
     IntentMetadataTypeDef,
-    GetIntentsRequestGetIntentsPaginateTypeDef,
     GetIntentsRequestRequestTypeDef,
     GetMigrationRequestRequestTypeDef,
     MigrationAlertTypeDef,
     GetMigrationsRequestRequestTypeDef,
     MigrationSummaryTypeDef,
     GetSlotTypeRequestRequestTypeDef,
-    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     GetSlotTypeVersionsRequestRequestTypeDef,
     SlotTypeMetadataTypeDef,
-    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetSlotTypesRequestRequestTypeDef,
     GetUtterancesViewRequestRequestTypeDef,
-    InputContextTypeDef,
-    IntentTypeDef,
-    KendraConfigurationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    MessageOutputTypeDef,
-    MessageTypeDef,
-    OutputContextTypeDef,
-    PaginatorConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
-    SlotDefaultValueOutputTypeDef,
+    MessageTypeDef,
     SlotDefaultValueTypeDef,
-    SlotTypeRegexConfigurationOutputTypeDef,
     SlotTypeRegexConfigurationTypeDef,
     StartMigrationRequestRequestTypeDef,
-    StartMigrationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UtteranceDataTypeDef,
+    FulfillmentActivityTypeDef,
+    ConversationLogsRequestTypeDef,
+    ConversationLogsResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotVersionsResponseTypeDef,
     GetBotsResponseTypeDef,
-    GetBuiltinIntentsResponseTypeDef,
     GetBuiltinIntentResponseTypeDef,
+    GetBuiltinIntentsResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
-    FulfillmentActivityOutputTypeDef,
-    FulfillmentActivityTypeDef,
-    ConversationLogsRequestTypeDef,
-    ConversationLogsResponseTypeDef,
+    GetExportResponseTypeDef,
+    GetImportResponseTypeDef,
+    StartMigrationResponseTypeDef,
+    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+    GetBotsRequestGetBotsPaginateTypeDef,
+    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
+    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
+    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+    GetIntentsRequestGetIntentsPaginateTypeDef,
+    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetIntentVersionsResponseTypeDef,
     GetIntentsResponseTypeDef,
     GetMigrationResponseTypeDef,
     GetMigrationsResponseTypeDef,
     GetSlotTypeVersionsResponseTypeDef,
     GetSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     PromptOutputTypeDef,
-    StatementOutputTypeDef,
     PromptTypeDef,
+    StatementOutputTypeDef,
     StatementTypeDef,
-    StartImportRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     SlotDefaultValueSpecOutputTypeDef,
     SlotDefaultValueSpecTypeDef,
-    SlotTypeConfigurationOutputTypeDef,
     SlotTypeConfigurationTypeDef,
     UtteranceListTypeDef,
     PutBotAliasRequestRequestTypeDef,
     BotAliasMetadataTypeDef,
     GetBotAliasResponseTypeDef,
     PutBotAliasResponseTypeDef,
     CreateBotVersionResponseTypeDef,
@@ -477,16 +466,16 @@
     PutBotResponseTypeDef,
     FollowUpPromptTypeDef,
     PutBotRequestRequestTypeDef,
     SlotOutputTypeDef,
     SlotTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     GetSlotTypeResponseTypeDef,
-    PutSlotTypeResponseTypeDef,
     PutSlotTypeRequestRequestTypeDef,
+    PutSlotTypeResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     GetBotAliasesResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     GetIntentResponseTypeDef,
     PutIntentResponseTypeDef,
     PutIntentRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/__init__.py` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/__init__.pyi` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/__main__.py` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexModelBuildingService 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.LexModelBuildingService 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService\nOther"
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

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/client.py` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/client.pyi` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/literals.py` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/literals.pyi` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/paginator.py` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     """
 
     def paginate(
         self,
         *,
         botName: str,
         nameContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBotAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotaliasespaginator)
         """
 
 
@@ -107,45 +107,45 @@
 
     def paginate(
         self,
         *,
         botName: str,
         botAlias: str,
         nameContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBotChannelAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotchannelassociationspaginator)
         """
 
 
 class GetBotVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBotVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotversionspaginator)
         """
 
 
 class GetBotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotspaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotspaginator)
         """
 
 
@@ -156,15 +156,15 @@
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBuiltinIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbuiltinintentspaginator)
         """
 
 
@@ -175,73 +175,73 @@
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBuiltinSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbuiltinslottypespaginator)
         """
 
 
 class GetIntentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetIntentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentversionspaginator)
         """
 
 
 class GetIntentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentspaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentspaginator)
         """
 
 
 class GetSlotTypeVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypeversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetSlotTypeVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypeversionspaginator)
         """
 
 
 class GetSlotTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypespaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypespaginator)
         """
```

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/paginator.pyi` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     """
 
     def paginate(
         self,
         *,
         botName: str,
         nameContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBotAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotaliasespaginator)
         """
 
 class GetBotChannelAssociationsPaginator(Paginator):
@@ -103,43 +103,43 @@
 
     def paginate(
         self,
         *,
         botName: str,
         botAlias: str,
         nameContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBotChannelAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotchannelassociationspaginator)
         """
 
 class GetBotVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBotVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotversionspaginator)
         """
 
 class GetBotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotspaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbotspaginator)
         """
 
 class GetBuiltinIntentsPaginator(Paginator):
@@ -149,15 +149,15 @@
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBuiltinIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbuiltinintentspaginator)
         """
 
 class GetBuiltinSlotTypesPaginator(Paginator):
@@ -167,69 +167,69 @@
     """
 
     def paginate(
         self,
         *,
         locale: LocaleType = ...,
         signatureContains: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBuiltinSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getbuiltinslottypespaginator)
         """
 
 class GetIntentVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetIntentVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentversionspaginator)
         """
 
 class GetIntentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentspaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetIntentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getintentspaginator)
         """
 
 class GetSlotTypeVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypeversionspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetSlotTypeVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypeversionspaginator)
         """
 
 class GetSlotTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypespaginator)
     """
 
     def paginate(
-        self, *, nameContains: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, nameContains: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetSlotTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/paginators/#getslottypespaginator)
         """
```

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/type_defs.py` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -44,128 +44,116 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BotChannelAssociationTypeDef",
     "BotMetadataTypeDef",
     "BuiltinIntentMetadataTypeDef",
     "BuiltinIntentSlotTypeDef",
     "BuiltinSlotTypeMetadataTypeDef",
-    "CodeHookOutputTypeDef",
     "CodeHookTypeDef",
     "LogSettingsRequestTypeDef",
     "LogSettingsResponseTypeDef",
     "CreateBotVersionRequestRequestTypeDef",
-    "IntentOutputTypeDef",
+    "IntentTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateIntentVersionRequestRequestTypeDef",
-    "InputContextOutputTypeDef",
-    "KendraConfigurationOutputTypeDef",
-    "OutputContextOutputTypeDef",
+    "InputContextTypeDef",
+    "KendraConfigurationTypeDef",
+    "OutputContextTypeDef",
     "CreateSlotTypeVersionRequestRequestTypeDef",
     "EnumerationValueOutputTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
     "DeleteBotChannelAssociationRequestRequestTypeDef",
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteIntentVersionRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteSlotTypeVersionRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnumerationValueTypeDef",
     "GetBotAliasRequestRequestTypeDef",
-    "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetBotAliasesRequestRequestTypeDef",
     "GetBotChannelAssociationRequestRequestTypeDef",
-    "GetBotChannelAssociationResponseTypeDef",
-    "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     "GetBotChannelAssociationsRequestRequestTypeDef",
     "GetBotRequestRequestTypeDef",
-    "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     "GetBotVersionsRequestRequestTypeDef",
-    "GetBotsRequestGetBotsPaginateTypeDef",
     "GetBotsRequestRequestTypeDef",
     "GetBuiltinIntentRequestRequestTypeDef",
-    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     "GetBuiltinIntentsRequestRequestTypeDef",
-    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
     "GetBuiltinSlotTypesRequestRequestTypeDef",
     "GetExportRequestRequestTypeDef",
-    "GetExportResponseTypeDef",
     "GetImportRequestRequestTypeDef",
-    "GetImportResponseTypeDef",
     "GetIntentRequestRequestTypeDef",
-    "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
     "GetIntentVersionsRequestRequestTypeDef",
     "IntentMetadataTypeDef",
-    "GetIntentsRequestGetIntentsPaginateTypeDef",
     "GetIntentsRequestRequestTypeDef",
     "GetMigrationRequestRequestTypeDef",
     "MigrationAlertTypeDef",
     "GetMigrationsRequestRequestTypeDef",
     "MigrationSummaryTypeDef",
     "GetSlotTypeRequestRequestTypeDef",
-    "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     "GetSlotTypeVersionsRequestRequestTypeDef",
     "SlotTypeMetadataTypeDef",
-    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     "GetSlotTypesRequestRequestTypeDef",
     "GetUtterancesViewRequestRequestTypeDef",
-    "InputContextTypeDef",
-    "IntentTypeDef",
-    "KendraConfigurationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "MessageOutputTypeDef",
-    "MessageTypeDef",
-    "OutputContextTypeDef",
-    "PaginatorConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
-    "SlotDefaultValueOutputTypeDef",
+    "MessageTypeDef",
     "SlotDefaultValueTypeDef",
-    "SlotTypeRegexConfigurationOutputTypeDef",
     "SlotTypeRegexConfigurationTypeDef",
     "StartMigrationRequestRequestTypeDef",
-    "StartMigrationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UtteranceDataTypeDef",
+    "FulfillmentActivityTypeDef",
+    "ConversationLogsRequestTypeDef",
+    "ConversationLogsResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetBotChannelAssociationResponseTypeDef",
     "GetBotChannelAssociationsResponseTypeDef",
     "GetBotVersionsResponseTypeDef",
     "GetBotsResponseTypeDef",
-    "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinIntentResponseTypeDef",
+    "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinSlotTypesResponseTypeDef",
-    "FulfillmentActivityOutputTypeDef",
-    "FulfillmentActivityTypeDef",
-    "ConversationLogsRequestTypeDef",
-    "ConversationLogsResponseTypeDef",
+    "GetExportResponseTypeDef",
+    "GetImportResponseTypeDef",
+    "StartMigrationResponseTypeDef",
+    "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
+    "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    "GetBotsRequestGetBotsPaginateTypeDef",
+    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
+    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
+    "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+    "GetIntentsRequestGetIntentsPaginateTypeDef",
+    "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     "GetIntentVersionsResponseTypeDef",
     "GetIntentsResponseTypeDef",
     "GetMigrationResponseTypeDef",
     "GetMigrationsResponseTypeDef",
     "GetSlotTypeVersionsResponseTypeDef",
     "GetSlotTypesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "PromptOutputTypeDef",
-    "StatementOutputTypeDef",
     "PromptTypeDef",
+    "StatementOutputTypeDef",
     "StatementTypeDef",
-    "StartImportRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "SlotDefaultValueSpecOutputTypeDef",
     "SlotDefaultValueSpecTypeDef",
-    "SlotTypeConfigurationOutputTypeDef",
     "SlotTypeConfigurationTypeDef",
     "UtteranceListTypeDef",
     "PutBotAliasRequestRequestTypeDef",
     "BotAliasMetadataTypeDef",
     "GetBotAliasResponseTypeDef",
     "PutBotAliasResponseTypeDef",
     "CreateBotVersionResponseTypeDef",
@@ -174,16 +162,16 @@
     "PutBotResponseTypeDef",
     "FollowUpPromptTypeDef",
     "PutBotRequestRequestTypeDef",
     "SlotOutputTypeDef",
     "SlotTypeDef",
     "CreateSlotTypeVersionResponseTypeDef",
     "GetSlotTypeResponseTypeDef",
-    "PutSlotTypeResponseTypeDef",
     "PutSlotTypeRequestRequestTypeDef",
+    "PutSlotTypeResponseTypeDef",
     "GetUtterancesViewResponseTypeDef",
     "GetBotAliasesResponseTypeDef",
     "CreateIntentVersionResponseTypeDef",
     "GetIntentResponseTypeDef",
     "PutIntentResponseTypeDef",
     "PutIntentRequestRequestTypeDef",
 )
@@ -239,22 +227,14 @@
     {
         "signature": str,
         "supportedLocales": List[LocaleType],
     },
     total=False,
 )
 
-CodeHookOutputTypeDef = TypedDict(
-    "CodeHookOutputTypeDef",
-    {
-        "uri": str,
-        "messageVersion": str,
-    },
-)
-
 CodeHookTypeDef = TypedDict(
     "CodeHookTypeDef",
     {
         "uri": str,
         "messageVersion": str,
     },
 )
@@ -271,21 +251,19 @@
     "_OptionalLogSettingsRequestTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-
 class LogSettingsRequestTypeDef(
     _RequiredLogSettingsRequestTypeDef, _OptionalLogSettingsRequestTypeDef
 ):
     pass
 
-
 LogSettingsResponseTypeDef = TypedDict(
     "LogSettingsResponseTypeDef",
     {
         "logType": LogTypeType,
         "destination": DestinationType,
         "kmsKeyArn": str,
         "resourceArn": str,
@@ -304,82 +282,87 @@
     "_OptionalCreateBotVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
-
 class CreateBotVersionRequestRequestTypeDef(
     _RequiredCreateBotVersionRequestRequestTypeDef, _OptionalCreateBotVersionRequestRequestTypeDef
 ):
     pass
 
-
-IntentOutputTypeDef = TypedDict(
-    "IntentOutputTypeDef",
+IntentTypeDef = TypedDict(
+    "IntentTypeDef",
     {
         "intentName": str,
         "intentVersion": str,
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
 _RequiredCreateIntentVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntentVersionRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateIntentVersionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateIntentVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
-
 class CreateIntentVersionRequestRequestTypeDef(
     _RequiredCreateIntentVersionRequestRequestTypeDef,
     _OptionalCreateIntentVersionRequestRequestTypeDef,
 ):
     pass
 
-
-InputContextOutputTypeDef = TypedDict(
-    "InputContextOutputTypeDef",
+InputContextTypeDef = TypedDict(
+    "InputContextTypeDef",
     {
         "name": str,
     },
 )
 
-_RequiredKendraConfigurationOutputTypeDef = TypedDict(
-    "_RequiredKendraConfigurationOutputTypeDef",
+_RequiredKendraConfigurationTypeDef = TypedDict(
+    "_RequiredKendraConfigurationTypeDef",
     {
         "kendraIndex": str,
         "role": str,
     },
 )
-_OptionalKendraConfigurationOutputTypeDef = TypedDict(
-    "_OptionalKendraConfigurationOutputTypeDef",
+_OptionalKendraConfigurationTypeDef = TypedDict(
+    "_OptionalKendraConfigurationTypeDef",
     {
         "queryFilterString": str,
     },
     total=False,
 )
 
-
-class KendraConfigurationOutputTypeDef(
-    _RequiredKendraConfigurationOutputTypeDef, _OptionalKendraConfigurationOutputTypeDef
+class KendraConfigurationTypeDef(
+    _RequiredKendraConfigurationTypeDef, _OptionalKendraConfigurationTypeDef
 ):
     pass
 
-
-OutputContextOutputTypeDef = TypedDict(
-    "OutputContextOutputTypeDef",
+OutputContextTypeDef = TypedDict(
+    "OutputContextTypeDef",
     {
         "name": str,
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
 )
 
@@ -393,43 +376,39 @@
     "_OptionalCreateSlotTypeVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
-
 class CreateSlotTypeVersionRequestRequestTypeDef(
     _RequiredCreateSlotTypeVersionRequestRequestTypeDef,
     _OptionalCreateSlotTypeVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredEnumerationValueOutputTypeDef = TypedDict(
     "_RequiredEnumerationValueOutputTypeDef",
     {
         "value": str,
     },
 )
 _OptionalEnumerationValueOutputTypeDef = TypedDict(
     "_OptionalEnumerationValueOutputTypeDef",
     {
         "synonyms": List[str],
     },
     total=False,
 )
 
-
 class EnumerationValueOutputTypeDef(
     _RequiredEnumerationValueOutputTypeDef, _OptionalEnumerationValueOutputTypeDef
 ):
     pass
 
-
 DeleteBotAliasRequestRequestTypeDef = TypedDict(
     "DeleteBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
@@ -492,71 +471,49 @@
     "DeleteUtterancesRequestRequestTypeDef",
     {
         "botName": str,
         "userId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnumerationValueTypeDef = TypedDict(
     "_RequiredEnumerationValueTypeDef",
     {
         "value": str,
     },
 )
 _OptionalEnumerationValueTypeDef = TypedDict(
     "_OptionalEnumerationValueTypeDef",
     {
         "synonyms": Sequence[str],
     },
     total=False,
 )
 
-
 class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
     pass
 
-
 GetBotAliasRequestRequestTypeDef = TypedDict(
     "GetBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
 
-_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
-    "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
-    {
-        "botName": str,
-    },
-)
-_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
-    "_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
-    _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-    _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetBotAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotAliasesRequestRequestTypeDef",
     {
         "botName": str,
     },
 )
 _OptionalGetBotAliasesRequestRequestTypeDef = TypedDict(
@@ -565,70 +522,28 @@
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
     total=False,
 )
 
-
 class GetBotAliasesRequestRequestTypeDef(
     _RequiredGetBotAliasesRequestRequestTypeDef, _OptionalGetBotAliasesRequestRequestTypeDef
 ):
     pass
 
-
 GetBotChannelAssociationRequestRequestTypeDef = TypedDict(
     "GetBotChannelAssociationRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
         "botAlias": str,
     },
 )
 
-GetBotChannelAssociationResponseTypeDef = TypedDict(
-    "GetBotChannelAssociationResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "botAlias": str,
-        "botName": str,
-        "createdDate": datetime,
-        "type": ChannelTypeType,
-        "botConfiguration": Dict[str, str],
-        "status": ChannelStatusType,
-        "failureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    {
-        "botName": str,
-        "botAlias": str,
-    },
-)
-_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
-    _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-    _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetBotChannelAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotChannelAssociationsRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
     },
 )
@@ -638,52 +553,28 @@
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
     total=False,
 )
 
-
 class GetBotChannelAssociationsRequestRequestTypeDef(
     _RequiredGetBotChannelAssociationsRequestRequestTypeDef,
     _OptionalGetBotChannelAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 GetBotRequestRequestTypeDef = TypedDict(
     "GetBotRequestRequestTypeDef",
     {
         "name": str,
         "versionOrAlias": str,
     },
 )
 
-_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
-    _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-    _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetBotVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetBotVersionsRequestRequestTypeDef = TypedDict(
@@ -691,30 +582,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetBotVersionsRequestRequestTypeDef(
     _RequiredGetBotVersionsRequestRequestTypeDef, _OptionalGetBotVersionsRequestRequestTypeDef
 ):
     pass
 
-
-GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
-    "GetBotsRequestGetBotsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBotsRequestRequestTypeDef = TypedDict(
     "GetBotsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -724,45 +604,25 @@
 GetBuiltinIntentRequestRequestTypeDef = TypedDict(
     "GetBuiltinIntentRequestRequestTypeDef",
     {
         "signature": str,
     },
 )
 
-GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = TypedDict(
-    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
-    {
-        "locale": LocaleType,
-        "signatureContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBuiltinIntentsRequestRequestTypeDef = TypedDict(
     "GetBuiltinIntentsRequestRequestTypeDef",
     {
         "locale": LocaleType,
         "signatureContains": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = TypedDict(
-    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
-    {
-        "locale": LocaleType,
-        "signatureContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBuiltinSlotTypesRequestRequestTypeDef = TypedDict(
     "GetBuiltinSlotTypesRequestRequestTypeDef",
     {
         "locale": LocaleType,
         "signatureContains": str,
         "nextToken": str,
         "maxResults": int,
@@ -776,79 +636,29 @@
         "name": str,
         "version": str,
         "resourceType": ResourceTypeType,
         "exportType": ExportTypeType,
     },
 )
 
-GetExportResponseTypeDef = TypedDict(
-    "GetExportResponseTypeDef",
-    {
-        "name": str,
-        "version": str,
-        "resourceType": ResourceTypeType,
-        "exportType": ExportTypeType,
-        "exportStatus": ExportStatusType,
-        "failureReason": str,
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetImportRequestRequestTypeDef = TypedDict(
     "GetImportRequestRequestTypeDef",
     {
         "importId": str,
     },
 )
 
-GetImportResponseTypeDef = TypedDict(
-    "GetImportResponseTypeDef",
-    {
-        "name": str,
-        "resourceType": ResourceTypeType,
-        "mergeStrategy": MergeStrategyType,
-        "importId": str,
-        "importStatus": ImportStatusType,
-        "failureReason": List[str],
-        "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIntentRequestRequestTypeDef = TypedDict(
     "GetIntentRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
-_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
-    _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-    _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetIntentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntentVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetIntentVersionsRequestRequestTypeDef = TypedDict(
@@ -856,42 +666,31 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetIntentVersionsRequestRequestTypeDef(
     _RequiredGetIntentVersionsRequestRequestTypeDef, _OptionalGetIntentVersionsRequestRequestTypeDef
 ):
     pass
 
-
 IntentMetadataTypeDef = TypedDict(
     "IntentMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
     },
     total=False,
 )
 
-GetIntentsRequestGetIntentsPaginateTypeDef = TypedDict(
-    "GetIntentsRequestGetIntentsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetIntentsRequestRequestTypeDef = TypedDict(
     "GetIntentsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -949,36 +748,14 @@
     "GetSlotTypeRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
-_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
-    _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-    _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSlotTypeVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
@@ -986,43 +763,32 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetSlotTypeVersionsRequestRequestTypeDef(
     _RequiredGetSlotTypeVersionsRequestRequestTypeDef,
     _OptionalGetSlotTypeVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 SlotTypeMetadataTypeDef = TypedDict(
     "SlotTypeMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
     },
     total=False,
 )
 
-GetSlotTypesRequestGetSlotTypesPaginateTypeDef = TypedDict(
-    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetSlotTypesRequestRequestTypeDef = TypedDict(
     "GetSlotTypesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -1034,347 +800,414 @@
     {
         "botName": str,
         "botVersions": Sequence[str],
         "statusType": StatusTypeType,
     },
 )
 
-InputContextTypeDef = TypedDict(
-    "InputContextTypeDef",
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
     {
-        "name": str,
+        "resourceArn": str,
     },
 )
 
-IntentTypeDef = TypedDict(
-    "IntentTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "intentName": str,
-        "intentVersion": str,
+        "key": str,
+        "value": str,
     },
 )
 
-_RequiredKendraConfigurationTypeDef = TypedDict(
-    "_RequiredKendraConfigurationTypeDef",
+_RequiredMessageTypeDef = TypedDict(
+    "_RequiredMessageTypeDef",
     {
-        "kendraIndex": str,
-        "role": str,
+        "contentType": ContentTypeType,
+        "content": str,
     },
 )
-_OptionalKendraConfigurationTypeDef = TypedDict(
-    "_OptionalKendraConfigurationTypeDef",
+_OptionalMessageTypeDef = TypedDict(
+    "_OptionalMessageTypeDef",
     {
-        "queryFilterString": str,
+        "groupNumber": int,
     },
     total=False,
 )
 
-
-class KendraConfigurationTypeDef(
-    _RequiredKendraConfigurationTypeDef, _OptionalKendraConfigurationTypeDef
-):
+class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
     pass
 
+SlotDefaultValueTypeDef = TypedDict(
+    "SlotDefaultValueTypeDef",
+    {
+        "defaultValue": str,
+    },
+)
 
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
+SlotTypeRegexConfigurationTypeDef = TypedDict(
+    "SlotTypeRegexConfigurationTypeDef",
     {
-        "resourceArn": str,
+        "pattern": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+StartMigrationRequestRequestTypeDef = TypedDict(
+    "StartMigrationRequestRequestTypeDef",
     {
-        "key": str,
-        "value": str,
+        "v1BotName": str,
+        "v1BotVersion": str,
+        "v2BotName": str,
+        "v2BotRole": str,
+        "migrationStrategy": MigrationStrategyType,
     },
 )
 
-_RequiredMessageOutputTypeDef = TypedDict(
-    "_RequiredMessageOutputTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "contentType": ContentTypeType,
-        "content": str,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
-_OptionalMessageOutputTypeDef = TypedDict(
-    "_OptionalMessageOutputTypeDef",
+
+UtteranceDataTypeDef = TypedDict(
+    "UtteranceDataTypeDef",
     {
-        "groupNumber": int,
+        "utteranceString": str,
+        "count": int,
+        "distinctUsers": int,
+        "firstUtteredDate": datetime,
+        "lastUtteredDate": datetime,
     },
     total=False,
 )
 
+_RequiredFulfillmentActivityTypeDef = TypedDict(
+    "_RequiredFulfillmentActivityTypeDef",
+    {
+        "type": FulfillmentActivityTypeType,
+    },
+)
+_OptionalFulfillmentActivityTypeDef = TypedDict(
+    "_OptionalFulfillmentActivityTypeDef",
+    {
+        "codeHook": CodeHookTypeDef,
+    },
+    total=False,
+)
 
-class MessageOutputTypeDef(_RequiredMessageOutputTypeDef, _OptionalMessageOutputTypeDef):
+class FulfillmentActivityTypeDef(
+    _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
+):
     pass
 
-
-_RequiredMessageTypeDef = TypedDict(
-    "_RequiredMessageTypeDef",
+ConversationLogsRequestTypeDef = TypedDict(
+    "ConversationLogsRequestTypeDef",
     {
-        "contentType": ContentTypeType,
-        "content": str,
+        "logSettings": Sequence[LogSettingsRequestTypeDef],
+        "iamRoleArn": str,
     },
 )
-_OptionalMessageTypeDef = TypedDict(
-    "_OptionalMessageTypeDef",
+
+ConversationLogsResponseTypeDef = TypedDict(
+    "ConversationLogsResponseTypeDef",
     {
-        "groupNumber": int,
+        "logSettings": List[LogSettingsResponseTypeDef],
+        "iamRoleArn": str,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
-    pass
-
-
-OutputContextTypeDef = TypedDict(
-    "OutputContextTypeDef",
+GetBotChannelAssociationResponseTypeDef = TypedDict(
+    "GetBotChannelAssociationResponseTypeDef",
     {
         "name": str,
-        "timeToLiveInSeconds": int,
-        "turnsToLive": int,
+        "description": str,
+        "botAlias": str,
+        "botName": str,
+        "createdDate": datetime,
+        "type": ChannelTypeType,
+        "botConfiguration": Dict[str, str],
+        "status": ChannelStatusType,
+        "failureReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetBotChannelAssociationsResponseTypeDef = TypedDict(
+    "GetBotChannelAssociationsResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "botChannelAssociations": List[BotChannelAssociationTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+GetBotVersionsResponseTypeDef = TypedDict(
+    "GetBotVersionsResponseTypeDef",
     {
-        "key": str,
-        "value": str,
+        "bots": List[BotMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetBotsResponseTypeDef = TypedDict(
+    "GetBotsResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "bots": List[BotMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SlotDefaultValueOutputTypeDef = TypedDict(
-    "SlotDefaultValueOutputTypeDef",
+GetBuiltinIntentResponseTypeDef = TypedDict(
+    "GetBuiltinIntentResponseTypeDef",
     {
-        "defaultValue": str,
+        "signature": str,
+        "supportedLocales": List[LocaleType],
+        "slots": List[BuiltinIntentSlotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SlotDefaultValueTypeDef = TypedDict(
-    "SlotDefaultValueTypeDef",
+GetBuiltinIntentsResponseTypeDef = TypedDict(
+    "GetBuiltinIntentsResponseTypeDef",
     {
-        "defaultValue": str,
+        "intents": List[BuiltinIntentMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SlotTypeRegexConfigurationOutputTypeDef = TypedDict(
-    "SlotTypeRegexConfigurationOutputTypeDef",
+GetBuiltinSlotTypesResponseTypeDef = TypedDict(
+    "GetBuiltinSlotTypesResponseTypeDef",
     {
-        "pattern": str,
+        "slotTypes": List[BuiltinSlotTypeMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SlotTypeRegexConfigurationTypeDef = TypedDict(
-    "SlotTypeRegexConfigurationTypeDef",
+GetExportResponseTypeDef = TypedDict(
+    "GetExportResponseTypeDef",
     {
-        "pattern": str,
+        "name": str,
+        "version": str,
+        "resourceType": ResourceTypeType,
+        "exportType": ExportTypeType,
+        "exportStatus": ExportStatusType,
+        "failureReason": str,
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartMigrationRequestRequestTypeDef = TypedDict(
-    "StartMigrationRequestRequestTypeDef",
+GetImportResponseTypeDef = TypedDict(
+    "GetImportResponseTypeDef",
     {
-        "v1BotName": str,
-        "v1BotVersion": str,
-        "v2BotName": str,
-        "v2BotRole": str,
-        "migrationStrategy": MigrationStrategyType,
+        "name": str,
+        "resourceType": ResourceTypeType,
+        "mergeStrategy": MergeStrategyType,
+        "importId": str,
+        "importStatus": ImportStatusType,
+        "failureReason": List[str],
+        "createdDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMigrationResponseTypeDef = TypedDict(
     "StartMigrationResponseTypeDef",
     {
         "v1BotName": str,
         "v1BotVersion": str,
         "v1BotLocale": LocaleType,
         "v2BotId": str,
         "v2BotRole": str,
         "migrationId": str,
         "migrationStrategy": MigrationStrategyType,
         "migrationTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
+    "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "botName": str,
     },
 )
-
-UtteranceDataTypeDef = TypedDict(
-    "UtteranceDataTypeDef",
+_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
+    "_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     {
-        "utteranceString": str,
-        "count": int,
-        "distinctUsers": int,
-        "firstUtteredDate": datetime,
-        "lastUtteredDate": datetime,
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-GetBotChannelAssociationsResponseTypeDef = TypedDict(
-    "GetBotChannelAssociationsResponseTypeDef",
+class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
+    _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     {
-        "botChannelAssociations": List[BotChannelAssociationTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "botName": str,
+        "botAlias": str,
     },
 )
-
-GetBotVersionsResponseTypeDef = TypedDict(
-    "GetBotVersionsResponseTypeDef",
+_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     {
-        "bots": List[BotMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetBotsResponseTypeDef = TypedDict(
-    "GetBotsResponseTypeDef",
+class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
+    _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+    _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     {
-        "bots": List[BotMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+    },
+)
+_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetBuiltinIntentsResponseTypeDef = TypedDict(
-    "GetBuiltinIntentsResponseTypeDef",
+class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
+    _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+    _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+):
+    pass
+
+GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
+    "GetBotsRequestGetBotsPaginateTypeDef",
     {
-        "intents": List[BuiltinIntentMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetBuiltinIntentResponseTypeDef = TypedDict(
-    "GetBuiltinIntentResponseTypeDef",
+GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = TypedDict(
+    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     {
-        "signature": str,
-        "supportedLocales": List[LocaleType],
-        "slots": List[BuiltinIntentSlotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "locale": LocaleType,
+        "signatureContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetBuiltinSlotTypesResponseTypeDef = TypedDict(
-    "GetBuiltinSlotTypesResponseTypeDef",
+GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = TypedDict(
+    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
     {
-        "slotTypes": List[BuiltinSlotTypeMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "locale": LocaleType,
+        "signatureContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredFulfillmentActivityOutputTypeDef = TypedDict(
-    "_RequiredFulfillmentActivityOutputTypeDef",
+_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
     {
-        "type": FulfillmentActivityTypeType,
+        "name": str,
     },
 )
-_OptionalFulfillmentActivityOutputTypeDef = TypedDict(
-    "_OptionalFulfillmentActivityOutputTypeDef",
+_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
     {
-        "codeHook": CodeHookOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class FulfillmentActivityOutputTypeDef(
-    _RequiredFulfillmentActivityOutputTypeDef, _OptionalFulfillmentActivityOutputTypeDef
+class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
+    _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+    _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
 ):
     pass
 
+GetIntentsRequestGetIntentsPaginateTypeDef = TypedDict(
+    "GetIntentsRequestGetIntentsPaginateTypeDef",
+    {
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-_RequiredFulfillmentActivityTypeDef = TypedDict(
-    "_RequiredFulfillmentActivityTypeDef",
+_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     {
-        "type": FulfillmentActivityTypeType,
+        "name": str,
     },
 )
-_OptionalFulfillmentActivityTypeDef = TypedDict(
-    "_OptionalFulfillmentActivityTypeDef",
+_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     {
-        "codeHook": CodeHookTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class FulfillmentActivityTypeDef(
-    _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
+class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
+    _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+    _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
 ):
     pass
 
-
-ConversationLogsRequestTypeDef = TypedDict(
-    "ConversationLogsRequestTypeDef",
-    {
-        "logSettings": Sequence[LogSettingsRequestTypeDef],
-        "iamRoleArn": str,
-    },
-)
-
-ConversationLogsResponseTypeDef = TypedDict(
-    "ConversationLogsResponseTypeDef",
+GetSlotTypesRequestGetSlotTypesPaginateTypeDef = TypedDict(
+    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     {
-        "logSettings": List[LogSettingsResponseTypeDef],
-        "iamRoleArn": str,
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetIntentVersionsResponseTypeDef = TypedDict(
     "GetIntentVersionsResponseTypeDef",
     {
         "intents": List[IntentMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntentsResponseTypeDef = TypedDict(
     "GetIntentsResponseTypeDef",
     {
         "intents": List[IntentMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMigrationResponseTypeDef = TypedDict(
     "GetMigrationResponseTypeDef",
     {
         "migrationId": str,
@@ -1383,106 +1216,114 @@
         "v1BotLocale": LocaleType,
         "v2BotId": str,
         "v2BotRole": str,
         "migrationStatus": MigrationStatusType,
         "migrationStrategy": MigrationStrategyType,
         "migrationTimestamp": datetime,
         "alerts": List[MigrationAlertTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMigrationsResponseTypeDef = TypedDict(
     "GetMigrationsResponseTypeDef",
     {
         "migrationSummaries": List[MigrationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSlotTypeVersionsResponseTypeDef = TypedDict(
     "GetSlotTypeVersionsResponseTypeDef",
     {
         "slotTypes": List[SlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSlotTypesResponseTypeDef = TypedDict(
     "GetSlotTypesResponseTypeDef",
     {
         "slotTypes": List[SlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartImportRequestRequestTypeDef = TypedDict(
+    "_RequiredStartImportRequestRequestTypeDef",
+    {
+        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "resourceType": ResourceTypeType,
+        "mergeStrategy": MergeStrategyType,
+    },
+)
+_OptionalStartImportRequestRequestTypeDef = TypedDict(
+    "_OptionalStartImportRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class StartImportRequestRequestTypeDef(
+    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
+):
+    pass
+
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "name": str,
         "resourceType": ResourceTypeType,
         "mergeStrategy": MergeStrategyType,
         "importId": str,
         "importStatus": ImportStatusType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
 _RequiredPromptOutputTypeDef = TypedDict(
     "_RequiredPromptOutputTypeDef",
     {
-        "messages": List[MessageOutputTypeDef],
+        "messages": List[MessageTypeDef],
         "maxAttempts": int,
     },
 )
 _OptionalPromptOutputTypeDef = TypedDict(
     "_OptionalPromptOutputTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
-
 class PromptOutputTypeDef(_RequiredPromptOutputTypeDef, _OptionalPromptOutputTypeDef):
     pass
 
-
-_RequiredStatementOutputTypeDef = TypedDict(
-    "_RequiredStatementOutputTypeDef",
-    {
-        "messages": List[MessageOutputTypeDef],
-    },
-)
-_OptionalStatementOutputTypeDef = TypedDict(
-    "_OptionalStatementOutputTypeDef",
-    {
-        "responseCard": str,
-    },
-    total=False,
-)
-
-
-class StatementOutputTypeDef(_RequiredStatementOutputTypeDef, _OptionalStatementOutputTypeDef):
-    pass
-
-
 _RequiredPromptTypeDef = TypedDict(
     "_RequiredPromptTypeDef",
     {
         "messages": Sequence[MessageTypeDef],
         "maxAttempts": int,
     },
 )
@@ -1490,91 +1331,65 @@
     "_OptionalPromptTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
-
 class PromptTypeDef(_RequiredPromptTypeDef, _OptionalPromptTypeDef):
     pass
 
-
-_RequiredStatementTypeDef = TypedDict(
-    "_RequiredStatementTypeDef",
+_RequiredStatementOutputTypeDef = TypedDict(
+    "_RequiredStatementOutputTypeDef",
     {
-        "messages": Sequence[MessageTypeDef],
+        "messages": List[MessageTypeDef],
     },
 )
-_OptionalStatementTypeDef = TypedDict(
-    "_OptionalStatementTypeDef",
+_OptionalStatementOutputTypeDef = TypedDict(
+    "_OptionalStatementOutputTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
-
-class StatementTypeDef(_RequiredStatementTypeDef, _OptionalStatementTypeDef):
+class StatementOutputTypeDef(_RequiredStatementOutputTypeDef, _OptionalStatementOutputTypeDef):
     pass
 
-
-_RequiredStartImportRequestRequestTypeDef = TypedDict(
-    "_RequiredStartImportRequestRequestTypeDef",
+_RequiredStatementTypeDef = TypedDict(
+    "_RequiredStatementTypeDef",
     {
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
-        "resourceType": ResourceTypeType,
-        "mergeStrategy": MergeStrategyType,
+        "messages": Sequence[MessageTypeDef],
     },
 )
-_OptionalStartImportRequestRequestTypeDef = TypedDict(
-    "_OptionalStartImportRequestRequestTypeDef",
+_OptionalStatementTypeDef = TypedDict(
+    "_OptionalStatementTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "responseCard": str,
     },
     total=False,
 )
 
-
-class StartImportRequestRequestTypeDef(
-    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
-):
+class StatementTypeDef(_RequiredStatementTypeDef, _OptionalStatementTypeDef):
     pass
 
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
-
 SlotDefaultValueSpecOutputTypeDef = TypedDict(
     "SlotDefaultValueSpecOutputTypeDef",
     {
-        "defaultValueList": List[SlotDefaultValueOutputTypeDef],
+        "defaultValueList": List[SlotDefaultValueTypeDef],
     },
 )
 
 SlotDefaultValueSpecTypeDef = TypedDict(
     "SlotDefaultValueSpecTypeDef",
     {
         "defaultValueList": Sequence[SlotDefaultValueTypeDef],
     },
 )
 
-SlotTypeConfigurationOutputTypeDef = TypedDict(
-    "SlotTypeConfigurationOutputTypeDef",
-    {
-        "regexConfiguration": SlotTypeRegexConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 SlotTypeConfigurationTypeDef = TypedDict(
     "SlotTypeConfigurationTypeDef",
     {
         "regexConfiguration": SlotTypeRegexConfigurationTypeDef,
     },
     total=False,
 )
@@ -1603,21 +1418,19 @@
         "checksum": str,
         "conversationLogs": ConversationLogsRequestTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutBotAliasRequestRequestTypeDef(
     _RequiredPutBotAliasRequestRequestTypeDef, _OptionalPutBotAliasRequestRequestTypeDef
 ):
     pass
 
-
 BotAliasMetadataTypeDef = TypedDict(
     "BotAliasMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "botVersion": str,
         "botName": str,
@@ -1636,55 +1449,55 @@
         "description": str,
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBotAliasResponseTypeDef = TypedDict(
     "PutBotAliasResponseTypeDef",
     {
         "name": str,
         "description": str,
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "intents": List[IntentOutputTypeDef],
+        "intents": List[IntentTypeDef],
         "clarificationPrompt": PromptOutputTypeDef,
         "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "enableModelImprovements": bool,
         "detectSentiment": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FollowUpPromptOutputTypeDef = TypedDict(
     "FollowUpPromptOutputTypeDef",
     {
         "prompt": PromptOutputTypeDef,
@@ -1693,15 +1506,15 @@
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "intents": List[IntentOutputTypeDef],
+        "intents": List[IntentTypeDef],
         "enableModelImprovements": bool,
         "nluIntentConfidenceThreshold": float,
         "clarificationPrompt": PromptOutputTypeDef,
         "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
@@ -1709,24 +1522,24 @@
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "detectSentiment": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBotResponseTypeDef = TypedDict(
     "PutBotResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "intents": List[IntentOutputTypeDef],
+        "intents": List[IntentTypeDef],
         "enableModelImprovements": bool,
         "nluIntentConfidenceThreshold": float,
         "clarificationPrompt": PromptOutputTypeDef,
         "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
@@ -1735,16 +1548,16 @@
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "createVersion": bool,
         "detectSentiment": bool,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FollowUpPromptTypeDef = TypedDict(
     "FollowUpPromptTypeDef",
     {
         "prompt": PromptTypeDef,
@@ -1776,21 +1589,19 @@
         "detectSentiment": bool,
         "createVersion": bool,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutBotRequestRequestTypeDef(
     _RequiredPutBotRequestRequestTypeDef, _OptionalPutBotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSlotOutputTypeDef = TypedDict(
     "_RequiredSlotOutputTypeDef",
     {
         "name": str,
         "slotConstraint": SlotConstraintType,
     },
 )
@@ -1806,19 +1617,17 @@
         "responseCard": str,
         "obfuscationSetting": ObfuscationSettingType,
         "defaultValueSpec": SlotDefaultValueSpecOutputTypeDef,
     },
     total=False,
 )
 
-
 class SlotOutputTypeDef(_RequiredSlotOutputTypeDef, _OptionalSlotOutputTypeDef):
     pass
 
-
 _RequiredSlotTypeDef = TypedDict(
     "_RequiredSlotTypeDef",
     {
         "name": str,
         "slotConstraint": SlotConstraintType,
     },
 )
@@ -1834,33 +1643,31 @@
         "responseCard": str,
         "obfuscationSetting": ObfuscationSettingType,
         "defaultValueSpec": SlotDefaultValueSpecTypeDef,
     },
     total=False,
 )
 
-
 class SlotTypeDef(_RequiredSlotTypeDef, _OptionalSlotTypeDef):
     pass
 
-
 CreateSlotTypeVersionResponseTypeDef = TypedDict(
     "CreateSlotTypeVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
         "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
-        "slotTypeConfigurations": List[SlotTypeConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSlotTypeResponseTypeDef = TypedDict(
     "GetSlotTypeResponseTypeDef",
     {
         "name": str,
@@ -1868,34 +1675,16 @@
         "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
-        "slotTypeConfigurations": List[SlotTypeConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutSlotTypeResponseTypeDef = TypedDict(
-    "PutSlotTypeResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "enumerationValues": List[EnumerationValueOutputTypeDef],
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "version": str,
-        "checksum": str,
-        "valueSelectionStrategy": SlotValueSelectionStrategyType,
-        "createVersion": bool,
-        "parentSlotTypeSignature": str,
-        "slotTypeConfigurations": List[SlotTypeConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutSlotTypeRequestRequestTypeDef",
     {
         "name": str,
@@ -1911,112 +1700,128 @@
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": Sequence[SlotTypeConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class PutSlotTypeRequestRequestTypeDef(
     _RequiredPutSlotTypeRequestRequestTypeDef, _OptionalPutSlotTypeRequestRequestTypeDef
 ):
     pass
 
+PutSlotTypeResponseTypeDef = TypedDict(
+    "PutSlotTypeResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "version": str,
+        "checksum": str,
+        "valueSelectionStrategy": SlotValueSelectionStrategyType,
+        "createVersion": bool,
+        "parentSlotTypeSignature": str,
+        "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetUtterancesViewResponseTypeDef = TypedDict(
     "GetUtterancesViewResponseTypeDef",
     {
         "botName": str,
         "utterances": List[UtteranceListTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBotAliasesResponseTypeDef = TypedDict(
     "GetBotAliasesResponseTypeDef",
     {
         "BotAliases": List[BotAliasMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateIntentVersionResponseTypeDef = TypedDict(
     "CreateIntentVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
         "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
         "confirmationPrompt": PromptOutputTypeDef,
         "rejectionStatement": StatementOutputTypeDef,
         "followUpPrompt": FollowUpPromptOutputTypeDef,
         "conclusionStatement": StatementOutputTypeDef,
-        "dialogCodeHook": CodeHookOutputTypeDef,
-        "fulfillmentActivity": FulfillmentActivityOutputTypeDef,
+        "dialogCodeHook": CodeHookTypeDef,
+        "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
-        "kendraConfiguration": KendraConfigurationOutputTypeDef,
-        "inputContexts": List[InputContextOutputTypeDef],
-        "outputContexts": List[OutputContextOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "kendraConfiguration": KendraConfigurationTypeDef,
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntentResponseTypeDef = TypedDict(
     "GetIntentResponseTypeDef",
     {
         "name": str,
         "description": str,
         "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
         "confirmationPrompt": PromptOutputTypeDef,
         "rejectionStatement": StatementOutputTypeDef,
         "followUpPrompt": FollowUpPromptOutputTypeDef,
         "conclusionStatement": StatementOutputTypeDef,
-        "dialogCodeHook": CodeHookOutputTypeDef,
-        "fulfillmentActivity": FulfillmentActivityOutputTypeDef,
+        "dialogCodeHook": CodeHookTypeDef,
+        "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
-        "kendraConfiguration": KendraConfigurationOutputTypeDef,
-        "inputContexts": List[InputContextOutputTypeDef],
-        "outputContexts": List[OutputContextOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "kendraConfiguration": KendraConfigurationTypeDef,
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutIntentResponseTypeDef = TypedDict(
     "PutIntentResponseTypeDef",
     {
         "name": str,
         "description": str,
         "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
         "confirmationPrompt": PromptOutputTypeDef,
         "rejectionStatement": StatementOutputTypeDef,
         "followUpPrompt": FollowUpPromptOutputTypeDef,
         "conclusionStatement": StatementOutputTypeDef,
-        "dialogCodeHook": CodeHookOutputTypeDef,
-        "fulfillmentActivity": FulfillmentActivityOutputTypeDef,
+        "dialogCodeHook": CodeHookTypeDef,
+        "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "createVersion": bool,
-        "kendraConfiguration": KendraConfigurationOutputTypeDef,
-        "inputContexts": List[InputContextOutputTypeDef],
-        "outputContexts": List[OutputContextOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "kendraConfiguration": KendraConfigurationTypeDef,
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutIntentRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntentRequestRequestTypeDef",
     {
         "name": str,
@@ -2040,12 +1845,11 @@
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": Sequence[InputContextTypeDef],
         "outputContexts": Sequence[OutputContextTypeDef],
     },
     total=False,
 )
 
-
 class PutIntentRequestRequestTypeDef(
     _RequiredPutIntentRequestRequestTypeDef, _OptionalPutIntentRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models/type_defs.pyi` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,127 +44,117 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BotChannelAssociationTypeDef",
     "BotMetadataTypeDef",
     "BuiltinIntentMetadataTypeDef",
     "BuiltinIntentSlotTypeDef",
     "BuiltinSlotTypeMetadataTypeDef",
-    "CodeHookOutputTypeDef",
     "CodeHookTypeDef",
     "LogSettingsRequestTypeDef",
     "LogSettingsResponseTypeDef",
     "CreateBotVersionRequestRequestTypeDef",
-    "IntentOutputTypeDef",
+    "IntentTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateIntentVersionRequestRequestTypeDef",
-    "InputContextOutputTypeDef",
-    "KendraConfigurationOutputTypeDef",
-    "OutputContextOutputTypeDef",
+    "InputContextTypeDef",
+    "KendraConfigurationTypeDef",
+    "OutputContextTypeDef",
     "CreateSlotTypeVersionRequestRequestTypeDef",
     "EnumerationValueOutputTypeDef",
     "DeleteBotAliasRequestRequestTypeDef",
     "DeleteBotChannelAssociationRequestRequestTypeDef",
     "DeleteBotRequestRequestTypeDef",
     "DeleteBotVersionRequestRequestTypeDef",
     "DeleteIntentRequestRequestTypeDef",
     "DeleteIntentVersionRequestRequestTypeDef",
     "DeleteSlotTypeRequestRequestTypeDef",
     "DeleteSlotTypeVersionRequestRequestTypeDef",
     "DeleteUtterancesRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnumerationValueTypeDef",
     "GetBotAliasRequestRequestTypeDef",
-    "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetBotAliasesRequestRequestTypeDef",
     "GetBotChannelAssociationRequestRequestTypeDef",
-    "GetBotChannelAssociationResponseTypeDef",
-    "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     "GetBotChannelAssociationsRequestRequestTypeDef",
     "GetBotRequestRequestTypeDef",
-    "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     "GetBotVersionsRequestRequestTypeDef",
-    "GetBotsRequestGetBotsPaginateTypeDef",
     "GetBotsRequestRequestTypeDef",
     "GetBuiltinIntentRequestRequestTypeDef",
-    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     "GetBuiltinIntentsRequestRequestTypeDef",
-    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
     "GetBuiltinSlotTypesRequestRequestTypeDef",
     "GetExportRequestRequestTypeDef",
-    "GetExportResponseTypeDef",
     "GetImportRequestRequestTypeDef",
-    "GetImportResponseTypeDef",
     "GetIntentRequestRequestTypeDef",
-    "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
     "GetIntentVersionsRequestRequestTypeDef",
     "IntentMetadataTypeDef",
-    "GetIntentsRequestGetIntentsPaginateTypeDef",
     "GetIntentsRequestRequestTypeDef",
     "GetMigrationRequestRequestTypeDef",
     "MigrationAlertTypeDef",
     "GetMigrationsRequestRequestTypeDef",
     "MigrationSummaryTypeDef",
     "GetSlotTypeRequestRequestTypeDef",
-    "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     "GetSlotTypeVersionsRequestRequestTypeDef",
     "SlotTypeMetadataTypeDef",
-    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     "GetSlotTypesRequestRequestTypeDef",
     "GetUtterancesViewRequestRequestTypeDef",
-    "InputContextTypeDef",
-    "IntentTypeDef",
-    "KendraConfigurationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "MessageOutputTypeDef",
-    "MessageTypeDef",
-    "OutputContextTypeDef",
-    "PaginatorConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
-    "SlotDefaultValueOutputTypeDef",
+    "MessageTypeDef",
     "SlotDefaultValueTypeDef",
-    "SlotTypeRegexConfigurationOutputTypeDef",
     "SlotTypeRegexConfigurationTypeDef",
     "StartMigrationRequestRequestTypeDef",
-    "StartMigrationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UtteranceDataTypeDef",
+    "FulfillmentActivityTypeDef",
+    "ConversationLogsRequestTypeDef",
+    "ConversationLogsResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetBotChannelAssociationResponseTypeDef",
     "GetBotChannelAssociationsResponseTypeDef",
     "GetBotVersionsResponseTypeDef",
     "GetBotsResponseTypeDef",
-    "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinIntentResponseTypeDef",
+    "GetBuiltinIntentsResponseTypeDef",
     "GetBuiltinSlotTypesResponseTypeDef",
-    "FulfillmentActivityOutputTypeDef",
-    "FulfillmentActivityTypeDef",
-    "ConversationLogsRequestTypeDef",
-    "ConversationLogsResponseTypeDef",
+    "GetExportResponseTypeDef",
+    "GetImportResponseTypeDef",
+    "StartMigrationResponseTypeDef",
+    "GetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+    "GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
+    "GetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    "GetBotsRequestGetBotsPaginateTypeDef",
+    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
+    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
+    "GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
+    "GetIntentsRequestGetIntentsPaginateTypeDef",
+    "GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     "GetIntentVersionsResponseTypeDef",
     "GetIntentsResponseTypeDef",
     "GetMigrationResponseTypeDef",
     "GetMigrationsResponseTypeDef",
     "GetSlotTypeVersionsResponseTypeDef",
     "GetSlotTypesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "PromptOutputTypeDef",
-    "StatementOutputTypeDef",
     "PromptTypeDef",
+    "StatementOutputTypeDef",
     "StatementTypeDef",
-    "StartImportRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "SlotDefaultValueSpecOutputTypeDef",
     "SlotDefaultValueSpecTypeDef",
-    "SlotTypeConfigurationOutputTypeDef",
     "SlotTypeConfigurationTypeDef",
     "UtteranceListTypeDef",
     "PutBotAliasRequestRequestTypeDef",
     "BotAliasMetadataTypeDef",
     "GetBotAliasResponseTypeDef",
     "PutBotAliasResponseTypeDef",
     "CreateBotVersionResponseTypeDef",
@@ -173,16 +163,16 @@
     "PutBotResponseTypeDef",
     "FollowUpPromptTypeDef",
     "PutBotRequestRequestTypeDef",
     "SlotOutputTypeDef",
     "SlotTypeDef",
     "CreateSlotTypeVersionResponseTypeDef",
     "GetSlotTypeResponseTypeDef",
-    "PutSlotTypeResponseTypeDef",
     "PutSlotTypeRequestRequestTypeDef",
+    "PutSlotTypeResponseTypeDef",
     "GetUtterancesViewResponseTypeDef",
     "GetBotAliasesResponseTypeDef",
     "CreateIntentVersionResponseTypeDef",
     "GetIntentResponseTypeDef",
     "PutIntentResponseTypeDef",
     "PutIntentRequestRequestTypeDef",
 )
@@ -238,22 +228,14 @@
     {
         "signature": str,
         "supportedLocales": List[LocaleType],
     },
     total=False,
 )
 
-CodeHookOutputTypeDef = TypedDict(
-    "CodeHookOutputTypeDef",
-    {
-        "uri": str,
-        "messageVersion": str,
-    },
-)
-
 CodeHookTypeDef = TypedDict(
     "CodeHookTypeDef",
     {
         "uri": str,
         "messageVersion": str,
     },
 )
@@ -270,19 +252,21 @@
     "_OptionalLogSettingsRequestTypeDef",
     {
         "kmsKeyArn": str,
     },
     total=False,
 )
 
+
 class LogSettingsRequestTypeDef(
     _RequiredLogSettingsRequestTypeDef, _OptionalLogSettingsRequestTypeDef
 ):
     pass
 
+
 LogSettingsResponseTypeDef = TypedDict(
     "LogSettingsResponseTypeDef",
     {
         "logType": LogTypeType,
         "destination": DestinationType,
         "kmsKeyArn": str,
         "resourceArn": str,
@@ -301,76 +285,93 @@
     "_OptionalCreateBotVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
+
 class CreateBotVersionRequestRequestTypeDef(
     _RequiredCreateBotVersionRequestRequestTypeDef, _OptionalCreateBotVersionRequestRequestTypeDef
 ):
     pass
 
-IntentOutputTypeDef = TypedDict(
-    "IntentOutputTypeDef",
+
+IntentTypeDef = TypedDict(
+    "IntentTypeDef",
     {
         "intentName": str,
         "intentVersion": str,
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
 _RequiredCreateIntentVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntentVersionRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateIntentVersionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateIntentVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
+
 class CreateIntentVersionRequestRequestTypeDef(
     _RequiredCreateIntentVersionRequestRequestTypeDef,
     _OptionalCreateIntentVersionRequestRequestTypeDef,
 ):
     pass
 
-InputContextOutputTypeDef = TypedDict(
-    "InputContextOutputTypeDef",
+
+InputContextTypeDef = TypedDict(
+    "InputContextTypeDef",
     {
         "name": str,
     },
 )
 
-_RequiredKendraConfigurationOutputTypeDef = TypedDict(
-    "_RequiredKendraConfigurationOutputTypeDef",
+_RequiredKendraConfigurationTypeDef = TypedDict(
+    "_RequiredKendraConfigurationTypeDef",
     {
         "kendraIndex": str,
         "role": str,
     },
 )
-_OptionalKendraConfigurationOutputTypeDef = TypedDict(
-    "_OptionalKendraConfigurationOutputTypeDef",
+_OptionalKendraConfigurationTypeDef = TypedDict(
+    "_OptionalKendraConfigurationTypeDef",
     {
         "queryFilterString": str,
     },
     total=False,
 )
 
-class KendraConfigurationOutputTypeDef(
-    _RequiredKendraConfigurationOutputTypeDef, _OptionalKendraConfigurationOutputTypeDef
+
+class KendraConfigurationTypeDef(
+    _RequiredKendraConfigurationTypeDef, _OptionalKendraConfigurationTypeDef
 ):
     pass
 
-OutputContextOutputTypeDef = TypedDict(
-    "OutputContextOutputTypeDef",
+
+OutputContextTypeDef = TypedDict(
+    "OutputContextTypeDef",
     {
         "name": str,
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
 )
 
@@ -384,39 +385,43 @@
     "_OptionalCreateSlotTypeVersionRequestRequestTypeDef",
     {
         "checksum": str,
     },
     total=False,
 )
 
+
 class CreateSlotTypeVersionRequestRequestTypeDef(
     _RequiredCreateSlotTypeVersionRequestRequestTypeDef,
     _OptionalCreateSlotTypeVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredEnumerationValueOutputTypeDef = TypedDict(
     "_RequiredEnumerationValueOutputTypeDef",
     {
         "value": str,
     },
 )
 _OptionalEnumerationValueOutputTypeDef = TypedDict(
     "_OptionalEnumerationValueOutputTypeDef",
     {
         "synonyms": List[str],
     },
     total=False,
 )
 
+
 class EnumerationValueOutputTypeDef(
     _RequiredEnumerationValueOutputTypeDef, _OptionalEnumerationValueOutputTypeDef
 ):
     pass
 
+
 DeleteBotAliasRequestRequestTypeDef = TypedDict(
     "DeleteBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
@@ -479,67 +484,51 @@
     "DeleteUtterancesRequestRequestTypeDef",
     {
         "botName": str,
         "userId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnumerationValueTypeDef = TypedDict(
     "_RequiredEnumerationValueTypeDef",
     {
         "value": str,
     },
 )
 _OptionalEnumerationValueTypeDef = TypedDict(
     "_OptionalEnumerationValueTypeDef",
     {
         "synonyms": Sequence[str],
     },
     total=False,
 )
 
+
 class EnumerationValueTypeDef(_RequiredEnumerationValueTypeDef, _OptionalEnumerationValueTypeDef):
     pass
 
+
 GetBotAliasRequestRequestTypeDef = TypedDict(
     "GetBotAliasRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
     },
 )
 
-_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
-    "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
-    {
-        "botName": str,
-    },
-)
-_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
-    "_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
-    _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-    _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetBotAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotAliasesRequestRequestTypeDef",
     {
         "botName": str,
     },
 )
 _OptionalGetBotAliasesRequestRequestTypeDef = TypedDict(
@@ -548,66 +537,30 @@
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
     total=False,
 )
 
+
 class GetBotAliasesRequestRequestTypeDef(
     _RequiredGetBotAliasesRequestRequestTypeDef, _OptionalGetBotAliasesRequestRequestTypeDef
 ):
     pass
 
+
 GetBotChannelAssociationRequestRequestTypeDef = TypedDict(
     "GetBotChannelAssociationRequestRequestTypeDef",
     {
         "name": str,
         "botName": str,
         "botAlias": str,
     },
 )
 
-GetBotChannelAssociationResponseTypeDef = TypedDict(
-    "GetBotChannelAssociationResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "botAlias": str,
-        "botName": str,
-        "createdDate": datetime,
-        "type": ChannelTypeType,
-        "botConfiguration": Dict[str, str],
-        "status": ChannelStatusType,
-        "failureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    {
-        "botName": str,
-        "botAlias": str,
-    },
-)
-_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
-    _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-    _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetBotChannelAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotChannelAssociationsRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
     },
 )
@@ -617,48 +570,30 @@
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
     total=False,
 )
 
+
 class GetBotChannelAssociationsRequestRequestTypeDef(
     _RequiredGetBotChannelAssociationsRequestRequestTypeDef,
     _OptionalGetBotChannelAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 GetBotRequestRequestTypeDef = TypedDict(
     "GetBotRequestRequestTypeDef",
     {
         "name": str,
         "versionOrAlias": str,
     },
 )
 
-_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
-    _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-    _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetBotVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetBotVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetBotVersionsRequestRequestTypeDef = TypedDict(
@@ -666,27 +601,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetBotVersionsRequestRequestTypeDef(
     _RequiredGetBotVersionsRequestRequestTypeDef, _OptionalGetBotVersionsRequestRequestTypeDef
 ):
     pass
 
-GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
-    "GetBotsRequestGetBotsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 GetBotsRequestRequestTypeDef = TypedDict(
     "GetBotsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
@@ -697,45 +625,25 @@
 GetBuiltinIntentRequestRequestTypeDef = TypedDict(
     "GetBuiltinIntentRequestRequestTypeDef",
     {
         "signature": str,
     },
 )
 
-GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = TypedDict(
-    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
-    {
-        "locale": LocaleType,
-        "signatureContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBuiltinIntentsRequestRequestTypeDef = TypedDict(
     "GetBuiltinIntentsRequestRequestTypeDef",
     {
         "locale": LocaleType,
         "signatureContains": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = TypedDict(
-    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
-    {
-        "locale": LocaleType,
-        "signatureContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBuiltinSlotTypesRequestRequestTypeDef = TypedDict(
     "GetBuiltinSlotTypesRequestRequestTypeDef",
     {
         "locale": LocaleType,
         "signatureContains": str,
         "nextToken": str,
         "maxResults": int,
@@ -749,77 +657,29 @@
         "name": str,
         "version": str,
         "resourceType": ResourceTypeType,
         "exportType": ExportTypeType,
     },
 )
 
-GetExportResponseTypeDef = TypedDict(
-    "GetExportResponseTypeDef",
-    {
-        "name": str,
-        "version": str,
-        "resourceType": ResourceTypeType,
-        "exportType": ExportTypeType,
-        "exportStatus": ExportStatusType,
-        "failureReason": str,
-        "url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetImportRequestRequestTypeDef = TypedDict(
     "GetImportRequestRequestTypeDef",
     {
         "importId": str,
     },
 )
 
-GetImportResponseTypeDef = TypedDict(
-    "GetImportResponseTypeDef",
-    {
-        "name": str,
-        "resourceType": ResourceTypeType,
-        "mergeStrategy": MergeStrategyType,
-        "importId": str,
-        "importStatus": ImportStatusType,
-        "failureReason": List[str],
-        "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetIntentRequestRequestTypeDef = TypedDict(
     "GetIntentRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
-_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
-    _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-    _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetIntentVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntentVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetIntentVersionsRequestRequestTypeDef = TypedDict(
@@ -827,40 +687,33 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetIntentVersionsRequestRequestTypeDef(
     _RequiredGetIntentVersionsRequestRequestTypeDef, _OptionalGetIntentVersionsRequestRequestTypeDef
 ):
     pass
 
+
 IntentMetadataTypeDef = TypedDict(
     "IntentMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
     },
     total=False,
 )
 
-GetIntentsRequestGetIntentsPaginateTypeDef = TypedDict(
-    "GetIntentsRequestGetIntentsPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetIntentsRequestRequestTypeDef = TypedDict(
     "GetIntentsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -918,34 +771,14 @@
     "GetSlotTypeRequestRequestTypeDef",
     {
         "name": str,
         "version": str,
     },
 )
 
-_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
-    "_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
-    "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
-    _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-    _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSlotTypeVersionsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGetSlotTypeVersionsRequestRequestTypeDef = TypedDict(
@@ -953,41 +786,34 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetSlotTypeVersionsRequestRequestTypeDef(
     _RequiredGetSlotTypeVersionsRequestRequestTypeDef,
     _OptionalGetSlotTypeVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 SlotTypeMetadataTypeDef = TypedDict(
     "SlotTypeMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
     },
     total=False,
 )
 
-GetSlotTypesRequestGetSlotTypesPaginateTypeDef = TypedDict(
-    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
-    {
-        "nameContains": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetSlotTypesRequestRequestTypeDef = TypedDict(
     "GetSlotTypesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "nameContains": str,
     },
@@ -999,337 +825,428 @@
     {
         "botName": str,
         "botVersions": Sequence[str],
         "statusType": StatusTypeType,
     },
 )
 
-InputContextTypeDef = TypedDict(
-    "InputContextTypeDef",
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
     {
-        "name": str,
+        "resourceArn": str,
     },
 )
 
-IntentTypeDef = TypedDict(
-    "IntentTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "intentName": str,
-        "intentVersion": str,
+        "key": str,
+        "value": str,
     },
 )
 
-_RequiredKendraConfigurationTypeDef = TypedDict(
-    "_RequiredKendraConfigurationTypeDef",
+_RequiredMessageTypeDef = TypedDict(
+    "_RequiredMessageTypeDef",
     {
-        "kendraIndex": str,
-        "role": str,
+        "contentType": ContentTypeType,
+        "content": str,
     },
 )
-_OptionalKendraConfigurationTypeDef = TypedDict(
-    "_OptionalKendraConfigurationTypeDef",
+_OptionalMessageTypeDef = TypedDict(
+    "_OptionalMessageTypeDef",
     {
-        "queryFilterString": str,
+        "groupNumber": int,
     },
     total=False,
 )
 
-class KendraConfigurationTypeDef(
-    _RequiredKendraConfigurationTypeDef, _OptionalKendraConfigurationTypeDef
-):
+
+class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
     pass
 
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
+
+SlotDefaultValueTypeDef = TypedDict(
+    "SlotDefaultValueTypeDef",
+    {
+        "defaultValue": str,
+    },
+)
+
+SlotTypeRegexConfigurationTypeDef = TypedDict(
+    "SlotTypeRegexConfigurationTypeDef",
+    {
+        "pattern": str,
+    },
+)
+
+StartMigrationRequestRequestTypeDef = TypedDict(
+    "StartMigrationRequestRequestTypeDef",
+    {
+        "v1BotName": str,
+        "v1BotVersion": str,
+        "v2BotName": str,
+        "v2BotRole": str,
+        "migrationStrategy": MigrationStrategyType,
+    },
+)
+
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+UtteranceDataTypeDef = TypedDict(
+    "UtteranceDataTypeDef",
     {
-        "key": str,
-        "value": str,
+        "utteranceString": str,
+        "count": int,
+        "distinctUsers": int,
+        "firstUtteredDate": datetime,
+        "lastUtteredDate": datetime,
     },
+    total=False,
 )
 
-_RequiredMessageOutputTypeDef = TypedDict(
-    "_RequiredMessageOutputTypeDef",
+_RequiredFulfillmentActivityTypeDef = TypedDict(
+    "_RequiredFulfillmentActivityTypeDef",
     {
-        "contentType": ContentTypeType,
-        "content": str,
+        "type": FulfillmentActivityTypeType,
     },
 )
-_OptionalMessageOutputTypeDef = TypedDict(
-    "_OptionalMessageOutputTypeDef",
+_OptionalFulfillmentActivityTypeDef = TypedDict(
+    "_OptionalFulfillmentActivityTypeDef",
     {
-        "groupNumber": int,
+        "codeHook": CodeHookTypeDef,
     },
     total=False,
 )
 
-class MessageOutputTypeDef(_RequiredMessageOutputTypeDef, _OptionalMessageOutputTypeDef):
+
+class FulfillmentActivityTypeDef(
+    _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
+):
     pass
 
-_RequiredMessageTypeDef = TypedDict(
-    "_RequiredMessageTypeDef",
+
+ConversationLogsRequestTypeDef = TypedDict(
+    "ConversationLogsRequestTypeDef",
     {
-        "contentType": ContentTypeType,
-        "content": str,
+        "logSettings": Sequence[LogSettingsRequestTypeDef],
+        "iamRoleArn": str,
     },
 )
-_OptionalMessageTypeDef = TypedDict(
-    "_OptionalMessageTypeDef",
+
+ConversationLogsResponseTypeDef = TypedDict(
+    "ConversationLogsResponseTypeDef",
     {
-        "groupNumber": int,
+        "logSettings": List[LogSettingsResponseTypeDef],
+        "iamRoleArn": str,
     },
     total=False,
 )
 
-class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
-    pass
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-OutputContextTypeDef = TypedDict(
-    "OutputContextTypeDef",
+GetBotChannelAssociationResponseTypeDef = TypedDict(
+    "GetBotChannelAssociationResponseTypeDef",
     {
         "name": str,
-        "timeToLiveInSeconds": int,
-        "turnsToLive": int,
+        "description": str,
+        "botAlias": str,
+        "botName": str,
+        "createdDate": datetime,
+        "type": ChannelTypeType,
+        "botConfiguration": Dict[str, str],
+        "status": ChannelStatusType,
+        "failureReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetBotChannelAssociationsResponseTypeDef = TypedDict(
+    "GetBotChannelAssociationsResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "botChannelAssociations": List[BotChannelAssociationTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+GetBotVersionsResponseTypeDef = TypedDict(
+    "GetBotVersionsResponseTypeDef",
     {
-        "key": str,
-        "value": str,
+        "bots": List[BotMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetBotsResponseTypeDef = TypedDict(
+    "GetBotsResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "bots": List[BotMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SlotDefaultValueOutputTypeDef = TypedDict(
-    "SlotDefaultValueOutputTypeDef",
+GetBuiltinIntentResponseTypeDef = TypedDict(
+    "GetBuiltinIntentResponseTypeDef",
     {
-        "defaultValue": str,
+        "signature": str,
+        "supportedLocales": List[LocaleType],
+        "slots": List[BuiltinIntentSlotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SlotDefaultValueTypeDef = TypedDict(
-    "SlotDefaultValueTypeDef",
+GetBuiltinIntentsResponseTypeDef = TypedDict(
+    "GetBuiltinIntentsResponseTypeDef",
     {
-        "defaultValue": str,
+        "intents": List[BuiltinIntentMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SlotTypeRegexConfigurationOutputTypeDef = TypedDict(
-    "SlotTypeRegexConfigurationOutputTypeDef",
+GetBuiltinSlotTypesResponseTypeDef = TypedDict(
+    "GetBuiltinSlotTypesResponseTypeDef",
     {
-        "pattern": str,
+        "slotTypes": List[BuiltinSlotTypeMetadataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SlotTypeRegexConfigurationTypeDef = TypedDict(
-    "SlotTypeRegexConfigurationTypeDef",
+GetExportResponseTypeDef = TypedDict(
+    "GetExportResponseTypeDef",
     {
-        "pattern": str,
+        "name": str,
+        "version": str,
+        "resourceType": ResourceTypeType,
+        "exportType": ExportTypeType,
+        "exportStatus": ExportStatusType,
+        "failureReason": str,
+        "url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartMigrationRequestRequestTypeDef = TypedDict(
-    "StartMigrationRequestRequestTypeDef",
+GetImportResponseTypeDef = TypedDict(
+    "GetImportResponseTypeDef",
     {
-        "v1BotName": str,
-        "v1BotVersion": str,
-        "v2BotName": str,
-        "v2BotRole": str,
-        "migrationStrategy": MigrationStrategyType,
+        "name": str,
+        "resourceType": ResourceTypeType,
+        "mergeStrategy": MergeStrategyType,
+        "importId": str,
+        "importStatus": ImportStatusType,
+        "failureReason": List[str],
+        "createdDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMigrationResponseTypeDef = TypedDict(
     "StartMigrationResponseTypeDef",
     {
         "v1BotName": str,
         "v1BotVersion": str,
         "v1BotLocale": LocaleType,
         "v2BotId": str,
         "v2BotRole": str,
         "migrationId": str,
         "migrationStrategy": MigrationStrategyType,
         "migrationTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
+    "_RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "botName": str,
     },
 )
-
-UtteranceDataTypeDef = TypedDict(
-    "UtteranceDataTypeDef",
+_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef = TypedDict(
+    "_OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef",
     {
-        "utteranceString": str,
-        "count": int,
-        "distinctUsers": int,
-        "firstUtteredDate": datetime,
-        "lastUtteredDate": datetime,
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-GetBotChannelAssociationsResponseTypeDef = TypedDict(
-    "GetBotChannelAssociationsResponseTypeDef",
+
+class GetBotAliasesRequestGetBotAliasesPaginateTypeDef(
+    _RequiredGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    _OptionalGetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     {
-        "botChannelAssociations": List[BotChannelAssociationTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "botName": str,
+        "botAlias": str,
     },
 )
-
-GetBotVersionsResponseTypeDef = TypedDict(
-    "GetBotVersionsResponseTypeDef",
+_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef",
     {
-        "bots": List[BotMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetBotsResponseTypeDef = TypedDict(
-    "GetBotsResponseTypeDef",
+
+class GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef(
+    _RequiredGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+    _OptionalGetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
     {
-        "bots": List[BotMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
     },
 )
+_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-GetBuiltinIntentsResponseTypeDef = TypedDict(
-    "GetBuiltinIntentsResponseTypeDef",
+
+class GetBotVersionsRequestGetBotVersionsPaginateTypeDef(
+    _RequiredGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+    _OptionalGetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+):
+    pass
+
+
+GetBotsRequestGetBotsPaginateTypeDef = TypedDict(
+    "GetBotsRequestGetBotsPaginateTypeDef",
     {
-        "intents": List[BuiltinIntentMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetBuiltinIntentResponseTypeDef = TypedDict(
-    "GetBuiltinIntentResponseTypeDef",
+GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = TypedDict(
+    "GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef",
     {
-        "signature": str,
-        "supportedLocales": List[LocaleType],
-        "slots": List[BuiltinIntentSlotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "locale": LocaleType,
+        "signatureContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetBuiltinSlotTypesResponseTypeDef = TypedDict(
-    "GetBuiltinSlotTypesResponseTypeDef",
+GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = TypedDict(
+    "GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef",
     {
-        "slotTypes": List[BuiltinSlotTypeMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "locale": LocaleType,
+        "signatureContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredFulfillmentActivityOutputTypeDef = TypedDict(
-    "_RequiredFulfillmentActivityOutputTypeDef",
+_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
     {
-        "type": FulfillmentActivityTypeType,
+        "name": str,
     },
 )
-_OptionalFulfillmentActivityOutputTypeDef = TypedDict(
-    "_OptionalFulfillmentActivityOutputTypeDef",
+_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef",
     {
-        "codeHook": CodeHookOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class FulfillmentActivityOutputTypeDef(
-    _RequiredFulfillmentActivityOutputTypeDef, _OptionalFulfillmentActivityOutputTypeDef
+
+class GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef(
+    _RequiredGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+    _OptionalGetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
 ):
     pass
 
-_RequiredFulfillmentActivityTypeDef = TypedDict(
-    "_RequiredFulfillmentActivityTypeDef",
+
+GetIntentsRequestGetIntentsPaginateTypeDef = TypedDict(
+    "GetIntentsRequestGetIntentsPaginateTypeDef",
     {
-        "type": FulfillmentActivityTypeType,
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalFulfillmentActivityTypeDef = TypedDict(
-    "_OptionalFulfillmentActivityTypeDef",
+
+_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
+    "_RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
     {
-        "codeHook": CodeHookTypeDef,
+        "name": str,
+    },
+)
+_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = TypedDict(
+    "_OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class FulfillmentActivityTypeDef(
-    _RequiredFulfillmentActivityTypeDef, _OptionalFulfillmentActivityTypeDef
+
+class GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef(
+    _RequiredGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+    _OptionalGetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
 ):
     pass
 
-ConversationLogsRequestTypeDef = TypedDict(
-    "ConversationLogsRequestTypeDef",
-    {
-        "logSettings": Sequence[LogSettingsRequestTypeDef],
-        "iamRoleArn": str,
-    },
-)
 
-ConversationLogsResponseTypeDef = TypedDict(
-    "ConversationLogsResponseTypeDef",
+GetSlotTypesRequestGetSlotTypesPaginateTypeDef = TypedDict(
+    "GetSlotTypesRequestGetSlotTypesPaginateTypeDef",
     {
-        "logSettings": List[LogSettingsResponseTypeDef],
-        "iamRoleArn": str,
+        "nameContains": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetIntentVersionsResponseTypeDef = TypedDict(
     "GetIntentVersionsResponseTypeDef",
     {
         "intents": List[IntentMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntentsResponseTypeDef = TypedDict(
     "GetIntentsResponseTypeDef",
     {
         "intents": List[IntentMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMigrationResponseTypeDef = TypedDict(
     "GetMigrationResponseTypeDef",
     {
         "migrationId": str,
@@ -1338,101 +1255,117 @@
         "v1BotLocale": LocaleType,
         "v2BotId": str,
         "v2BotRole": str,
         "migrationStatus": MigrationStatusType,
         "migrationStrategy": MigrationStrategyType,
         "migrationTimestamp": datetime,
         "alerts": List[MigrationAlertTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMigrationsResponseTypeDef = TypedDict(
     "GetMigrationsResponseTypeDef",
     {
         "migrationSummaries": List[MigrationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSlotTypeVersionsResponseTypeDef = TypedDict(
     "GetSlotTypeVersionsResponseTypeDef",
     {
         "slotTypes": List[SlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSlotTypesResponseTypeDef = TypedDict(
     "GetSlotTypesResponseTypeDef",
     {
         "slotTypes": List[SlotTypeMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartImportRequestRequestTypeDef = TypedDict(
+    "_RequiredStartImportRequestRequestTypeDef",
+    {
+        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "resourceType": ResourceTypeType,
+        "mergeStrategy": MergeStrategyType,
+    },
+)
+_OptionalStartImportRequestRequestTypeDef = TypedDict(
+    "_OptionalStartImportRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class StartImportRequestRequestTypeDef(
+    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
+):
+    pass
+
+
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "name": str,
         "resourceType": ResourceTypeType,
         "mergeStrategy": MergeStrategyType,
         "importId": str,
         "importStatus": ImportStatusType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
     },
 )
 
 _RequiredPromptOutputTypeDef = TypedDict(
     "_RequiredPromptOutputTypeDef",
     {
-        "messages": List[MessageOutputTypeDef],
+        "messages": List[MessageTypeDef],
         "maxAttempts": int,
     },
 )
 _OptionalPromptOutputTypeDef = TypedDict(
     "_OptionalPromptOutputTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
+
 class PromptOutputTypeDef(_RequiredPromptOutputTypeDef, _OptionalPromptOutputTypeDef):
     pass
 
-_RequiredStatementOutputTypeDef = TypedDict(
-    "_RequiredStatementOutputTypeDef",
-    {
-        "messages": List[MessageOutputTypeDef],
-    },
-)
-_OptionalStatementOutputTypeDef = TypedDict(
-    "_OptionalStatementOutputTypeDef",
-    {
-        "responseCard": str,
-    },
-    total=False,
-)
-
-class StatementOutputTypeDef(_RequiredStatementOutputTypeDef, _OptionalStatementOutputTypeDef):
-    pass
 
 _RequiredPromptTypeDef = TypedDict(
     "_RequiredPromptTypeDef",
     {
         "messages": Sequence[MessageTypeDef],
         "maxAttempts": int,
     },
@@ -1441,85 +1374,71 @@
     "_OptionalPromptTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
+
 class PromptTypeDef(_RequiredPromptTypeDef, _OptionalPromptTypeDef):
     pass
 
-_RequiredStatementTypeDef = TypedDict(
-    "_RequiredStatementTypeDef",
+
+_RequiredStatementOutputTypeDef = TypedDict(
+    "_RequiredStatementOutputTypeDef",
     {
-        "messages": Sequence[MessageTypeDef],
+        "messages": List[MessageTypeDef],
     },
 )
-_OptionalStatementTypeDef = TypedDict(
-    "_OptionalStatementTypeDef",
+_OptionalStatementOutputTypeDef = TypedDict(
+    "_OptionalStatementOutputTypeDef",
     {
         "responseCard": str,
     },
     total=False,
 )
 
-class StatementTypeDef(_RequiredStatementTypeDef, _OptionalStatementTypeDef):
+
+class StatementOutputTypeDef(_RequiredStatementOutputTypeDef, _OptionalStatementOutputTypeDef):
     pass
 
-_RequiredStartImportRequestRequestTypeDef = TypedDict(
-    "_RequiredStartImportRequestRequestTypeDef",
+
+_RequiredStatementTypeDef = TypedDict(
+    "_RequiredStatementTypeDef",
     {
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
-        "resourceType": ResourceTypeType,
-        "mergeStrategy": MergeStrategyType,
+        "messages": Sequence[MessageTypeDef],
     },
 )
-_OptionalStartImportRequestRequestTypeDef = TypedDict(
-    "_OptionalStartImportRequestRequestTypeDef",
+_OptionalStatementTypeDef = TypedDict(
+    "_OptionalStatementTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "responseCard": str,
     },
     total=False,
 )
 
-class StartImportRequestRequestTypeDef(
-    _RequiredStartImportRequestRequestTypeDef, _OptionalStartImportRequestRequestTypeDef
-):
+
+class StatementTypeDef(_RequiredStatementTypeDef, _OptionalStatementTypeDef):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
-    },
-)
 
 SlotDefaultValueSpecOutputTypeDef = TypedDict(
     "SlotDefaultValueSpecOutputTypeDef",
     {
-        "defaultValueList": List[SlotDefaultValueOutputTypeDef],
+        "defaultValueList": List[SlotDefaultValueTypeDef],
     },
 )
 
 SlotDefaultValueSpecTypeDef = TypedDict(
     "SlotDefaultValueSpecTypeDef",
     {
         "defaultValueList": Sequence[SlotDefaultValueTypeDef],
     },
 )
 
-SlotTypeConfigurationOutputTypeDef = TypedDict(
-    "SlotTypeConfigurationOutputTypeDef",
-    {
-        "regexConfiguration": SlotTypeRegexConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 SlotTypeConfigurationTypeDef = TypedDict(
     "SlotTypeConfigurationTypeDef",
     {
         "regexConfiguration": SlotTypeRegexConfigurationTypeDef,
     },
     total=False,
 )
@@ -1548,19 +1467,21 @@
         "checksum": str,
         "conversationLogs": ConversationLogsRequestTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutBotAliasRequestRequestTypeDef(
     _RequiredPutBotAliasRequestRequestTypeDef, _OptionalPutBotAliasRequestRequestTypeDef
 ):
     pass
 
+
 BotAliasMetadataTypeDef = TypedDict(
     "BotAliasMetadataTypeDef",
     {
         "name": str,
         "description": str,
         "botVersion": str,
         "botName": str,
@@ -1579,55 +1500,55 @@
         "description": str,
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBotAliasResponseTypeDef = TypedDict(
     "PutBotAliasResponseTypeDef",
     {
         "name": str,
         "description": str,
         "botVersion": str,
         "botName": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "checksum": str,
         "conversationLogs": ConversationLogsResponseTypeDef,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBotVersionResponseTypeDef = TypedDict(
     "CreateBotVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "intents": List[IntentOutputTypeDef],
+        "intents": List[IntentTypeDef],
         "clarificationPrompt": PromptOutputTypeDef,
         "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "enableModelImprovements": bool,
         "detectSentiment": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FollowUpPromptOutputTypeDef = TypedDict(
     "FollowUpPromptOutputTypeDef",
     {
         "prompt": PromptOutputTypeDef,
@@ -1636,15 +1557,15 @@
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "intents": List[IntentOutputTypeDef],
+        "intents": List[IntentTypeDef],
         "enableModelImprovements": bool,
         "nluIntentConfidenceThreshold": float,
         "clarificationPrompt": PromptOutputTypeDef,
         "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
@@ -1652,24 +1573,24 @@
         "idleSessionTTLInSeconds": int,
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "detectSentiment": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBotResponseTypeDef = TypedDict(
     "PutBotResponseTypeDef",
     {
         "name": str,
         "description": str,
-        "intents": List[IntentOutputTypeDef],
+        "intents": List[IntentTypeDef],
         "enableModelImprovements": bool,
         "nluIntentConfidenceThreshold": float,
         "clarificationPrompt": PromptOutputTypeDef,
         "abortStatement": StatementOutputTypeDef,
         "status": StatusType,
         "failureReason": str,
         "lastUpdatedDate": datetime,
@@ -1678,16 +1599,16 @@
         "voiceId": str,
         "checksum": str,
         "version": str,
         "locale": LocaleType,
         "childDirected": bool,
         "createVersion": bool,
         "detectSentiment": bool,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FollowUpPromptTypeDef = TypedDict(
     "FollowUpPromptTypeDef",
     {
         "prompt": PromptTypeDef,
@@ -1719,19 +1640,21 @@
         "detectSentiment": bool,
         "createVersion": bool,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutBotRequestRequestTypeDef(
     _RequiredPutBotRequestRequestTypeDef, _OptionalPutBotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSlotOutputTypeDef = TypedDict(
     "_RequiredSlotOutputTypeDef",
     {
         "name": str,
         "slotConstraint": SlotConstraintType,
     },
 )
@@ -1747,17 +1670,19 @@
         "responseCard": str,
         "obfuscationSetting": ObfuscationSettingType,
         "defaultValueSpec": SlotDefaultValueSpecOutputTypeDef,
     },
     total=False,
 )
 
+
 class SlotOutputTypeDef(_RequiredSlotOutputTypeDef, _OptionalSlotOutputTypeDef):
     pass
 
+
 _RequiredSlotTypeDef = TypedDict(
     "_RequiredSlotTypeDef",
     {
         "name": str,
         "slotConstraint": SlotConstraintType,
     },
 )
@@ -1773,31 +1698,33 @@
         "responseCard": str,
         "obfuscationSetting": ObfuscationSettingType,
         "defaultValueSpec": SlotDefaultValueSpecTypeDef,
     },
     total=False,
 )
 
+
 class SlotTypeDef(_RequiredSlotTypeDef, _OptionalSlotTypeDef):
     pass
 
+
 CreateSlotTypeVersionResponseTypeDef = TypedDict(
     "CreateSlotTypeVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
         "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
-        "slotTypeConfigurations": List[SlotTypeConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSlotTypeResponseTypeDef = TypedDict(
     "GetSlotTypeResponseTypeDef",
     {
         "name": str,
@@ -1805,34 +1732,16 @@
         "enumerationValues": List[EnumerationValueOutputTypeDef],
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "valueSelectionStrategy": SlotValueSelectionStrategyType,
         "parentSlotTypeSignature": str,
-        "slotTypeConfigurations": List[SlotTypeConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutSlotTypeResponseTypeDef = TypedDict(
-    "PutSlotTypeResponseTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "enumerationValues": List[EnumerationValueOutputTypeDef],
-        "lastUpdatedDate": datetime,
-        "createdDate": datetime,
-        "version": str,
-        "checksum": str,
-        "valueSelectionStrategy": SlotValueSelectionStrategyType,
-        "createVersion": bool,
-        "parentSlotTypeSignature": str,
-        "slotTypeConfigurations": List[SlotTypeConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutSlotTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutSlotTypeRequestRequestTypeDef",
     {
         "name": str,
@@ -1848,110 +1757,130 @@
         "createVersion": bool,
         "parentSlotTypeSignature": str,
         "slotTypeConfigurations": Sequence[SlotTypeConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class PutSlotTypeRequestRequestTypeDef(
     _RequiredPutSlotTypeRequestRequestTypeDef, _OptionalPutSlotTypeRequestRequestTypeDef
 ):
     pass
 
+
+PutSlotTypeResponseTypeDef = TypedDict(
+    "PutSlotTypeResponseTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "enumerationValues": List[EnumerationValueOutputTypeDef],
+        "lastUpdatedDate": datetime,
+        "createdDate": datetime,
+        "version": str,
+        "checksum": str,
+        "valueSelectionStrategy": SlotValueSelectionStrategyType,
+        "createVersion": bool,
+        "parentSlotTypeSignature": str,
+        "slotTypeConfigurations": List[SlotTypeConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetUtterancesViewResponseTypeDef = TypedDict(
     "GetUtterancesViewResponseTypeDef",
     {
         "botName": str,
         "utterances": List[UtteranceListTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBotAliasesResponseTypeDef = TypedDict(
     "GetBotAliasesResponseTypeDef",
     {
         "BotAliases": List[BotAliasMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateIntentVersionResponseTypeDef = TypedDict(
     "CreateIntentVersionResponseTypeDef",
     {
         "name": str,
         "description": str,
         "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
         "confirmationPrompt": PromptOutputTypeDef,
         "rejectionStatement": StatementOutputTypeDef,
         "followUpPrompt": FollowUpPromptOutputTypeDef,
         "conclusionStatement": StatementOutputTypeDef,
-        "dialogCodeHook": CodeHookOutputTypeDef,
-        "fulfillmentActivity": FulfillmentActivityOutputTypeDef,
+        "dialogCodeHook": CodeHookTypeDef,
+        "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
-        "kendraConfiguration": KendraConfigurationOutputTypeDef,
-        "inputContexts": List[InputContextOutputTypeDef],
-        "outputContexts": List[OutputContextOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "kendraConfiguration": KendraConfigurationTypeDef,
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntentResponseTypeDef = TypedDict(
     "GetIntentResponseTypeDef",
     {
         "name": str,
         "description": str,
         "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
         "confirmationPrompt": PromptOutputTypeDef,
         "rejectionStatement": StatementOutputTypeDef,
         "followUpPrompt": FollowUpPromptOutputTypeDef,
         "conclusionStatement": StatementOutputTypeDef,
-        "dialogCodeHook": CodeHookOutputTypeDef,
-        "fulfillmentActivity": FulfillmentActivityOutputTypeDef,
+        "dialogCodeHook": CodeHookTypeDef,
+        "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
-        "kendraConfiguration": KendraConfigurationOutputTypeDef,
-        "inputContexts": List[InputContextOutputTypeDef],
-        "outputContexts": List[OutputContextOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "kendraConfiguration": KendraConfigurationTypeDef,
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutIntentResponseTypeDef = TypedDict(
     "PutIntentResponseTypeDef",
     {
         "name": str,
         "description": str,
         "slots": List[SlotOutputTypeDef],
         "sampleUtterances": List[str],
         "confirmationPrompt": PromptOutputTypeDef,
         "rejectionStatement": StatementOutputTypeDef,
         "followUpPrompt": FollowUpPromptOutputTypeDef,
         "conclusionStatement": StatementOutputTypeDef,
-        "dialogCodeHook": CodeHookOutputTypeDef,
-        "fulfillmentActivity": FulfillmentActivityOutputTypeDef,
+        "dialogCodeHook": CodeHookTypeDef,
+        "fulfillmentActivity": FulfillmentActivityTypeDef,
         "parentIntentSignature": str,
         "lastUpdatedDate": datetime,
         "createdDate": datetime,
         "version": str,
         "checksum": str,
         "createVersion": bool,
-        "kendraConfiguration": KendraConfigurationOutputTypeDef,
-        "inputContexts": List[InputContextOutputTypeDef],
-        "outputContexts": List[OutputContextOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "kendraConfiguration": KendraConfigurationTypeDef,
+        "inputContexts": List[InputContextTypeDef],
+        "outputContexts": List[OutputContextTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutIntentRequestRequestTypeDef = TypedDict(
     "_RequiredPutIntentRequestRequestTypeDef",
     {
         "name": str,
@@ -1975,11 +1904,12 @@
         "kendraConfiguration": KendraConfigurationTypeDef,
         "inputContexts": Sequence[InputContextTypeDef],
         "outputContexts": Sequence[OutputContextTypeDef],
     },
     total=False,
 )
 
+
 class PutIntentRequestRequestTypeDef(
     _RequiredPutIntentRequestRequestTypeDef, _OptionalPutIntentRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/PKG-INFO` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-models
-Version: 1.28.12
-Summary: Type annotations for boto3.LexModelBuildingService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LexModelBuildingService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-models.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-models)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-models)](https://pepy.tech/project/mypy-boto3-lex-models)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexModelBuildingService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
+[boto3.LexModelBuildingService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
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
 [mypy-boto3-lex-models docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_models/).
 
 See how it helps to find and fix potential bugs:
 
@@ -386,121 +386,110 @@
 ```python
 from mypy_boto3_lex_models.type_defs import (
     BotChannelAssociationTypeDef,
     BotMetadataTypeDef,
     BuiltinIntentMetadataTypeDef,
     BuiltinIntentSlotTypeDef,
     BuiltinSlotTypeMetadataTypeDef,
-    CodeHookOutputTypeDef,
     CodeHookTypeDef,
     LogSettingsRequestTypeDef,
     LogSettingsResponseTypeDef,
     CreateBotVersionRequestRequestTypeDef,
-    IntentOutputTypeDef,
+    IntentTypeDef,
+    ResponseMetadataTypeDef,
     CreateIntentVersionRequestRequestTypeDef,
-    InputContextOutputTypeDef,
-    KendraConfigurationOutputTypeDef,
-    OutputContextOutputTypeDef,
+    InputContextTypeDef,
+    KendraConfigurationTypeDef,
+    OutputContextTypeDef,
     CreateSlotTypeVersionRequestRequestTypeDef,
     EnumerationValueOutputTypeDef,
     DeleteBotAliasRequestRequestTypeDef,
     DeleteBotChannelAssociationRequestRequestTypeDef,
     DeleteBotRequestRequestTypeDef,
     DeleteBotVersionRequestRequestTypeDef,
     DeleteIntentRequestRequestTypeDef,
     DeleteIntentVersionRequestRequestTypeDef,
     DeleteSlotTypeRequestRequestTypeDef,
     DeleteSlotTypeVersionRequestRequestTypeDef,
     DeleteUtterancesRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnumerationValueTypeDef,
     GetBotAliasRequestRequestTypeDef,
-    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetBotAliasesRequestRequestTypeDef,
     GetBotChannelAssociationRequestRequestTypeDef,
-    GetBotChannelAssociationResponseTypeDef,
-    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
     GetBotChannelAssociationsRequestRequestTypeDef,
     GetBotRequestRequestTypeDef,
-    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
     GetBotVersionsRequestRequestTypeDef,
-    GetBotsRequestGetBotsPaginateTypeDef,
     GetBotsRequestRequestTypeDef,
     GetBuiltinIntentRequestRequestTypeDef,
-    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
     GetBuiltinIntentsRequestRequestTypeDef,
-    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
     GetBuiltinSlotTypesRequestRequestTypeDef,
     GetExportRequestRequestTypeDef,
-    GetExportResponseTypeDef,
     GetImportRequestRequestTypeDef,
-    GetImportResponseTypeDef,
     GetIntentRequestRequestTypeDef,
-    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
     GetIntentVersionsRequestRequestTypeDef,
     IntentMetadataTypeDef,
-    GetIntentsRequestGetIntentsPaginateTypeDef,
     GetIntentsRequestRequestTypeDef,
     GetMigrationRequestRequestTypeDef,
     MigrationAlertTypeDef,
     GetMigrationsRequestRequestTypeDef,
     MigrationSummaryTypeDef,
     GetSlotTypeRequestRequestTypeDef,
-    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
     GetSlotTypeVersionsRequestRequestTypeDef,
     SlotTypeMetadataTypeDef,
-    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetSlotTypesRequestRequestTypeDef,
     GetUtterancesViewRequestRequestTypeDef,
-    InputContextTypeDef,
-    IntentTypeDef,
-    KendraConfigurationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    MessageOutputTypeDef,
-    MessageTypeDef,
-    OutputContextTypeDef,
-    PaginatorConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
-    SlotDefaultValueOutputTypeDef,
+    MessageTypeDef,
     SlotDefaultValueTypeDef,
-    SlotTypeRegexConfigurationOutputTypeDef,
     SlotTypeRegexConfigurationTypeDef,
     StartMigrationRequestRequestTypeDef,
-    StartMigrationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UtteranceDataTypeDef,
+    FulfillmentActivityTypeDef,
+    ConversationLogsRequestTypeDef,
+    ConversationLogsResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetBotChannelAssociationResponseTypeDef,
     GetBotChannelAssociationsResponseTypeDef,
     GetBotVersionsResponseTypeDef,
     GetBotsResponseTypeDef,
-    GetBuiltinIntentsResponseTypeDef,
     GetBuiltinIntentResponseTypeDef,
+    GetBuiltinIntentsResponseTypeDef,
     GetBuiltinSlotTypesResponseTypeDef,
-    FulfillmentActivityOutputTypeDef,
-    FulfillmentActivityTypeDef,
-    ConversationLogsRequestTypeDef,
-    ConversationLogsResponseTypeDef,
+    GetExportResponseTypeDef,
+    GetImportResponseTypeDef,
+    StartMigrationResponseTypeDef,
+    GetBotAliasesRequestGetBotAliasesPaginateTypeDef,
+    GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef,
+    GetBotVersionsRequestGetBotVersionsPaginateTypeDef,
+    GetBotsRequestGetBotsPaginateTypeDef,
+    GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef,
+    GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef,
+    GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef,
+    GetIntentsRequestGetIntentsPaginateTypeDef,
+    GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef,
+    GetSlotTypesRequestGetSlotTypesPaginateTypeDef,
     GetIntentVersionsResponseTypeDef,
     GetIntentsResponseTypeDef,
     GetMigrationResponseTypeDef,
     GetMigrationsResponseTypeDef,
     GetSlotTypeVersionsResponseTypeDef,
     GetSlotTypesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     PromptOutputTypeDef,
-    StatementOutputTypeDef,
     PromptTypeDef,
+    StatementOutputTypeDef,
     StatementTypeDef,
-    StartImportRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     SlotDefaultValueSpecOutputTypeDef,
     SlotDefaultValueSpecTypeDef,
-    SlotTypeConfigurationOutputTypeDef,
     SlotTypeConfigurationTypeDef,
     UtteranceListTypeDef,
     PutBotAliasRequestRequestTypeDef,
     BotAliasMetadataTypeDef,
     GetBotAliasResponseTypeDef,
     PutBotAliasResponseTypeDef,
     CreateBotVersionResponseTypeDef,
@@ -509,16 +498,16 @@
     PutBotResponseTypeDef,
     FollowUpPromptTypeDef,
     PutBotRequestRequestTypeDef,
     SlotOutputTypeDef,
     SlotTypeDef,
     CreateSlotTypeVersionResponseTypeDef,
     GetSlotTypeResponseTypeDef,
-    PutSlotTypeResponseTypeDef,
     PutSlotTypeRequestRequestTypeDef,
+    PutSlotTypeResponseTypeDef,
     GetUtterancesViewResponseTypeDef,
     GetBotAliasesResponseTypeDef,
     CreateIntentVersionResponseTypeDef,
     GetIntentResponseTypeDef,
     PutIntentResponseTypeDef,
     PutIntentRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-lex-models-1.28.12/mypy_boto3_lex_models.egg-info/SOURCES.txt` & `mypy-boto3-lex-models-1.28.15/mypy_boto3_lex_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-models-1.28.12/setup.py` & `mypy-boto3-lex-models-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lex-models",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_lex_models"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexModelBuildingService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.LexModelBuildingService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

