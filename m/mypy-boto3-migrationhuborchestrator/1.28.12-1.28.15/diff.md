# Comparing `tmp/mypy-boto3-migrationhuborchestrator-1.28.12.tar.gz` & `tmp/mypy-boto3-migrationhuborchestrator-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhuborchestrator-1.28.12.tar", last modified: Thu Jul 27 05:35:03 2023, max compression
+gzip compressed data, was "mypy-boto3-migrationhuborchestrator-1.28.15.tar", last modified: Fri Jul 28 20:43:20 2023, max compression
```

## Comparing `mypy-boto3-migrationhuborchestrator-1.28.12.tar` & `mypy-boto3-migrationhuborchestrator-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.860431 mypy-boto3-migrationhuborchestrator-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-07-27 05:35:03.860431 mypy-boto3-migrationhuborchestrator-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.852431 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25168 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9380 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33023 2023-07-27 05:26:42.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32995 2023-07-27 05:26:42.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.860431 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18188 2023-07-27 05:35:03.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-27 05:35:03.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:03.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 05:35:03.000000 mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:03.860431 mypy-boto3-migrationhuborchestrator-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-27 05:26:41.000000 mypy-boto3-migrationhuborchestrator-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:20.233542 mypy-boto3-migrationhuborchestrator-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-07-28 20:43:20.233542 mypy-boto3-migrationhuborchestrator-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:20.221542 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25168 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25126 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-28 20:32:04.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-28 20:32:04.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32109 2023-07-28 20:32:05.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-07-28 20:32:04.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:20.233542 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-07-28 20:43:20.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-28 20:43:20.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:20.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-28 20:43:20.000000 mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:20.233542 mypy-boto3-migrationhuborchestrator-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-28 20:32:03.000000 mypy-boto3-migrationhuborchestrator-1.28.15/setup.py
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/LICENSE` & `mypy-boto3-migrationhuborchestrator-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/PKG-INFO` & `mypy-boto3-migrationhuborchestrator-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhuborchestrator
-Version: 1.28.12
-Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhuborchestrator)](https://pepy.tech/project/mypy-boto3-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubOrchestrator 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[boto3.MigrationHubOrchestrator 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,89 +359,86 @@
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
     StepInputTypeDef,
+    ResponseMetadataTypeDef,
     StepInputOutputTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
-    CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
-    DeleteMigrationWorkflowResponseTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
     GetMigrationWorkflowRequestRequestTypeDef,
     GetMigrationWorkflowTemplateRequestRequestTypeDef,
     TemplateInputTypeDef,
     GetTemplateStepGroupRequestRequestTypeDef,
     GetTemplateStepRequestRequestTypeDef,
     StepOutputTypeDef,
     GetWorkflowStepGroupRequestRequestTypeDef,
     GetWorkflowStepRequestRequestTypeDef,
-    ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMigrationWorkflowTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
-    ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListMigrationWorkflowsRequestRequestTypeDef,
     MigrationWorkflowSummaryTypeDef,
-    ListPluginsRequestListPluginsPaginateTypeDef,
     ListPluginsRequestRequestTypeDef,
     PluginSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
     ListTemplateStepGroupsRequestRequestTypeDef,
     TemplateStepGroupSummaryTypeDef,
-    ListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
     ListTemplateStepsRequestRequestTypeDef,
     TemplateStepSummaryTypeDef,
-    ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
     ListWorkflowStepGroupsRequestRequestTypeDef,
     WorkflowStepGroupSummaryTypeDef,
-    ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListWorkflowStepsRequestRequestTypeDef,
     WorkflowStepSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    PlatformCommandOutputTypeDef,
     PlatformCommandTypeDef,
-    PlatformScriptKeyOutputTypeDef,
     PlatformScriptKeyTypeDef,
-    ResponseMetadataTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
-    RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
-    StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
-    StopMigrationWorkflowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
-    UpdateWorkflowStepResponseTypeDef,
     WorkflowStepOutputUnionTypeDef,
     CreateMigrationWorkflowRequestRequestTypeDef,
     UpdateMigrationWorkflowRequestRequestTypeDef,
+    CreateWorkflowStepResponseTypeDef,
+    DeleteMigrationWorkflowResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RetryWorkflowStepResponseTypeDef,
+    StartMigrationWorkflowResponseTypeDef,
+    StopMigrationWorkflowResponseTypeDef,
+    UpdateWorkflowStepResponseTypeDef,
     CreateMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
+    ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
+    ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef,
+    ListPluginsRequestListPluginsPaginateTypeDef,
+    ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
+    ListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
+    ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
+    ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListMigrationWorkflowTemplatesResponseTypeDef,
     ListMigrationWorkflowsResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     StepAutomationConfigurationTypeDef,
-    WorkflowStepAutomationConfigurationOutputTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
     WorkflowStepOutputTypeDef,
     GetTemplateStepResponseTypeDef,
     CreateWorkflowStepRequestRequestTypeDef,
     GetWorkflowStepResponseTypeDef,
     UpdateWorkflowStepRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/README.md` & `mypy-boto3-migrationhuborchestrator-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhuborchestrator)](https://pepy.tech/project/mypy-boto3-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubOrchestrator 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[boto3.MigrationHubOrchestrator 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,89 +327,86 @@
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
     StepInputTypeDef,
+    ResponseMetadataTypeDef,
     StepInputOutputTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
-    CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
-    DeleteMigrationWorkflowResponseTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
     GetMigrationWorkflowRequestRequestTypeDef,
     GetMigrationWorkflowTemplateRequestRequestTypeDef,
     TemplateInputTypeDef,
     GetTemplateStepGroupRequestRequestTypeDef,
     GetTemplateStepRequestRequestTypeDef,
     StepOutputTypeDef,
     GetWorkflowStepGroupRequestRequestTypeDef,
     GetWorkflowStepRequestRequestTypeDef,
-    ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMigrationWorkflowTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
-    ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListMigrationWorkflowsRequestRequestTypeDef,
     MigrationWorkflowSummaryTypeDef,
-    ListPluginsRequestListPluginsPaginateTypeDef,
     ListPluginsRequestRequestTypeDef,
     PluginSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
     ListTemplateStepGroupsRequestRequestTypeDef,
     TemplateStepGroupSummaryTypeDef,
-    ListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
     ListTemplateStepsRequestRequestTypeDef,
     TemplateStepSummaryTypeDef,
-    ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
     ListWorkflowStepGroupsRequestRequestTypeDef,
     WorkflowStepGroupSummaryTypeDef,
-    ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListWorkflowStepsRequestRequestTypeDef,
     WorkflowStepSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    PlatformCommandOutputTypeDef,
     PlatformCommandTypeDef,
-    PlatformScriptKeyOutputTypeDef,
     PlatformScriptKeyTypeDef,
-    ResponseMetadataTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
-    RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
-    StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
-    StopMigrationWorkflowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
-    UpdateWorkflowStepResponseTypeDef,
     WorkflowStepOutputUnionTypeDef,
     CreateMigrationWorkflowRequestRequestTypeDef,
     UpdateMigrationWorkflowRequestRequestTypeDef,
+    CreateWorkflowStepResponseTypeDef,
+    DeleteMigrationWorkflowResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RetryWorkflowStepResponseTypeDef,
+    StartMigrationWorkflowResponseTypeDef,
+    StopMigrationWorkflowResponseTypeDef,
+    UpdateWorkflowStepResponseTypeDef,
     CreateMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
+    ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
+    ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef,
+    ListPluginsRequestListPluginsPaginateTypeDef,
+    ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
+    ListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
+    ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
+    ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListMigrationWorkflowTemplatesResponseTypeDef,
     ListMigrationWorkflowsResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     StepAutomationConfigurationTypeDef,
-    WorkflowStepAutomationConfigurationOutputTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
     WorkflowStepOutputTypeDef,
     GetTemplateStepResponseTypeDef,
     CreateWorkflowStepRequestRequestTypeDef,
     GetWorkflowStepResponseTypeDef,
     UpdateWorkflowStepRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/__init__.py` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/__init__.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/__main__.py` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubOrchestrator 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MigrationHubOrchestrator 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator\nOther"
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

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/client.py` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/client.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/literals.py` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/literals.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/paginator.py` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -53,127 +53,118 @@
     "ListTemplateStepsPaginator",
     "ListTemplatesPaginator",
     "ListWorkflowStepGroupsPaginator",
     "ListWorkflowStepsPaginator",
     "ListWorkflowsPaginator",
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
 class ListPluginsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListPlugins)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listpluginspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPluginsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListPlugins.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listpluginspaginator)
         """
 
-
 class ListTemplateStepGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateStepGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepgroupspaginator)
     """
 
     def paginate(
-        self, *, templateId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, templateId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTemplateStepGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateStepGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepgroupspaginator)
         """
 
-
 class ListTemplateStepsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateSteps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepspaginator)
     """
 
     def paginate(
-        self, *, templateId: str, stepGroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, templateId: str, stepGroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTemplateStepsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateSteps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepspaginator)
         """
 
-
 class ListTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatespaginator)
     """
 
     def paginate(
-        self, *, name: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMigrationWorkflowTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatespaginator)
         """
 
-
 class ListWorkflowStepGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowStepGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepgroupspaginator)
     """
 
     def paginate(
-        self, *, workflowId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workflowId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkflowStepGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowStepGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepgroupspaginator)
         """
 
-
 class ListWorkflowStepsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowSteps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepspaginator)
     """
 
     def paginate(
-        self, *, workflowId: str, stepGroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workflowId: str, stepGroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkflowStepsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowSteps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepspaginator)
         """
 
-
 class ListWorkflowsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflows)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowspaginator)
     """
 
     def paginate(
         self,
         *,
         templateId: str = ...,
         adsApplicationConfigurationName: str = ...,
         status: MigrationWorkflowStatusEnumType = ...,
         name: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMigrationWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowspaginator)
         """
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/paginator.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,118 +53,127 @@
     "ListTemplateStepsPaginator",
     "ListTemplatesPaginator",
     "ListWorkflowStepGroupsPaginator",
     "ListWorkflowStepsPaginator",
     "ListWorkflowsPaginator",
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
 class ListPluginsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListPlugins)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listpluginspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPluginsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListPlugins.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listpluginspaginator)
         """
 
+
 class ListTemplateStepGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateStepGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepgroupspaginator)
     """
 
     def paginate(
-        self, *, templateId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, templateId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTemplateStepGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateStepGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepgroupspaginator)
         """
 
+
 class ListTemplateStepsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateSteps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepspaginator)
     """
 
     def paginate(
-        self, *, templateId: str, stepGroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, templateId: str, stepGroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTemplateStepsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplateSteps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatestepspaginator)
         """
 
+
 class ListTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatespaginator)
     """
 
     def paginate(
-        self, *, name: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMigrationWorkflowTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listtemplatespaginator)
         """
 
+
 class ListWorkflowStepGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowStepGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepgroupspaginator)
     """
 
     def paginate(
-        self, *, workflowId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workflowId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkflowStepGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowStepGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepgroupspaginator)
         """
 
+
 class ListWorkflowStepsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowSteps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepspaginator)
     """
 
     def paginate(
-        self, *, workflowId: str, stepGroupId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workflowId: str, stepGroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkflowStepsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflowSteps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowstepspaginator)
         """
 
+
 class ListWorkflowsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflows)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowspaginator)
     """
 
     def paginate(
         self,
         *,
         templateId: str = ...,
         adsApplicationConfigurationName: str = ...,
         status: MigrationWorkflowStatusEnumType = ...,
         name: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMigrationWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Paginator.ListWorkflows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/paginators/#listworkflowspaginator)
         """
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/type_defs.py` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -32,92 +32,88 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "StepInputTypeDef",
+    "ResponseMetadataTypeDef",
     "StepInputOutputTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
-    "CreateWorkflowStepResponseTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
-    "DeleteMigrationWorkflowResponseTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     "DeleteWorkflowStepRequestRequestTypeDef",
     "GetMigrationWorkflowRequestRequestTypeDef",
     "GetMigrationWorkflowTemplateRequestRequestTypeDef",
     "TemplateInputTypeDef",
     "GetTemplateStepGroupRequestRequestTypeDef",
     "GetTemplateStepRequestRequestTypeDef",
     "StepOutputTypeDef",
     "GetWorkflowStepGroupRequestRequestTypeDef",
     "GetWorkflowStepRequestRequestTypeDef",
-    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListMigrationWorkflowTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
-    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListMigrationWorkflowsRequestRequestTypeDef",
     "MigrationWorkflowSummaryTypeDef",
-    "ListPluginsRequestListPluginsPaginateTypeDef",
     "ListPluginsRequestRequestTypeDef",
     "PluginSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
     "ListTemplateStepGroupsRequestRequestTypeDef",
     "TemplateStepGroupSummaryTypeDef",
-    "ListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
     "ListTemplateStepsRequestRequestTypeDef",
     "TemplateStepSummaryTypeDef",
-    "ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
     "ListWorkflowStepGroupsRequestRequestTypeDef",
     "WorkflowStepGroupSummaryTypeDef",
-    "ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
     "ListWorkflowStepsRequestRequestTypeDef",
     "WorkflowStepSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "PlatformCommandOutputTypeDef",
     "PlatformCommandTypeDef",
-    "PlatformScriptKeyOutputTypeDef",
     "PlatformScriptKeyTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryWorkflowStepRequestRequestTypeDef",
-    "RetryWorkflowStepResponseTypeDef",
     "StartMigrationWorkflowRequestRequestTypeDef",
-    "StartMigrationWorkflowResponseTypeDef",
     "StopMigrationWorkflowRequestRequestTypeDef",
-    "StopMigrationWorkflowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkflowStepGroupRequestRequestTypeDef",
-    "UpdateWorkflowStepResponseTypeDef",
     "WorkflowStepOutputUnionTypeDef",
     "CreateMigrationWorkflowRequestRequestTypeDef",
     "UpdateMigrationWorkflowRequestRequestTypeDef",
+    "CreateWorkflowStepResponseTypeDef",
+    "DeleteMigrationWorkflowResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RetryWorkflowStepResponseTypeDef",
+    "StartMigrationWorkflowResponseTypeDef",
+    "StopMigrationWorkflowResponseTypeDef",
+    "UpdateWorkflowStepResponseTypeDef",
     "CreateMigrationWorkflowResponseTypeDef",
     "UpdateMigrationWorkflowResponseTypeDef",
     "CreateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowResponseTypeDef",
     "GetTemplateStepGroupResponseTypeDef",
     "GetWorkflowStepGroupResponseTypeDef",
     "UpdateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowTemplateResponseTypeDef",
+    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
+    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
+    "ListPluginsRequestListPluginsPaginateTypeDef",
+    "ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
+    "ListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
+    "ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
+    "ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
     "ListMigrationWorkflowTemplatesResponseTypeDef",
     "ListMigrationWorkflowsResponseTypeDef",
     "ListPluginsResponseTypeDef",
     "ListTemplateStepGroupsResponseTypeDef",
     "ListTemplateStepsResponseTypeDef",
     "ListWorkflowStepGroupsResponseTypeDef",
     "ListWorkflowStepsResponseTypeDef",
     "StepAutomationConfigurationTypeDef",
-    "WorkflowStepAutomationConfigurationOutputTypeDef",
     "WorkflowStepAutomationConfigurationTypeDef",
     "WorkflowStepOutputTypeDef",
     "GetTemplateStepResponseTypeDef",
     "CreateWorkflowStepRequestRequestTypeDef",
     "GetWorkflowStepResponseTypeDef",
     "UpdateWorkflowStepRequestRequestTypeDef",
 )
@@ -129,14 +125,25 @@
         "stringValue": str,
         "listOfStringsValue": Sequence[str],
         "mapOfStringValue": Mapping[str, str],
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
 StepInputOutputTypeDef = TypedDict(
     "StepInputOutputTypeDef",
     {
         "integerValue": int,
         "stringValue": str,
         "listOfStringsValue": List[str],
         "mapOfStringValue": Dict[str, str],
@@ -157,59 +164,36 @@
         "description": str,
         "next": Sequence[str],
         "previous": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateWorkflowStepGroupRequestRequestTypeDef(
     _RequiredCreateWorkflowStepGroupRequestRequestTypeDef,
     _OptionalCreateWorkflowStepGroupRequestRequestTypeDef,
 ):
     pass
 
-
 ToolTypeDef = TypedDict(
     "ToolTypeDef",
     {
         "name": str,
         "url": str,
     },
     total=False,
 )
 
-CreateWorkflowStepResponseTypeDef = TypedDict(
-    "CreateWorkflowStepResponseTypeDef",
-    {
-        "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DeleteMigrationWorkflowResponseTypeDef = TypedDict(
-    "DeleteMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "id": str,
     },
 )
@@ -287,19 +271,20 @@
     {
         "workflowId": str,
         "stepGroupId": str,
         "id": str,
     },
 )
 
-ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
-    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListMigrationWorkflowTemplatesRequestRequestTypeDef = TypedDict(
     "ListMigrationWorkflowTemplatesRequestRequestTypeDef",
     {
@@ -317,26 +302,14 @@
         "name": str,
         "arn": str,
         "description": str,
     },
     total=False,
 )
 
-ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
-    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
-    {
-        "templateId": str,
-        "adsApplicationConfigurationName": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMigrationWorkflowsRequestRequestTypeDef = TypedDict(
     "ListMigrationWorkflowsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "templateId": str,
         "adsApplicationConfigurationName": str,
@@ -359,22 +332,14 @@
         "statusMessage": str,
         "completedSteps": int,
         "totalSteps": int,
     },
     total=False,
 )
 
-ListPluginsRequestListPluginsPaginateTypeDef = TypedDict(
-    "ListPluginsRequestListPluginsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPluginsRequestRequestTypeDef = TypedDict(
     "ListPluginsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -396,44 +361,14 @@
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
-_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
-    {
-        "templateId": str,
-    },
-)
-_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef(
-    _RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
-    _OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTemplateStepGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateStepGroupsRequestRequestTypeDef",
     {
         "templateId": str,
     },
 )
 _OptionalListTemplateStepGroupsRequestRequestTypeDef = TypedDict(
@@ -441,56 +376,31 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTemplateStepGroupsRequestRequestTypeDef(
     _RequiredListTemplateStepGroupsRequestRequestTypeDef,
     _OptionalListTemplateStepGroupsRequestRequestTypeDef,
 ):
     pass
 
-
 TemplateStepGroupSummaryTypeDef = TypedDict(
     "TemplateStepGroupSummaryTypeDef",
     {
         "id": str,
         "name": str,
         "previous": List[str],
         "next": List[str],
     },
     total=False,
 )
 
-_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
-    "_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
-    {
-        "templateId": str,
-        "stepGroupId": str,
-    },
-)
-_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
-    "_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTemplateStepsRequestListTemplateStepsPaginateTypeDef(
-    _RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
-    _OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTemplateStepsRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateStepsRequestRequestTypeDef",
     {
         "templateId": str,
         "stepGroupId": str,
     },
 )
@@ -499,21 +409,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTemplateStepsRequestRequestTypeDef(
     _RequiredListTemplateStepsRequestRequestTypeDef, _OptionalListTemplateStepsRequestRequestTypeDef
 ):
     pass
 
-
 TemplateStepSummaryTypeDef = TypedDict(
     "TemplateStepSummaryTypeDef",
     {
         "id": str,
         "stepGroupId": str,
         "templateId": str,
         "name": str,
@@ -522,36 +430,14 @@
         "owner": OwnerType,
         "previous": List[str],
         "next": List[str],
     },
     total=False,
 )
 
-_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
-    {
-        "workflowId": str,
-    },
-)
-_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef(
-    _RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
-    _OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListWorkflowStepGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkflowStepGroupsRequestRequestTypeDef",
     {
         "workflowId": str,
     },
 )
 _OptionalListWorkflowStepGroupsRequestRequestTypeDef = TypedDict(
@@ -559,58 +445,33 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListWorkflowStepGroupsRequestRequestTypeDef(
     _RequiredListWorkflowStepGroupsRequestRequestTypeDef,
     _OptionalListWorkflowStepGroupsRequestRequestTypeDef,
 ):
     pass
 
-
 WorkflowStepGroupSummaryTypeDef = TypedDict(
     "WorkflowStepGroupSummaryTypeDef",
     {
         "id": str,
         "name": str,
         "owner": OwnerType,
         "status": StepGroupStatusType,
         "previous": List[str],
         "next": List[str],
     },
     total=False,
 )
 
-_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
-    {
-        "workflowId": str,
-        "stepGroupId": str,
-    },
-)
-_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef(
-    _RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
-    _OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListWorkflowStepsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkflowStepsRequestRequestTypeDef",
     {
         "workflowId": str,
         "stepGroupId": str,
     },
 )
@@ -619,21 +480,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListWorkflowStepsRequestRequestTypeDef(
     _RequiredListWorkflowStepsRequestRequestTypeDef, _OptionalListWorkflowStepsRequestRequestTypeDef
 ):
     pass
 
-
 WorkflowStepSummaryTypeDef = TypedDict(
     "WorkflowStepSummaryTypeDef",
     {
         "stepId": str,
         "name": str,
         "stepActionType": StepActionTypeType,
         "owner": OwnerType,
@@ -646,129 +505,55 @@
         "totalNoOfSrv": int,
         "description": str,
         "scriptLocation": str,
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
-PlatformCommandOutputTypeDef = TypedDict(
-    "PlatformCommandOutputTypeDef",
-    {
-        "linux": str,
-        "windows": str,
-    },
-    total=False,
-)
-
 PlatformCommandTypeDef = TypedDict(
     "PlatformCommandTypeDef",
     {
         "linux": str,
         "windows": str,
     },
     total=False,
 )
 
-PlatformScriptKeyOutputTypeDef = TypedDict(
-    "PlatformScriptKeyOutputTypeDef",
-    {
-        "linux": str,
-        "windows": str,
-    },
-    total=False,
-)
-
 PlatformScriptKeyTypeDef = TypedDict(
     "PlatformScriptKeyTypeDef",
     {
         "linux": str,
         "windows": str,
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
 RetryWorkflowStepRequestRequestTypeDef = TypedDict(
     "RetryWorkflowStepRequestRequestTypeDef",
     {
         "workflowId": str,
         "stepGroupId": str,
         "id": str,
     },
 )
 
-RetryWorkflowStepResponseTypeDef = TypedDict(
-    "RetryWorkflowStepResponseTypeDef",
-    {
-        "stepGroupId": str,
-        "workflowId": str,
-        "id": str,
-        "status": StepStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StartMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-StartMigrationWorkflowResponseTypeDef = TypedDict(
-    "StartMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "statusMessage": str,
-        "lastStartTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StopMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-StopMigrationWorkflowResponseTypeDef = TypedDict(
-    "StopMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "statusMessage": str,
-        "lastStopTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -795,33 +580,20 @@
         "description": str,
         "next": Sequence[str],
         "previous": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateWorkflowStepGroupRequestRequestTypeDef(
     _RequiredUpdateWorkflowStepGroupRequestRequestTypeDef,
     _OptionalUpdateWorkflowStepGroupRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateWorkflowStepResponseTypeDef = TypedDict(
-    "UpdateWorkflowStepResponseTypeDef",
-    {
-        "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkflowStepOutputUnionTypeDef = TypedDict(
     "WorkflowStepOutputUnionTypeDef",
     {
         "integerValue": int,
         "stringValue": str,
         "listOfStringValue": Sequence[str],
     },
@@ -843,22 +615,20 @@
         "description": str,
         "stepTargets": Sequence[str],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateMigrationWorkflowRequestRequestTypeDef(
     _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
     _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
@@ -868,21 +638,94 @@
         "description": str,
         "inputParameters": Mapping[str, StepInputTypeDef],
         "stepTargets": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateMigrationWorkflowRequestRequestTypeDef(
     _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
     _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
+CreateWorkflowStepResponseTypeDef = TypedDict(
+    "CreateWorkflowStepResponseTypeDef",
+    {
+        "id": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteMigrationWorkflowResponseTypeDef = TypedDict(
+    "DeleteMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "status": MigrationWorkflowStatusEnumType,
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
+RetryWorkflowStepResponseTypeDef = TypedDict(
+    "RetryWorkflowStepResponseTypeDef",
+    {
+        "stepGroupId": str,
+        "workflowId": str,
+        "id": str,
+        "status": StepStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartMigrationWorkflowResponseTypeDef = TypedDict(
+    "StartMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "statusMessage": str,
+        "lastStartTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopMigrationWorkflowResponseTypeDef = TypedDict(
+    "StopMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "statusMessage": str,
+        "lastStopTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorkflowStepResponseTypeDef = TypedDict(
+    "UpdateWorkflowStepResponseTypeDef",
+    {
+        "id": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 CreateMigrationWorkflowResponseTypeDef = TypedDict(
     "CreateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
@@ -890,15 +733,15 @@
         "templateId": str,
         "adsApplicationConfigurationId": str,
         "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMigrationWorkflowResponseTypeDef = TypedDict(
     "UpdateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
@@ -909,30 +752,30 @@
         "adsApplicationConfigurationId": str,
         "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkflowStepGroupResponseTypeDef = TypedDict(
     "CreateWorkflowStepGroupResponseTypeDef",
     {
         "workflowId": str,
         "name": str,
         "id": str,
         "description": str,
         "tools": List[ToolTypeDef],
         "next": List[str],
         "previous": List[str],
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMigrationWorkflowResponseTypeDef = TypedDict(
     "GetMigrationWorkflowResponseTypeDef",
     {
         "id": str,
@@ -951,15 +794,15 @@
         "endTime": datetime,
         "tools": List[ToolTypeDef],
         "totalSteps": int,
         "completedSteps": int,
         "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "tags": Dict[str, str],
         "workflowBucket": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTemplateStepGroupResponseTypeDef = TypedDict(
     "GetTemplateStepGroupResponseTypeDef",
     {
         "templateId": str,
@@ -968,15 +811,15 @@
         "description": str,
         "status": StepGroupStatusType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "tools": List[ToolTypeDef],
         "previous": List[str],
         "next": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkflowStepGroupResponseTypeDef = TypedDict(
     "GetWorkflowStepGroupResponseTypeDef",
     {
         "id": str,
@@ -987,128 +830,227 @@
         "owner": OwnerType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "endTime": datetime,
         "tools": List[ToolTypeDef],
         "previous": List[str],
         "next": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkflowStepGroupResponseTypeDef = TypedDict(
     "UpdateWorkflowStepGroupResponseTypeDef",
     {
         "workflowId": str,
         "name": str,
         "id": str,
         "description": str,
         "tools": List[ToolTypeDef],
         "next": List[str],
         "previous": List[str],
         "lastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMigrationWorkflowTemplateResponseTypeDef = TypedDict(
     "GetMigrationWorkflowTemplateResponseTypeDef",
     {
         "id": str,
         "name": str,
         "description": str,
         "inputs": List[TemplateInputTypeDef],
         "tools": List[ToolTypeDef],
         "status": Literal["CREATED"],
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
+    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
+    {
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
+    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
+    {
+        "templateId": str,
+        "adsApplicationConfigurationName": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPluginsRequestListPluginsPaginateTypeDef = TypedDict(
+    "ListPluginsRequestListPluginsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
+    {
+        "templateId": str,
+    },
+)
+_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef(
+    _RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
+    _OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
+    "_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
+    {
+        "templateId": str,
+        "stepGroupId": str,
+    },
+)
+_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
+    "_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTemplateStepsRequestListTemplateStepsPaginateTypeDef(
+    _RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
+    _OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
+):
+    pass
+
+_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
+    {
+        "workflowId": str,
+    },
+)
+_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef(
+    _RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
+    _OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
+    {
+        "workflowId": str,
+        "stepGroupId": str,
+    },
+)
+_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef(
+    _RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
+    _OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
+):
+    pass
+
 ListMigrationWorkflowTemplatesResponseTypeDef = TypedDict(
     "ListMigrationWorkflowTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "templateSummary": List[TemplateSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMigrationWorkflowsResponseTypeDef = TypedDict(
     "ListMigrationWorkflowsResponseTypeDef",
     {
         "nextToken": str,
         "migrationWorkflowSummary": List[MigrationWorkflowSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPluginsResponseTypeDef = TypedDict(
     "ListPluginsResponseTypeDef",
     {
         "nextToken": str,
         "plugins": List[PluginSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplateStepGroupsResponseTypeDef = TypedDict(
     "ListTemplateStepGroupsResponseTypeDef",
     {
         "nextToken": str,
         "templateStepGroupSummary": List[TemplateStepGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplateStepsResponseTypeDef = TypedDict(
     "ListTemplateStepsResponseTypeDef",
     {
         "nextToken": str,
         "templateStepSummaryList": List[TemplateStepSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowStepGroupsResponseTypeDef = TypedDict(
     "ListWorkflowStepGroupsResponseTypeDef",
     {
         "nextToken": str,
         "workflowStepGroupsSummary": List[WorkflowStepGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowStepsResponseTypeDef = TypedDict(
     "ListWorkflowStepsResponseTypeDef",
     {
         "nextToken": str,
         "workflowStepsSummary": List[WorkflowStepSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StepAutomationConfigurationTypeDef = TypedDict(
     "StepAutomationConfigurationTypeDef",
     {
         "scriptLocationS3Bucket": str,
-        "scriptLocationS3Key": PlatformScriptKeyOutputTypeDef,
-        "command": PlatformCommandOutputTypeDef,
-        "runEnvironment": RunEnvironmentType,
-        "targetType": TargetTypeType,
-    },
-    total=False,
-)
-
-WorkflowStepAutomationConfigurationOutputTypeDef = TypedDict(
-    "WorkflowStepAutomationConfigurationOutputTypeDef",
-    {
-        "scriptLocationS3Bucket": str,
-        "scriptLocationS3Key": PlatformScriptKeyOutputTypeDef,
-        "command": PlatformCommandOutputTypeDef,
+        "scriptLocationS3Key": PlatformScriptKeyTypeDef,
+        "command": PlatformCommandTypeDef,
         "runEnvironment": RunEnvironmentType,
         "targetType": TargetTypeType,
     },
     total=False,
 )
 
 WorkflowStepAutomationConfigurationTypeDef = TypedDict(
@@ -1144,15 +1086,15 @@
         "description": str,
         "stepActionType": StepActionTypeType,
         "creationTime": str,
         "previous": List[str],
         "next": List[str],
         "outputs": List[StepOutputTypeDef],
         "stepAutomationConfiguration": StepAutomationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepRequestRequestTypeDef",
     {
         "name": str,
@@ -1170,47 +1112,45 @@
         "outputs": Sequence[WorkflowStepOutputTypeDef],
         "previous": Sequence[str],
         "next": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateWorkflowStepRequestRequestTypeDef(
     _RequiredCreateWorkflowStepRequestRequestTypeDef,
     _OptionalCreateWorkflowStepRequestRequestTypeDef,
 ):
     pass
 
-
 GetWorkflowStepResponseTypeDef = TypedDict(
     "GetWorkflowStepResponseTypeDef",
     {
         "name": str,
         "stepGroupId": str,
         "workflowId": str,
         "stepId": str,
         "description": str,
         "stepActionType": StepActionTypeType,
         "owner": OwnerType,
-        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationOutputTypeDef,
+        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
         "stepTarget": List[str],
         "outputs": List[WorkflowStepOutputTypeDef],
         "previous": List[str],
         "next": List[str],
         "status": StepStatusType,
         "statusMessage": str,
         "scriptOutputLocation": str,
         "creationTime": datetime,
         "lastStartTime": datetime,
         "endTime": datetime,
         "noOfSrvCompleted": int,
         "noOfSrvFailed": int,
         "totalNoOfSrv": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkflowStepRequestRequestTypeDef",
     {
         "id": str,
@@ -1230,13 +1170,12 @@
         "previous": Sequence[str],
         "next": Sequence[str],
         "status": StepStatusType,
     },
     total=False,
 )
 
-
 class UpdateWorkflowStepRequestRequestTypeDef(
     _RequiredUpdateWorkflowStepRequestRequestTypeDef,
     _OptionalUpdateWorkflowStepRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator/type_defs.pyi` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,91 +32,89 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "StepInputTypeDef",
+    "ResponseMetadataTypeDef",
     "StepInputOutputTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
-    "CreateWorkflowStepResponseTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
-    "DeleteMigrationWorkflowResponseTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     "DeleteWorkflowStepRequestRequestTypeDef",
     "GetMigrationWorkflowRequestRequestTypeDef",
     "GetMigrationWorkflowTemplateRequestRequestTypeDef",
     "TemplateInputTypeDef",
     "GetTemplateStepGroupRequestRequestTypeDef",
     "GetTemplateStepRequestRequestTypeDef",
     "StepOutputTypeDef",
     "GetWorkflowStepGroupRequestRequestTypeDef",
     "GetWorkflowStepRequestRequestTypeDef",
-    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListMigrationWorkflowTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
-    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListMigrationWorkflowsRequestRequestTypeDef",
     "MigrationWorkflowSummaryTypeDef",
-    "ListPluginsRequestListPluginsPaginateTypeDef",
     "ListPluginsRequestRequestTypeDef",
     "PluginSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
     "ListTemplateStepGroupsRequestRequestTypeDef",
     "TemplateStepGroupSummaryTypeDef",
-    "ListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
     "ListTemplateStepsRequestRequestTypeDef",
     "TemplateStepSummaryTypeDef",
-    "ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
     "ListWorkflowStepGroupsRequestRequestTypeDef",
     "WorkflowStepGroupSummaryTypeDef",
-    "ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
     "ListWorkflowStepsRequestRequestTypeDef",
     "WorkflowStepSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "PlatformCommandOutputTypeDef",
     "PlatformCommandTypeDef",
-    "PlatformScriptKeyOutputTypeDef",
     "PlatformScriptKeyTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryWorkflowStepRequestRequestTypeDef",
-    "RetryWorkflowStepResponseTypeDef",
     "StartMigrationWorkflowRequestRequestTypeDef",
-    "StartMigrationWorkflowResponseTypeDef",
     "StopMigrationWorkflowRequestRequestTypeDef",
-    "StopMigrationWorkflowResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkflowStepGroupRequestRequestTypeDef",
-    "UpdateWorkflowStepResponseTypeDef",
     "WorkflowStepOutputUnionTypeDef",
     "CreateMigrationWorkflowRequestRequestTypeDef",
     "UpdateMigrationWorkflowRequestRequestTypeDef",
+    "CreateWorkflowStepResponseTypeDef",
+    "DeleteMigrationWorkflowResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RetryWorkflowStepResponseTypeDef",
+    "StartMigrationWorkflowResponseTypeDef",
+    "StopMigrationWorkflowResponseTypeDef",
+    "UpdateWorkflowStepResponseTypeDef",
     "CreateMigrationWorkflowResponseTypeDef",
     "UpdateMigrationWorkflowResponseTypeDef",
     "CreateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowResponseTypeDef",
     "GetTemplateStepGroupResponseTypeDef",
     "GetWorkflowStepGroupResponseTypeDef",
     "UpdateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowTemplateResponseTypeDef",
+    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
+    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
+    "ListPluginsRequestListPluginsPaginateTypeDef",
+    "ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
+    "ListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
+    "ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
+    "ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
     "ListMigrationWorkflowTemplatesResponseTypeDef",
     "ListMigrationWorkflowsResponseTypeDef",
     "ListPluginsResponseTypeDef",
     "ListTemplateStepGroupsResponseTypeDef",
     "ListTemplateStepsResponseTypeDef",
     "ListWorkflowStepGroupsResponseTypeDef",
     "ListWorkflowStepsResponseTypeDef",
     "StepAutomationConfigurationTypeDef",
-    "WorkflowStepAutomationConfigurationOutputTypeDef",
     "WorkflowStepAutomationConfigurationTypeDef",
     "WorkflowStepOutputTypeDef",
     "GetTemplateStepResponseTypeDef",
     "CreateWorkflowStepRequestRequestTypeDef",
     "GetWorkflowStepResponseTypeDef",
     "UpdateWorkflowStepRequestRequestTypeDef",
 )
@@ -128,14 +126,25 @@
         "stringValue": str,
         "listOfStringsValue": Sequence[str],
         "mapOfStringValue": Mapping[str, str],
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
 StepInputOutputTypeDef = TypedDict(
     "StepInputOutputTypeDef",
     {
         "integerValue": int,
         "stringValue": str,
         "listOfStringsValue": List[str],
         "mapOfStringValue": Dict[str, str],
@@ -156,57 +165,38 @@
         "description": str,
         "next": Sequence[str],
         "previous": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateWorkflowStepGroupRequestRequestTypeDef(
     _RequiredCreateWorkflowStepGroupRequestRequestTypeDef,
     _OptionalCreateWorkflowStepGroupRequestRequestTypeDef,
 ):
     pass
 
+
 ToolTypeDef = TypedDict(
     "ToolTypeDef",
     {
         "name": str,
         "url": str,
     },
     total=False,
 )
 
-CreateWorkflowStepResponseTypeDef = TypedDict(
-    "CreateWorkflowStepResponseTypeDef",
-    {
-        "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DeleteMigrationWorkflowResponseTypeDef = TypedDict(
-    "DeleteMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "id": str,
     },
 )
@@ -284,19 +274,20 @@
     {
         "workflowId": str,
         "stepGroupId": str,
         "id": str,
     },
 )
 
-ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
-    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListMigrationWorkflowTemplatesRequestRequestTypeDef = TypedDict(
     "ListMigrationWorkflowTemplatesRequestRequestTypeDef",
     {
@@ -314,26 +305,14 @@
         "name": str,
         "arn": str,
         "description": str,
     },
     total=False,
 )
 
-ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
-    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
-    {
-        "templateId": str,
-        "adsApplicationConfigurationName": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMigrationWorkflowsRequestRequestTypeDef = TypedDict(
     "ListMigrationWorkflowsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "templateId": str,
         "adsApplicationConfigurationName": str,
@@ -356,22 +335,14 @@
         "statusMessage": str,
         "completedSteps": int,
         "totalSteps": int,
     },
     total=False,
 )
 
-ListPluginsRequestListPluginsPaginateTypeDef = TypedDict(
-    "ListPluginsRequestListPluginsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPluginsRequestRequestTypeDef = TypedDict(
     "ListPluginsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -393,42 +364,14 @@
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
-_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
-    {
-        "templateId": str,
-    },
-)
-_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef(
-    _RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
-    _OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListTemplateStepGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateStepGroupsRequestRequestTypeDef",
     {
         "templateId": str,
     },
 )
 _OptionalListTemplateStepGroupsRequestRequestTypeDef = TypedDict(
@@ -436,52 +379,33 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTemplateStepGroupsRequestRequestTypeDef(
     _RequiredListTemplateStepGroupsRequestRequestTypeDef,
     _OptionalListTemplateStepGroupsRequestRequestTypeDef,
 ):
     pass
 
+
 TemplateStepGroupSummaryTypeDef = TypedDict(
     "TemplateStepGroupSummaryTypeDef",
     {
         "id": str,
         "name": str,
         "previous": List[str],
         "next": List[str],
     },
     total=False,
 )
 
-_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
-    "_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
-    {
-        "templateId": str,
-        "stepGroupId": str,
-    },
-)
-_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
-    "_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTemplateStepsRequestListTemplateStepsPaginateTypeDef(
-    _RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
-    _OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
-):
-    pass
-
 _RequiredListTemplateStepsRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplateStepsRequestRequestTypeDef",
     {
         "templateId": str,
         "stepGroupId": str,
     },
 )
@@ -490,19 +414,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTemplateStepsRequestRequestTypeDef(
     _RequiredListTemplateStepsRequestRequestTypeDef, _OptionalListTemplateStepsRequestRequestTypeDef
 ):
     pass
 
+
 TemplateStepSummaryTypeDef = TypedDict(
     "TemplateStepSummaryTypeDef",
     {
         "id": str,
         "stepGroupId": str,
         "templateId": str,
         "name": str,
@@ -511,34 +437,14 @@
         "owner": OwnerType,
         "previous": List[str],
         "next": List[str],
     },
     total=False,
 )
 
-_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
-    {
-        "workflowId": str,
-    },
-)
-_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef(
-    _RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
-    _OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListWorkflowStepGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkflowStepGroupsRequestRequestTypeDef",
     {
         "workflowId": str,
     },
 )
 _OptionalListWorkflowStepGroupsRequestRequestTypeDef = TypedDict(
@@ -546,54 +452,35 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListWorkflowStepGroupsRequestRequestTypeDef(
     _RequiredListWorkflowStepGroupsRequestRequestTypeDef,
     _OptionalListWorkflowStepGroupsRequestRequestTypeDef,
 ):
     pass
 
+
 WorkflowStepGroupSummaryTypeDef = TypedDict(
     "WorkflowStepGroupSummaryTypeDef",
     {
         "id": str,
         "name": str,
         "owner": OwnerType,
         "status": StepGroupStatusType,
         "previous": List[str],
         "next": List[str],
     },
     total=False,
 )
 
-_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
-    {
-        "workflowId": str,
-        "stepGroupId": str,
-    },
-)
-_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef(
-    _RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
-    _OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
-):
-    pass
-
 _RequiredListWorkflowStepsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkflowStepsRequestRequestTypeDef",
     {
         "workflowId": str,
         "stepGroupId": str,
     },
 )
@@ -602,19 +489,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListWorkflowStepsRequestRequestTypeDef(
     _RequiredListWorkflowStepsRequestRequestTypeDef, _OptionalListWorkflowStepsRequestRequestTypeDef
 ):
     pass
 
+
 WorkflowStepSummaryTypeDef = TypedDict(
     "WorkflowStepSummaryTypeDef",
     {
         "stepId": str,
         "name": str,
         "stepActionType": StepActionTypeType,
         "owner": OwnerType,
@@ -627,129 +516,55 @@
         "totalNoOfSrv": int,
         "description": str,
         "scriptLocation": str,
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
-PlatformCommandOutputTypeDef = TypedDict(
-    "PlatformCommandOutputTypeDef",
-    {
-        "linux": str,
-        "windows": str,
-    },
-    total=False,
-)
-
 PlatformCommandTypeDef = TypedDict(
     "PlatformCommandTypeDef",
     {
         "linux": str,
         "windows": str,
     },
     total=False,
 )
 
-PlatformScriptKeyOutputTypeDef = TypedDict(
-    "PlatformScriptKeyOutputTypeDef",
-    {
-        "linux": str,
-        "windows": str,
-    },
-    total=False,
-)
-
 PlatformScriptKeyTypeDef = TypedDict(
     "PlatformScriptKeyTypeDef",
     {
         "linux": str,
         "windows": str,
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
 RetryWorkflowStepRequestRequestTypeDef = TypedDict(
     "RetryWorkflowStepRequestRequestTypeDef",
     {
         "workflowId": str,
         "stepGroupId": str,
         "id": str,
     },
 )
 
-RetryWorkflowStepResponseTypeDef = TypedDict(
-    "RetryWorkflowStepResponseTypeDef",
-    {
-        "stepGroupId": str,
-        "workflowId": str,
-        "id": str,
-        "status": StepStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StartMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-StartMigrationWorkflowResponseTypeDef = TypedDict(
-    "StartMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "statusMessage": str,
-        "lastStartTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StopMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-StopMigrationWorkflowResponseTypeDef = TypedDict(
-    "StopMigrationWorkflowResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "status": MigrationWorkflowStatusEnumType,
-        "statusMessage": str,
-        "lastStopTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -776,30 +591,21 @@
         "description": str,
         "next": Sequence[str],
         "previous": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateWorkflowStepGroupRequestRequestTypeDef(
     _RequiredUpdateWorkflowStepGroupRequestRequestTypeDef,
     _OptionalUpdateWorkflowStepGroupRequestRequestTypeDef,
 ):
     pass
 
-UpdateWorkflowStepResponseTypeDef = TypedDict(
-    "UpdateWorkflowStepResponseTypeDef",
-    {
-        "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 WorkflowStepOutputUnionTypeDef = TypedDict(
     "WorkflowStepOutputUnionTypeDef",
     {
         "integerValue": int,
         "stringValue": str,
         "listOfStringValue": Sequence[str],
@@ -822,20 +628,22 @@
         "description": str,
         "stepTargets": Sequence[str],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateMigrationWorkflowRequestRequestTypeDef(
     _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
     _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
@@ -845,35 +653,112 @@
         "description": str,
         "inputParameters": Mapping[str, StepInputTypeDef],
         "stepTargets": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateMigrationWorkflowRequestRequestTypeDef(
     _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
     _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
 ):
     pass
 
+
+CreateWorkflowStepResponseTypeDef = TypedDict(
+    "CreateWorkflowStepResponseTypeDef",
+    {
+        "id": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteMigrationWorkflowResponseTypeDef = TypedDict(
+    "DeleteMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "status": MigrationWorkflowStatusEnumType,
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
+RetryWorkflowStepResponseTypeDef = TypedDict(
+    "RetryWorkflowStepResponseTypeDef",
+    {
+        "stepGroupId": str,
+        "workflowId": str,
+        "id": str,
+        "status": StepStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartMigrationWorkflowResponseTypeDef = TypedDict(
+    "StartMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "statusMessage": str,
+        "lastStartTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopMigrationWorkflowResponseTypeDef = TypedDict(
+    "StopMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "statusMessage": str,
+        "lastStopTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorkflowStepResponseTypeDef = TypedDict(
+    "UpdateWorkflowStepResponseTypeDef",
+    {
+        "id": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateMigrationWorkflowResponseTypeDef = TypedDict(
     "CreateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "templateId": str,
         "adsApplicationConfigurationId": str,
         "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMigrationWorkflowResponseTypeDef = TypedDict(
     "UpdateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
@@ -884,30 +769,30 @@
         "adsApplicationConfigurationId": str,
         "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkflowStepGroupResponseTypeDef = TypedDict(
     "CreateWorkflowStepGroupResponseTypeDef",
     {
         "workflowId": str,
         "name": str,
         "id": str,
         "description": str,
         "tools": List[ToolTypeDef],
         "next": List[str],
         "previous": List[str],
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMigrationWorkflowResponseTypeDef = TypedDict(
     "GetMigrationWorkflowResponseTypeDef",
     {
         "id": str,
@@ -926,15 +811,15 @@
         "endTime": datetime,
         "tools": List[ToolTypeDef],
         "totalSteps": int,
         "completedSteps": int,
         "workflowInputs": Dict[str, StepInputOutputTypeDef],
         "tags": Dict[str, str],
         "workflowBucket": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTemplateStepGroupResponseTypeDef = TypedDict(
     "GetTemplateStepGroupResponseTypeDef",
     {
         "templateId": str,
@@ -943,15 +828,15 @@
         "description": str,
         "status": StepGroupStatusType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "tools": List[ToolTypeDef],
         "previous": List[str],
         "next": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkflowStepGroupResponseTypeDef = TypedDict(
     "GetWorkflowStepGroupResponseTypeDef",
     {
         "id": str,
@@ -962,128 +847,235 @@
         "owner": OwnerType,
         "creationTime": datetime,
         "lastModifiedTime": datetime,
         "endTime": datetime,
         "tools": List[ToolTypeDef],
         "previous": List[str],
         "next": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkflowStepGroupResponseTypeDef = TypedDict(
     "UpdateWorkflowStepGroupResponseTypeDef",
     {
         "workflowId": str,
         "name": str,
         "id": str,
         "description": str,
         "tools": List[ToolTypeDef],
         "next": List[str],
         "previous": List[str],
         "lastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMigrationWorkflowTemplateResponseTypeDef = TypedDict(
     "GetMigrationWorkflowTemplateResponseTypeDef",
     {
         "id": str,
         "name": str,
         "description": str,
         "inputs": List[TemplateInputTypeDef],
         "tools": List[ToolTypeDef],
         "status": Literal["CREATED"],
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
+    "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
+    {
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
+    "ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef",
+    {
+        "templateId": str,
+        "adsApplicationConfigurationName": str,
+        "status": MigrationWorkflowStatusEnumType,
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPluginsRequestListPluginsPaginateTypeDef = TypedDict(
+    "ListPluginsRequestListPluginsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
+    {
+        "templateId": str,
+    },
+)
+_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef(
+    _RequiredListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
+    _OptionalListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
+    "_RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
+    {
+        "templateId": str,
+        "stepGroupId": str,
+    },
+)
+_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef = TypedDict(
+    "_OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTemplateStepsRequestListTemplateStepsPaginateTypeDef(
+    _RequiredListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
+    _OptionalListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
+    {
+        "workflowId": str,
+    },
+)
+_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef(
+    _RequiredListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
+    _OptionalListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
+    {
+        "workflowId": str,
+        "stepGroupId": str,
+    },
+)
+_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef(
+    _RequiredListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
+    _OptionalListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
+):
+    pass
+
+
 ListMigrationWorkflowTemplatesResponseTypeDef = TypedDict(
     "ListMigrationWorkflowTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "templateSummary": List[TemplateSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMigrationWorkflowsResponseTypeDef = TypedDict(
     "ListMigrationWorkflowsResponseTypeDef",
     {
         "nextToken": str,
         "migrationWorkflowSummary": List[MigrationWorkflowSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPluginsResponseTypeDef = TypedDict(
     "ListPluginsResponseTypeDef",
     {
         "nextToken": str,
         "plugins": List[PluginSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplateStepGroupsResponseTypeDef = TypedDict(
     "ListTemplateStepGroupsResponseTypeDef",
     {
         "nextToken": str,
         "templateStepGroupSummary": List[TemplateStepGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplateStepsResponseTypeDef = TypedDict(
     "ListTemplateStepsResponseTypeDef",
     {
         "nextToken": str,
         "templateStepSummaryList": List[TemplateStepSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowStepGroupsResponseTypeDef = TypedDict(
     "ListWorkflowStepGroupsResponseTypeDef",
     {
         "nextToken": str,
         "workflowStepGroupsSummary": List[WorkflowStepGroupSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowStepsResponseTypeDef = TypedDict(
     "ListWorkflowStepsResponseTypeDef",
     {
         "nextToken": str,
         "workflowStepsSummary": List[WorkflowStepSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StepAutomationConfigurationTypeDef = TypedDict(
     "StepAutomationConfigurationTypeDef",
     {
         "scriptLocationS3Bucket": str,
-        "scriptLocationS3Key": PlatformScriptKeyOutputTypeDef,
-        "command": PlatformCommandOutputTypeDef,
-        "runEnvironment": RunEnvironmentType,
-        "targetType": TargetTypeType,
-    },
-    total=False,
-)
-
-WorkflowStepAutomationConfigurationOutputTypeDef = TypedDict(
-    "WorkflowStepAutomationConfigurationOutputTypeDef",
-    {
-        "scriptLocationS3Bucket": str,
-        "scriptLocationS3Key": PlatformScriptKeyOutputTypeDef,
-        "command": PlatformCommandOutputTypeDef,
+        "scriptLocationS3Key": PlatformScriptKeyTypeDef,
+        "command": PlatformCommandTypeDef,
         "runEnvironment": RunEnvironmentType,
         "targetType": TargetTypeType,
     },
     total=False,
 )
 
 WorkflowStepAutomationConfigurationTypeDef = TypedDict(
@@ -1119,15 +1111,15 @@
         "description": str,
         "stepActionType": StepActionTypeType,
         "creationTime": str,
         "previous": List[str],
         "next": List[str],
         "outputs": List[StepOutputTypeDef],
         "stepAutomationConfiguration": StepAutomationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepRequestRequestTypeDef",
     {
         "name": str,
@@ -1145,45 +1137,47 @@
         "outputs": Sequence[WorkflowStepOutputTypeDef],
         "previous": Sequence[str],
         "next": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateWorkflowStepRequestRequestTypeDef(
     _RequiredCreateWorkflowStepRequestRequestTypeDef,
     _OptionalCreateWorkflowStepRequestRequestTypeDef,
 ):
     pass
 
+
 GetWorkflowStepResponseTypeDef = TypedDict(
     "GetWorkflowStepResponseTypeDef",
     {
         "name": str,
         "stepGroupId": str,
         "workflowId": str,
         "stepId": str,
         "description": str,
         "stepActionType": StepActionTypeType,
         "owner": OwnerType,
-        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationOutputTypeDef,
+        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
         "stepTarget": List[str],
         "outputs": List[WorkflowStepOutputTypeDef],
         "previous": List[str],
         "next": List[str],
         "status": StepStatusType,
         "statusMessage": str,
         "scriptOutputLocation": str,
         "creationTime": datetime,
         "lastStartTime": datetime,
         "endTime": datetime,
         "noOfSrvCompleted": int,
         "noOfSrvFailed": int,
         "totalNoOfSrv": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkflowStepRequestRequestTypeDef",
     {
         "id": str,
@@ -1203,12 +1197,13 @@
         "previous": Sequence[str],
         "next": Sequence[str],
         "status": StepStatusType,
     },
     total=False,
 )
 
+
 class UpdateWorkflowStepRequestRequestTypeDef(
     _RequiredUpdateWorkflowStepRequestRequestTypeDef,
     _OptionalUpdateWorkflowStepRequestRequestTypeDef,
 ):
     pass
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhuborchestrator
-Version: 1.28.12
-Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MigrationHubOrchestrator 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhuborchestrator.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhuborchestrator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhuborchestrator)](https://pepy.tech/project/mypy-boto3-migrationhuborchestrator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubOrchestrator 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
+[boto3.MigrationHubOrchestrator 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator)
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
 [mypy-boto3-migrationhuborchestrator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhuborchestrator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,89 +359,86 @@
 
 `mypy_boto3_migrationhuborchestrator.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhuborchestrator.type_defs import (
     StepInputTypeDef,
+    ResponseMetadataTypeDef,
     StepInputOutputTypeDef,
     CreateWorkflowStepGroupRequestRequestTypeDef,
     ToolTypeDef,
-    CreateWorkflowStepResponseTypeDef,
     DeleteMigrationWorkflowRequestRequestTypeDef,
-    DeleteMigrationWorkflowResponseTypeDef,
     DeleteWorkflowStepGroupRequestRequestTypeDef,
     DeleteWorkflowStepRequestRequestTypeDef,
     GetMigrationWorkflowRequestRequestTypeDef,
     GetMigrationWorkflowTemplateRequestRequestTypeDef,
     TemplateInputTypeDef,
     GetTemplateStepGroupRequestRequestTypeDef,
     GetTemplateStepRequestRequestTypeDef,
     StepOutputTypeDef,
     GetWorkflowStepGroupRequestRequestTypeDef,
     GetWorkflowStepRequestRequestTypeDef,
-    ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMigrationWorkflowTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
-    ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListMigrationWorkflowsRequestRequestTypeDef,
     MigrationWorkflowSummaryTypeDef,
-    ListPluginsRequestListPluginsPaginateTypeDef,
     ListPluginsRequestRequestTypeDef,
     PluginSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
     ListTemplateStepGroupsRequestRequestTypeDef,
     TemplateStepGroupSummaryTypeDef,
-    ListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
     ListTemplateStepsRequestRequestTypeDef,
     TemplateStepSummaryTypeDef,
-    ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
     ListWorkflowStepGroupsRequestRequestTypeDef,
     WorkflowStepGroupSummaryTypeDef,
-    ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListWorkflowStepsRequestRequestTypeDef,
     WorkflowStepSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    PlatformCommandOutputTypeDef,
     PlatformCommandTypeDef,
-    PlatformScriptKeyOutputTypeDef,
     PlatformScriptKeyTypeDef,
-    ResponseMetadataTypeDef,
     RetryWorkflowStepRequestRequestTypeDef,
-    RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowRequestRequestTypeDef,
-    StartMigrationWorkflowResponseTypeDef,
     StopMigrationWorkflowRequestRequestTypeDef,
-    StopMigrationWorkflowResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWorkflowStepGroupRequestRequestTypeDef,
-    UpdateWorkflowStepResponseTypeDef,
     WorkflowStepOutputUnionTypeDef,
     CreateMigrationWorkflowRequestRequestTypeDef,
     UpdateMigrationWorkflowRequestRequestTypeDef,
+    CreateWorkflowStepResponseTypeDef,
+    DeleteMigrationWorkflowResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RetryWorkflowStepResponseTypeDef,
+    StartMigrationWorkflowResponseTypeDef,
+    StopMigrationWorkflowResponseTypeDef,
+    UpdateWorkflowStepResponseTypeDef,
     CreateMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
     CreateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowResponseTypeDef,
     GetTemplateStepGroupResponseTypeDef,
     GetWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     GetMigrationWorkflowTemplateResponseTypeDef,
+    ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef,
+    ListMigrationWorkflowsRequestListWorkflowsPaginateTypeDef,
+    ListPluginsRequestListPluginsPaginateTypeDef,
+    ListTemplateStepGroupsRequestListTemplateStepGroupsPaginateTypeDef,
+    ListTemplateStepsRequestListTemplateStepsPaginateTypeDef,
+    ListWorkflowStepGroupsRequestListWorkflowStepGroupsPaginateTypeDef,
+    ListWorkflowStepsRequestListWorkflowStepsPaginateTypeDef,
     ListMigrationWorkflowTemplatesResponseTypeDef,
     ListMigrationWorkflowsResponseTypeDef,
     ListPluginsResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     StepAutomationConfigurationTypeDef,
-    WorkflowStepAutomationConfigurationOutputTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
     WorkflowStepOutputTypeDef,
     GetTemplateStepResponseTypeDef,
     CreateWorkflowStepRequestRequestTypeDef,
     GetWorkflowStepResponseTypeDef,
     UpdateWorkflowStepRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt` & `mypy-boto3-migrationhuborchestrator-1.28.15/mypy_boto3_migrationhuborchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhuborchestrator-1.28.12/setup.py` & `mypy-boto3-migrationhuborchestrator-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhuborchestrator",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_migrationhuborchestrator"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubOrchestrator 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MigrationHubOrchestrator 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

