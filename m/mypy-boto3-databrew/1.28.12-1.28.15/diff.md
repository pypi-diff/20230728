# Comparing `tmp/mypy-boto3-databrew-1.28.12.tar.gz` & `tmp/mypy-boto3-databrew-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-databrew-1.28.12.tar", last modified: Thu Jul 27 05:34:33 2023, max compression
+gzip compressed data, was "mypy-boto3-databrew-1.28.15.tar", last modified: Fri Jul 28 20:42:35 2023, max compression
```

## Comparing `mypy-boto3-databrew-1.28.12.tar` & `mypy-boto3-databrew-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.292537 mypy-boto3-databrew-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20150 2023-07-27 05:34:33.292537 mypy-boto3-databrew-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18655 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.288537 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33726 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    67166 2023-07-27 05:19:58.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    67034 2023-07-27 05:19:56.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.292537 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20150 2023-07-27 05:34:33.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:34:33.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:33.000000 mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:33.292537 mypy-boto3-databrew-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-27 05:19:55.000000 mypy-boto3-databrew-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:35.032918 mypy-boto3-databrew-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-07-28 20:42:35.028918 mypy-boto3-databrew-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:35.016918 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-07-28 20:22:29.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33726 2023-07-28 20:22:29.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-07-28 20:22:30.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-28 20:22:30.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-07-28 20:22:30.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-07-28 20:22:30.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59540 2023-07-28 20:22:32.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59430 2023-07-28 20:22:31.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:35.028918 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-07-28 20:42:34.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:42:34.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:34.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:42:34.000000 mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:35.032918 mypy-boto3-databrew-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-28 20:22:28.000000 mypy-boto3-databrew-1.28.15/setup.py
```

### Comparing `mypy-boto3-databrew-1.28.12/LICENSE` & `mypy-boto3-databrew-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.12/PKG-INFO` & `mypy-boto3-databrew-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-databrew
-Version: 1.28.12
-Summary: Type annotations for boto3.GlueDataBrew 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 databrew type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-databrew"></a>
 
 # mypy-boto3-databrew
 
 [![PyPI - mypy-boto3-databrew](https://img.shields.io/pypi/v/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-databrew)](https://pepy.tech/project/mypy-boto3-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlueDataBrew 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[boto3.GlueDataBrew 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,157 +334,137 @@
 
 ```python
 from mypy_boto3_databrew.type_defs import (
     AllowedStatisticsOutputTypeDef,
     AllowedStatisticsTypeDef,
     BatchDeleteRecipeVersionRequestRequestTypeDef,
     RecipeVersionErrorDetailTypeDef,
-    ColumnSelectorOutputTypeDef,
+    ResponseMetadataTypeDef,
     ColumnSelectorTypeDef,
-    ConditionExpressionOutputTypeDef,
     ConditionExpressionTypeDef,
-    CreateDatasetResponseTypeDef,
     JobSampleTypeDef,
     S3LocationTypeDef,
     ValidationConfigurationTypeDef,
-    CreateProfileJobResponseTypeDef,
     SampleTypeDef,
-    CreateProjectResponseTypeDef,
     RecipeReferenceTypeDef,
-    CreateRecipeJobResponseTypeDef,
-    CreateRecipeResponseTypeDef,
-    CreateRulesetResponseTypeDef,
     CreateScheduleRequestRequestTypeDef,
-    CreateScheduleResponseTypeDef,
-    CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
-    CsvOutputOptionsOutputTypeDef,
     CsvOutputOptionsTypeDef,
-    S3LocationOutputTypeDef,
-    DatetimeOptionsOutputTypeDef,
-    FilterExpressionOutputTypeDef,
     DatetimeOptionsTypeDef,
+    FilterExpressionOutputTypeDef,
     FilterExpressionTypeDef,
     DeleteDatasetRequestRequestTypeDef,
-    DeleteDatasetResponseTypeDef,
     DeleteJobRequestRequestTypeDef,
-    DeleteJobResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DeleteRecipeVersionRequestRequestTypeDef,
-    DeleteRecipeVersionResponseTypeDef,
     DeleteRulesetRequestRequestTypeDef,
-    DeleteRulesetResponseTypeDef,
     DeleteScheduleRequestRequestTypeDef,
-    DeleteScheduleResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
-    JobSampleOutputTypeDef,
-    RecipeReferenceOutputTypeDef,
-    ValidationConfigurationOutputTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
-    SampleOutputTypeDef,
     DescribeRecipeRequestRequestTypeDef,
     DescribeRulesetRequestRequestTypeDef,
     DescribeScheduleRequestRequestTypeDef,
-    DescribeScheduleResponseTypeDef,
     ExcelOptionsOutputTypeDef,
     ExcelOptionsTypeDef,
-    FilesLimitOutputTypeDef,
     FilesLimitTypeDef,
-    JsonOptionsOutputTypeDef,
     JsonOptionsTypeDef,
-    MetadataOutputTypeDef,
     MetadataTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDatasetsRequestRequestTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
-    ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
     ListRecipeVersionsRequestRequestTypeDef,
-    ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
-    ListRulesetsRequestListRulesetsPaginateTypeDef,
     ListRulesetsRequestRequestTypeDef,
     RulesetItemTypeDef,
-    ListSchedulesRequestListSchedulesPaginateTypeDef,
     ListSchedulesRequestRequestTypeDef,
     ScheduleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PublishRecipeRequestRequestTypeDef,
-    PublishRecipeResponseTypeDef,
     RecipeActionOutputTypeDef,
     RecipeActionTypeDef,
-    ResponseMetadataTypeDef,
-    ThresholdOutputTypeDef,
     ThresholdTypeDef,
     ViewFrameTypeDef,
-    SendProjectSessionActionResponseTypeDef,
     StartJobRunRequestRequestTypeDef,
-    StartJobRunResponseTypeDef,
     StartProjectSessionRequestRequestTypeDef,
-    StartProjectSessionResponseTypeDef,
     StatisticOverrideOutputTypeDef,
     StatisticOverrideTypeDef,
     StopJobRunRequestRequestTypeDef,
-    StopJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateScheduleRequestRequestTypeDef,
+    EntityDetectorConfigurationOutputTypeDef,
+    EntityDetectorConfigurationTypeDef,
+    BatchDeleteRecipeVersionResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateProfileJobResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateRecipeJobResponseTypeDef,
+    CreateRecipeResponseTypeDef,
+    CreateRulesetResponseTypeDef,
+    CreateScheduleResponseTypeDef,
+    DeleteDatasetResponseTypeDef,
+    DeleteJobResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteRecipeVersionResponseTypeDef,
+    DeleteRulesetResponseTypeDef,
+    DeleteScheduleResponseTypeDef,
+    DescribeScheduleResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PublishRecipeResponseTypeDef,
+    SendProjectSessionActionResponseTypeDef,
+    StartJobRunResponseTypeDef,
+    StartProjectSessionResponseTypeDef,
+    StopJobRunResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
-    UpdateScheduleRequestRequestTypeDef,
     UpdateScheduleResponseTypeDef,
-    EntityDetectorConfigurationOutputTypeDef,
-    EntityDetectorConfigurationTypeDef,
-    BatchDeleteRecipeVersionResponseTypeDef,
     DataCatalogInputDefinitionTypeDef,
     DatabaseInputDefinitionTypeDef,
     DatabaseTableOutputOptionsTypeDef,
     S3TableOutputOptionsTypeDef,
     CreateProjectRequestRequestTypeDef,
+    DescribeProjectResponseTypeDef,
+    ProjectTypeDef,
     UpdateProjectRequestRequestTypeDef,
-    OutputFormatOptionsOutputTypeDef,
     OutputFormatOptionsTypeDef,
-    DataCatalogInputDefinitionOutputTypeDef,
-    DatabaseInputDefinitionOutputTypeDef,
-    DatabaseTableOutputOptionsOutputTypeDef,
-    S3TableOutputOptionsOutputTypeDef,
     DatasetParameterOutputTypeDef,
     DatasetParameterTypeDef,
-    DescribeProjectResponseTypeDef,
-    ProjectTypeDef,
     FormatOptionsOutputTypeDef,
     FormatOptionsTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
+    ListRecipesRequestListRecipesPaginateTypeDef,
+    ListRulesetsRequestListRulesetsPaginateTypeDef,
+    ListSchedulesRequestListSchedulesPaginateTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
     RecipeStepOutputTypeDef,
     RecipeStepTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
     StatisticsConfigurationOutputTypeDef,
     StatisticsConfigurationTypeDef,
     InputTypeDef,
     DatabaseOutputTypeDef,
     DataCatalogOutputTypeDef,
+    ListProjectsResponseTypeDef,
     OutputTypeDef,
-    InputOutputTypeDef,
     PathOptionsOutputTypeDef,
     PathOptionsTypeDef,
-    ListProjectsResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     RecipeTypeDef,
     CreateRecipeRequestRequestTypeDef,
     SendProjectSessionActionRequestRequestTypeDef,
     UpdateRecipeRequestRequestTypeDef,
     DescribeRulesetResponseTypeDef,
     CreateRulesetRequestRequestTypeDef,
```

### Comparing `mypy-boto3-databrew-1.28.12/README.md` & `mypy-boto3-databrew-1.28.15/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-databrew
+Version: 1.28.15
+Summary: Type annotations for boto3.GlueDataBrew 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 databrew type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-databrew"></a>
 
 # mypy-boto3-databrew
 
 [![PyPI - mypy-boto3-databrew](https://img.shields.io/pypi/v/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-databrew)](https://pepy.tech/project/mypy-boto3-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlueDataBrew 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[boto3.GlueDataBrew 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,157 +366,137 @@
 
 ```python
 from mypy_boto3_databrew.type_defs import (
     AllowedStatisticsOutputTypeDef,
     AllowedStatisticsTypeDef,
     BatchDeleteRecipeVersionRequestRequestTypeDef,
     RecipeVersionErrorDetailTypeDef,
-    ColumnSelectorOutputTypeDef,
+    ResponseMetadataTypeDef,
     ColumnSelectorTypeDef,
-    ConditionExpressionOutputTypeDef,
     ConditionExpressionTypeDef,
-    CreateDatasetResponseTypeDef,
     JobSampleTypeDef,
     S3LocationTypeDef,
     ValidationConfigurationTypeDef,
-    CreateProfileJobResponseTypeDef,
     SampleTypeDef,
-    CreateProjectResponseTypeDef,
     RecipeReferenceTypeDef,
-    CreateRecipeJobResponseTypeDef,
-    CreateRecipeResponseTypeDef,
-    CreateRulesetResponseTypeDef,
     CreateScheduleRequestRequestTypeDef,
-    CreateScheduleResponseTypeDef,
-    CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
-    CsvOutputOptionsOutputTypeDef,
     CsvOutputOptionsTypeDef,
-    S3LocationOutputTypeDef,
-    DatetimeOptionsOutputTypeDef,
-    FilterExpressionOutputTypeDef,
     DatetimeOptionsTypeDef,
+    FilterExpressionOutputTypeDef,
     FilterExpressionTypeDef,
     DeleteDatasetRequestRequestTypeDef,
-    DeleteDatasetResponseTypeDef,
     DeleteJobRequestRequestTypeDef,
-    DeleteJobResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DeleteRecipeVersionRequestRequestTypeDef,
-    DeleteRecipeVersionResponseTypeDef,
     DeleteRulesetRequestRequestTypeDef,
-    DeleteRulesetResponseTypeDef,
     DeleteScheduleRequestRequestTypeDef,
-    DeleteScheduleResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
-    JobSampleOutputTypeDef,
-    RecipeReferenceOutputTypeDef,
-    ValidationConfigurationOutputTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
-    SampleOutputTypeDef,
     DescribeRecipeRequestRequestTypeDef,
     DescribeRulesetRequestRequestTypeDef,
     DescribeScheduleRequestRequestTypeDef,
-    DescribeScheduleResponseTypeDef,
     ExcelOptionsOutputTypeDef,
     ExcelOptionsTypeDef,
-    FilesLimitOutputTypeDef,
     FilesLimitTypeDef,
-    JsonOptionsOutputTypeDef,
     JsonOptionsTypeDef,
-    MetadataOutputTypeDef,
     MetadataTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDatasetsRequestRequestTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
-    ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
     ListRecipeVersionsRequestRequestTypeDef,
-    ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
-    ListRulesetsRequestListRulesetsPaginateTypeDef,
     ListRulesetsRequestRequestTypeDef,
     RulesetItemTypeDef,
-    ListSchedulesRequestListSchedulesPaginateTypeDef,
     ListSchedulesRequestRequestTypeDef,
     ScheduleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PublishRecipeRequestRequestTypeDef,
-    PublishRecipeResponseTypeDef,
     RecipeActionOutputTypeDef,
     RecipeActionTypeDef,
-    ResponseMetadataTypeDef,
-    ThresholdOutputTypeDef,
     ThresholdTypeDef,
     ViewFrameTypeDef,
-    SendProjectSessionActionResponseTypeDef,
     StartJobRunRequestRequestTypeDef,
-    StartJobRunResponseTypeDef,
     StartProjectSessionRequestRequestTypeDef,
-    StartProjectSessionResponseTypeDef,
     StatisticOverrideOutputTypeDef,
     StatisticOverrideTypeDef,
     StopJobRunRequestRequestTypeDef,
-    StopJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateScheduleRequestRequestTypeDef,
+    EntityDetectorConfigurationOutputTypeDef,
+    EntityDetectorConfigurationTypeDef,
+    BatchDeleteRecipeVersionResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateProfileJobResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateRecipeJobResponseTypeDef,
+    CreateRecipeResponseTypeDef,
+    CreateRulesetResponseTypeDef,
+    CreateScheduleResponseTypeDef,
+    DeleteDatasetResponseTypeDef,
+    DeleteJobResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteRecipeVersionResponseTypeDef,
+    DeleteRulesetResponseTypeDef,
+    DeleteScheduleResponseTypeDef,
+    DescribeScheduleResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PublishRecipeResponseTypeDef,
+    SendProjectSessionActionResponseTypeDef,
+    StartJobRunResponseTypeDef,
+    StartProjectSessionResponseTypeDef,
+    StopJobRunResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
-    UpdateScheduleRequestRequestTypeDef,
     UpdateScheduleResponseTypeDef,
-    EntityDetectorConfigurationOutputTypeDef,
-    EntityDetectorConfigurationTypeDef,
-    BatchDeleteRecipeVersionResponseTypeDef,
     DataCatalogInputDefinitionTypeDef,
     DatabaseInputDefinitionTypeDef,
     DatabaseTableOutputOptionsTypeDef,
     S3TableOutputOptionsTypeDef,
     CreateProjectRequestRequestTypeDef,
+    DescribeProjectResponseTypeDef,
+    ProjectTypeDef,
     UpdateProjectRequestRequestTypeDef,
-    OutputFormatOptionsOutputTypeDef,
     OutputFormatOptionsTypeDef,
-    DataCatalogInputDefinitionOutputTypeDef,
-    DatabaseInputDefinitionOutputTypeDef,
-    DatabaseTableOutputOptionsOutputTypeDef,
-    S3TableOutputOptionsOutputTypeDef,
     DatasetParameterOutputTypeDef,
     DatasetParameterTypeDef,
-    DescribeProjectResponseTypeDef,
-    ProjectTypeDef,
     FormatOptionsOutputTypeDef,
     FormatOptionsTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
+    ListRecipesRequestListRecipesPaginateTypeDef,
+    ListRulesetsRequestListRulesetsPaginateTypeDef,
+    ListSchedulesRequestListSchedulesPaginateTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
     RecipeStepOutputTypeDef,
     RecipeStepTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
     StatisticsConfigurationOutputTypeDef,
     StatisticsConfigurationTypeDef,
     InputTypeDef,
     DatabaseOutputTypeDef,
     DataCatalogOutputTypeDef,
+    ListProjectsResponseTypeDef,
     OutputTypeDef,
-    InputOutputTypeDef,
     PathOptionsOutputTypeDef,
     PathOptionsTypeDef,
-    ListProjectsResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     RecipeTypeDef,
     CreateRecipeRequestRequestTypeDef,
     SendProjectSessionActionRequestRequestTypeDef,
     UpdateRecipeRequestRequestTypeDef,
     DescribeRulesetResponseTypeDef,
     CreateRulesetRequestRequestTypeDef,
```

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/__init__.py` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/__init__.pyi` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/__main__.py` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GlueDataBrew 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.GlueDataBrew 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew\nOther"
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

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/client.py` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/client.pyi` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/literals.py` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/literals.pyi` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/paginator.py` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,30 +74,30 @@
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listdatasetspaginator)
         """
 
 
 class ListJobRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listjobrunspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listjobrunspaginator)
         """
 
 
@@ -108,88 +108,88 @@
     """
 
     def paginate(
         self,
         *,
         DatasetName: str = ...,
         ProjectName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listjobspaginator)
         """
 
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listprojectspaginator)
         """
 
 
 class ListRecipeVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipeVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipeversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecipeVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipeVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipeversionspaginator)
         """
 
 
 class ListRecipesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipespaginator)
     """
 
     def paginate(
-        self, *, RecipeVersion: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RecipeVersion: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipespaginator)
         """
 
 
 class ListRulesetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRulesets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrulesetspaginator)
     """
 
     def paginate(
-        self, *, TargetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TargetArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRulesets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrulesetspaginator)
         """
 
 
 class ListSchedulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListSchedules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listschedulespaginator)
     """
 
     def paginate(
-        self, *, JobName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, JobName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchedulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listschedulespaginator)
         """
```

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/paginator.pyi` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -71,29 +71,29 @@
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listdatasetspaginator)
         """
 
 class ListJobRunsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobRuns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listjobrunspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listjobrunspaginator)
         """
 
 class ListJobsPaginator(Paginator):
@@ -103,83 +103,83 @@
     """
 
     def paginate(
         self,
         *,
         DatasetName: str = ...,
         ProjectName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listjobspaginator)
         """
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listprojectspaginator)
         """
 
 class ListRecipeVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipeVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipeversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecipeVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipeVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipeversionspaginator)
         """
 
 class ListRecipesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipespaginator)
     """
 
     def paginate(
-        self, *, RecipeVersion: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RecipeVersion: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRecipes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrecipespaginator)
         """
 
 class ListRulesetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRulesets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrulesetspaginator)
     """
 
     def paginate(
-        self, *, TargetArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TargetArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRulesetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListRulesets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listrulesetspaginator)
         """
 
 class ListSchedulesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListSchedules)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listschedulespaginator)
     """
 
     def paginate(
-        self, *, JobName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, JobName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSchedulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListSchedules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/paginators/#listschedulespaginator)
         """
```

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/type_defs.py` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,157 +45,137 @@
 
 
 __all__ = (
     "AllowedStatisticsOutputTypeDef",
     "AllowedStatisticsTypeDef",
     "BatchDeleteRecipeVersionRequestRequestTypeDef",
     "RecipeVersionErrorDetailTypeDef",
-    "ColumnSelectorOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "ColumnSelectorTypeDef",
-    "ConditionExpressionOutputTypeDef",
     "ConditionExpressionTypeDef",
-    "CreateDatasetResponseTypeDef",
     "JobSampleTypeDef",
     "S3LocationTypeDef",
     "ValidationConfigurationTypeDef",
-    "CreateProfileJobResponseTypeDef",
     "SampleTypeDef",
-    "CreateProjectResponseTypeDef",
     "RecipeReferenceTypeDef",
-    "CreateRecipeJobResponseTypeDef",
-    "CreateRecipeResponseTypeDef",
-    "CreateRulesetResponseTypeDef",
     "CreateScheduleRequestRequestTypeDef",
-    "CreateScheduleResponseTypeDef",
-    "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
-    "CsvOutputOptionsOutputTypeDef",
     "CsvOutputOptionsTypeDef",
-    "S3LocationOutputTypeDef",
-    "DatetimeOptionsOutputTypeDef",
-    "FilterExpressionOutputTypeDef",
     "DatetimeOptionsTypeDef",
+    "FilterExpressionOutputTypeDef",
     "FilterExpressionTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
-    "DeleteDatasetResponseTypeDef",
     "DeleteJobRequestRequestTypeDef",
-    "DeleteJobResponseTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResponseTypeDef",
     "DeleteRecipeVersionRequestRequestTypeDef",
-    "DeleteRecipeVersionResponseTypeDef",
     "DeleteRulesetRequestRequestTypeDef",
-    "DeleteRulesetResponseTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
-    "DeleteScheduleResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
-    "JobSampleOutputTypeDef",
-    "RecipeReferenceOutputTypeDef",
-    "ValidationConfigurationOutputTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
-    "SampleOutputTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
     "DescribeRulesetRequestRequestTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
-    "DescribeScheduleResponseTypeDef",
     "ExcelOptionsOutputTypeDef",
     "ExcelOptionsTypeDef",
-    "FilesLimitOutputTypeDef",
     "FilesLimitTypeDef",
-    "JsonOptionsOutputTypeDef",
     "JsonOptionsTypeDef",
-    "MetadataOutputTypeDef",
     "MetadataTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDatasetsRequestRequestTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
-    "ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     "ListRecipeVersionsRequestRequestTypeDef",
-    "ListRecipesRequestListRecipesPaginateTypeDef",
     "ListRecipesRequestRequestTypeDef",
-    "ListRulesetsRequestListRulesetsPaginateTypeDef",
     "ListRulesetsRequestRequestTypeDef",
     "RulesetItemTypeDef",
-    "ListSchedulesRequestListSchedulesPaginateTypeDef",
     "ListSchedulesRequestRequestTypeDef",
     "ScheduleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PublishRecipeRequestRequestTypeDef",
-    "PublishRecipeResponseTypeDef",
     "RecipeActionOutputTypeDef",
     "RecipeActionTypeDef",
-    "ResponseMetadataTypeDef",
-    "ThresholdOutputTypeDef",
     "ThresholdTypeDef",
     "ViewFrameTypeDef",
-    "SendProjectSessionActionResponseTypeDef",
     "StartJobRunRequestRequestTypeDef",
-    "StartJobRunResponseTypeDef",
     "StartProjectSessionRequestRequestTypeDef",
-    "StartProjectSessionResponseTypeDef",
     "StatisticOverrideOutputTypeDef",
     "StatisticOverrideTypeDef",
     "StopJobRunRequestRequestTypeDef",
-    "StopJobRunResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateScheduleRequestRequestTypeDef",
+    "EntityDetectorConfigurationOutputTypeDef",
+    "EntityDetectorConfigurationTypeDef",
+    "BatchDeleteRecipeVersionResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateProfileJobResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateRecipeJobResponseTypeDef",
+    "CreateRecipeResponseTypeDef",
+    "CreateRulesetResponseTypeDef",
+    "CreateScheduleResponseTypeDef",
+    "DeleteDatasetResponseTypeDef",
+    "DeleteJobResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "DeleteRecipeVersionResponseTypeDef",
+    "DeleteRulesetResponseTypeDef",
+    "DeleteScheduleResponseTypeDef",
+    "DescribeScheduleResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PublishRecipeResponseTypeDef",
+    "SendProjectSessionActionResponseTypeDef",
+    "StartJobRunResponseTypeDef",
+    "StartProjectSessionResponseTypeDef",
+    "StopJobRunResponseTypeDef",
     "UpdateDatasetResponseTypeDef",
     "UpdateProfileJobResponseTypeDef",
     "UpdateProjectResponseTypeDef",
     "UpdateRecipeJobResponseTypeDef",
     "UpdateRecipeResponseTypeDef",
     "UpdateRulesetResponseTypeDef",
-    "UpdateScheduleRequestRequestTypeDef",
     "UpdateScheduleResponseTypeDef",
-    "EntityDetectorConfigurationOutputTypeDef",
-    "EntityDetectorConfigurationTypeDef",
-    "BatchDeleteRecipeVersionResponseTypeDef",
     "DataCatalogInputDefinitionTypeDef",
     "DatabaseInputDefinitionTypeDef",
     "DatabaseTableOutputOptionsTypeDef",
     "S3TableOutputOptionsTypeDef",
     "CreateProjectRequestRequestTypeDef",
+    "DescribeProjectResponseTypeDef",
+    "ProjectTypeDef",
     "UpdateProjectRequestRequestTypeDef",
-    "OutputFormatOptionsOutputTypeDef",
     "OutputFormatOptionsTypeDef",
-    "DataCatalogInputDefinitionOutputTypeDef",
-    "DatabaseInputDefinitionOutputTypeDef",
-    "DatabaseTableOutputOptionsOutputTypeDef",
-    "S3TableOutputOptionsOutputTypeDef",
     "DatasetParameterOutputTypeDef",
     "DatasetParameterTypeDef",
-    "DescribeProjectResponseTypeDef",
-    "ProjectTypeDef",
     "FormatOptionsOutputTypeDef",
     "FormatOptionsTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
+    "ListRecipesRequestListRecipesPaginateTypeDef",
+    "ListRulesetsRequestListRulesetsPaginateTypeDef",
+    "ListSchedulesRequestListSchedulesPaginateTypeDef",
     "ListRulesetsResponseTypeDef",
     "ListSchedulesResponseTypeDef",
     "RecipeStepOutputTypeDef",
     "RecipeStepTypeDef",
     "RuleOutputTypeDef",
     "RuleTypeDef",
     "StatisticsConfigurationOutputTypeDef",
     "StatisticsConfigurationTypeDef",
     "InputTypeDef",
     "DatabaseOutputTypeDef",
     "DataCatalogOutputTypeDef",
+    "ListProjectsResponseTypeDef",
     "OutputTypeDef",
-    "InputOutputTypeDef",
     "PathOptionsOutputTypeDef",
     "PathOptionsTypeDef",
-    "ListProjectsResponseTypeDef",
     "DescribeRecipeResponseTypeDef",
     "RecipeTypeDef",
     "CreateRecipeRequestRequestTypeDef",
     "SendProjectSessionActionRequestRequestTypeDef",
     "UpdateRecipeRequestRequestTypeDef",
     "DescribeRulesetResponseTypeDef",
     "CreateRulesetRequestRequestTypeDef",
@@ -251,54 +231,34 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "RecipeVersion": str,
     },
     total=False,
 )
 
-ColumnSelectorOutputTypeDef = TypedDict(
-    "ColumnSelectorOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Regex": str,
-        "Name": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 ColumnSelectorTypeDef = TypedDict(
     "ColumnSelectorTypeDef",
     {
         "Regex": str,
         "Name": str,
     },
     total=False,
 )
 
-_RequiredConditionExpressionOutputTypeDef = TypedDict(
-    "_RequiredConditionExpressionOutputTypeDef",
-    {
-        "Condition": str,
-        "TargetColumn": str,
-    },
-)
-_OptionalConditionExpressionOutputTypeDef = TypedDict(
-    "_OptionalConditionExpressionOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-
-class ConditionExpressionOutputTypeDef(
-    _RequiredConditionExpressionOutputTypeDef, _OptionalConditionExpressionOutputTypeDef
-):
-    pass
-
-
 _RequiredConditionExpressionTypeDef = TypedDict(
     "_RequiredConditionExpressionTypeDef",
     {
         "Condition": str,
         "TargetColumn": str,
     },
 )
@@ -313,22 +273,14 @@
 
 class ConditionExpressionTypeDef(
     _RequiredConditionExpressionTypeDef, _OptionalConditionExpressionTypeDef
 ):
     pass
 
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 JobSampleTypeDef = TypedDict(
     "JobSampleTypeDef",
     {
         "Mode": SampleModeType,
         "Size": int,
     },
     total=False,
@@ -371,22 +323,14 @@
 
 class ValidationConfigurationTypeDef(
     _RequiredValidationConfigurationTypeDef, _OptionalValidationConfigurationTypeDef
 ):
     pass
 
 
-CreateProfileJobResponseTypeDef = TypedDict(
-    "CreateProfileJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSampleTypeDef = TypedDict(
     "_RequiredSampleTypeDef",
     {
         "Type": SampleTypeType,
     },
 )
 _OptionalSampleTypeDef = TypedDict(
@@ -398,22 +342,14 @@
 )
 
 
 class SampleTypeDef(_RequiredSampleTypeDef, _OptionalSampleTypeDef):
     pass
 
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecipeReferenceTypeDef = TypedDict(
     "_RequiredRecipeReferenceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalRecipeReferenceTypeDef = TypedDict(
@@ -425,38 +361,14 @@
 )
 
 
 class RecipeReferenceTypeDef(_RequiredRecipeReferenceTypeDef, _OptionalRecipeReferenceTypeDef):
     pass
 
 
-CreateRecipeJobResponseTypeDef = TypedDict(
-    "CreateRecipeJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRecipeResponseTypeDef = TypedDict(
-    "CreateRecipeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRulesetResponseTypeDef = TypedDict(
-    "CreateRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScheduleRequestRequestTypeDef",
     {
         "CronExpression": str,
         "Name": str,
     },
 )
@@ -472,126 +384,59 @@
 
 class CreateScheduleRequestRequestTypeDef(
     _RequiredCreateScheduleRequestRequestTypeDef, _OptionalCreateScheduleRequestRequestTypeDef
 ):
     pass
 
 
-CreateScheduleResponseTypeDef = TypedDict(
-    "CreateScheduleResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CsvOptionsOutputTypeDef = TypedDict(
-    "CsvOptionsOutputTypeDef",
-    {
-        "Delimiter": str,
-        "HeaderRow": bool,
-    },
-    total=False,
-)
-
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderRow": bool,
     },
     total=False,
 )
 
-CsvOutputOptionsOutputTypeDef = TypedDict(
-    "CsvOutputOptionsOutputTypeDef",
-    {
-        "Delimiter": str,
-    },
-    total=False,
-)
-
 CsvOutputOptionsTypeDef = TypedDict(
     "CsvOutputOptionsTypeDef",
     {
         "Delimiter": str,
     },
     total=False,
 )
 
-_RequiredS3LocationOutputTypeDef = TypedDict(
-    "_RequiredS3LocationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalS3LocationOutputTypeDef = TypedDict(
-    "_OptionalS3LocationOutputTypeDef",
-    {
-        "Key": str,
-        "BucketOwner": str,
-    },
-    total=False,
-)
-
-
-class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
-    pass
-
-
-_RequiredDatetimeOptionsOutputTypeDef = TypedDict(
-    "_RequiredDatetimeOptionsOutputTypeDef",
+_RequiredDatetimeOptionsTypeDef = TypedDict(
+    "_RequiredDatetimeOptionsTypeDef",
     {
         "Format": str,
     },
 )
-_OptionalDatetimeOptionsOutputTypeDef = TypedDict(
-    "_OptionalDatetimeOptionsOutputTypeDef",
+_OptionalDatetimeOptionsTypeDef = TypedDict(
+    "_OptionalDatetimeOptionsTypeDef",
     {
         "TimezoneOffset": str,
         "LocaleCode": str,
     },
     total=False,
 )
 
 
-class DatetimeOptionsOutputTypeDef(
-    _RequiredDatetimeOptionsOutputTypeDef, _OptionalDatetimeOptionsOutputTypeDef
-):
+class DatetimeOptionsTypeDef(_RequiredDatetimeOptionsTypeDef, _OptionalDatetimeOptionsTypeDef):
     pass
 
 
 FilterExpressionOutputTypeDef = TypedDict(
     "FilterExpressionOutputTypeDef",
     {
         "Expression": str,
         "ValuesMap": Dict[str, str],
     },
 )
 
-_RequiredDatetimeOptionsTypeDef = TypedDict(
-    "_RequiredDatetimeOptionsTypeDef",
-    {
-        "Format": str,
-    },
-)
-_OptionalDatetimeOptionsTypeDef = TypedDict(
-    "_OptionalDatetimeOptionsTypeDef",
-    {
-        "TimezoneOffset": str,
-        "LocaleCode": str,
-    },
-    total=False,
-)
-
-
-class DatetimeOptionsTypeDef(_RequiredDatetimeOptionsTypeDef, _OptionalDatetimeOptionsTypeDef):
-    pass
-
-
 FilterExpressionTypeDef = TypedDict(
     "FilterExpressionTypeDef",
     {
         "Expression": str,
         "ValuesMap": Mapping[str, str],
     },
 )
@@ -599,164 +444,64 @@
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteDatasetResponseTypeDef = TypedDict(
-    "DeleteDatasetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteJobRequestRequestTypeDef = TypedDict(
     "DeleteJobRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteJobResponseTypeDef = TypedDict(
-    "DeleteJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRecipeVersionRequestRequestTypeDef = TypedDict(
     "DeleteRecipeVersionRequestRequestTypeDef",
     {
         "Name": str,
         "RecipeVersion": str,
     },
 )
 
-DeleteRecipeVersionResponseTypeDef = TypedDict(
-    "DeleteRecipeVersionResponseTypeDef",
-    {
-        "Name": str,
-        "RecipeVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRulesetRequestRequestTypeDef = TypedDict(
     "DeleteRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteRulesetResponseTypeDef = TypedDict(
-    "DeleteRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteScheduleRequestRequestTypeDef = TypedDict(
     "DeleteScheduleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteScheduleResponseTypeDef = TypedDict(
-    "DeleteScheduleResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 DescribeJobRequestRequestTypeDef = TypedDict(
     "DescribeJobRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-JobSampleOutputTypeDef = TypedDict(
-    "JobSampleOutputTypeDef",
-    {
-        "Mode": SampleModeType,
-        "Size": int,
-    },
-    total=False,
-)
-
-_RequiredRecipeReferenceOutputTypeDef = TypedDict(
-    "_RequiredRecipeReferenceOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalRecipeReferenceOutputTypeDef = TypedDict(
-    "_OptionalRecipeReferenceOutputTypeDef",
-    {
-        "RecipeVersion": str,
-    },
-    total=False,
-)
-
-
-class RecipeReferenceOutputTypeDef(
-    _RequiredRecipeReferenceOutputTypeDef, _OptionalRecipeReferenceOutputTypeDef
-):
-    pass
-
-
-_RequiredValidationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredValidationConfigurationOutputTypeDef",
-    {
-        "RulesetArn": str,
-    },
-)
-_OptionalValidationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalValidationConfigurationOutputTypeDef",
-    {
-        "ValidationMode": Literal["CHECK_ALL"],
-    },
-    total=False,
-)
-
-
-class ValidationConfigurationOutputTypeDef(
-    _RequiredValidationConfigurationOutputTypeDef, _OptionalValidationConfigurationOutputTypeDef
-):
-    pass
-
-
 DescribeJobRunRequestRequestTypeDef = TypedDict(
     "DescribeJobRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
@@ -764,33 +509,14 @@
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-_RequiredSampleOutputTypeDef = TypedDict(
-    "_RequiredSampleOutputTypeDef",
-    {
-        "Type": SampleTypeType,
-    },
-)
-_OptionalSampleOutputTypeDef = TypedDict(
-    "_OptionalSampleOutputTypeDef",
-    {
-        "Size": int,
-    },
-    total=False,
-)
-
-
-class SampleOutputTypeDef(_RequiredSampleOutputTypeDef, _OptionalSampleOutputTypeDef):
-    pass
-
-
 _RequiredDescribeRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRecipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeRecipeRequestRequestTypeDef = TypedDict(
@@ -818,30 +544,14 @@
 DescribeScheduleRequestRequestTypeDef = TypedDict(
     "DescribeScheduleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeScheduleResponseTypeDef = TypedDict(
-    "DescribeScheduleResponseTypeDef",
-    {
-        "CreateDate": datetime,
-        "CreatedBy": str,
-        "JobNames": List[str],
-        "LastModifiedBy": str,
-        "LastModifiedDate": datetime,
-        "ResourceArn": str,
-        "CronExpression": str,
-        "Tags": Dict[str, str],
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExcelOptionsOutputTypeDef = TypedDict(
     "ExcelOptionsOutputTypeDef",
     {
         "SheetNames": List[str],
         "SheetIndexes": List[int],
         "HeaderRow": bool,
     },
@@ -854,34 +564,14 @@
         "SheetNames": Sequence[str],
         "SheetIndexes": Sequence[int],
         "HeaderRow": bool,
     },
     total=False,
 )
 
-_RequiredFilesLimitOutputTypeDef = TypedDict(
-    "_RequiredFilesLimitOutputTypeDef",
-    {
-        "MaxFiles": int,
-    },
-)
-_OptionalFilesLimitOutputTypeDef = TypedDict(
-    "_OptionalFilesLimitOutputTypeDef",
-    {
-        "OrderedBy": Literal["LAST_MODIFIED_DATE"],
-        "Order": OrderType,
-    },
-    total=False,
-)
-
-
-class FilesLimitOutputTypeDef(_RequiredFilesLimitOutputTypeDef, _OptionalFilesLimitOutputTypeDef):
-    pass
-
-
 _RequiredFilesLimitTypeDef = TypedDict(
     "_RequiredFilesLimitTypeDef",
     {
         "MaxFiles": int,
     },
 )
 _OptionalFilesLimitTypeDef = TypedDict(
@@ -894,85 +584,49 @@
 )
 
 
 class FilesLimitTypeDef(_RequiredFilesLimitTypeDef, _OptionalFilesLimitTypeDef):
     pass
 
 
-JsonOptionsOutputTypeDef = TypedDict(
-    "JsonOptionsOutputTypeDef",
-    {
-        "MultiLine": bool,
-    },
-    total=False,
-)
-
 JsonOptionsTypeDef = TypedDict(
     "JsonOptionsTypeDef",
     {
         "MultiLine": bool,
     },
     total=False,
 )
 
-MetadataOutputTypeDef = TypedDict(
-    "MetadataOutputTypeDef",
-    {
-        "SourceArn": str,
-    },
-    total=False,
-)
-
 MetadataTypeDef = TypedDict(
     "MetadataTypeDef",
     {
         "SourceArn": str,
     },
     total=False,
 )
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
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
 
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -987,74 +641,34 @@
 
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "DatasetName": str,
-        "ProjectName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "DatasetName": str,
         "MaxResults": int,
         "NextToken": str,
         "ProjectName": str,
     },
     total=False,
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
-    _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
-    _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRecipeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecipeVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListRecipeVersionsRequestRequestTypeDef = TypedDict(
@@ -1070,42 +684,24 @@
 class ListRecipeVersionsRequestRequestTypeDef(
     _RequiredListRecipeVersionsRequestRequestTypeDef,
     _OptionalListRecipeVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
-    "ListRecipesRequestListRecipesPaginateTypeDef",
-    {
-        "RecipeVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRecipesRequestRequestTypeDef = TypedDict(
     "ListRecipesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RecipeVersion": str,
     },
     total=False,
 )
 
-ListRulesetsRequestListRulesetsPaginateTypeDef = TypedDict(
-    "ListRulesetsRequestListRulesetsPaginateTypeDef",
-    {
-        "TargetArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRulesetsRequestRequestTypeDef = TypedDict(
     "ListRulesetsRequestRequestTypeDef",
     {
         "TargetArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1136,23 +732,14 @@
 )
 
 
 class RulesetItemTypeDef(_RequiredRulesetItemTypeDef, _OptionalRulesetItemTypeDef):
     pass
 
 
-ListSchedulesRequestListSchedulesPaginateTypeDef = TypedDict(
-    "ListSchedulesRequestListSchedulesPaginateTypeDef",
-    {
-        "JobName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSchedulesRequestRequestTypeDef = TypedDict(
     "ListSchedulesRequestRequestTypeDef",
     {
         "JobName": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1189,32 +776,14 @@
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
 _RequiredPublishRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredPublishRecipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalPublishRecipeRequestRequestTypeDef = TypedDict(
@@ -1228,22 +797,14 @@
 
 class PublishRecipeRequestRequestTypeDef(
     _RequiredPublishRecipeRequestRequestTypeDef, _OptionalPublishRecipeRequestRequestTypeDef
 ):
     pass
 
 
-PublishRecipeResponseTypeDef = TypedDict(
-    "PublishRecipeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecipeActionOutputTypeDef = TypedDict(
     "_RequiredRecipeActionOutputTypeDef",
     {
         "Operation": str,
     },
 )
 _OptionalRecipeActionOutputTypeDef = TypedDict(
@@ -1276,45 +837,14 @@
 )
 
 
 class RecipeActionTypeDef(_RequiredRecipeActionTypeDef, _OptionalRecipeActionTypeDef):
     pass
 
 
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
-_RequiredThresholdOutputTypeDef = TypedDict(
-    "_RequiredThresholdOutputTypeDef",
-    {
-        "Value": float,
-    },
-)
-_OptionalThresholdOutputTypeDef = TypedDict(
-    "_OptionalThresholdOutputTypeDef",
-    {
-        "Type": ThresholdTypeType,
-        "Unit": ThresholdUnitType,
-    },
-    total=False,
-)
-
-
-class ThresholdOutputTypeDef(_RequiredThresholdOutputTypeDef, _OptionalThresholdOutputTypeDef):
-    pass
-
-
 _RequiredThresholdTypeDef = TypedDict(
     "_RequiredThresholdTypeDef",
     {
         "Value": float,
     },
 )
 _OptionalThresholdTypeDef = TypedDict(
@@ -1350,39 +880,21 @@
 )
 
 
 class ViewFrameTypeDef(_RequiredViewFrameTypeDef, _OptionalViewFrameTypeDef):
     pass
 
 
-SendProjectSessionActionResponseTypeDef = TypedDict(
-    "SendProjectSessionActionResponseTypeDef",
-    {
-        "Result": str,
-        "Name": str,
-        "ActionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartJobRunRequestRequestTypeDef = TypedDict(
     "StartJobRunRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartProjectSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartProjectSessionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalStartProjectSessionRequestRequestTypeDef = TypedDict(
@@ -1397,23 +909,14 @@
 class StartProjectSessionRequestRequestTypeDef(
     _RequiredStartProjectSessionRequestRequestTypeDef,
     _OptionalStartProjectSessionRequestRequestTypeDef,
 ):
     pass
 
 
-StartProjectSessionResponseTypeDef = TypedDict(
-    "StartProjectSessionResponseTypeDef",
-    {
-        "Name": str,
-        "ClientSessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StatisticOverrideOutputTypeDef = TypedDict(
     "StatisticOverrideOutputTypeDef",
     {
         "Statistic": str,
         "Parameters": Dict[str, str],
     },
 )
@@ -1430,22 +933,14 @@
     "StopJobRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
 
-StopJobRunResponseTypeDef = TypedDict(
-    "StopJobRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1454,63 +949,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateDatasetResponseTypeDef = TypedDict(
-    "UpdateDatasetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateProfileJobResponseTypeDef = TypedDict(
-    "UpdateProfileJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateProjectResponseTypeDef = TypedDict(
-    "UpdateProjectResponseTypeDef",
-    {
-        "LastModifiedDate": datetime,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateRecipeJobResponseTypeDef = TypedDict(
-    "UpdateRecipeJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateRecipeResponseTypeDef = TypedDict(
-    "UpdateRecipeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateRulesetResponseTypeDef = TypedDict(
-    "UpdateRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduleRequestRequestTypeDef",
     {
         "CronExpression": str,
         "Name": str,
     },
 )
@@ -1525,22 +971,14 @@
 
 class UpdateScheduleRequestRequestTypeDef(
     _RequiredUpdateScheduleRequestRequestTypeDef, _OptionalUpdateScheduleRequestRequestTypeDef
 ):
     pass
 
 
-UpdateScheduleResponseTypeDef = TypedDict(
-    "UpdateScheduleResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEntityDetectorConfigurationOutputTypeDef = TypedDict(
     "_RequiredEntityDetectorConfigurationOutputTypeDef",
     {
         "EntityTypes": List[str],
     },
 )
 _OptionalEntityDetectorConfigurationOutputTypeDef = TypedDict(
@@ -1581,15 +1019,244 @@
 
 
 BatchDeleteRecipeVersionResponseTypeDef = TypedDict(
     "BatchDeleteRecipeVersionResponseTypeDef",
     {
         "Name": str,
         "Errors": List[RecipeVersionErrorDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileJobResponseTypeDef = TypedDict(
+    "CreateProfileJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRecipeJobResponseTypeDef = TypedDict(
+    "CreateRecipeJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRecipeResponseTypeDef = TypedDict(
+    "CreateRecipeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRulesetResponseTypeDef = TypedDict(
+    "CreateRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScheduleResponseTypeDef = TypedDict(
+    "CreateScheduleResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDatasetResponseTypeDef = TypedDict(
+    "DeleteDatasetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteJobResponseTypeDef = TypedDict(
+    "DeleteJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRecipeVersionResponseTypeDef = TypedDict(
+    "DeleteRecipeVersionResponseTypeDef",
+    {
+        "Name": str,
+        "RecipeVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRulesetResponseTypeDef = TypedDict(
+    "DeleteRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteScheduleResponseTypeDef = TypedDict(
+    "DeleteScheduleResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeScheduleResponseTypeDef = TypedDict(
+    "DescribeScheduleResponseTypeDef",
+    {
+        "CreateDate": datetime,
+        "CreatedBy": str,
+        "JobNames": List[str],
+        "LastModifiedBy": str,
+        "LastModifiedDate": datetime,
+        "ResourceArn": str,
+        "CronExpression": str,
+        "Tags": Dict[str, str],
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishRecipeResponseTypeDef = TypedDict(
+    "PublishRecipeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendProjectSessionActionResponseTypeDef = TypedDict(
+    "SendProjectSessionActionResponseTypeDef",
+    {
+        "Result": str,
+        "Name": str,
+        "ActionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartProjectSessionResponseTypeDef = TypedDict(
+    "StartProjectSessionResponseTypeDef",
+    {
+        "Name": str,
+        "ClientSessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopJobRunResponseTypeDef = TypedDict(
+    "StopJobRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDatasetResponseTypeDef = TypedDict(
+    "UpdateDatasetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProfileJobResponseTypeDef = TypedDict(
+    "UpdateProfileJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProjectResponseTypeDef = TypedDict(
+    "UpdateProjectResponseTypeDef",
+    {
+        "LastModifiedDate": datetime,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRecipeJobResponseTypeDef = TypedDict(
+    "UpdateRecipeJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRecipeResponseTypeDef = TypedDict(
+    "UpdateRecipeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRulesetResponseTypeDef = TypedDict(
+    "UpdateRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateScheduleResponseTypeDef = TypedDict(
+    "UpdateScheduleResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDataCatalogInputDefinitionTypeDef = TypedDict(
     "_RequiredDataCatalogInputDefinitionTypeDef",
     {
         "DatabaseName": str,
@@ -1684,14 +1351,66 @@
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
 
+DescribeProjectResponseTypeDef = TypedDict(
+    "DescribeProjectResponseTypeDef",
+    {
+        "CreateDate": datetime,
+        "CreatedBy": str,
+        "DatasetName": str,
+        "LastModifiedDate": datetime,
+        "LastModifiedBy": str,
+        "Name": str,
+        "RecipeName": str,
+        "ResourceArn": str,
+        "Sample": SampleTypeDef,
+        "RoleArn": str,
+        "Tags": Dict[str, str],
+        "SessionStatus": SessionStatusType,
+        "OpenedBy": str,
+        "OpenDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredProjectTypeDef = TypedDict(
+    "_RequiredProjectTypeDef",
+    {
+        "Name": str,
+        "RecipeName": str,
+    },
+)
+_OptionalProjectTypeDef = TypedDict(
+    "_OptionalProjectTypeDef",
+    {
+        "AccountId": str,
+        "CreateDate": datetime,
+        "CreatedBy": str,
+        "DatasetName": str,
+        "LastModifiedDate": datetime,
+        "LastModifiedBy": str,
+        "ResourceArn": str,
+        "Sample": SampleTypeDef,
+        "Tags": Dict[str, str],
+        "RoleArn": str,
+        "OpenedBy": str,
+        "OpenDate": datetime,
+    },
+    total=False,
+)
+
+
+class ProjectTypeDef(_RequiredProjectTypeDef, _OptionalProjectTypeDef):
+    pass
+
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "RoleArn": str,
         "Name": str,
     },
 )
@@ -1706,252 +1425,213 @@
 
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
     pass
 
 
-OutputFormatOptionsOutputTypeDef = TypedDict(
-    "OutputFormatOptionsOutputTypeDef",
-    {
-        "Csv": CsvOutputOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 OutputFormatOptionsTypeDef = TypedDict(
     "OutputFormatOptionsTypeDef",
     {
         "Csv": CsvOutputOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredDataCatalogInputDefinitionOutputTypeDef = TypedDict(
-    "_RequiredDataCatalogInputDefinitionOutputTypeDef",
+_RequiredDatasetParameterOutputTypeDef = TypedDict(
+    "_RequiredDatasetParameterOutputTypeDef",
     {
-        "DatabaseName": str,
-        "TableName": str,
+        "Name": str,
+        "Type": ParameterTypeType,
     },
 )
-_OptionalDataCatalogInputDefinitionOutputTypeDef = TypedDict(
-    "_OptionalDataCatalogInputDefinitionOutputTypeDef",
+_OptionalDatasetParameterOutputTypeDef = TypedDict(
+    "_OptionalDatasetParameterOutputTypeDef",
     {
-        "CatalogId": str,
-        "TempDirectory": S3LocationOutputTypeDef,
+        "DatetimeOptions": DatetimeOptionsTypeDef,
+        "CreateColumn": bool,
+        "Filter": FilterExpressionOutputTypeDef,
     },
     total=False,
 )
 
 
-class DataCatalogInputDefinitionOutputTypeDef(
-    _RequiredDataCatalogInputDefinitionOutputTypeDef,
-    _OptionalDataCatalogInputDefinitionOutputTypeDef,
+class DatasetParameterOutputTypeDef(
+    _RequiredDatasetParameterOutputTypeDef, _OptionalDatasetParameterOutputTypeDef
 ):
     pass
 
 
-_RequiredDatabaseInputDefinitionOutputTypeDef = TypedDict(
-    "_RequiredDatabaseInputDefinitionOutputTypeDef",
+_RequiredDatasetParameterTypeDef = TypedDict(
+    "_RequiredDatasetParameterTypeDef",
     {
-        "GlueConnectionName": str,
+        "Name": str,
+        "Type": ParameterTypeType,
     },
 )
-_OptionalDatabaseInputDefinitionOutputTypeDef = TypedDict(
-    "_OptionalDatabaseInputDefinitionOutputTypeDef",
+_OptionalDatasetParameterTypeDef = TypedDict(
+    "_OptionalDatasetParameterTypeDef",
     {
-        "DatabaseTableName": str,
-        "TempDirectory": S3LocationOutputTypeDef,
-        "QueryString": str,
+        "DatetimeOptions": DatetimeOptionsTypeDef,
+        "CreateColumn": bool,
+        "Filter": FilterExpressionTypeDef,
     },
     total=False,
 )
 
 
-class DatabaseInputDefinitionOutputTypeDef(
-    _RequiredDatabaseInputDefinitionOutputTypeDef, _OptionalDatabaseInputDefinitionOutputTypeDef
-):
+class DatasetParameterTypeDef(_RequiredDatasetParameterTypeDef, _OptionalDatasetParameterTypeDef):
     pass
 
 
-_RequiredDatabaseTableOutputOptionsOutputTypeDef = TypedDict(
-    "_RequiredDatabaseTableOutputOptionsOutputTypeDef",
+FormatOptionsOutputTypeDef = TypedDict(
+    "FormatOptionsOutputTypeDef",
     {
-        "TableName": str,
+        "Json": JsonOptionsTypeDef,
+        "Excel": ExcelOptionsOutputTypeDef,
+        "Csv": CsvOptionsTypeDef,
     },
+    total=False,
 )
-_OptionalDatabaseTableOutputOptionsOutputTypeDef = TypedDict(
-    "_OptionalDatabaseTableOutputOptionsOutputTypeDef",
+
+FormatOptionsTypeDef = TypedDict(
+    "FormatOptionsTypeDef",
     {
-        "TempDirectory": S3LocationOutputTypeDef,
+        "Json": JsonOptionsTypeDef,
+        "Excel": ExcelOptionsTypeDef,
+        "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
 
-
-class DatabaseTableOutputOptionsOutputTypeDef(
-    _RequiredDatabaseTableOutputOptionsOutputTypeDef,
-    _OptionalDatabaseTableOutputOptionsOutputTypeDef,
-):
-    pass
-
-
-S3TableOutputOptionsOutputTypeDef = TypedDict(
-    "S3TableOutputOptionsOutputTypeDef",
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     {
-        "Location": S3LocationOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredDatasetParameterOutputTypeDef = TypedDict(
-    "_RequiredDatasetParameterOutputTypeDef",
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
     {
         "Name": str,
-        "Type": ParameterTypeType,
     },
 )
-_OptionalDatasetParameterOutputTypeDef = TypedDict(
-    "_OptionalDatasetParameterOutputTypeDef",
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
     {
-        "DatetimeOptions": DatetimeOptionsOutputTypeDef,
-        "CreateColumn": bool,
-        "Filter": FilterExpressionOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class DatasetParameterOutputTypeDef(
-    _RequiredDatasetParameterOutputTypeDef, _OptionalDatasetParameterOutputTypeDef
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredDatasetParameterTypeDef = TypedDict(
-    "_RequiredDatasetParameterTypeDef",
-    {
-        "Name": str,
-        "Type": ParameterTypeType,
-    },
-)
-_OptionalDatasetParameterTypeDef = TypedDict(
-    "_OptionalDatasetParameterTypeDef",
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
     {
-        "DatetimeOptions": DatetimeOptionsTypeDef,
-        "CreateColumn": bool,
-        "Filter": FilterExpressionTypeDef,
+        "DatasetName": str,
+        "ProjectName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class DatasetParameterTypeDef(_RequiredDatasetParameterTypeDef, _OptionalDatasetParameterTypeDef):
-    pass
-
-
-DescribeProjectResponseTypeDef = TypedDict(
-    "DescribeProjectResponseTypeDef",
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     {
-        "CreateDate": datetime,
-        "CreatedBy": str,
-        "DatasetName": str,
-        "LastModifiedDate": datetime,
-        "LastModifiedBy": str,
-        "Name": str,
-        "RecipeName": str,
-        "ResourceArn": str,
-        "Sample": SampleOutputTypeDef,
-        "RoleArn": str,
-        "Tags": Dict[str, str],
-        "SessionStatus": SessionStatusType,
-        "OpenedBy": str,
-        "OpenDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredProjectTypeDef = TypedDict(
-    "_RequiredProjectTypeDef",
+_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     {
         "Name": str,
-        "RecipeName": str,
     },
 )
-_OptionalProjectTypeDef = TypedDict(
-    "_OptionalProjectTypeDef",
+_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     {
-        "AccountId": str,
-        "CreateDate": datetime,
-        "CreatedBy": str,
-        "DatasetName": str,
-        "LastModifiedDate": datetime,
-        "LastModifiedBy": str,
-        "ResourceArn": str,
-        "Sample": SampleOutputTypeDef,
-        "Tags": Dict[str, str],
-        "RoleArn": str,
-        "OpenedBy": str,
-        "OpenDate": datetime,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ProjectTypeDef(_RequiredProjectTypeDef, _OptionalProjectTypeDef):
+class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
+    _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
+    _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
+):
     pass
 
 
-FormatOptionsOutputTypeDef = TypedDict(
-    "FormatOptionsOutputTypeDef",
+ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
+    "ListRecipesRequestListRecipesPaginateTypeDef",
     {
-        "Json": JsonOptionsOutputTypeDef,
-        "Excel": ExcelOptionsOutputTypeDef,
-        "Csv": CsvOptionsOutputTypeDef,
+        "RecipeVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-FormatOptionsTypeDef = TypedDict(
-    "FormatOptionsTypeDef",
+ListRulesetsRequestListRulesetsPaginateTypeDef = TypedDict(
+    "ListRulesetsRequestListRulesetsPaginateTypeDef",
     {
-        "Json": JsonOptionsTypeDef,
-        "Excel": ExcelOptionsTypeDef,
-        "Csv": CsvOptionsTypeDef,
+        "TargetArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSchedulesRequestListSchedulesPaginateTypeDef = TypedDict(
+    "ListSchedulesRequestListSchedulesPaginateTypeDef",
+    {
+        "JobName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListRulesetsResponseTypeDef = TypedDict(
     "ListRulesetsResponseTypeDef",
     {
         "Rulesets": List[RulesetItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchedulesResponseTypeDef = TypedDict(
     "ListSchedulesResponseTypeDef",
     {
         "Schedules": List[ScheduleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRecipeStepOutputTypeDef = TypedDict(
     "_RequiredRecipeStepOutputTypeDef",
     {
         "Action": RecipeActionOutputTypeDef,
     },
 )
 _OptionalRecipeStepOutputTypeDef = TypedDict(
     "_OptionalRecipeStepOutputTypeDef",
     {
-        "ConditionExpressions": List[ConditionExpressionOutputTypeDef],
+        "ConditionExpressions": List[ConditionExpressionTypeDef],
     },
     total=False,
 )
 
 
 class RecipeStepOutputTypeDef(_RequiredRecipeStepOutputTypeDef, _OptionalRecipeStepOutputTypeDef):
     pass
@@ -1984,16 +1664,16 @@
     },
 )
 _OptionalRuleOutputTypeDef = TypedDict(
     "_OptionalRuleOutputTypeDef",
     {
         "Disabled": bool,
         "SubstitutionMap": Dict[str, str],
-        "Threshold": ThresholdOutputTypeDef,
-        "ColumnSelectors": List[ColumnSelectorOutputTypeDef],
+        "Threshold": ThresholdTypeDef,
+        "ColumnSelectors": List[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
 
 class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
     pass
@@ -2092,14 +1772,23 @@
 
 class DataCatalogOutputTypeDef(
     _RequiredDataCatalogOutputTypeDef, _OptionalDataCatalogOutputTypeDef
 ):
     pass
 
 
+ListProjectsResponseTypeDef = TypedDict(
+    "ListProjectsResponseTypeDef",
+    {
+        "Projects": List[ProjectTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
         "Location": S3LocationTypeDef,
     },
 )
 _OptionalOutputTypeDef = TypedDict(
@@ -2116,30 +1805,19 @@
 )
 
 
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
 
-InputOutputTypeDef = TypedDict(
-    "InputOutputTypeDef",
-    {
-        "S3InputDefinition": S3LocationOutputTypeDef,
-        "DataCatalogInputDefinition": DataCatalogInputDefinitionOutputTypeDef,
-        "DatabaseInputDefinition": DatabaseInputDefinitionOutputTypeDef,
-        "Metadata": MetadataOutputTypeDef,
-    },
-    total=False,
-)
-
 PathOptionsOutputTypeDef = TypedDict(
     "PathOptionsOutputTypeDef",
     {
         "LastModifiedDateCondition": FilterExpressionOutputTypeDef,
-        "FilesLimit": FilesLimitOutputTypeDef,
+        "FilesLimit": FilesLimitTypeDef,
         "Parameters": Dict[str, DatasetParameterOutputTypeDef],
     },
     total=False,
 )
 
 PathOptionsTypeDef = TypedDict(
     "PathOptionsTypeDef",
@@ -2147,23 +1825,14 @@
         "LastModifiedDateCondition": FilterExpressionTypeDef,
         "FilesLimit": FilesLimitTypeDef,
         "Parameters": Mapping[str, DatasetParameterTypeDef],
     },
     total=False,
 )
 
-ListProjectsResponseTypeDef = TypedDict(
-    "ListProjectsResponseTypeDef",
-    {
-        "Projects": List[ProjectTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRecipeResponseTypeDef = TypedDict(
     "DescribeRecipeResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
@@ -2172,15 +1841,15 @@
         "PublishedDate": datetime,
         "Description": str,
         "Name": str,
         "Steps": List[RecipeStepOutputTypeDef],
         "Tags": Dict[str, str],
         "ResourceArn": str,
         "RecipeVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRecipeTypeDef = TypedDict(
     "_RequiredRecipeTypeDef",
     {
         "Name": str,
@@ -2290,15 +1959,15 @@
         "Rules": List[RuleOutputTypeDef],
         "CreateDate": datetime,
         "CreatedBy": str,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ResourceArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRulesetRequestRequestTypeDef",
     {
         "Name": str,
@@ -2349,15 +2018,15 @@
     {
         "Statistics": StatisticsConfigurationOutputTypeDef,
     },
 )
 _OptionalColumnStatisticsConfigurationOutputTypeDef = TypedDict(
     "_OptionalColumnStatisticsConfigurationOutputTypeDef",
     {
-        "Selectors": List[ColumnSelectorOutputTypeDef],
+        "Selectors": List[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
 
 class ColumnStatisticsConfigurationOutputTypeDef(
     _RequiredColumnStatisticsConfigurationOutputTypeDef,
@@ -2433,19 +2102,19 @@
         "RunId": str,
         "State": JobRunStateType,
         "LogSubscription": LogSubscriptionType,
         "LogGroupName": str,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
-        "RecipeReference": RecipeReferenceOutputTypeDef,
+        "RecipeReference": RecipeReferenceTypeDef,
         "StartedBy": str,
         "StartedOn": datetime,
-        "JobSample": JobSampleOutputTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
+        "JobSample": JobSampleTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
@@ -2467,21 +2136,21 @@
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
         "ProjectName": str,
-        "RecipeReference": RecipeReferenceOutputTypeDef,
+        "RecipeReference": RecipeReferenceTypeDef,
         "ResourceArn": str,
         "RoleArn": str,
         "Timeout": int,
         "Tags": Dict[str, str],
-        "JobSample": JobSampleOutputTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
+        "JobSample": JobSampleTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
@@ -2517,15 +2186,15 @@
     pass
 
 
 _RequiredDatasetTypeDef = TypedDict(
     "_RequiredDatasetTypeDef",
     {
         "Name": str,
-        "Input": InputOutputTypeDef,
+        "Input": InputTypeDef,
     },
 )
 _OptionalDatasetTypeDef = TypedDict(
     "_OptionalDatasetTypeDef",
     {
         "AccountId": str,
         "CreatedBy": str,
@@ -2551,22 +2220,22 @@
     "DescribeDatasetResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "Name": str,
         "Format": InputFormatType,
         "FormatOptions": FormatOptionsOutputTypeDef,
-        "Input": InputOutputTypeDef,
+        "Input": InputTypeDef,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Source": SourceType,
         "PathOptions": PathOptionsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "Name": str,
@@ -2616,32 +2285,32 @@
 
 
 ListRecipeVersionsResponseTypeDef = TypedDict(
     "ListRecipeVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Recipes": List[RecipeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecipesResponseTypeDef = TypedDict(
     "ListRecipesResponseTypeDef",
     {
         "Recipes": List[RecipeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProfileConfigurationOutputTypeDef = TypedDict(
     "ProfileConfigurationOutputTypeDef",
     {
         "DatasetStatisticsConfiguration": StatisticsConfigurationOutputTypeDef,
-        "ProfileColumns": List[ColumnSelectorOutputTypeDef],
+        "ProfileColumns": List[ColumnSelectorTypeDef],
         "ColumnStatisticsConfigurations": List[ColumnStatisticsConfigurationOutputTypeDef],
         "EntityDetectorConfiguration": EntityDetectorConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 ProfileConfigurationTypeDef = TypedDict(
@@ -2656,33 +2325,33 @@
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "JobRuns": List[JobRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobResponseTypeDef = TypedDict(
     "DescribeJobResponseTypeDef",
     {
         "CreateDate": datetime,
@@ -2698,48 +2367,48 @@
         "MaxCapacity": int,
         "MaxRetries": int,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
         "ProjectName": str,
         "ProfileConfiguration": ProfileConfigurationOutputTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
-        "RecipeReference": RecipeReferenceOutputTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
+        "RecipeReference": RecipeReferenceTypeDef,
         "ResourceArn": str,
         "RoleArn": str,
         "Tags": Dict[str, str],
         "Timeout": int,
-        "JobSample": JobSampleOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobSample": JobSampleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobRunResponseTypeDef = TypedDict(
     "DescribeJobRunResponseTypeDef",
     {
         "Attempt": int,
         "CompletedOn": datetime,
         "DatasetName": str,
         "ErrorMessage": str,
         "ExecutionTime": int,
         "JobName": str,
         "ProfileConfiguration": ProfileConfigurationOutputTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
+        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
         "RunId": str,
         "State": JobRunStateType,
         "LogSubscription": LogSubscriptionType,
         "LogGroupName": str,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
-        "RecipeReference": RecipeReferenceOutputTypeDef,
+        "RecipeReference": RecipeReferenceTypeDef,
         "StartedBy": str,
         "StartedOn": datetime,
-        "JobSample": JobSampleOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobSample": JobSampleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProfileJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfileJobRequestRequestTypeDef",
     {
         "DatasetName": str,
```

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew/type_defs.pyi` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -44,157 +44,137 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AllowedStatisticsOutputTypeDef",
     "AllowedStatisticsTypeDef",
     "BatchDeleteRecipeVersionRequestRequestTypeDef",
     "RecipeVersionErrorDetailTypeDef",
-    "ColumnSelectorOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "ColumnSelectorTypeDef",
-    "ConditionExpressionOutputTypeDef",
     "ConditionExpressionTypeDef",
-    "CreateDatasetResponseTypeDef",
     "JobSampleTypeDef",
     "S3LocationTypeDef",
     "ValidationConfigurationTypeDef",
-    "CreateProfileJobResponseTypeDef",
     "SampleTypeDef",
-    "CreateProjectResponseTypeDef",
     "RecipeReferenceTypeDef",
-    "CreateRecipeJobResponseTypeDef",
-    "CreateRecipeResponseTypeDef",
-    "CreateRulesetResponseTypeDef",
     "CreateScheduleRequestRequestTypeDef",
-    "CreateScheduleResponseTypeDef",
-    "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
-    "CsvOutputOptionsOutputTypeDef",
     "CsvOutputOptionsTypeDef",
-    "S3LocationOutputTypeDef",
-    "DatetimeOptionsOutputTypeDef",
-    "FilterExpressionOutputTypeDef",
     "DatetimeOptionsTypeDef",
+    "FilterExpressionOutputTypeDef",
     "FilterExpressionTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
-    "DeleteDatasetResponseTypeDef",
     "DeleteJobRequestRequestTypeDef",
-    "DeleteJobResponseTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResponseTypeDef",
     "DeleteRecipeVersionRequestRequestTypeDef",
-    "DeleteRecipeVersionResponseTypeDef",
     "DeleteRulesetRequestRequestTypeDef",
-    "DeleteRulesetResponseTypeDef",
     "DeleteScheduleRequestRequestTypeDef",
-    "DeleteScheduleResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
-    "JobSampleOutputTypeDef",
-    "RecipeReferenceOutputTypeDef",
-    "ValidationConfigurationOutputTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
-    "SampleOutputTypeDef",
     "DescribeRecipeRequestRequestTypeDef",
     "DescribeRulesetRequestRequestTypeDef",
     "DescribeScheduleRequestRequestTypeDef",
-    "DescribeScheduleResponseTypeDef",
     "ExcelOptionsOutputTypeDef",
     "ExcelOptionsTypeDef",
-    "FilesLimitOutputTypeDef",
     "FilesLimitTypeDef",
-    "JsonOptionsOutputTypeDef",
     "JsonOptionsTypeDef",
-    "MetadataOutputTypeDef",
     "MetadataTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDatasetsRequestRequestTypeDef",
-    "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
-    "ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     "ListRecipeVersionsRequestRequestTypeDef",
-    "ListRecipesRequestListRecipesPaginateTypeDef",
     "ListRecipesRequestRequestTypeDef",
-    "ListRulesetsRequestListRulesetsPaginateTypeDef",
     "ListRulesetsRequestRequestTypeDef",
     "RulesetItemTypeDef",
-    "ListSchedulesRequestListSchedulesPaginateTypeDef",
     "ListSchedulesRequestRequestTypeDef",
     "ScheduleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PublishRecipeRequestRequestTypeDef",
-    "PublishRecipeResponseTypeDef",
     "RecipeActionOutputTypeDef",
     "RecipeActionTypeDef",
-    "ResponseMetadataTypeDef",
-    "ThresholdOutputTypeDef",
     "ThresholdTypeDef",
     "ViewFrameTypeDef",
-    "SendProjectSessionActionResponseTypeDef",
     "StartJobRunRequestRequestTypeDef",
-    "StartJobRunResponseTypeDef",
     "StartProjectSessionRequestRequestTypeDef",
-    "StartProjectSessionResponseTypeDef",
     "StatisticOverrideOutputTypeDef",
     "StatisticOverrideTypeDef",
     "StopJobRunRequestRequestTypeDef",
-    "StopJobRunResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateScheduleRequestRequestTypeDef",
+    "EntityDetectorConfigurationOutputTypeDef",
+    "EntityDetectorConfigurationTypeDef",
+    "BatchDeleteRecipeVersionResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateProfileJobResponseTypeDef",
+    "CreateProjectResponseTypeDef",
+    "CreateRecipeJobResponseTypeDef",
+    "CreateRecipeResponseTypeDef",
+    "CreateRulesetResponseTypeDef",
+    "CreateScheduleResponseTypeDef",
+    "DeleteDatasetResponseTypeDef",
+    "DeleteJobResponseTypeDef",
+    "DeleteProjectResponseTypeDef",
+    "DeleteRecipeVersionResponseTypeDef",
+    "DeleteRulesetResponseTypeDef",
+    "DeleteScheduleResponseTypeDef",
+    "DescribeScheduleResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PublishRecipeResponseTypeDef",
+    "SendProjectSessionActionResponseTypeDef",
+    "StartJobRunResponseTypeDef",
+    "StartProjectSessionResponseTypeDef",
+    "StopJobRunResponseTypeDef",
     "UpdateDatasetResponseTypeDef",
     "UpdateProfileJobResponseTypeDef",
     "UpdateProjectResponseTypeDef",
     "UpdateRecipeJobResponseTypeDef",
     "UpdateRecipeResponseTypeDef",
     "UpdateRulesetResponseTypeDef",
-    "UpdateScheduleRequestRequestTypeDef",
     "UpdateScheduleResponseTypeDef",
-    "EntityDetectorConfigurationOutputTypeDef",
-    "EntityDetectorConfigurationTypeDef",
-    "BatchDeleteRecipeVersionResponseTypeDef",
     "DataCatalogInputDefinitionTypeDef",
     "DatabaseInputDefinitionTypeDef",
     "DatabaseTableOutputOptionsTypeDef",
     "S3TableOutputOptionsTypeDef",
     "CreateProjectRequestRequestTypeDef",
+    "DescribeProjectResponseTypeDef",
+    "ProjectTypeDef",
     "UpdateProjectRequestRequestTypeDef",
-    "OutputFormatOptionsOutputTypeDef",
     "OutputFormatOptionsTypeDef",
-    "DataCatalogInputDefinitionOutputTypeDef",
-    "DatabaseInputDefinitionOutputTypeDef",
-    "DatabaseTableOutputOptionsOutputTypeDef",
-    "S3TableOutputOptionsOutputTypeDef",
     "DatasetParameterOutputTypeDef",
     "DatasetParameterTypeDef",
-    "DescribeProjectResponseTypeDef",
-    "ProjectTypeDef",
     "FormatOptionsOutputTypeDef",
     "FormatOptionsTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "ListJobRunsRequestListJobRunsPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
+    "ListRecipesRequestListRecipesPaginateTypeDef",
+    "ListRulesetsRequestListRulesetsPaginateTypeDef",
+    "ListSchedulesRequestListSchedulesPaginateTypeDef",
     "ListRulesetsResponseTypeDef",
     "ListSchedulesResponseTypeDef",
     "RecipeStepOutputTypeDef",
     "RecipeStepTypeDef",
     "RuleOutputTypeDef",
     "RuleTypeDef",
     "StatisticsConfigurationOutputTypeDef",
     "StatisticsConfigurationTypeDef",
     "InputTypeDef",
     "DatabaseOutputTypeDef",
     "DataCatalogOutputTypeDef",
+    "ListProjectsResponseTypeDef",
     "OutputTypeDef",
-    "InputOutputTypeDef",
     "PathOptionsOutputTypeDef",
     "PathOptionsTypeDef",
-    "ListProjectsResponseTypeDef",
     "DescribeRecipeResponseTypeDef",
     "RecipeTypeDef",
     "CreateRecipeRequestRequestTypeDef",
     "SendProjectSessionActionRequestRequestTypeDef",
     "UpdateRecipeRequestRequestTypeDef",
     "DescribeRulesetResponseTypeDef",
     "CreateRulesetRequestRequestTypeDef",
@@ -250,52 +230,34 @@
         "ErrorCode": str,
         "ErrorMessage": str,
         "RecipeVersion": str,
     },
     total=False,
 )
 
-ColumnSelectorOutputTypeDef = TypedDict(
-    "ColumnSelectorOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Regex": str,
-        "Name": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 ColumnSelectorTypeDef = TypedDict(
     "ColumnSelectorTypeDef",
     {
         "Regex": str,
         "Name": str,
     },
     total=False,
 )
 
-_RequiredConditionExpressionOutputTypeDef = TypedDict(
-    "_RequiredConditionExpressionOutputTypeDef",
-    {
-        "Condition": str,
-        "TargetColumn": str,
-    },
-)
-_OptionalConditionExpressionOutputTypeDef = TypedDict(
-    "_OptionalConditionExpressionOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-class ConditionExpressionOutputTypeDef(
-    _RequiredConditionExpressionOutputTypeDef, _OptionalConditionExpressionOutputTypeDef
-):
-    pass
-
 _RequiredConditionExpressionTypeDef = TypedDict(
     "_RequiredConditionExpressionTypeDef",
     {
         "Condition": str,
         "TargetColumn": str,
     },
 )
@@ -308,22 +270,14 @@
 )
 
 class ConditionExpressionTypeDef(
     _RequiredConditionExpressionTypeDef, _OptionalConditionExpressionTypeDef
 ):
     pass
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 JobSampleTypeDef = TypedDict(
     "JobSampleTypeDef",
     {
         "Mode": SampleModeType,
         "Size": int,
     },
     total=False,
@@ -362,22 +316,14 @@
 )
 
 class ValidationConfigurationTypeDef(
     _RequiredValidationConfigurationTypeDef, _OptionalValidationConfigurationTypeDef
 ):
     pass
 
-CreateProfileJobResponseTypeDef = TypedDict(
-    "CreateProfileJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSampleTypeDef = TypedDict(
     "_RequiredSampleTypeDef",
     {
         "Type": SampleTypeType,
     },
 )
 _OptionalSampleTypeDef = TypedDict(
@@ -387,22 +333,14 @@
     },
     total=False,
 )
 
 class SampleTypeDef(_RequiredSampleTypeDef, _OptionalSampleTypeDef):
     pass
 
-CreateProjectResponseTypeDef = TypedDict(
-    "CreateProjectResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecipeReferenceTypeDef = TypedDict(
     "_RequiredRecipeReferenceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalRecipeReferenceTypeDef = TypedDict(
@@ -412,38 +350,14 @@
     },
     total=False,
 )
 
 class RecipeReferenceTypeDef(_RequiredRecipeReferenceTypeDef, _OptionalRecipeReferenceTypeDef):
     pass
 
-CreateRecipeJobResponseTypeDef = TypedDict(
-    "CreateRecipeJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRecipeResponseTypeDef = TypedDict(
-    "CreateRecipeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRulesetResponseTypeDef = TypedDict(
-    "CreateRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScheduleRequestRequestTypeDef",
     {
         "CronExpression": str,
         "Name": str,
     },
 )
@@ -457,120 +371,57 @@
 )
 
 class CreateScheduleRequestRequestTypeDef(
     _RequiredCreateScheduleRequestRequestTypeDef, _OptionalCreateScheduleRequestRequestTypeDef
 ):
     pass
 
-CreateScheduleResponseTypeDef = TypedDict(
-    "CreateScheduleResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CsvOptionsOutputTypeDef = TypedDict(
-    "CsvOptionsOutputTypeDef",
-    {
-        "Delimiter": str,
-        "HeaderRow": bool,
-    },
-    total=False,
-)
-
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderRow": bool,
     },
     total=False,
 )
 
-CsvOutputOptionsOutputTypeDef = TypedDict(
-    "CsvOutputOptionsOutputTypeDef",
-    {
-        "Delimiter": str,
-    },
-    total=False,
-)
-
 CsvOutputOptionsTypeDef = TypedDict(
     "CsvOutputOptionsTypeDef",
     {
         "Delimiter": str,
     },
     total=False,
 )
 
-_RequiredS3LocationOutputTypeDef = TypedDict(
-    "_RequiredS3LocationOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalS3LocationOutputTypeDef = TypedDict(
-    "_OptionalS3LocationOutputTypeDef",
-    {
-        "Key": str,
-        "BucketOwner": str,
-    },
-    total=False,
-)
-
-class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
-    pass
-
-_RequiredDatetimeOptionsOutputTypeDef = TypedDict(
-    "_RequiredDatetimeOptionsOutputTypeDef",
+_RequiredDatetimeOptionsTypeDef = TypedDict(
+    "_RequiredDatetimeOptionsTypeDef",
     {
         "Format": str,
     },
 )
-_OptionalDatetimeOptionsOutputTypeDef = TypedDict(
-    "_OptionalDatetimeOptionsOutputTypeDef",
+_OptionalDatetimeOptionsTypeDef = TypedDict(
+    "_OptionalDatetimeOptionsTypeDef",
     {
         "TimezoneOffset": str,
         "LocaleCode": str,
     },
     total=False,
 )
 
-class DatetimeOptionsOutputTypeDef(
-    _RequiredDatetimeOptionsOutputTypeDef, _OptionalDatetimeOptionsOutputTypeDef
-):
+class DatetimeOptionsTypeDef(_RequiredDatetimeOptionsTypeDef, _OptionalDatetimeOptionsTypeDef):
     pass
 
 FilterExpressionOutputTypeDef = TypedDict(
     "FilterExpressionOutputTypeDef",
     {
         "Expression": str,
         "ValuesMap": Dict[str, str],
     },
 )
 
-_RequiredDatetimeOptionsTypeDef = TypedDict(
-    "_RequiredDatetimeOptionsTypeDef",
-    {
-        "Format": str,
-    },
-)
-_OptionalDatetimeOptionsTypeDef = TypedDict(
-    "_OptionalDatetimeOptionsTypeDef",
-    {
-        "TimezoneOffset": str,
-        "LocaleCode": str,
-    },
-    total=False,
-)
-
-class DatetimeOptionsTypeDef(_RequiredDatetimeOptionsTypeDef, _OptionalDatetimeOptionsTypeDef):
-    pass
-
 FilterExpressionTypeDef = TypedDict(
     "FilterExpressionTypeDef",
     {
         "Expression": str,
         "ValuesMap": Mapping[str, str],
     },
 )
@@ -578,160 +429,64 @@
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteDatasetResponseTypeDef = TypedDict(
-    "DeleteDatasetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteJobRequestRequestTypeDef = TypedDict(
     "DeleteJobRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteJobResponseTypeDef = TypedDict(
-    "DeleteJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteProjectResponseTypeDef = TypedDict(
-    "DeleteProjectResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRecipeVersionRequestRequestTypeDef = TypedDict(
     "DeleteRecipeVersionRequestRequestTypeDef",
     {
         "Name": str,
         "RecipeVersion": str,
     },
 )
 
-DeleteRecipeVersionResponseTypeDef = TypedDict(
-    "DeleteRecipeVersionResponseTypeDef",
-    {
-        "Name": str,
-        "RecipeVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRulesetRequestRequestTypeDef = TypedDict(
     "DeleteRulesetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteRulesetResponseTypeDef = TypedDict(
-    "DeleteRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteScheduleRequestRequestTypeDef = TypedDict(
     "DeleteScheduleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteScheduleResponseTypeDef = TypedDict(
-    "DeleteScheduleResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 DescribeJobRequestRequestTypeDef = TypedDict(
     "DescribeJobRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-JobSampleOutputTypeDef = TypedDict(
-    "JobSampleOutputTypeDef",
-    {
-        "Mode": SampleModeType,
-        "Size": int,
-    },
-    total=False,
-)
-
-_RequiredRecipeReferenceOutputTypeDef = TypedDict(
-    "_RequiredRecipeReferenceOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalRecipeReferenceOutputTypeDef = TypedDict(
-    "_OptionalRecipeReferenceOutputTypeDef",
-    {
-        "RecipeVersion": str,
-    },
-    total=False,
-)
-
-class RecipeReferenceOutputTypeDef(
-    _RequiredRecipeReferenceOutputTypeDef, _OptionalRecipeReferenceOutputTypeDef
-):
-    pass
-
-_RequiredValidationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredValidationConfigurationOutputTypeDef",
-    {
-        "RulesetArn": str,
-    },
-)
-_OptionalValidationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalValidationConfigurationOutputTypeDef",
-    {
-        "ValidationMode": Literal["CHECK_ALL"],
-    },
-    total=False,
-)
-
-class ValidationConfigurationOutputTypeDef(
-    _RequiredValidationConfigurationOutputTypeDef, _OptionalValidationConfigurationOutputTypeDef
-):
-    pass
-
 DescribeJobRunRequestRequestTypeDef = TypedDict(
     "DescribeJobRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
@@ -739,31 +494,14 @@
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-_RequiredSampleOutputTypeDef = TypedDict(
-    "_RequiredSampleOutputTypeDef",
-    {
-        "Type": SampleTypeType,
-    },
-)
-_OptionalSampleOutputTypeDef = TypedDict(
-    "_OptionalSampleOutputTypeDef",
-    {
-        "Size": int,
-    },
-    total=False,
-)
-
-class SampleOutputTypeDef(_RequiredSampleOutputTypeDef, _OptionalSampleOutputTypeDef):
-    pass
-
 _RequiredDescribeRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRecipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDescribeRecipeRequestRequestTypeDef = TypedDict(
@@ -789,30 +527,14 @@
 DescribeScheduleRequestRequestTypeDef = TypedDict(
     "DescribeScheduleRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeScheduleResponseTypeDef = TypedDict(
-    "DescribeScheduleResponseTypeDef",
-    {
-        "CreateDate": datetime,
-        "CreatedBy": str,
-        "JobNames": List[str],
-        "LastModifiedBy": str,
-        "LastModifiedDate": datetime,
-        "ResourceArn": str,
-        "CronExpression": str,
-        "Tags": Dict[str, str],
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExcelOptionsOutputTypeDef = TypedDict(
     "ExcelOptionsOutputTypeDef",
     {
         "SheetNames": List[str],
         "SheetIndexes": List[int],
         "HeaderRow": bool,
     },
@@ -825,32 +547,14 @@
         "SheetNames": Sequence[str],
         "SheetIndexes": Sequence[int],
         "HeaderRow": bool,
     },
     total=False,
 )
 
-_RequiredFilesLimitOutputTypeDef = TypedDict(
-    "_RequiredFilesLimitOutputTypeDef",
-    {
-        "MaxFiles": int,
-    },
-)
-_OptionalFilesLimitOutputTypeDef = TypedDict(
-    "_OptionalFilesLimitOutputTypeDef",
-    {
-        "OrderedBy": Literal["LAST_MODIFIED_DATE"],
-        "Order": OrderType,
-    },
-    total=False,
-)
-
-class FilesLimitOutputTypeDef(_RequiredFilesLimitOutputTypeDef, _OptionalFilesLimitOutputTypeDef):
-    pass
-
 _RequiredFilesLimitTypeDef = TypedDict(
     "_RequiredFilesLimitTypeDef",
     {
         "MaxFiles": int,
     },
 )
 _OptionalFilesLimitTypeDef = TypedDict(
@@ -861,83 +565,49 @@
     },
     total=False,
 )
 
 class FilesLimitTypeDef(_RequiredFilesLimitTypeDef, _OptionalFilesLimitTypeDef):
     pass
 
-JsonOptionsOutputTypeDef = TypedDict(
-    "JsonOptionsOutputTypeDef",
-    {
-        "MultiLine": bool,
-    },
-    total=False,
-)
-
 JsonOptionsTypeDef = TypedDict(
     "JsonOptionsTypeDef",
     {
         "MultiLine": bool,
     },
     total=False,
 )
 
-MetadataOutputTypeDef = TypedDict(
-    "MetadataOutputTypeDef",
-    {
-        "SourceArn": str,
-    },
-    total=False,
-)
-
 MetadataTypeDef = TypedDict(
     "MetadataTypeDef",
     {
         "SourceArn": str,
     },
     total=False,
 )
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
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
 
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
-    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListJobRunsRequestListJobRunsPaginateTypeDef(
-    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
-    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
-):
-    pass
-
 _RequiredListJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredListJobRunsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListJobRunsRequestRequestTypeDef = TypedDict(
@@ -950,72 +620,34 @@
 )
 
 class ListJobRunsRequestRequestTypeDef(
     _RequiredListJobRunsRequestRequestTypeDef, _OptionalListJobRunsRequestRequestTypeDef
 ):
     pass
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "DatasetName": str,
-        "ProjectName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "DatasetName": str,
         "MaxResults": int,
         "NextToken": str,
         "ProjectName": str,
     },
     total=False,
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
-    _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
-    _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListRecipeVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecipeVersionsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListRecipeVersionsRequestRequestTypeDef = TypedDict(
@@ -1029,42 +661,24 @@
 
 class ListRecipeVersionsRequestRequestTypeDef(
     _RequiredListRecipeVersionsRequestRequestTypeDef,
     _OptionalListRecipeVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
-    "ListRecipesRequestListRecipesPaginateTypeDef",
-    {
-        "RecipeVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRecipesRequestRequestTypeDef = TypedDict(
     "ListRecipesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RecipeVersion": str,
     },
     total=False,
 )
 
-ListRulesetsRequestListRulesetsPaginateTypeDef = TypedDict(
-    "ListRulesetsRequestListRulesetsPaginateTypeDef",
-    {
-        "TargetArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRulesetsRequestRequestTypeDef = TypedDict(
     "ListRulesetsRequestRequestTypeDef",
     {
         "TargetArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1093,23 +707,14 @@
     },
     total=False,
 )
 
 class RulesetItemTypeDef(_RequiredRulesetItemTypeDef, _OptionalRulesetItemTypeDef):
     pass
 
-ListSchedulesRequestListSchedulesPaginateTypeDef = TypedDict(
-    "ListSchedulesRequestListSchedulesPaginateTypeDef",
-    {
-        "JobName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSchedulesRequestRequestTypeDef = TypedDict(
     "ListSchedulesRequestRequestTypeDef",
     {
         "JobName": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1144,32 +749,14 @@
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
 _RequiredPublishRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredPublishRecipeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalPublishRecipeRequestRequestTypeDef = TypedDict(
@@ -1181,22 +768,14 @@
 )
 
 class PublishRecipeRequestRequestTypeDef(
     _RequiredPublishRecipeRequestRequestTypeDef, _OptionalPublishRecipeRequestRequestTypeDef
 ):
     pass
 
-PublishRecipeResponseTypeDef = TypedDict(
-    "PublishRecipeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecipeActionOutputTypeDef = TypedDict(
     "_RequiredRecipeActionOutputTypeDef",
     {
         "Operation": str,
     },
 )
 _OptionalRecipeActionOutputTypeDef = TypedDict(
@@ -1225,43 +804,14 @@
     },
     total=False,
 )
 
 class RecipeActionTypeDef(_RequiredRecipeActionTypeDef, _OptionalRecipeActionTypeDef):
     pass
 
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
-_RequiredThresholdOutputTypeDef = TypedDict(
-    "_RequiredThresholdOutputTypeDef",
-    {
-        "Value": float,
-    },
-)
-_OptionalThresholdOutputTypeDef = TypedDict(
-    "_OptionalThresholdOutputTypeDef",
-    {
-        "Type": ThresholdTypeType,
-        "Unit": ThresholdUnitType,
-    },
-    total=False,
-)
-
-class ThresholdOutputTypeDef(_RequiredThresholdOutputTypeDef, _OptionalThresholdOutputTypeDef):
-    pass
-
 _RequiredThresholdTypeDef = TypedDict(
     "_RequiredThresholdTypeDef",
     {
         "Value": float,
     },
 )
 _OptionalThresholdTypeDef = TypedDict(
@@ -1293,39 +843,21 @@
     },
     total=False,
 )
 
 class ViewFrameTypeDef(_RequiredViewFrameTypeDef, _OptionalViewFrameTypeDef):
     pass
 
-SendProjectSessionActionResponseTypeDef = TypedDict(
-    "SendProjectSessionActionResponseTypeDef",
-    {
-        "Result": str,
-        "Name": str,
-        "ActionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartJobRunRequestRequestTypeDef = TypedDict(
     "StartJobRunRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-StartJobRunResponseTypeDef = TypedDict(
-    "StartJobRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartProjectSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartProjectSessionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalStartProjectSessionRequestRequestTypeDef = TypedDict(
@@ -1338,23 +870,14 @@
 
 class StartProjectSessionRequestRequestTypeDef(
     _RequiredStartProjectSessionRequestRequestTypeDef,
     _OptionalStartProjectSessionRequestRequestTypeDef,
 ):
     pass
 
-StartProjectSessionResponseTypeDef = TypedDict(
-    "StartProjectSessionResponseTypeDef",
-    {
-        "Name": str,
-        "ClientSessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StatisticOverrideOutputTypeDef = TypedDict(
     "StatisticOverrideOutputTypeDef",
     {
         "Statistic": str,
         "Parameters": Dict[str, str],
     },
 )
@@ -1371,22 +894,14 @@
     "StopJobRunRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
 
-StopJobRunResponseTypeDef = TypedDict(
-    "StopJobRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1395,63 +910,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateDatasetResponseTypeDef = TypedDict(
-    "UpdateDatasetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateProfileJobResponseTypeDef = TypedDict(
-    "UpdateProfileJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateProjectResponseTypeDef = TypedDict(
-    "UpdateProjectResponseTypeDef",
-    {
-        "LastModifiedDate": datetime,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateRecipeJobResponseTypeDef = TypedDict(
-    "UpdateRecipeJobResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateRecipeResponseTypeDef = TypedDict(
-    "UpdateRecipeResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateRulesetResponseTypeDef = TypedDict(
-    "UpdateRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduleRequestRequestTypeDef",
     {
         "CronExpression": str,
         "Name": str,
     },
 )
@@ -1464,22 +930,14 @@
 )
 
 class UpdateScheduleRequestRequestTypeDef(
     _RequiredUpdateScheduleRequestRequestTypeDef, _OptionalUpdateScheduleRequestRequestTypeDef
 ):
     pass
 
-UpdateScheduleResponseTypeDef = TypedDict(
-    "UpdateScheduleResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEntityDetectorConfigurationOutputTypeDef = TypedDict(
     "_RequiredEntityDetectorConfigurationOutputTypeDef",
     {
         "EntityTypes": List[str],
     },
 )
 _OptionalEntityDetectorConfigurationOutputTypeDef = TypedDict(
@@ -1516,15 +974,244 @@
     pass
 
 BatchDeleteRecipeVersionResponseTypeDef = TypedDict(
     "BatchDeleteRecipeVersionResponseTypeDef",
     {
         "Name": str,
         "Errors": List[RecipeVersionErrorDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileJobResponseTypeDef = TypedDict(
+    "CreateProfileJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectResponseTypeDef = TypedDict(
+    "CreateProjectResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRecipeJobResponseTypeDef = TypedDict(
+    "CreateRecipeJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRecipeResponseTypeDef = TypedDict(
+    "CreateRecipeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRulesetResponseTypeDef = TypedDict(
+    "CreateRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScheduleResponseTypeDef = TypedDict(
+    "CreateScheduleResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDatasetResponseTypeDef = TypedDict(
+    "DeleteDatasetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteJobResponseTypeDef = TypedDict(
+    "DeleteJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectResponseTypeDef = TypedDict(
+    "DeleteProjectResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRecipeVersionResponseTypeDef = TypedDict(
+    "DeleteRecipeVersionResponseTypeDef",
+    {
+        "Name": str,
+        "RecipeVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRulesetResponseTypeDef = TypedDict(
+    "DeleteRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteScheduleResponseTypeDef = TypedDict(
+    "DeleteScheduleResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeScheduleResponseTypeDef = TypedDict(
+    "DescribeScheduleResponseTypeDef",
+    {
+        "CreateDate": datetime,
+        "CreatedBy": str,
+        "JobNames": List[str],
+        "LastModifiedBy": str,
+        "LastModifiedDate": datetime,
+        "ResourceArn": str,
+        "CronExpression": str,
+        "Tags": Dict[str, str],
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishRecipeResponseTypeDef = TypedDict(
+    "PublishRecipeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendProjectSessionActionResponseTypeDef = TypedDict(
+    "SendProjectSessionActionResponseTypeDef",
+    {
+        "Result": str,
+        "Name": str,
+        "ActionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartJobRunResponseTypeDef = TypedDict(
+    "StartJobRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartProjectSessionResponseTypeDef = TypedDict(
+    "StartProjectSessionResponseTypeDef",
+    {
+        "Name": str,
+        "ClientSessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopJobRunResponseTypeDef = TypedDict(
+    "StopJobRunResponseTypeDef",
+    {
+        "RunId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDatasetResponseTypeDef = TypedDict(
+    "UpdateDatasetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProfileJobResponseTypeDef = TypedDict(
+    "UpdateProfileJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProjectResponseTypeDef = TypedDict(
+    "UpdateProjectResponseTypeDef",
+    {
+        "LastModifiedDate": datetime,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRecipeJobResponseTypeDef = TypedDict(
+    "UpdateRecipeJobResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRecipeResponseTypeDef = TypedDict(
+    "UpdateRecipeResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRulesetResponseTypeDef = TypedDict(
+    "UpdateRulesetResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateScheduleResponseTypeDef = TypedDict(
+    "UpdateScheduleResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDataCatalogInputDefinitionTypeDef = TypedDict(
     "_RequiredDataCatalogInputDefinitionTypeDef",
     {
         "DatabaseName": str,
@@ -1611,14 +1298,64 @@
 )
 
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+DescribeProjectResponseTypeDef = TypedDict(
+    "DescribeProjectResponseTypeDef",
+    {
+        "CreateDate": datetime,
+        "CreatedBy": str,
+        "DatasetName": str,
+        "LastModifiedDate": datetime,
+        "LastModifiedBy": str,
+        "Name": str,
+        "RecipeName": str,
+        "ResourceArn": str,
+        "Sample": SampleTypeDef,
+        "RoleArn": str,
+        "Tags": Dict[str, str],
+        "SessionStatus": SessionStatusType,
+        "OpenedBy": str,
+        "OpenDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredProjectTypeDef = TypedDict(
+    "_RequiredProjectTypeDef",
+    {
+        "Name": str,
+        "RecipeName": str,
+    },
+)
+_OptionalProjectTypeDef = TypedDict(
+    "_OptionalProjectTypeDef",
+    {
+        "AccountId": str,
+        "CreateDate": datetime,
+        "CreatedBy": str,
+        "DatasetName": str,
+        "LastModifiedDate": datetime,
+        "LastModifiedBy": str,
+        "ResourceArn": str,
+        "Sample": SampleTypeDef,
+        "Tags": Dict[str, str],
+        "RoleArn": str,
+        "OpenedBy": str,
+        "OpenDate": datetime,
+    },
+    total=False,
+)
+
+class ProjectTypeDef(_RequiredProjectTypeDef, _OptionalProjectTypeDef):
+    pass
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "RoleArn": str,
         "Name": str,
     },
 )
@@ -1631,240 +1368,205 @@
 )
 
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
     pass
 
-OutputFormatOptionsOutputTypeDef = TypedDict(
-    "OutputFormatOptionsOutputTypeDef",
-    {
-        "Csv": CsvOutputOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 OutputFormatOptionsTypeDef = TypedDict(
     "OutputFormatOptionsTypeDef",
     {
         "Csv": CsvOutputOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredDataCatalogInputDefinitionOutputTypeDef = TypedDict(
-    "_RequiredDataCatalogInputDefinitionOutputTypeDef",
+_RequiredDatasetParameterOutputTypeDef = TypedDict(
+    "_RequiredDatasetParameterOutputTypeDef",
     {
-        "DatabaseName": str,
-        "TableName": str,
+        "Name": str,
+        "Type": ParameterTypeType,
     },
 )
-_OptionalDataCatalogInputDefinitionOutputTypeDef = TypedDict(
-    "_OptionalDataCatalogInputDefinitionOutputTypeDef",
+_OptionalDatasetParameterOutputTypeDef = TypedDict(
+    "_OptionalDatasetParameterOutputTypeDef",
     {
-        "CatalogId": str,
-        "TempDirectory": S3LocationOutputTypeDef,
+        "DatetimeOptions": DatetimeOptionsTypeDef,
+        "CreateColumn": bool,
+        "Filter": FilterExpressionOutputTypeDef,
     },
     total=False,
 )
 
-class DataCatalogInputDefinitionOutputTypeDef(
-    _RequiredDataCatalogInputDefinitionOutputTypeDef,
-    _OptionalDataCatalogInputDefinitionOutputTypeDef,
+class DatasetParameterOutputTypeDef(
+    _RequiredDatasetParameterOutputTypeDef, _OptionalDatasetParameterOutputTypeDef
 ):
     pass
 
-_RequiredDatabaseInputDefinitionOutputTypeDef = TypedDict(
-    "_RequiredDatabaseInputDefinitionOutputTypeDef",
+_RequiredDatasetParameterTypeDef = TypedDict(
+    "_RequiredDatasetParameterTypeDef",
     {
-        "GlueConnectionName": str,
+        "Name": str,
+        "Type": ParameterTypeType,
     },
 )
-_OptionalDatabaseInputDefinitionOutputTypeDef = TypedDict(
-    "_OptionalDatabaseInputDefinitionOutputTypeDef",
+_OptionalDatasetParameterTypeDef = TypedDict(
+    "_OptionalDatasetParameterTypeDef",
     {
-        "DatabaseTableName": str,
-        "TempDirectory": S3LocationOutputTypeDef,
-        "QueryString": str,
+        "DatetimeOptions": DatetimeOptionsTypeDef,
+        "CreateColumn": bool,
+        "Filter": FilterExpressionTypeDef,
     },
     total=False,
 )
 
-class DatabaseInputDefinitionOutputTypeDef(
-    _RequiredDatabaseInputDefinitionOutputTypeDef, _OptionalDatabaseInputDefinitionOutputTypeDef
-):
+class DatasetParameterTypeDef(_RequiredDatasetParameterTypeDef, _OptionalDatasetParameterTypeDef):
     pass
 
-_RequiredDatabaseTableOutputOptionsOutputTypeDef = TypedDict(
-    "_RequiredDatabaseTableOutputOptionsOutputTypeDef",
+FormatOptionsOutputTypeDef = TypedDict(
+    "FormatOptionsOutputTypeDef",
     {
-        "TableName": str,
+        "Json": JsonOptionsTypeDef,
+        "Excel": ExcelOptionsOutputTypeDef,
+        "Csv": CsvOptionsTypeDef,
     },
+    total=False,
 )
-_OptionalDatabaseTableOutputOptionsOutputTypeDef = TypedDict(
-    "_OptionalDatabaseTableOutputOptionsOutputTypeDef",
+
+FormatOptionsTypeDef = TypedDict(
+    "FormatOptionsTypeDef",
     {
-        "TempDirectory": S3LocationOutputTypeDef,
+        "Json": JsonOptionsTypeDef,
+        "Excel": ExcelOptionsTypeDef,
+        "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
 
-class DatabaseTableOutputOptionsOutputTypeDef(
-    _RequiredDatabaseTableOutputOptionsOutputTypeDef,
-    _OptionalDatabaseTableOutputOptionsOutputTypeDef,
-):
-    pass
-
-S3TableOutputOptionsOutputTypeDef = TypedDict(
-    "S3TableOutputOptionsOutputTypeDef",
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     {
-        "Location": S3LocationOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredDatasetParameterOutputTypeDef = TypedDict(
-    "_RequiredDatasetParameterOutputTypeDef",
+_RequiredListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_RequiredListJobRunsRequestListJobRunsPaginateTypeDef",
     {
         "Name": str,
-        "Type": ParameterTypeType,
     },
 )
-_OptionalDatasetParameterOutputTypeDef = TypedDict(
-    "_OptionalDatasetParameterOutputTypeDef",
+_OptionalListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
+    "_OptionalListJobRunsRequestListJobRunsPaginateTypeDef",
     {
-        "DatetimeOptions": DatetimeOptionsOutputTypeDef,
-        "CreateColumn": bool,
-        "Filter": FilterExpressionOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class DatasetParameterOutputTypeDef(
-    _RequiredDatasetParameterOutputTypeDef, _OptionalDatasetParameterOutputTypeDef
+class ListJobRunsRequestListJobRunsPaginateTypeDef(
+    _RequiredListJobRunsRequestListJobRunsPaginateTypeDef,
+    _OptionalListJobRunsRequestListJobRunsPaginateTypeDef,
 ):
     pass
 
-_RequiredDatasetParameterTypeDef = TypedDict(
-    "_RequiredDatasetParameterTypeDef",
-    {
-        "Name": str,
-        "Type": ParameterTypeType,
-    },
-)
-_OptionalDatasetParameterTypeDef = TypedDict(
-    "_OptionalDatasetParameterTypeDef",
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
     {
-        "DatetimeOptions": DatetimeOptionsTypeDef,
-        "CreateColumn": bool,
-        "Filter": FilterExpressionTypeDef,
+        "DatasetName": str,
+        "ProjectName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class DatasetParameterTypeDef(_RequiredDatasetParameterTypeDef, _OptionalDatasetParameterTypeDef):
-    pass
-
-DescribeProjectResponseTypeDef = TypedDict(
-    "DescribeProjectResponseTypeDef",
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     {
-        "CreateDate": datetime,
-        "CreatedBy": str,
-        "DatasetName": str,
-        "LastModifiedDate": datetime,
-        "LastModifiedBy": str,
-        "Name": str,
-        "RecipeName": str,
-        "ResourceArn": str,
-        "Sample": SampleOutputTypeDef,
-        "RoleArn": str,
-        "Tags": Dict[str, str],
-        "SessionStatus": SessionStatusType,
-        "OpenedBy": str,
-        "OpenDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredProjectTypeDef = TypedDict(
-    "_RequiredProjectTypeDef",
+_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     {
         "Name": str,
-        "RecipeName": str,
     },
 )
-_OptionalProjectTypeDef = TypedDict(
-    "_OptionalProjectTypeDef",
+_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef",
     {
-        "AccountId": str,
-        "CreateDate": datetime,
-        "CreatedBy": str,
-        "DatasetName": str,
-        "LastModifiedDate": datetime,
-        "LastModifiedBy": str,
-        "ResourceArn": str,
-        "Sample": SampleOutputTypeDef,
-        "Tags": Dict[str, str],
-        "RoleArn": str,
-        "OpenedBy": str,
-        "OpenDate": datetime,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ProjectTypeDef(_RequiredProjectTypeDef, _OptionalProjectTypeDef):
+class ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef(
+    _RequiredListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
+    _OptionalListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
+):
     pass
 
-FormatOptionsOutputTypeDef = TypedDict(
-    "FormatOptionsOutputTypeDef",
+ListRecipesRequestListRecipesPaginateTypeDef = TypedDict(
+    "ListRecipesRequestListRecipesPaginateTypeDef",
     {
-        "Json": JsonOptionsOutputTypeDef,
-        "Excel": ExcelOptionsOutputTypeDef,
-        "Csv": CsvOptionsOutputTypeDef,
+        "RecipeVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-FormatOptionsTypeDef = TypedDict(
-    "FormatOptionsTypeDef",
+ListRulesetsRequestListRulesetsPaginateTypeDef = TypedDict(
+    "ListRulesetsRequestListRulesetsPaginateTypeDef",
     {
-        "Json": JsonOptionsTypeDef,
-        "Excel": ExcelOptionsTypeDef,
-        "Csv": CsvOptionsTypeDef,
+        "TargetArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSchedulesRequestListSchedulesPaginateTypeDef = TypedDict(
+    "ListSchedulesRequestListSchedulesPaginateTypeDef",
+    {
+        "JobName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListRulesetsResponseTypeDef = TypedDict(
     "ListRulesetsResponseTypeDef",
     {
         "Rulesets": List[RulesetItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchedulesResponseTypeDef = TypedDict(
     "ListSchedulesResponseTypeDef",
     {
         "Schedules": List[ScheduleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRecipeStepOutputTypeDef = TypedDict(
     "_RequiredRecipeStepOutputTypeDef",
     {
         "Action": RecipeActionOutputTypeDef,
     },
 )
 _OptionalRecipeStepOutputTypeDef = TypedDict(
     "_OptionalRecipeStepOutputTypeDef",
     {
-        "ConditionExpressions": List[ConditionExpressionOutputTypeDef],
+        "ConditionExpressions": List[ConditionExpressionTypeDef],
     },
     total=False,
 )
 
 class RecipeStepOutputTypeDef(_RequiredRecipeStepOutputTypeDef, _OptionalRecipeStepOutputTypeDef):
     pass
 
@@ -1893,16 +1595,16 @@
     },
 )
 _OptionalRuleOutputTypeDef = TypedDict(
     "_OptionalRuleOutputTypeDef",
     {
         "Disabled": bool,
         "SubstitutionMap": Dict[str, str],
-        "Threshold": ThresholdOutputTypeDef,
-        "ColumnSelectors": List[ColumnSelectorOutputTypeDef],
+        "Threshold": ThresholdTypeDef,
+        "ColumnSelectors": List[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
 class RuleOutputTypeDef(_RequiredRuleOutputTypeDef, _OptionalRuleOutputTypeDef):
     pass
 
@@ -1993,14 +1695,23 @@
 )
 
 class DataCatalogOutputTypeDef(
     _RequiredDataCatalogOutputTypeDef, _OptionalDataCatalogOutputTypeDef
 ):
     pass
 
+ListProjectsResponseTypeDef = TypedDict(
+    "ListProjectsResponseTypeDef",
+    {
+        "Projects": List[ProjectTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredOutputTypeDef = TypedDict(
     "_RequiredOutputTypeDef",
     {
         "Location": S3LocationTypeDef,
     },
 )
 _OptionalOutputTypeDef = TypedDict(
@@ -2015,30 +1726,19 @@
     },
     total=False,
 )
 
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
-InputOutputTypeDef = TypedDict(
-    "InputOutputTypeDef",
-    {
-        "S3InputDefinition": S3LocationOutputTypeDef,
-        "DataCatalogInputDefinition": DataCatalogInputDefinitionOutputTypeDef,
-        "DatabaseInputDefinition": DatabaseInputDefinitionOutputTypeDef,
-        "Metadata": MetadataOutputTypeDef,
-    },
-    total=False,
-)
-
 PathOptionsOutputTypeDef = TypedDict(
     "PathOptionsOutputTypeDef",
     {
         "LastModifiedDateCondition": FilterExpressionOutputTypeDef,
-        "FilesLimit": FilesLimitOutputTypeDef,
+        "FilesLimit": FilesLimitTypeDef,
         "Parameters": Dict[str, DatasetParameterOutputTypeDef],
     },
     total=False,
 )
 
 PathOptionsTypeDef = TypedDict(
     "PathOptionsTypeDef",
@@ -2046,23 +1746,14 @@
         "LastModifiedDateCondition": FilterExpressionTypeDef,
         "FilesLimit": FilesLimitTypeDef,
         "Parameters": Mapping[str, DatasetParameterTypeDef],
     },
     total=False,
 )
 
-ListProjectsResponseTypeDef = TypedDict(
-    "ListProjectsResponseTypeDef",
-    {
-        "Projects": List[ProjectTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRecipeResponseTypeDef = TypedDict(
     "DescribeRecipeResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
@@ -2071,15 +1762,15 @@
         "PublishedDate": datetime,
         "Description": str,
         "Name": str,
         "Steps": List[RecipeStepOutputTypeDef],
         "Tags": Dict[str, str],
         "ResourceArn": str,
         "RecipeVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRecipeTypeDef = TypedDict(
     "_RequiredRecipeTypeDef",
     {
         "Name": str,
@@ -2181,15 +1872,15 @@
         "Rules": List[RuleOutputTypeDef],
         "CreateDate": datetime,
         "CreatedBy": str,
         "LastModifiedBy": str,
         "LastModifiedDate": datetime,
         "ResourceArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRulesetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRulesetRequestRequestTypeDef",
     {
         "Name": str,
@@ -2236,15 +1927,15 @@
     {
         "Statistics": StatisticsConfigurationOutputTypeDef,
     },
 )
 _OptionalColumnStatisticsConfigurationOutputTypeDef = TypedDict(
     "_OptionalColumnStatisticsConfigurationOutputTypeDef",
     {
-        "Selectors": List[ColumnSelectorOutputTypeDef],
+        "Selectors": List[ColumnSelectorTypeDef],
     },
     total=False,
 )
 
 class ColumnStatisticsConfigurationOutputTypeDef(
     _RequiredColumnStatisticsConfigurationOutputTypeDef,
     _OptionalColumnStatisticsConfigurationOutputTypeDef,
@@ -2314,19 +2005,19 @@
         "RunId": str,
         "State": JobRunStateType,
         "LogSubscription": LogSubscriptionType,
         "LogGroupName": str,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
-        "RecipeReference": RecipeReferenceOutputTypeDef,
+        "RecipeReference": RecipeReferenceTypeDef,
         "StartedBy": str,
         "StartedOn": datetime,
-        "JobSample": JobSampleOutputTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
+        "JobSample": JobSampleTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
@@ -2348,21 +2039,21 @@
         "LogSubscription": LogSubscriptionType,
         "MaxCapacity": int,
         "MaxRetries": int,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
         "ProjectName": str,
-        "RecipeReference": RecipeReferenceOutputTypeDef,
+        "RecipeReference": RecipeReferenceTypeDef,
         "ResourceArn": str,
         "RoleArn": str,
         "Timeout": int,
         "Tags": Dict[str, str],
-        "JobSample": JobSampleOutputTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
+        "JobSample": JobSampleTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
     },
     total=False,
 )
 
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
 
@@ -2394,15 +2085,15 @@
 ):
     pass
 
 _RequiredDatasetTypeDef = TypedDict(
     "_RequiredDatasetTypeDef",
     {
         "Name": str,
-        "Input": InputOutputTypeDef,
+        "Input": InputTypeDef,
     },
 )
 _OptionalDatasetTypeDef = TypedDict(
     "_OptionalDatasetTypeDef",
     {
         "AccountId": str,
         "CreatedBy": str,
@@ -2426,22 +2117,22 @@
     "DescribeDatasetResponseTypeDef",
     {
         "CreatedBy": str,
         "CreateDate": datetime,
         "Name": str,
         "Format": InputFormatType,
         "FormatOptions": FormatOptionsOutputTypeDef,
-        "Input": InputOutputTypeDef,
+        "Input": InputTypeDef,
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "Source": SourceType,
         "PathOptions": PathOptionsOutputTypeDef,
         "Tags": Dict[str, str],
         "ResourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "Name": str,
@@ -2487,32 +2178,32 @@
     pass
 
 ListRecipeVersionsResponseTypeDef = TypedDict(
     "ListRecipeVersionsResponseTypeDef",
     {
         "NextToken": str,
         "Recipes": List[RecipeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecipesResponseTypeDef = TypedDict(
     "ListRecipesResponseTypeDef",
     {
         "Recipes": List[RecipeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProfileConfigurationOutputTypeDef = TypedDict(
     "ProfileConfigurationOutputTypeDef",
     {
         "DatasetStatisticsConfiguration": StatisticsConfigurationOutputTypeDef,
-        "ProfileColumns": List[ColumnSelectorOutputTypeDef],
+        "ProfileColumns": List[ColumnSelectorTypeDef],
         "ColumnStatisticsConfigurations": List[ColumnStatisticsConfigurationOutputTypeDef],
         "EntityDetectorConfiguration": EntityDetectorConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 ProfileConfigurationTypeDef = TypedDict(
@@ -2527,33 +2218,33 @@
 )
 
 ListJobRunsResponseTypeDef = TypedDict(
     "ListJobRunsResponseTypeDef",
     {
         "JobRuns": List[JobRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobResponseTypeDef = TypedDict(
     "DescribeJobResponseTypeDef",
     {
         "CreateDate": datetime,
@@ -2569,48 +2260,48 @@
         "MaxCapacity": int,
         "MaxRetries": int,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
         "ProjectName": str,
         "ProfileConfiguration": ProfileConfigurationOutputTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
-        "RecipeReference": RecipeReferenceOutputTypeDef,
+        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
+        "RecipeReference": RecipeReferenceTypeDef,
         "ResourceArn": str,
         "RoleArn": str,
         "Tags": Dict[str, str],
         "Timeout": int,
-        "JobSample": JobSampleOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobSample": JobSampleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobRunResponseTypeDef = TypedDict(
     "DescribeJobRunResponseTypeDef",
     {
         "Attempt": int,
         "CompletedOn": datetime,
         "DatasetName": str,
         "ErrorMessage": str,
         "ExecutionTime": int,
         "JobName": str,
         "ProfileConfiguration": ProfileConfigurationOutputTypeDef,
-        "ValidationConfigurations": List[ValidationConfigurationOutputTypeDef],
+        "ValidationConfigurations": List[ValidationConfigurationTypeDef],
         "RunId": str,
         "State": JobRunStateType,
         "LogSubscription": LogSubscriptionType,
         "LogGroupName": str,
         "Outputs": List[OutputTypeDef],
         "DataCatalogOutputs": List[DataCatalogOutputTypeDef],
         "DatabaseOutputs": List[DatabaseOutputTypeDef],
-        "RecipeReference": RecipeReferenceOutputTypeDef,
+        "RecipeReference": RecipeReferenceTypeDef,
         "StartedBy": str,
         "StartedOn": datetime,
-        "JobSample": JobSampleOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobSample": JobSampleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProfileJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfileJobRequestRequestTypeDef",
     {
         "DatasetName": str,
```

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/PKG-INFO` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-databrew
-Version: 1.28.12
-Summary: Type annotations for boto3.GlueDataBrew 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.GlueDataBrew 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-databrew.svg?color=blue)](https://pypi.org/project/mypy-boto3-databrew)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-databrew)](https://pepy.tech/project/mypy-boto3-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlueDataBrew 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[boto3.GlueDataBrew 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [mypy-boto3-databrew docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_databrew/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,157 +366,137 @@
 
 ```python
 from mypy_boto3_databrew.type_defs import (
     AllowedStatisticsOutputTypeDef,
     AllowedStatisticsTypeDef,
     BatchDeleteRecipeVersionRequestRequestTypeDef,
     RecipeVersionErrorDetailTypeDef,
-    ColumnSelectorOutputTypeDef,
+    ResponseMetadataTypeDef,
     ColumnSelectorTypeDef,
-    ConditionExpressionOutputTypeDef,
     ConditionExpressionTypeDef,
-    CreateDatasetResponseTypeDef,
     JobSampleTypeDef,
     S3LocationTypeDef,
     ValidationConfigurationTypeDef,
-    CreateProfileJobResponseTypeDef,
     SampleTypeDef,
-    CreateProjectResponseTypeDef,
     RecipeReferenceTypeDef,
-    CreateRecipeJobResponseTypeDef,
-    CreateRecipeResponseTypeDef,
-    CreateRulesetResponseTypeDef,
     CreateScheduleRequestRequestTypeDef,
-    CreateScheduleResponseTypeDef,
-    CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
-    CsvOutputOptionsOutputTypeDef,
     CsvOutputOptionsTypeDef,
-    S3LocationOutputTypeDef,
-    DatetimeOptionsOutputTypeDef,
-    FilterExpressionOutputTypeDef,
     DatetimeOptionsTypeDef,
+    FilterExpressionOutputTypeDef,
     FilterExpressionTypeDef,
     DeleteDatasetRequestRequestTypeDef,
-    DeleteDatasetResponseTypeDef,
     DeleteJobRequestRequestTypeDef,
-    DeleteJobResponseTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResponseTypeDef,
     DeleteRecipeVersionRequestRequestTypeDef,
-    DeleteRecipeVersionResponseTypeDef,
     DeleteRulesetRequestRequestTypeDef,
-    DeleteRulesetResponseTypeDef,
     DeleteScheduleRequestRequestTypeDef,
-    DeleteScheduleResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
-    JobSampleOutputTypeDef,
-    RecipeReferenceOutputTypeDef,
-    ValidationConfigurationOutputTypeDef,
     DescribeJobRunRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
-    SampleOutputTypeDef,
     DescribeRecipeRequestRequestTypeDef,
     DescribeRulesetRequestRequestTypeDef,
     DescribeScheduleRequestRequestTypeDef,
-    DescribeScheduleResponseTypeDef,
     ExcelOptionsOutputTypeDef,
     ExcelOptionsTypeDef,
-    FilesLimitOutputTypeDef,
     FilesLimitTypeDef,
-    JsonOptionsOutputTypeDef,
     JsonOptionsTypeDef,
-    MetadataOutputTypeDef,
     MetadataTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDatasetsRequestRequestTypeDef,
-    ListJobRunsRequestListJobRunsPaginateTypeDef,
     ListJobRunsRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
-    ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
     ListRecipeVersionsRequestRequestTypeDef,
-    ListRecipesRequestListRecipesPaginateTypeDef,
     ListRecipesRequestRequestTypeDef,
-    ListRulesetsRequestListRulesetsPaginateTypeDef,
     ListRulesetsRequestRequestTypeDef,
     RulesetItemTypeDef,
-    ListSchedulesRequestListSchedulesPaginateTypeDef,
     ListSchedulesRequestRequestTypeDef,
     ScheduleTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PublishRecipeRequestRequestTypeDef,
-    PublishRecipeResponseTypeDef,
     RecipeActionOutputTypeDef,
     RecipeActionTypeDef,
-    ResponseMetadataTypeDef,
-    ThresholdOutputTypeDef,
     ThresholdTypeDef,
     ViewFrameTypeDef,
-    SendProjectSessionActionResponseTypeDef,
     StartJobRunRequestRequestTypeDef,
-    StartJobRunResponseTypeDef,
     StartProjectSessionRequestRequestTypeDef,
-    StartProjectSessionResponseTypeDef,
     StatisticOverrideOutputTypeDef,
     StatisticOverrideTypeDef,
     StopJobRunRequestRequestTypeDef,
-    StopJobRunResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateScheduleRequestRequestTypeDef,
+    EntityDetectorConfigurationOutputTypeDef,
+    EntityDetectorConfigurationTypeDef,
+    BatchDeleteRecipeVersionResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateProfileJobResponseTypeDef,
+    CreateProjectResponseTypeDef,
+    CreateRecipeJobResponseTypeDef,
+    CreateRecipeResponseTypeDef,
+    CreateRulesetResponseTypeDef,
+    CreateScheduleResponseTypeDef,
+    DeleteDatasetResponseTypeDef,
+    DeleteJobResponseTypeDef,
+    DeleteProjectResponseTypeDef,
+    DeleteRecipeVersionResponseTypeDef,
+    DeleteRulesetResponseTypeDef,
+    DeleteScheduleResponseTypeDef,
+    DescribeScheduleResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PublishRecipeResponseTypeDef,
+    SendProjectSessionActionResponseTypeDef,
+    StartJobRunResponseTypeDef,
+    StartProjectSessionResponseTypeDef,
+    StopJobRunResponseTypeDef,
     UpdateDatasetResponseTypeDef,
     UpdateProfileJobResponseTypeDef,
     UpdateProjectResponseTypeDef,
     UpdateRecipeJobResponseTypeDef,
     UpdateRecipeResponseTypeDef,
     UpdateRulesetResponseTypeDef,
-    UpdateScheduleRequestRequestTypeDef,
     UpdateScheduleResponseTypeDef,
-    EntityDetectorConfigurationOutputTypeDef,
-    EntityDetectorConfigurationTypeDef,
-    BatchDeleteRecipeVersionResponseTypeDef,
     DataCatalogInputDefinitionTypeDef,
     DatabaseInputDefinitionTypeDef,
     DatabaseTableOutputOptionsTypeDef,
     S3TableOutputOptionsTypeDef,
     CreateProjectRequestRequestTypeDef,
+    DescribeProjectResponseTypeDef,
+    ProjectTypeDef,
     UpdateProjectRequestRequestTypeDef,
-    OutputFormatOptionsOutputTypeDef,
     OutputFormatOptionsTypeDef,
-    DataCatalogInputDefinitionOutputTypeDef,
-    DatabaseInputDefinitionOutputTypeDef,
-    DatabaseTableOutputOptionsOutputTypeDef,
-    S3TableOutputOptionsOutputTypeDef,
     DatasetParameterOutputTypeDef,
     DatasetParameterTypeDef,
-    DescribeProjectResponseTypeDef,
-    ProjectTypeDef,
     FormatOptionsOutputTypeDef,
     FormatOptionsTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListJobRunsRequestListJobRunsPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListRecipeVersionsRequestListRecipeVersionsPaginateTypeDef,
+    ListRecipesRequestListRecipesPaginateTypeDef,
+    ListRulesetsRequestListRulesetsPaginateTypeDef,
+    ListSchedulesRequestListSchedulesPaginateTypeDef,
     ListRulesetsResponseTypeDef,
     ListSchedulesResponseTypeDef,
     RecipeStepOutputTypeDef,
     RecipeStepTypeDef,
     RuleOutputTypeDef,
     RuleTypeDef,
     StatisticsConfigurationOutputTypeDef,
     StatisticsConfigurationTypeDef,
     InputTypeDef,
     DatabaseOutputTypeDef,
     DataCatalogOutputTypeDef,
+    ListProjectsResponseTypeDef,
     OutputTypeDef,
-    InputOutputTypeDef,
     PathOptionsOutputTypeDef,
     PathOptionsTypeDef,
-    ListProjectsResponseTypeDef,
     DescribeRecipeResponseTypeDef,
     RecipeTypeDef,
     CreateRecipeRequestRequestTypeDef,
     SendProjectSessionActionRequestRequestTypeDef,
     UpdateRecipeRequestRequestTypeDef,
     DescribeRulesetResponseTypeDef,
     CreateRulesetRequestRequestTypeDef,
```

### Comparing `mypy-boto3-databrew-1.28.12/mypy_boto3_databrew.egg-info/SOURCES.txt` & `mypy-boto3-databrew-1.28.15/mypy_boto3_databrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-databrew-1.28.12/setup.py` & `mypy-boto3-databrew-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-databrew",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_databrew"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GlueDataBrew 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.GlueDataBrew 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

