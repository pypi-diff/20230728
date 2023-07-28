# Comparing `tmp/mypy-boto3-amplifyuibuilder-1.28.12.tar.gz` & `tmp/mypy-boto3-amplifyuibuilder-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplifyuibuilder-1.28.12.tar", last modified: Thu Jul 27 05:34:16 2023, max compression
+gzip compressed data, was "mypy-boto3-amplifyuibuilder-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
```

## Comparing `mypy-boto3-amplifyuibuilder-1.28.12.tar` & `mypy-boto3-amplifyuibuilder-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.320584 mypy-boto3-amplifyuibuilder-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-07-27 05:34:16.316584 mypy-boto3-amplifyuibuilder-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18510 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.308584 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21995 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65450 2023-07-27 05:17:07.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65332 2023-07-27 05:17:06.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.316584 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-07-27 05:34:16.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:34:16.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:16.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:16.000000 mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:16.320584 mypy-boto3-amplifyuibuilder-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:17:05.000000 mypy-boto3-amplifyuibuilder-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.712609 mypy-boto3-amplifyuibuilder-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:56.000000 mypy-boto3-amplifyuibuilder-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-07-28 20:42:12.712609 mypy-boto3-amplifyuibuilder-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-07-28 20:18:56.000000 mypy-boto3-amplifyuibuilder-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.708609 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-28 20:18:56.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-28 20:18:56.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 20:18:56.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22014 2023-07-28 20:18:57.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-07-28 20:18:56.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-28 20:18:57.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-07-28 20:18:57.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-07-28 20:18:57.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-28 20:18:57.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:56.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58618 2023-07-28 20:18:59.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58508 2023-07-28 20:18:58.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:56.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.712609 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19243 2023-07-28 20:42:12.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:42:12.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:42:12.000000 mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.712609 mypy-boto3-amplifyuibuilder-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 20:18:56.000000 mypy-boto3-amplifyuibuilder-1.28.15/setup.py
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/LICENSE` & `mypy-boto3-amplifyuibuilder-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/PKG-INFO` & `mypy-boto3-amplifyuibuilder-1.28.15/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifyuibuilder
-Version: 1.28.12
-Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifyuibuilder)](https://pepy.tech/project/mypy-boto3-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyUIBuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[boto3.AmplifyUIBuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
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
 [mypy-boto3-amplifyuibuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,177 +355,157 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
-    ActionParametersOutputTypeDef,
-    ActionParametersTypeDef,
-    CodegenFeatureFlagsOutputTypeDef,
+    MutationActionSetStateParameterTypeDef,
     CodegenFeatureFlagsTypeDef,
     CodegenGenericDataEnumOutputTypeDef,
     CodegenGenericDataEnumTypeDef,
-    CodegenGenericDataFieldOutputTypeDef,
-    CodegenGenericDataFieldTypeDef,
-    CodegenGenericDataModelOutputTypeDef,
-    CodegenGenericDataModelTypeDef,
-    CodegenGenericDataNonModelOutputTypeDef,
-    CodegenGenericDataNonModelTypeDef,
     CodegenGenericDataRelationshipTypeOutputTypeDef,
     CodegenGenericDataRelationshipTypeTypeDef,
     CodegenJobAssetTypeDef,
-    CodegenJobGenericDataSchemaOutputTypeDef,
-    CodegenJobGenericDataSchemaTypeDef,
-    CodegenJobRenderConfigOutputTypeDef,
-    CodegenJobRenderConfigTypeDef,
+    ReactStartCodegenJobDataTypeDef,
     CodegenJobSummaryTypeDef,
-    CodegenJobTypeDef,
-    ComponentBindingPropertiesValueOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
-    ComponentBindingPropertiesValueTypeDef,
-    ComponentChildOutputTypeDef,
-    ComponentChildTypeDef,
-    ComponentConditionPropertyOutputTypeDef,
     ComponentConditionPropertyTypeDef,
-    ComponentDataConfigurationOutputTypeDef,
-    ComponentDataConfigurationTypeDef,
-    ComponentEventOutputTypeDef,
-    ComponentEventTypeDef,
-    ComponentPropertyBindingPropertiesOutputTypeDef,
+    SortPropertyTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
-    ComponentPropertyOutputTypeDef,
-    ComponentPropertyTypeDef,
+    FormBindingElementTypeDef,
     ComponentSummaryTypeDef,
-    ComponentTypeDef,
     ComponentVariantOutputTypeDef,
     ComponentVariantTypeDef,
-    CreateComponentDataTypeDef,
-    CreateComponentRequestRequestTypeDef,
-    CreateComponentResponseTypeDef,
-    CreateFormDataTypeDef,
-    CreateFormRequestRequestTypeDef,
-    CreateFormResponseTypeDef,
+    ResponseMetadataTypeDef,
+    FormDataTypeConfigTypeDef,
     CreateThemeDataTypeDef,
-    CreateThemeRequestRequestTypeDef,
-    CreateThemeResponseTypeDef,
+    ThemeTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteFormRequestRequestTypeDef,
     DeleteThemeRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExchangeCodeForTokenRequestBodyTypeDef,
-    ExchangeCodeForTokenRequestRequestTypeDef,
-    ExchangeCodeForTokenResponseTypeDef,
-    ExportComponentsRequestExportComponentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ExportComponentsRequestRequestTypeDef,
-    ExportComponentsResponseTypeDef,
-    ExportFormsRequestExportFormsPaginateTypeDef,
     ExportFormsRequestRequestTypeDef,
-    ExportFormsResponseTypeDef,
-    ExportThemesRequestExportThemesPaginateTypeDef,
     ExportThemesRequestRequestTypeDef,
-    ExportThemesResponseTypeDef,
-    FieldConfigOutputTypeDef,
-    FieldConfigTypeDef,
-    FieldInputConfigOutputTypeDef,
-    FieldInputConfigTypeDef,
-    FieldPositionOutputTypeDef,
     FieldPositionTypeDef,
     FieldValidationConfigurationOutputTypeDef,
     FieldValidationConfigurationTypeDef,
     FileUploaderFieldConfigOutputTypeDef,
     FileUploaderFieldConfigTypeDef,
-    FormBindingElementOutputTypeDef,
-    FormBindingElementTypeDef,
-    FormButtonOutputTypeDef,
-    FormButtonTypeDef,
-    FormCTAOutputTypeDef,
-    FormCTATypeDef,
-    FormDataTypeConfigOutputTypeDef,
-    FormDataTypeConfigTypeDef,
-    FormInputBindingPropertiesValueOutputTypeDef,
-    FormInputBindingPropertiesValuePropertiesOutputTypeDef,
     FormInputBindingPropertiesValuePropertiesTypeDef,
-    FormInputBindingPropertiesValueTypeDef,
-    FormInputValuePropertyBindingPropertiesOutputTypeDef,
     FormInputValuePropertyBindingPropertiesTypeDef,
-    FormInputValuePropertyOutputTypeDef,
-    FormInputValuePropertyTypeDef,
-    FormStyleConfigOutputTypeDef,
     FormStyleConfigTypeDef,
-    FormStyleOutputTypeDef,
-    FormStyleTypeDef,
-    FormSummaryTypeDef,
-    FormTypeDef,
     GetCodegenJobRequestRequestTypeDef,
-    GetCodegenJobResponseTypeDef,
     GetComponentRequestRequestTypeDef,
-    GetComponentResponseTypeDef,
     GetFormRequestRequestTypeDef,
-    GetFormResponseTypeDef,
     GetMetadataRequestRequestTypeDef,
-    GetMetadataResponseTypeDef,
     GetThemeRequestRequestTypeDef,
-    GetThemeResponseTypeDef,
-    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
     ListCodegenJobsRequestRequestTypeDef,
-    ListCodegenJobsResponseTypeDef,
-    ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListComponentsResponseTypeDef,
-    ListFormsRequestListFormsPaginateTypeDef,
     ListFormsRequestRequestTypeDef,
-    ListFormsResponseTypeDef,
-    ListThemesRequestListThemesPaginateTypeDef,
     ListThemesRequestRequestTypeDef,
-    ListThemesResponseTypeDef,
-    MutationActionSetStateParameterOutputTypeDef,
-    MutationActionSetStateParameterTypeDef,
-    PaginatorConfigTypeDef,
+    ThemeSummaryTypeDef,
     PredicateOutputTypeDef,
     PredicateTypeDef,
     PutMetadataFlagBodyTypeDef,
-    PutMetadataFlagRequestRequestTypeDef,
-    ReactStartCodegenJobDataOutputTypeDef,
-    ReactStartCodegenJobDataTypeDef,
     RefreshTokenRequestBodyTypeDef,
-    RefreshTokenRequestRequestTypeDef,
-    RefreshTokenResponseTypeDef,
-    ResponseMetadataTypeDef,
-    SectionalElementOutputTypeDef,
-    SectionalElementTypeDef,
-    SortPropertyOutputTypeDef,
-    SortPropertyTypeDef,
-    StartCodegenJobDataTypeDef,
-    StartCodegenJobRequestRequestTypeDef,
-    StartCodegenJobResponseTypeDef,
-    ThemeSummaryTypeDef,
-    ThemeTypeDef,
     ThemeValueOutputTypeDef,
     ThemeValueTypeDef,
     ThemeValuesOutputTypeDef,
     ThemeValuesTypeDef,
-    UpdateComponentDataTypeDef,
-    UpdateComponentRequestRequestTypeDef,
-    UpdateComponentResponseTypeDef,
-    UpdateFormDataTypeDef,
-    UpdateFormRequestRequestTypeDef,
-    UpdateFormResponseTypeDef,
     UpdateThemeDataTypeDef,
-    UpdateThemeRequestRequestTypeDef,
-    UpdateThemeResponseTypeDef,
-    ValueMappingOutputTypeDef,
     ValueMappingTypeDef,
+    ActionParametersOutputTypeDef,
+    ActionParametersTypeDef,
+    CodegenGenericDataFieldOutputTypeDef,
+    CodegenGenericDataFieldTypeDef,
+    CodegenJobRenderConfigTypeDef,
+    ComponentBindingPropertiesValueOutputTypeDef,
+    ComponentBindingPropertiesValueTypeDef,
+    ComponentDataConfigurationOutputTypeDef,
+    ComponentDataConfigurationTypeDef,
+    ComponentPropertyOutputTypeDef,
+    ComponentPropertyTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExchangeCodeForTokenResponseTypeDef,
+    GetMetadataResponseTypeDef,
+    ListCodegenJobsResponseTypeDef,
+    ListComponentsResponseTypeDef,
+    RefreshTokenResponseTypeDef,
+    FormSummaryTypeDef,
+    CreateThemeRequestRequestTypeDef,
+    CreateThemeResponseTypeDef,
+    ExportThemesResponseTypeDef,
+    GetThemeResponseTypeDef,
+    UpdateThemeResponseTypeDef,
+    ExchangeCodeForTokenRequestRequestTypeDef,
+    ExportComponentsRequestExportComponentsPaginateTypeDef,
+    ExportFormsRequestExportFormsPaginateTypeDef,
+    ExportThemesRequestExportThemesPaginateTypeDef,
+    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    ListComponentsRequestListComponentsPaginateTypeDef,
+    ListFormsRequestListFormsPaginateTypeDef,
+    ListThemesRequestListThemesPaginateTypeDef,
+    FormButtonTypeDef,
+    SectionalElementTypeDef,
+    FormInputBindingPropertiesValueTypeDef,
+    FormInputValuePropertyTypeDef,
+    FormStyleTypeDef,
+    ListThemesResponseTypeDef,
+    PutMetadataFlagRequestRequestTypeDef,
+    RefreshTokenRequestRequestTypeDef,
+    UpdateThemeRequestRequestTypeDef,
+    ComponentEventOutputTypeDef,
+    ComponentEventTypeDef,
+    CodegenGenericDataModelOutputTypeDef,
+    CodegenGenericDataNonModelOutputTypeDef,
+    CodegenGenericDataModelTypeDef,
+    CodegenGenericDataNonModelTypeDef,
+    ListFormsResponseTypeDef,
+    FormCTATypeDef,
     ValueMappingsOutputTypeDef,
     ValueMappingsTypeDef,
+    ComponentChildOutputTypeDef,
+    ComponentTypeDef,
+    ComponentChildTypeDef,
+    CreateComponentDataTypeDef,
+    UpdateComponentDataTypeDef,
+    CodegenJobGenericDataSchemaOutputTypeDef,
+    CodegenJobGenericDataSchemaTypeDef,
+    FieldInputConfigOutputTypeDef,
+    FieldInputConfigTypeDef,
+    CreateComponentResponseTypeDef,
+    ExportComponentsResponseTypeDef,
+    GetComponentResponseTypeDef,
+    UpdateComponentResponseTypeDef,
+    CreateComponentRequestRequestTypeDef,
+    UpdateComponentRequestRequestTypeDef,
+    CodegenJobTypeDef,
+    StartCodegenJobDataTypeDef,
+    FieldConfigOutputTypeDef,
+    FieldConfigTypeDef,
+    GetCodegenJobResponseTypeDef,
+    StartCodegenJobResponseTypeDef,
+    StartCodegenJobRequestRequestTypeDef,
+    FormTypeDef,
+    CreateFormDataTypeDef,
+    UpdateFormDataTypeDef,
+    CreateFormResponseTypeDef,
+    ExportFormsResponseTypeDef,
+    GetFormResponseTypeDef,
+    UpdateFormResponseTypeDef,
+    CreateFormRequestRequestTypeDef,
+    UpdateFormRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActionParametersOutputTypeDef:
+def get_structure() -> MutationActionSetStateParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/README.md` & `mypy-boto3-amplifyuibuilder-1.28.15/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifyuibuilder)](https://pepy.tech/project/mypy-boto3-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyUIBuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[boto3.AmplifyUIBuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
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
 [mypy-boto3-amplifyuibuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,177 +323,157 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
-    ActionParametersOutputTypeDef,
-    ActionParametersTypeDef,
-    CodegenFeatureFlagsOutputTypeDef,
+    MutationActionSetStateParameterTypeDef,
     CodegenFeatureFlagsTypeDef,
     CodegenGenericDataEnumOutputTypeDef,
     CodegenGenericDataEnumTypeDef,
-    CodegenGenericDataFieldOutputTypeDef,
-    CodegenGenericDataFieldTypeDef,
-    CodegenGenericDataModelOutputTypeDef,
-    CodegenGenericDataModelTypeDef,
-    CodegenGenericDataNonModelOutputTypeDef,
-    CodegenGenericDataNonModelTypeDef,
     CodegenGenericDataRelationshipTypeOutputTypeDef,
     CodegenGenericDataRelationshipTypeTypeDef,
     CodegenJobAssetTypeDef,
-    CodegenJobGenericDataSchemaOutputTypeDef,
-    CodegenJobGenericDataSchemaTypeDef,
-    CodegenJobRenderConfigOutputTypeDef,
-    CodegenJobRenderConfigTypeDef,
+    ReactStartCodegenJobDataTypeDef,
     CodegenJobSummaryTypeDef,
-    CodegenJobTypeDef,
-    ComponentBindingPropertiesValueOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
-    ComponentBindingPropertiesValueTypeDef,
-    ComponentChildOutputTypeDef,
-    ComponentChildTypeDef,
-    ComponentConditionPropertyOutputTypeDef,
     ComponentConditionPropertyTypeDef,
-    ComponentDataConfigurationOutputTypeDef,
-    ComponentDataConfigurationTypeDef,
-    ComponentEventOutputTypeDef,
-    ComponentEventTypeDef,
-    ComponentPropertyBindingPropertiesOutputTypeDef,
+    SortPropertyTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
-    ComponentPropertyOutputTypeDef,
-    ComponentPropertyTypeDef,
+    FormBindingElementTypeDef,
     ComponentSummaryTypeDef,
-    ComponentTypeDef,
     ComponentVariantOutputTypeDef,
     ComponentVariantTypeDef,
-    CreateComponentDataTypeDef,
-    CreateComponentRequestRequestTypeDef,
-    CreateComponentResponseTypeDef,
-    CreateFormDataTypeDef,
-    CreateFormRequestRequestTypeDef,
-    CreateFormResponseTypeDef,
+    ResponseMetadataTypeDef,
+    FormDataTypeConfigTypeDef,
     CreateThemeDataTypeDef,
-    CreateThemeRequestRequestTypeDef,
-    CreateThemeResponseTypeDef,
+    ThemeTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteFormRequestRequestTypeDef,
     DeleteThemeRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExchangeCodeForTokenRequestBodyTypeDef,
-    ExchangeCodeForTokenRequestRequestTypeDef,
-    ExchangeCodeForTokenResponseTypeDef,
-    ExportComponentsRequestExportComponentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ExportComponentsRequestRequestTypeDef,
-    ExportComponentsResponseTypeDef,
-    ExportFormsRequestExportFormsPaginateTypeDef,
     ExportFormsRequestRequestTypeDef,
-    ExportFormsResponseTypeDef,
-    ExportThemesRequestExportThemesPaginateTypeDef,
     ExportThemesRequestRequestTypeDef,
-    ExportThemesResponseTypeDef,
-    FieldConfigOutputTypeDef,
-    FieldConfigTypeDef,
-    FieldInputConfigOutputTypeDef,
-    FieldInputConfigTypeDef,
-    FieldPositionOutputTypeDef,
     FieldPositionTypeDef,
     FieldValidationConfigurationOutputTypeDef,
     FieldValidationConfigurationTypeDef,
     FileUploaderFieldConfigOutputTypeDef,
     FileUploaderFieldConfigTypeDef,
-    FormBindingElementOutputTypeDef,
-    FormBindingElementTypeDef,
-    FormButtonOutputTypeDef,
-    FormButtonTypeDef,
-    FormCTAOutputTypeDef,
-    FormCTATypeDef,
-    FormDataTypeConfigOutputTypeDef,
-    FormDataTypeConfigTypeDef,
-    FormInputBindingPropertiesValueOutputTypeDef,
-    FormInputBindingPropertiesValuePropertiesOutputTypeDef,
     FormInputBindingPropertiesValuePropertiesTypeDef,
-    FormInputBindingPropertiesValueTypeDef,
-    FormInputValuePropertyBindingPropertiesOutputTypeDef,
     FormInputValuePropertyBindingPropertiesTypeDef,
-    FormInputValuePropertyOutputTypeDef,
-    FormInputValuePropertyTypeDef,
-    FormStyleConfigOutputTypeDef,
     FormStyleConfigTypeDef,
-    FormStyleOutputTypeDef,
-    FormStyleTypeDef,
-    FormSummaryTypeDef,
-    FormTypeDef,
     GetCodegenJobRequestRequestTypeDef,
-    GetCodegenJobResponseTypeDef,
     GetComponentRequestRequestTypeDef,
-    GetComponentResponseTypeDef,
     GetFormRequestRequestTypeDef,
-    GetFormResponseTypeDef,
     GetMetadataRequestRequestTypeDef,
-    GetMetadataResponseTypeDef,
     GetThemeRequestRequestTypeDef,
-    GetThemeResponseTypeDef,
-    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
     ListCodegenJobsRequestRequestTypeDef,
-    ListCodegenJobsResponseTypeDef,
-    ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListComponentsResponseTypeDef,
-    ListFormsRequestListFormsPaginateTypeDef,
     ListFormsRequestRequestTypeDef,
-    ListFormsResponseTypeDef,
-    ListThemesRequestListThemesPaginateTypeDef,
     ListThemesRequestRequestTypeDef,
-    ListThemesResponseTypeDef,
-    MutationActionSetStateParameterOutputTypeDef,
-    MutationActionSetStateParameterTypeDef,
-    PaginatorConfigTypeDef,
+    ThemeSummaryTypeDef,
     PredicateOutputTypeDef,
     PredicateTypeDef,
     PutMetadataFlagBodyTypeDef,
-    PutMetadataFlagRequestRequestTypeDef,
-    ReactStartCodegenJobDataOutputTypeDef,
-    ReactStartCodegenJobDataTypeDef,
     RefreshTokenRequestBodyTypeDef,
-    RefreshTokenRequestRequestTypeDef,
-    RefreshTokenResponseTypeDef,
-    ResponseMetadataTypeDef,
-    SectionalElementOutputTypeDef,
-    SectionalElementTypeDef,
-    SortPropertyOutputTypeDef,
-    SortPropertyTypeDef,
-    StartCodegenJobDataTypeDef,
-    StartCodegenJobRequestRequestTypeDef,
-    StartCodegenJobResponseTypeDef,
-    ThemeSummaryTypeDef,
-    ThemeTypeDef,
     ThemeValueOutputTypeDef,
     ThemeValueTypeDef,
     ThemeValuesOutputTypeDef,
     ThemeValuesTypeDef,
-    UpdateComponentDataTypeDef,
-    UpdateComponentRequestRequestTypeDef,
-    UpdateComponentResponseTypeDef,
-    UpdateFormDataTypeDef,
-    UpdateFormRequestRequestTypeDef,
-    UpdateFormResponseTypeDef,
     UpdateThemeDataTypeDef,
-    UpdateThemeRequestRequestTypeDef,
-    UpdateThemeResponseTypeDef,
-    ValueMappingOutputTypeDef,
     ValueMappingTypeDef,
+    ActionParametersOutputTypeDef,
+    ActionParametersTypeDef,
+    CodegenGenericDataFieldOutputTypeDef,
+    CodegenGenericDataFieldTypeDef,
+    CodegenJobRenderConfigTypeDef,
+    ComponentBindingPropertiesValueOutputTypeDef,
+    ComponentBindingPropertiesValueTypeDef,
+    ComponentDataConfigurationOutputTypeDef,
+    ComponentDataConfigurationTypeDef,
+    ComponentPropertyOutputTypeDef,
+    ComponentPropertyTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExchangeCodeForTokenResponseTypeDef,
+    GetMetadataResponseTypeDef,
+    ListCodegenJobsResponseTypeDef,
+    ListComponentsResponseTypeDef,
+    RefreshTokenResponseTypeDef,
+    FormSummaryTypeDef,
+    CreateThemeRequestRequestTypeDef,
+    CreateThemeResponseTypeDef,
+    ExportThemesResponseTypeDef,
+    GetThemeResponseTypeDef,
+    UpdateThemeResponseTypeDef,
+    ExchangeCodeForTokenRequestRequestTypeDef,
+    ExportComponentsRequestExportComponentsPaginateTypeDef,
+    ExportFormsRequestExportFormsPaginateTypeDef,
+    ExportThemesRequestExportThemesPaginateTypeDef,
+    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    ListComponentsRequestListComponentsPaginateTypeDef,
+    ListFormsRequestListFormsPaginateTypeDef,
+    ListThemesRequestListThemesPaginateTypeDef,
+    FormButtonTypeDef,
+    SectionalElementTypeDef,
+    FormInputBindingPropertiesValueTypeDef,
+    FormInputValuePropertyTypeDef,
+    FormStyleTypeDef,
+    ListThemesResponseTypeDef,
+    PutMetadataFlagRequestRequestTypeDef,
+    RefreshTokenRequestRequestTypeDef,
+    UpdateThemeRequestRequestTypeDef,
+    ComponentEventOutputTypeDef,
+    ComponentEventTypeDef,
+    CodegenGenericDataModelOutputTypeDef,
+    CodegenGenericDataNonModelOutputTypeDef,
+    CodegenGenericDataModelTypeDef,
+    CodegenGenericDataNonModelTypeDef,
+    ListFormsResponseTypeDef,
+    FormCTATypeDef,
     ValueMappingsOutputTypeDef,
     ValueMappingsTypeDef,
+    ComponentChildOutputTypeDef,
+    ComponentTypeDef,
+    ComponentChildTypeDef,
+    CreateComponentDataTypeDef,
+    UpdateComponentDataTypeDef,
+    CodegenJobGenericDataSchemaOutputTypeDef,
+    CodegenJobGenericDataSchemaTypeDef,
+    FieldInputConfigOutputTypeDef,
+    FieldInputConfigTypeDef,
+    CreateComponentResponseTypeDef,
+    ExportComponentsResponseTypeDef,
+    GetComponentResponseTypeDef,
+    UpdateComponentResponseTypeDef,
+    CreateComponentRequestRequestTypeDef,
+    UpdateComponentRequestRequestTypeDef,
+    CodegenJobTypeDef,
+    StartCodegenJobDataTypeDef,
+    FieldConfigOutputTypeDef,
+    FieldConfigTypeDef,
+    GetCodegenJobResponseTypeDef,
+    StartCodegenJobResponseTypeDef,
+    StartCodegenJobRequestRequestTypeDef,
+    FormTypeDef,
+    CreateFormDataTypeDef,
+    UpdateFormDataTypeDef,
+    CreateFormResponseTypeDef,
+    ExportFormsResponseTypeDef,
+    GetFormResponseTypeDef,
+    UpdateFormResponseTypeDef,
+    CreateFormRequestRequestTypeDef,
+    UpdateFormRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActionParametersOutputTypeDef:
+def get_structure() -> MutationActionSetStateParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/__init__.py` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/__init__.pyi` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/__main__.py` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AmplifyUIBuilder 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.AmplifyUIBuilder 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder\nOther"
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

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/client.py` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,45 +124,45 @@
         """
 
     def create_component(
         self,
         *,
         appId: str,
         environmentName: str,
-        componentToCreate: "CreateComponentDataTypeDef",
+        componentToCreate: CreateComponentDataTypeDef,
         clientToken: str = ...
     ) -> CreateComponentResponseTypeDef:
         """
         Creates a new component for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#create_component)
         """
 
     def create_form(
         self,
         *,
         appId: str,
         environmentName: str,
-        formToCreate: "CreateFormDataTypeDef",
+        formToCreate: CreateFormDataTypeDef,
         clientToken: str = ...
     ) -> CreateFormResponseTypeDef:
         """
         Creates a new form for an Amplify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#create_form)
         """
 
     def create_theme(
         self,
         *,
         appId: str,
         environmentName: str,
-        themeToCreate: "CreateThemeDataTypeDef",
+        themeToCreate: CreateThemeDataTypeDef,
         clientToken: str = ...
     ) -> CreateThemeResponseTypeDef:
         """
         Creates a theme to apply to the components in an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#create_theme)
@@ -195,15 +195,15 @@
         Deletes a theme from an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.delete_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#delete_theme)
         """
 
     def exchange_code_for_token(
-        self, *, provider: Literal["figma"], request: "ExchangeCodeForTokenRequestBodyTypeDef"
+        self, *, provider: Literal["figma"], request: ExchangeCodeForTokenRequestBodyTypeDef
     ) -> ExchangeCodeForTokenResponseTypeDef:
         """
         Exchanges an access code for a token.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.exchange_code_for_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#exchange_code_for_token)
         """
@@ -343,39 +343,39 @@
 
     def put_metadata_flag(
         self,
         *,
         appId: str,
         environmentName: str,
         featureName: str,
-        body: "PutMetadataFlagBodyTypeDef"
+        body: PutMetadataFlagBodyTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Stores the metadata information about a feature on a form.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.put_metadata_flag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#put_metadata_flag)
         """
 
     def refresh_token(
-        self, *, provider: Literal["figma"], refreshTokenBody: "RefreshTokenRequestBodyTypeDef"
+        self, *, provider: Literal["figma"], refreshTokenBody: RefreshTokenRequestBodyTypeDef
     ) -> RefreshTokenResponseTypeDef:
         """
         Refreshes a previously issued access token that might have expired.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.refresh_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#refresh_token)
         """
 
     def start_codegen_job(
         self,
         *,
         appId: str,
         environmentName: str,
-        codegenJobToCreate: "StartCodegenJobDataTypeDef",
+        codegenJobToCreate: StartCodegenJobDataTypeDef,
         clientToken: str = ...
     ) -> StartCodegenJobResponseTypeDef:
         """
         Starts a code generation job for for a specified Amplify app and backend
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.start_codegen_job)
@@ -384,15 +384,15 @@
 
     def update_component(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
-        updatedComponent: "UpdateComponentDataTypeDef",
+        updatedComponent: UpdateComponentDataTypeDef,
         clientToken: str = ...
     ) -> UpdateComponentResponseTypeDef:
         """
         Updates an existing component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#update_component)
@@ -400,15 +400,15 @@
 
     def update_form(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
-        updatedForm: "UpdateFormDataTypeDef",
+        updatedForm: UpdateFormDataTypeDef,
         clientToken: str = ...
     ) -> UpdateFormResponseTypeDef:
         """
         Updates an existing form.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#update_form)
@@ -416,15 +416,15 @@
 
     def update_theme(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
-        updatedTheme: "UpdateThemeDataTypeDef",
+        updatedTheme: UpdateThemeDataTypeDef,
         clientToken: str = ...
     ) -> UpdateThemeResponseTypeDef:
         """
         Updates an existing theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#update_theme)
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/client.pyi` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -117,43 +117,43 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#close)
         """
     def create_component(
         self,
         *,
         appId: str,
         environmentName: str,
-        componentToCreate: "CreateComponentDataTypeDef",
+        componentToCreate: CreateComponentDataTypeDef,
         clientToken: str = ...
     ) -> CreateComponentResponseTypeDef:
         """
         Creates a new component for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#create_component)
         """
     def create_form(
         self,
         *,
         appId: str,
         environmentName: str,
-        formToCreate: "CreateFormDataTypeDef",
+        formToCreate: CreateFormDataTypeDef,
         clientToken: str = ...
     ) -> CreateFormResponseTypeDef:
         """
         Creates a new form for an Amplify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#create_form)
         """
     def create_theme(
         self,
         *,
         appId: str,
         environmentName: str,
-        themeToCreate: "CreateThemeDataTypeDef",
+        themeToCreate: CreateThemeDataTypeDef,
         clientToken: str = ...
     ) -> CreateThemeResponseTypeDef:
         """
         Creates a theme to apply to the components in an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#create_theme)
@@ -182,15 +182,15 @@
         """
         Deletes a theme from an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.delete_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#delete_theme)
         """
     def exchange_code_for_token(
-        self, *, provider: Literal["figma"], request: "ExchangeCodeForTokenRequestBodyTypeDef"
+        self, *, provider: Literal["figma"], request: ExchangeCodeForTokenRequestBodyTypeDef
     ) -> ExchangeCodeForTokenResponseTypeDef:
         """
         Exchanges an access code for a token.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.exchange_code_for_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#exchange_code_for_token)
         """
@@ -316,37 +316,37 @@
         """
     def put_metadata_flag(
         self,
         *,
         appId: str,
         environmentName: str,
         featureName: str,
-        body: "PutMetadataFlagBodyTypeDef"
+        body: PutMetadataFlagBodyTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Stores the metadata information about a feature on a form.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.put_metadata_flag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#put_metadata_flag)
         """
     def refresh_token(
-        self, *, provider: Literal["figma"], refreshTokenBody: "RefreshTokenRequestBodyTypeDef"
+        self, *, provider: Literal["figma"], refreshTokenBody: RefreshTokenRequestBodyTypeDef
     ) -> RefreshTokenResponseTypeDef:
         """
         Refreshes a previously issued access token that might have expired.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.refresh_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#refresh_token)
         """
     def start_codegen_job(
         self,
         *,
         appId: str,
         environmentName: str,
-        codegenJobToCreate: "StartCodegenJobDataTypeDef",
+        codegenJobToCreate: StartCodegenJobDataTypeDef,
         clientToken: str = ...
     ) -> StartCodegenJobResponseTypeDef:
         """
         Starts a code generation job for for a specified Amplify app and backend
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.start_codegen_job)
@@ -354,45 +354,45 @@
         """
     def update_component(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
-        updatedComponent: "UpdateComponentDataTypeDef",
+        updatedComponent: UpdateComponentDataTypeDef,
         clientToken: str = ...
     ) -> UpdateComponentResponseTypeDef:
         """
         Updates an existing component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_component)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#update_component)
         """
     def update_form(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
-        updatedForm: "UpdateFormDataTypeDef",
+        updatedForm: UpdateFormDataTypeDef,
         clientToken: str = ...
     ) -> UpdateFormResponseTypeDef:
         """
         Updates an existing form.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#update_form)
         """
     def update_theme(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
-        updatedTheme: "UpdateThemeDataTypeDef",
+        updatedTheme: UpdateThemeDataTypeDef,
         clientToken: str = ...
     ) -> UpdateThemeResponseTypeDef:
         """
         Updates an existing theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#update_theme)
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/literals.py` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/literals.pyi` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/paginator.py` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,103 +70,103 @@
 class ExportComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportcomponentspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ExportComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportcomponentspaginator)
         """
 
 
 class ExportFormsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportForms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportformspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ExportFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportForms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportformspaginator)
         """
 
 
 class ExportThemesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportthemespaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ExportThemesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportthemespaginator)
         """
 
 
 class ListCodegenJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListCodegenJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcodegenjobspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCodegenJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListCodegenJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcodegenjobspaginator)
         """
 
 
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcomponentspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcomponentspaginator)
         """
 
 
 class ListFormsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListForms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listformspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListForms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listformspaginator)
         """
 
 
 class ListThemesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listthemespaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThemesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listthemespaginator)
         """
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/paginator.pyi` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/paginator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -67,97 +67,97 @@
 class ExportComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportcomponentspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ExportComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportcomponentspaginator)
         """
 
 class ExportFormsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportForms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportformspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ExportFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportForms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportformspaginator)
         """
 
 class ExportThemesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportthemespaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ExportThemesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#exportthemespaginator)
         """
 
 class ListCodegenJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListCodegenJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcodegenjobspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCodegenJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListCodegenJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcodegenjobspaginator)
         """
 
 class ListComponentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcomponentspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listcomponentspaginator)
         """
 
 class ListFormsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListForms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listformspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListForms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listformspaginator)
         """
 
 class ListThemesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listthemespaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThemesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/paginators/#listthemespaginator)
         """
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/type_defs.py` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplifyuibuilder service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplifyuibuilder.type_defs import ActionParametersOutputTypeDef
+    from mypy_boto3_amplifyuibuilder.type_defs import MutationActionSetStateParameterTypeDef
 
-    data: ActionParametersOutputTypeDef = {...}
+    data: MutationActionSetStateParameterTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -37,214 +37,162 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ActionParametersOutputTypeDef",
-    "ActionParametersTypeDef",
-    "CodegenFeatureFlagsOutputTypeDef",
+    "MutationActionSetStateParameterTypeDef",
     "CodegenFeatureFlagsTypeDef",
     "CodegenGenericDataEnumOutputTypeDef",
     "CodegenGenericDataEnumTypeDef",
-    "CodegenGenericDataFieldOutputTypeDef",
-    "CodegenGenericDataFieldTypeDef",
-    "CodegenGenericDataModelOutputTypeDef",
-    "CodegenGenericDataModelTypeDef",
-    "CodegenGenericDataNonModelOutputTypeDef",
-    "CodegenGenericDataNonModelTypeDef",
     "CodegenGenericDataRelationshipTypeOutputTypeDef",
     "CodegenGenericDataRelationshipTypeTypeDef",
     "CodegenJobAssetTypeDef",
-    "CodegenJobGenericDataSchemaOutputTypeDef",
-    "CodegenJobGenericDataSchemaTypeDef",
-    "CodegenJobRenderConfigOutputTypeDef",
-    "CodegenJobRenderConfigTypeDef",
+    "ReactStartCodegenJobDataTypeDef",
     "CodegenJobSummaryTypeDef",
-    "CodegenJobTypeDef",
-    "ComponentBindingPropertiesValueOutputTypeDef",
     "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
-    "ComponentBindingPropertiesValueTypeDef",
-    "ComponentChildOutputTypeDef",
-    "ComponentChildTypeDef",
-    "ComponentConditionPropertyOutputTypeDef",
     "ComponentConditionPropertyTypeDef",
-    "ComponentDataConfigurationOutputTypeDef",
-    "ComponentDataConfigurationTypeDef",
-    "ComponentEventOutputTypeDef",
-    "ComponentEventTypeDef",
-    "ComponentPropertyBindingPropertiesOutputTypeDef",
+    "SortPropertyTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
-    "ComponentPropertyOutputTypeDef",
-    "ComponentPropertyTypeDef",
+    "FormBindingElementTypeDef",
     "ComponentSummaryTypeDef",
-    "ComponentTypeDef",
     "ComponentVariantOutputTypeDef",
     "ComponentVariantTypeDef",
-    "CreateComponentDataTypeDef",
-    "CreateComponentRequestRequestTypeDef",
-    "CreateComponentResponseTypeDef",
-    "CreateFormDataTypeDef",
-    "CreateFormRequestRequestTypeDef",
-    "CreateFormResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "FormDataTypeConfigTypeDef",
     "CreateThemeDataTypeDef",
-    "CreateThemeRequestRequestTypeDef",
-    "CreateThemeResponseTypeDef",
+    "ThemeTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteFormRequestRequestTypeDef",
     "DeleteThemeRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExchangeCodeForTokenRequestBodyTypeDef",
-    "ExchangeCodeForTokenRequestRequestTypeDef",
-    "ExchangeCodeForTokenResponseTypeDef",
-    "ExportComponentsRequestExportComponentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ExportComponentsRequestRequestTypeDef",
-    "ExportComponentsResponseTypeDef",
-    "ExportFormsRequestExportFormsPaginateTypeDef",
     "ExportFormsRequestRequestTypeDef",
-    "ExportFormsResponseTypeDef",
-    "ExportThemesRequestExportThemesPaginateTypeDef",
     "ExportThemesRequestRequestTypeDef",
-    "ExportThemesResponseTypeDef",
-    "FieldConfigOutputTypeDef",
-    "FieldConfigTypeDef",
-    "FieldInputConfigOutputTypeDef",
-    "FieldInputConfigTypeDef",
-    "FieldPositionOutputTypeDef",
     "FieldPositionTypeDef",
     "FieldValidationConfigurationOutputTypeDef",
     "FieldValidationConfigurationTypeDef",
     "FileUploaderFieldConfigOutputTypeDef",
     "FileUploaderFieldConfigTypeDef",
-    "FormBindingElementOutputTypeDef",
-    "FormBindingElementTypeDef",
-    "FormButtonOutputTypeDef",
-    "FormButtonTypeDef",
-    "FormCTAOutputTypeDef",
-    "FormCTATypeDef",
-    "FormDataTypeConfigOutputTypeDef",
-    "FormDataTypeConfigTypeDef",
-    "FormInputBindingPropertiesValueOutputTypeDef",
-    "FormInputBindingPropertiesValuePropertiesOutputTypeDef",
     "FormInputBindingPropertiesValuePropertiesTypeDef",
-    "FormInputBindingPropertiesValueTypeDef",
-    "FormInputValuePropertyBindingPropertiesOutputTypeDef",
     "FormInputValuePropertyBindingPropertiesTypeDef",
-    "FormInputValuePropertyOutputTypeDef",
-    "FormInputValuePropertyTypeDef",
-    "FormStyleConfigOutputTypeDef",
     "FormStyleConfigTypeDef",
-    "FormStyleOutputTypeDef",
-    "FormStyleTypeDef",
-    "FormSummaryTypeDef",
-    "FormTypeDef",
     "GetCodegenJobRequestRequestTypeDef",
-    "GetCodegenJobResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
-    "GetComponentResponseTypeDef",
     "GetFormRequestRequestTypeDef",
-    "GetFormResponseTypeDef",
     "GetMetadataRequestRequestTypeDef",
-    "GetMetadataResponseTypeDef",
     "GetThemeRequestRequestTypeDef",
-    "GetThemeResponseTypeDef",
-    "ListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
     "ListCodegenJobsRequestRequestTypeDef",
-    "ListCodegenJobsResponseTypeDef",
-    "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListComponentsRequestRequestTypeDef",
-    "ListComponentsResponseTypeDef",
-    "ListFormsRequestListFormsPaginateTypeDef",
     "ListFormsRequestRequestTypeDef",
-    "ListFormsResponseTypeDef",
-    "ListThemesRequestListThemesPaginateTypeDef",
     "ListThemesRequestRequestTypeDef",
-    "ListThemesResponseTypeDef",
-    "MutationActionSetStateParameterOutputTypeDef",
-    "MutationActionSetStateParameterTypeDef",
-    "PaginatorConfigTypeDef",
+    "ThemeSummaryTypeDef",
     "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "PutMetadataFlagBodyTypeDef",
-    "PutMetadataFlagRequestRequestTypeDef",
-    "ReactStartCodegenJobDataOutputTypeDef",
-    "ReactStartCodegenJobDataTypeDef",
     "RefreshTokenRequestBodyTypeDef",
-    "RefreshTokenRequestRequestTypeDef",
-    "RefreshTokenResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "SectionalElementOutputTypeDef",
-    "SectionalElementTypeDef",
-    "SortPropertyOutputTypeDef",
-    "SortPropertyTypeDef",
-    "StartCodegenJobDataTypeDef",
-    "StartCodegenJobRequestRequestTypeDef",
-    "StartCodegenJobResponseTypeDef",
-    "ThemeSummaryTypeDef",
-    "ThemeTypeDef",
     "ThemeValueOutputTypeDef",
     "ThemeValueTypeDef",
     "ThemeValuesOutputTypeDef",
     "ThemeValuesTypeDef",
-    "UpdateComponentDataTypeDef",
-    "UpdateComponentRequestRequestTypeDef",
-    "UpdateComponentResponseTypeDef",
-    "UpdateFormDataTypeDef",
-    "UpdateFormRequestRequestTypeDef",
-    "UpdateFormResponseTypeDef",
     "UpdateThemeDataTypeDef",
-    "UpdateThemeRequestRequestTypeDef",
-    "UpdateThemeResponseTypeDef",
-    "ValueMappingOutputTypeDef",
     "ValueMappingTypeDef",
-    "ValueMappingsOutputTypeDef",
-    "ValueMappingsTypeDef",
-)
-
-ActionParametersOutputTypeDef = TypedDict(
     "ActionParametersOutputTypeDef",
-    {
-        "type": "ComponentPropertyOutputTypeDef",
-        "url": "ComponentPropertyOutputTypeDef",
-        "anchor": "ComponentPropertyOutputTypeDef",
-        "target": "ComponentPropertyOutputTypeDef",
-        "global": "ComponentPropertyOutputTypeDef",
-        "model": str,
-        "id": "ComponentPropertyOutputTypeDef",
-        "fields": Dict[str, "ComponentPropertyOutputTypeDef"],
-        "state": "MutationActionSetStateParameterOutputTypeDef",
-    },
-    total=False,
-)
-
-ActionParametersTypeDef = TypedDict(
     "ActionParametersTypeDef",
-    {
-        "type": "ComponentPropertyTypeDef",
-        "url": "ComponentPropertyTypeDef",
-        "anchor": "ComponentPropertyTypeDef",
-        "target": "ComponentPropertyTypeDef",
-        "global": "ComponentPropertyTypeDef",
-        "model": str,
-        "id": "ComponentPropertyTypeDef",
-        "fields": Mapping[str, "ComponentPropertyTypeDef"],
-        "state": "MutationActionSetStateParameterTypeDef",
-    },
-    total=False,
+    "CodegenGenericDataFieldOutputTypeDef",
+    "CodegenGenericDataFieldTypeDef",
+    "CodegenJobRenderConfigTypeDef",
+    "ComponentBindingPropertiesValueOutputTypeDef",
+    "ComponentBindingPropertiesValueTypeDef",
+    "ComponentDataConfigurationOutputTypeDef",
+    "ComponentDataConfigurationTypeDef",
+    "ComponentPropertyOutputTypeDef",
+    "ComponentPropertyTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExchangeCodeForTokenResponseTypeDef",
+    "GetMetadataResponseTypeDef",
+    "ListCodegenJobsResponseTypeDef",
+    "ListComponentsResponseTypeDef",
+    "RefreshTokenResponseTypeDef",
+    "FormSummaryTypeDef",
+    "CreateThemeRequestRequestTypeDef",
+    "CreateThemeResponseTypeDef",
+    "ExportThemesResponseTypeDef",
+    "GetThemeResponseTypeDef",
+    "UpdateThemeResponseTypeDef",
+    "ExchangeCodeForTokenRequestRequestTypeDef",
+    "ExportComponentsRequestExportComponentsPaginateTypeDef",
+    "ExportFormsRequestExportFormsPaginateTypeDef",
+    "ExportThemesRequestExportThemesPaginateTypeDef",
+    "ListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+    "ListComponentsRequestListComponentsPaginateTypeDef",
+    "ListFormsRequestListFormsPaginateTypeDef",
+    "ListThemesRequestListThemesPaginateTypeDef",
+    "FormButtonTypeDef",
+    "SectionalElementTypeDef",
+    "FormInputBindingPropertiesValueTypeDef",
+    "FormInputValuePropertyTypeDef",
+    "FormStyleTypeDef",
+    "ListThemesResponseTypeDef",
+    "PutMetadataFlagRequestRequestTypeDef",
+    "RefreshTokenRequestRequestTypeDef",
+    "UpdateThemeRequestRequestTypeDef",
+    "ComponentEventOutputTypeDef",
+    "ComponentEventTypeDef",
+    "CodegenGenericDataModelOutputTypeDef",
+    "CodegenGenericDataNonModelOutputTypeDef",
+    "CodegenGenericDataModelTypeDef",
+    "CodegenGenericDataNonModelTypeDef",
+    "ListFormsResponseTypeDef",
+    "FormCTATypeDef",
+    "ValueMappingsOutputTypeDef",
+    "ValueMappingsTypeDef",
+    "ComponentChildOutputTypeDef",
+    "ComponentTypeDef",
+    "ComponentChildTypeDef",
+    "CreateComponentDataTypeDef",
+    "UpdateComponentDataTypeDef",
+    "CodegenJobGenericDataSchemaOutputTypeDef",
+    "CodegenJobGenericDataSchemaTypeDef",
+    "FieldInputConfigOutputTypeDef",
+    "FieldInputConfigTypeDef",
+    "CreateComponentResponseTypeDef",
+    "ExportComponentsResponseTypeDef",
+    "GetComponentResponseTypeDef",
+    "UpdateComponentResponseTypeDef",
+    "CreateComponentRequestRequestTypeDef",
+    "UpdateComponentRequestRequestTypeDef",
+    "CodegenJobTypeDef",
+    "StartCodegenJobDataTypeDef",
+    "FieldConfigOutputTypeDef",
+    "FieldConfigTypeDef",
+    "GetCodegenJobResponseTypeDef",
+    "StartCodegenJobResponseTypeDef",
+    "StartCodegenJobRequestRequestTypeDef",
+    "FormTypeDef",
+    "CreateFormDataTypeDef",
+    "UpdateFormDataTypeDef",
+    "CreateFormResponseTypeDef",
+    "ExportFormsResponseTypeDef",
+    "GetFormResponseTypeDef",
+    "UpdateFormResponseTypeDef",
+    "CreateFormRequestRequestTypeDef",
+    "UpdateFormRequestRequestTypeDef",
 )
 
-CodegenFeatureFlagsOutputTypeDef = TypedDict(
-    "CodegenFeatureFlagsOutputTypeDef",
+MutationActionSetStateParameterTypeDef = TypedDict(
+    "MutationActionSetStateParameterTypeDef",
     {
-        "isRelationshipSupported": bool,
-        "isNonModelSupported": bool,
+        "componentName": str,
+        "property": str,
+        "set": "ComponentPropertyTypeDef",
     },
-    total=False,
 )
 
 CodegenFeatureFlagsTypeDef = TypedDict(
     "CodegenFeatureFlagsTypeDef",
     {
         "isRelationshipSupported": bool,
         "isNonModelSupported": bool,
@@ -262,122 +210,14 @@
 CodegenGenericDataEnumTypeDef = TypedDict(
     "CodegenGenericDataEnumTypeDef",
     {
         "values": Sequence[str],
     },
 )
 
-_RequiredCodegenGenericDataFieldOutputTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataFieldOutputTypeDef",
-    {
-        "dataType": CodegenGenericDataFieldDataTypeType,
-        "dataTypeValue": str,
-        "required": bool,
-        "readOnly": bool,
-        "isArray": bool,
-    },
-)
-_OptionalCodegenGenericDataFieldOutputTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataFieldOutputTypeDef",
-    {
-        "relationship": "CodegenGenericDataRelationshipTypeOutputTypeDef",
-    },
-    total=False,
-)
-
-
-class CodegenGenericDataFieldOutputTypeDef(
-    _RequiredCodegenGenericDataFieldOutputTypeDef, _OptionalCodegenGenericDataFieldOutputTypeDef
-):
-    pass
-
-
-_RequiredCodegenGenericDataFieldTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataFieldTypeDef",
-    {
-        "dataType": CodegenGenericDataFieldDataTypeType,
-        "dataTypeValue": str,
-        "required": bool,
-        "readOnly": bool,
-        "isArray": bool,
-    },
-)
-_OptionalCodegenGenericDataFieldTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataFieldTypeDef",
-    {
-        "relationship": "CodegenGenericDataRelationshipTypeTypeDef",
-    },
-    total=False,
-)
-
-
-class CodegenGenericDataFieldTypeDef(
-    _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
-):
-    pass
-
-
-_RequiredCodegenGenericDataModelOutputTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataModelOutputTypeDef",
-    {
-        "fields": Dict[str, "CodegenGenericDataFieldOutputTypeDef"],
-        "primaryKeys": List[str],
-    },
-)
-_OptionalCodegenGenericDataModelOutputTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataModelOutputTypeDef",
-    {
-        "isJoinTable": bool,
-    },
-    total=False,
-)
-
-
-class CodegenGenericDataModelOutputTypeDef(
-    _RequiredCodegenGenericDataModelOutputTypeDef, _OptionalCodegenGenericDataModelOutputTypeDef
-):
-    pass
-
-
-_RequiredCodegenGenericDataModelTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataModelTypeDef",
-    {
-        "fields": Mapping[str, "CodegenGenericDataFieldTypeDef"],
-        "primaryKeys": Sequence[str],
-    },
-)
-_OptionalCodegenGenericDataModelTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataModelTypeDef",
-    {
-        "isJoinTable": bool,
-    },
-    total=False,
-)
-
-
-class CodegenGenericDataModelTypeDef(
-    _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
-):
-    pass
-
-
-CodegenGenericDataNonModelOutputTypeDef = TypedDict(
-    "CodegenGenericDataNonModelOutputTypeDef",
-    {
-        "fields": Dict[str, "CodegenGenericDataFieldOutputTypeDef"],
-    },
-)
-
-CodegenGenericDataNonModelTypeDef = TypedDict(
-    "CodegenGenericDataNonModelTypeDef",
-    {
-        "fields": Mapping[str, "CodegenGenericDataFieldTypeDef"],
-    },
-)
-
 _RequiredCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
     "_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef",
     {
         "type": GenericDataRelationshipTypeType,
         "relatedModelName": str,
     },
 )
@@ -436,46 +276,22 @@
     "CodegenJobAssetTypeDef",
     {
         "downloadUrl": str,
     },
     total=False,
 )
 
-CodegenJobGenericDataSchemaOutputTypeDef = TypedDict(
-    "CodegenJobGenericDataSchemaOutputTypeDef",
-    {
-        "dataSourceType": Literal["DataStore"],
-        "models": Dict[str, "CodegenGenericDataModelOutputTypeDef"],
-        "enums": Dict[str, "CodegenGenericDataEnumOutputTypeDef"],
-        "nonModels": Dict[str, "CodegenGenericDataNonModelOutputTypeDef"],
-    },
-)
-
-CodegenJobGenericDataSchemaTypeDef = TypedDict(
-    "CodegenJobGenericDataSchemaTypeDef",
-    {
-        "dataSourceType": Literal["DataStore"],
-        "models": Mapping[str, "CodegenGenericDataModelTypeDef"],
-        "enums": Mapping[str, "CodegenGenericDataEnumTypeDef"],
-        "nonModels": Mapping[str, "CodegenGenericDataNonModelTypeDef"],
-    },
-)
-
-CodegenJobRenderConfigOutputTypeDef = TypedDict(
-    "CodegenJobRenderConfigOutputTypeDef",
-    {
-        "react": "ReactStartCodegenJobDataOutputTypeDef",
-    },
-    total=False,
-)
-
-CodegenJobRenderConfigTypeDef = TypedDict(
-    "CodegenJobRenderConfigTypeDef",
+ReactStartCodegenJobDataTypeDef = TypedDict(
+    "ReactStartCodegenJobDataTypeDef",
     {
-        "react": "ReactStartCodegenJobDataTypeDef",
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
     },
     total=False,
 )
 
 _RequiredCodegenJobSummaryTypeDef = TypedDict(
     "_RequiredCodegenJobSummaryTypeDef",
     {
@@ -496,54 +312,14 @@
 
 class CodegenJobSummaryTypeDef(
     _RequiredCodegenJobSummaryTypeDef, _OptionalCodegenJobSummaryTypeDef
 ):
     pass
 
 
-_RequiredCodegenJobTypeDef = TypedDict(
-    "_RequiredCodegenJobTypeDef",
-    {
-        "id": str,
-        "appId": str,
-        "environmentName": str,
-    },
-)
-_OptionalCodegenJobTypeDef = TypedDict(
-    "_OptionalCodegenJobTypeDef",
-    {
-        "renderConfig": "CodegenJobRenderConfigOutputTypeDef",
-        "genericDataSchema": "CodegenJobGenericDataSchemaOutputTypeDef",
-        "autoGenerateForms": bool,
-        "features": "CodegenFeatureFlagsOutputTypeDef",
-        "status": CodegenJobStatusType,
-        "statusMessage": str,
-        "asset": "CodegenJobAssetTypeDef",
-        "tags": Dict[str, str],
-        "createdAt": datetime,
-        "modifiedAt": datetime,
-    },
-    total=False,
-)
-
-
-class CodegenJobTypeDef(_RequiredCodegenJobTypeDef, _OptionalCodegenJobTypeDef):
-    pass
-
-
-ComponentBindingPropertiesValueOutputTypeDef = TypedDict(
-    "ComponentBindingPropertiesValueOutputTypeDef",
-    {
-        "type": str,
-        "bindingProperties": "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
-        "defaultValue": str,
-    },
-    total=False,
-)
-
 ComponentBindingPropertiesValuePropertiesOutputTypeDef = TypedDict(
     "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     {
         "model": str,
         "field": str,
         "predicates": List["PredicateOutputTypeDef"],
         "userAttribute": str,
@@ -566,1852 +342,1732 @@
         "key": str,
         "defaultValue": str,
         "slotName": str,
     },
     total=False,
 )
 
-ComponentBindingPropertiesValueTypeDef = TypedDict(
-    "ComponentBindingPropertiesValueTypeDef",
+ComponentConditionPropertyTypeDef = TypedDict(
+    "ComponentConditionPropertyTypeDef",
     {
-        "type": str,
-        "bindingProperties": "ComponentBindingPropertiesValuePropertiesTypeDef",
-        "defaultValue": str,
+        "property": str,
+        "field": str,
+        "operator": str,
+        "operand": str,
+        "then": "ComponentPropertyTypeDef",
+        "else": "ComponentPropertyTypeDef",
+        "operandType": str,
     },
     total=False,
 )
 
-_RequiredComponentChildOutputTypeDef = TypedDict(
-    "_RequiredComponentChildOutputTypeDef",
-    {
-        "componentType": str,
-        "name": str,
-        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
-    },
-)
-_OptionalComponentChildOutputTypeDef = TypedDict(
-    "_OptionalComponentChildOutputTypeDef",
+SortPropertyTypeDef = TypedDict(
+    "SortPropertyTypeDef",
     {
-        "children": List[Dict[str, Any]],
-        "events": Dict[str, "ComponentEventOutputTypeDef"],
-        "sourceId": str,
+        "field": str,
+        "direction": SortDirectionType,
     },
-    total=False,
 )
 
-
-class ComponentChildOutputTypeDef(
-    _RequiredComponentChildOutputTypeDef, _OptionalComponentChildOutputTypeDef
-):
-    pass
-
-
-_RequiredComponentChildTypeDef = TypedDict(
-    "_RequiredComponentChildTypeDef",
+_RequiredComponentPropertyBindingPropertiesTypeDef = TypedDict(
+    "_RequiredComponentPropertyBindingPropertiesTypeDef",
     {
-        "componentType": str,
-        "name": str,
-        "properties": Mapping[str, "ComponentPropertyTypeDef"],
+        "property": str,
     },
 )
-_OptionalComponentChildTypeDef = TypedDict(
-    "_OptionalComponentChildTypeDef",
+_OptionalComponentPropertyBindingPropertiesTypeDef = TypedDict(
+    "_OptionalComponentPropertyBindingPropertiesTypeDef",
     {
-        "children": Sequence[Dict[str, Any]],
-        "events": Mapping[str, "ComponentEventTypeDef"],
-        "sourceId": str,
+        "field": str,
     },
     total=False,
 )
 
 
-class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
+class ComponentPropertyBindingPropertiesTypeDef(
+    _RequiredComponentPropertyBindingPropertiesTypeDef,
+    _OptionalComponentPropertyBindingPropertiesTypeDef,
+):
     pass
 
 
-ComponentConditionPropertyOutputTypeDef = TypedDict(
-    "ComponentConditionPropertyOutputTypeDef",
+FormBindingElementTypeDef = TypedDict(
+    "FormBindingElementTypeDef",
     {
+        "element": str,
         "property": str,
-        "field": str,
-        "operator": str,
-        "operand": str,
-        "then": Dict[str, Any],
-        "else": Dict[str, Any],
-        "operandType": str,
     },
-    total=False,
 )
 
-ComponentConditionPropertyTypeDef = TypedDict(
-    "ComponentConditionPropertyTypeDef",
+ComponentSummaryTypeDef = TypedDict(
+    "ComponentSummaryTypeDef",
     {
-        "property": str,
-        "field": str,
-        "operator": str,
-        "operand": str,
-        "then": Dict[str, Any],
-        "else": Dict[str, Any],
-        "operandType": str,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "name": str,
+        "componentType": str,
     },
-    total=False,
 )
 
-_RequiredComponentDataConfigurationOutputTypeDef = TypedDict(
-    "_RequiredComponentDataConfigurationOutputTypeDef",
-    {
-        "model": str,
-    },
-)
-_OptionalComponentDataConfigurationOutputTypeDef = TypedDict(
-    "_OptionalComponentDataConfigurationOutputTypeDef",
+ComponentVariantOutputTypeDef = TypedDict(
+    "ComponentVariantOutputTypeDef",
     {
-        "sort": List["SortPropertyOutputTypeDef"],
-        "predicate": "PredicateOutputTypeDef",
-        "identifiers": List[str],
+        "variantValues": Dict[str, str],
+        "overrides": Dict[str, Dict[str, str]],
     },
     total=False,
 )
 
-
-class ComponentDataConfigurationOutputTypeDef(
-    _RequiredComponentDataConfigurationOutputTypeDef,
-    _OptionalComponentDataConfigurationOutputTypeDef,
-):
-    pass
-
-
-_RequiredComponentDataConfigurationTypeDef = TypedDict(
-    "_RequiredComponentDataConfigurationTypeDef",
-    {
-        "model": str,
-    },
-)
-_OptionalComponentDataConfigurationTypeDef = TypedDict(
-    "_OptionalComponentDataConfigurationTypeDef",
+ComponentVariantTypeDef = TypedDict(
+    "ComponentVariantTypeDef",
     {
-        "sort": Sequence["SortPropertyTypeDef"],
-        "predicate": "PredicateTypeDef",
-        "identifiers": Sequence[str],
+        "variantValues": Mapping[str, str],
+        "overrides": Mapping[str, Mapping[str, str]],
     },
     total=False,
 )
 
-
-class ComponentDataConfigurationTypeDef(
-    _RequiredComponentDataConfigurationTypeDef, _OptionalComponentDataConfigurationTypeDef
-):
-    pass
-
-
-ComponentEventOutputTypeDef = TypedDict(
-    "ComponentEventOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "action": str,
-        "parameters": "ActionParametersOutputTypeDef",
-        "bindingEvent": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-ComponentEventTypeDef = TypedDict(
-    "ComponentEventTypeDef",
+FormDataTypeConfigTypeDef = TypedDict(
+    "FormDataTypeConfigTypeDef",
     {
-        "action": str,
-        "parameters": "ActionParametersTypeDef",
-        "bindingEvent": str,
+        "dataSourceType": FormDataSourceTypeType,
+        "dataTypeName": str,
     },
-    total=False,
 )
 
-_RequiredComponentPropertyBindingPropertiesOutputTypeDef = TypedDict(
-    "_RequiredComponentPropertyBindingPropertiesOutputTypeDef",
+_RequiredCreateThemeDataTypeDef = TypedDict(
+    "_RequiredCreateThemeDataTypeDef",
     {
-        "property": str,
+        "name": str,
+        "values": Sequence["ThemeValuesTypeDef"],
     },
 )
-_OptionalComponentPropertyBindingPropertiesOutputTypeDef = TypedDict(
-    "_OptionalComponentPropertyBindingPropertiesOutputTypeDef",
+_OptionalCreateThemeDataTypeDef = TypedDict(
+    "_OptionalCreateThemeDataTypeDef",
     {
-        "field": str,
+        "overrides": Sequence["ThemeValuesTypeDef"],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class ComponentPropertyBindingPropertiesOutputTypeDef(
-    _RequiredComponentPropertyBindingPropertiesOutputTypeDef,
-    _OptionalComponentPropertyBindingPropertiesOutputTypeDef,
-):
+class CreateThemeDataTypeDef(_RequiredCreateThemeDataTypeDef, _OptionalCreateThemeDataTypeDef):
     pass
 
 
-_RequiredComponentPropertyBindingPropertiesTypeDef = TypedDict(
-    "_RequiredComponentPropertyBindingPropertiesTypeDef",
+_RequiredThemeTypeDef = TypedDict(
+    "_RequiredThemeTypeDef",
     {
-        "property": str,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "name": str,
+        "createdAt": datetime,
+        "values": List["ThemeValuesOutputTypeDef"],
     },
 )
-_OptionalComponentPropertyBindingPropertiesTypeDef = TypedDict(
-    "_OptionalComponentPropertyBindingPropertiesTypeDef",
+_OptionalThemeTypeDef = TypedDict(
+    "_OptionalThemeTypeDef",
     {
-        "field": str,
+        "modifiedAt": datetime,
+        "overrides": List["ThemeValuesOutputTypeDef"],
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class ComponentPropertyBindingPropertiesTypeDef(
-    _RequiredComponentPropertyBindingPropertiesTypeDef,
-    _OptionalComponentPropertyBindingPropertiesTypeDef,
-):
+class ThemeTypeDef(_RequiredThemeTypeDef, _OptionalThemeTypeDef):
     pass
 
 
-ComponentPropertyOutputTypeDef = TypedDict(
-    "ComponentPropertyOutputTypeDef",
+DeleteComponentRequestRequestTypeDef = TypedDict(
+    "DeleteComponentRequestRequestTypeDef",
     {
-        "value": str,
-        "bindingProperties": "ComponentPropertyBindingPropertiesOutputTypeDef",
-        "collectionBindingProperties": "ComponentPropertyBindingPropertiesOutputTypeDef",
-        "defaultValue": str,
-        "model": str,
-        "bindings": Dict[str, "FormBindingElementOutputTypeDef"],
-        "event": str,
-        "userAttribute": str,
-        "concat": List[Dict[str, Any]],
-        "condition": Dict[str, Any],
-        "configured": bool,
-        "type": str,
-        "importedValue": str,
-        "componentName": str,
-        "property": str,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
-    total=False,
 )
 
-ComponentPropertyTypeDef = TypedDict(
-    "ComponentPropertyTypeDef",
+DeleteFormRequestRequestTypeDef = TypedDict(
+    "DeleteFormRequestRequestTypeDef",
     {
-        "value": str,
-        "bindingProperties": "ComponentPropertyBindingPropertiesTypeDef",
-        "collectionBindingProperties": "ComponentPropertyBindingPropertiesTypeDef",
-        "defaultValue": str,
-        "model": str,
-        "bindings": Mapping[str, "FormBindingElementTypeDef"],
-        "event": str,
-        "userAttribute": str,
-        "concat": Sequence[Dict[str, Any]],
-        "condition": Dict[str, Any],
-        "configured": bool,
-        "type": str,
-        "importedValue": str,
-        "componentName": str,
-        "property": str,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
-    total=False,
 )
 
-ComponentSummaryTypeDef = TypedDict(
-    "ComponentSummaryTypeDef",
+DeleteThemeRequestRequestTypeDef = TypedDict(
+    "DeleteThemeRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
-        "name": str,
-        "componentType": str,
     },
 )
 
-_RequiredComponentTypeDef = TypedDict(
-    "_RequiredComponentTypeDef",
+_RequiredExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
+    "_RequiredExchangeCodeForTokenRequestBodyTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "name": str,
-        "componentType": str,
-        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
-        "variants": List["ComponentVariantOutputTypeDef"],
-        "overrides": Dict[str, Dict[str, str]],
-        "bindingProperties": Dict[str, "ComponentBindingPropertiesValueOutputTypeDef"],
-        "createdAt": datetime,
+        "code": str,
+        "redirectUri": str,
     },
 )
-_OptionalComponentTypeDef = TypedDict(
-    "_OptionalComponentTypeDef",
+_OptionalExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
+    "_OptionalExchangeCodeForTokenRequestBodyTypeDef",
     {
-        "sourceId": str,
-        "children": List["ComponentChildOutputTypeDef"],
-        "collectionProperties": Dict[str, "ComponentDataConfigurationOutputTypeDef"],
-        "modifiedAt": datetime,
-        "tags": Dict[str, str],
-        "events": Dict[str, "ComponentEventOutputTypeDef"],
-        "schemaVersion": str,
+        "clientId": str,
     },
     total=False,
 )
 
 
-class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
+class ExchangeCodeForTokenRequestBodyTypeDef(
+    _RequiredExchangeCodeForTokenRequestBodyTypeDef, _OptionalExchangeCodeForTokenRequestBodyTypeDef
+):
     pass
 
 
-ComponentVariantOutputTypeDef = TypedDict(
-    "ComponentVariantOutputTypeDef",
-    {
-        "variantValues": Dict[str, str],
-        "overrides": Dict[str, Dict[str, str]],
-    },
-    total=False,
-)
-
-ComponentVariantTypeDef = TypedDict(
-    "ComponentVariantTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "variantValues": Mapping[str, str],
-        "overrides": Mapping[str, Mapping[str, str]],
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredCreateComponentDataTypeDef = TypedDict(
-    "_RequiredCreateComponentDataTypeDef",
+_RequiredExportComponentsRequestRequestTypeDef = TypedDict(
+    "_RequiredExportComponentsRequestRequestTypeDef",
     {
-        "name": str,
-        "componentType": str,
-        "properties": Mapping[str, "ComponentPropertyTypeDef"],
-        "variants": Sequence["ComponentVariantTypeDef"],
-        "overrides": Mapping[str, Mapping[str, str]],
-        "bindingProperties": Mapping[str, "ComponentBindingPropertiesValueTypeDef"],
+        "appId": str,
+        "environmentName": str,
     },
 )
-_OptionalCreateComponentDataTypeDef = TypedDict(
-    "_OptionalCreateComponentDataTypeDef",
+_OptionalExportComponentsRequestRequestTypeDef = TypedDict(
+    "_OptionalExportComponentsRequestRequestTypeDef",
     {
-        "sourceId": str,
-        "children": Sequence["ComponentChildTypeDef"],
-        "collectionProperties": Mapping[str, "ComponentDataConfigurationTypeDef"],
-        "tags": Mapping[str, str],
-        "events": Mapping[str, "ComponentEventTypeDef"],
-        "schemaVersion": str,
+        "nextToken": str,
     },
     total=False,
 )
 
 
-class CreateComponentDataTypeDef(
-    _RequiredCreateComponentDataTypeDef, _OptionalCreateComponentDataTypeDef
+class ExportComponentsRequestRequestTypeDef(
+    _RequiredExportComponentsRequestRequestTypeDef, _OptionalExportComponentsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredCreateComponentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateComponentRequestRequestTypeDef",
+_RequiredExportFormsRequestRequestTypeDef = TypedDict(
+    "_RequiredExportFormsRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
-        "componentToCreate": "CreateComponentDataTypeDef",
     },
 )
-_OptionalCreateComponentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateComponentRequestRequestTypeDef",
+_OptionalExportFormsRequestRequestTypeDef = TypedDict(
+    "_OptionalExportFormsRequestRequestTypeDef",
     {
-        "clientToken": str,
+        "nextToken": str,
     },
     total=False,
 )
 
 
-class CreateComponentRequestRequestTypeDef(
-    _RequiredCreateComponentRequestRequestTypeDef, _OptionalCreateComponentRequestRequestTypeDef
+class ExportFormsRequestRequestTypeDef(
+    _RequiredExportFormsRequestRequestTypeDef, _OptionalExportFormsRequestRequestTypeDef
 ):
     pass
 
 
-CreateComponentResponseTypeDef = TypedDict(
-    "CreateComponentResponseTypeDef",
-    {
-        "entity": "ComponentTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateFormDataTypeDef = TypedDict(
-    "_RequiredCreateFormDataTypeDef",
+_RequiredExportThemesRequestRequestTypeDef = TypedDict(
+    "_RequiredExportThemesRequestRequestTypeDef",
     {
-        "name": str,
-        "dataType": "FormDataTypeConfigTypeDef",
-        "formActionType": FormActionTypeType,
-        "fields": Mapping[str, "FieldConfigTypeDef"],
-        "style": "FormStyleTypeDef",
-        "sectionalElements": Mapping[str, "SectionalElementTypeDef"],
-        "schemaVersion": str,
+        "appId": str,
+        "environmentName": str,
     },
 )
-_OptionalCreateFormDataTypeDef = TypedDict(
-    "_OptionalCreateFormDataTypeDef",
+_OptionalExportThemesRequestRequestTypeDef = TypedDict(
+    "_OptionalExportThemesRequestRequestTypeDef",
     {
-        "cta": "FormCTATypeDef",
-        "tags": Mapping[str, str],
-        "labelDecorator": LabelDecoratorType,
+        "nextToken": str,
     },
     total=False,
 )
 
 
-class CreateFormDataTypeDef(_RequiredCreateFormDataTypeDef, _OptionalCreateFormDataTypeDef):
+class ExportThemesRequestRequestTypeDef(
+    _RequiredExportThemesRequestRequestTypeDef, _OptionalExportThemesRequestRequestTypeDef
+):
     pass
 
 
-_RequiredCreateFormRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFormRequestRequestTypeDef",
+FieldPositionTypeDef = TypedDict(
+    "FieldPositionTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "formToCreate": "CreateFormDataTypeDef",
+        "fixed": Literal["first"],
+        "rightOf": str,
+        "below": str,
     },
+    total=False,
 )
-_OptionalCreateFormRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFormRequestRequestTypeDef",
+
+_RequiredFieldValidationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFieldValidationConfigurationOutputTypeDef",
     {
-        "clientToken": str,
+        "type": str,
+    },
+)
+_OptionalFieldValidationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFieldValidationConfigurationOutputTypeDef",
+    {
+        "strValues": List[str],
+        "numValues": List[int],
+        "validationMessage": str,
     },
     total=False,
 )
 
 
-class CreateFormRequestRequestTypeDef(
-    _RequiredCreateFormRequestRequestTypeDef, _OptionalCreateFormRequestRequestTypeDef
+class FieldValidationConfigurationOutputTypeDef(
+    _RequiredFieldValidationConfigurationOutputTypeDef,
+    _OptionalFieldValidationConfigurationOutputTypeDef,
 ):
     pass
 
 
-CreateFormResponseTypeDef = TypedDict(
-    "CreateFormResponseTypeDef",
-    {
-        "entity": "FormTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateThemeDataTypeDef = TypedDict(
-    "_RequiredCreateThemeDataTypeDef",
+_RequiredFieldValidationConfigurationTypeDef = TypedDict(
+    "_RequiredFieldValidationConfigurationTypeDef",
     {
-        "name": str,
-        "values": Sequence["ThemeValuesTypeDef"],
+        "type": str,
     },
 )
-_OptionalCreateThemeDataTypeDef = TypedDict(
-    "_OptionalCreateThemeDataTypeDef",
+_OptionalFieldValidationConfigurationTypeDef = TypedDict(
+    "_OptionalFieldValidationConfigurationTypeDef",
     {
-        "overrides": Sequence["ThemeValuesTypeDef"],
-        "tags": Mapping[str, str],
+        "strValues": Sequence[str],
+        "numValues": Sequence[int],
+        "validationMessage": str,
     },
     total=False,
 )
 
 
-class CreateThemeDataTypeDef(_RequiredCreateThemeDataTypeDef, _OptionalCreateThemeDataTypeDef):
+class FieldValidationConfigurationTypeDef(
+    _RequiredFieldValidationConfigurationTypeDef, _OptionalFieldValidationConfigurationTypeDef
+):
     pass
 
 
-_RequiredCreateThemeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateThemeRequestRequestTypeDef",
+_RequiredFileUploaderFieldConfigOutputTypeDef = TypedDict(
+    "_RequiredFileUploaderFieldConfigOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "themeToCreate": "CreateThemeDataTypeDef",
+        "accessLevel": StorageAccessLevelType,
+        "acceptedFileTypes": List[str],
     },
 )
-_OptionalCreateThemeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateThemeRequestRequestTypeDef",
+_OptionalFileUploaderFieldConfigOutputTypeDef = TypedDict(
+    "_OptionalFileUploaderFieldConfigOutputTypeDef",
     {
-        "clientToken": str,
+        "showThumbnails": bool,
+        "isResumable": bool,
+        "maxFileCount": int,
+        "maxSize": int,
     },
     total=False,
 )
 
 
-class CreateThemeRequestRequestTypeDef(
-    _RequiredCreateThemeRequestRequestTypeDef, _OptionalCreateThemeRequestRequestTypeDef
+class FileUploaderFieldConfigOutputTypeDef(
+    _RequiredFileUploaderFieldConfigOutputTypeDef, _OptionalFileUploaderFieldConfigOutputTypeDef
 ):
     pass
 
 
-CreateThemeResponseTypeDef = TypedDict(
-    "CreateThemeResponseTypeDef",
+_RequiredFileUploaderFieldConfigTypeDef = TypedDict(
+    "_RequiredFileUploaderFieldConfigTypeDef",
     {
-        "entity": "ThemeTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "accessLevel": StorageAccessLevelType,
+        "acceptedFileTypes": Sequence[str],
     },
 )
-
-DeleteComponentRequestRequestTypeDef = TypedDict(
-    "DeleteComponentRequestRequestTypeDef",
+_OptionalFileUploaderFieldConfigTypeDef = TypedDict(
+    "_OptionalFileUploaderFieldConfigTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "showThumbnails": bool,
+        "isResumable": bool,
+        "maxFileCount": int,
+        "maxSize": int,
     },
+    total=False,
 )
 
-DeleteFormRequestRequestTypeDef = TypedDict(
-    "DeleteFormRequestRequestTypeDef",
-    {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-    },
-)
 
-DeleteThemeRequestRequestTypeDef = TypedDict(
-    "DeleteThemeRequestRequestTypeDef",
-    {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-    },
-)
+class FileUploaderFieldConfigTypeDef(
+    _RequiredFileUploaderFieldConfigTypeDef, _OptionalFileUploaderFieldConfigTypeDef
+):
+    pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+
+FormInputBindingPropertiesValuePropertiesTypeDef = TypedDict(
+    "FormInputBindingPropertiesValuePropertiesTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "model": str,
     },
+    total=False,
 )
 
-_RequiredExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
-    "_RequiredExchangeCodeForTokenRequestBodyTypeDef",
+_RequiredFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
+    "_RequiredFormInputValuePropertyBindingPropertiesTypeDef",
     {
-        "code": str,
-        "redirectUri": str,
+        "property": str,
     },
 )
-_OptionalExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
-    "_OptionalExchangeCodeForTokenRequestBodyTypeDef",
+_OptionalFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
+    "_OptionalFormInputValuePropertyBindingPropertiesTypeDef",
     {
-        "clientId": str,
+        "field": str,
     },
     total=False,
 )
 
 
-class ExchangeCodeForTokenRequestBodyTypeDef(
-    _RequiredExchangeCodeForTokenRequestBodyTypeDef, _OptionalExchangeCodeForTokenRequestBodyTypeDef
+class FormInputValuePropertyBindingPropertiesTypeDef(
+    _RequiredFormInputValuePropertyBindingPropertiesTypeDef,
+    _OptionalFormInputValuePropertyBindingPropertiesTypeDef,
 ):
     pass
 
 
-ExchangeCodeForTokenRequestRequestTypeDef = TypedDict(
-    "ExchangeCodeForTokenRequestRequestTypeDef",
+FormStyleConfigTypeDef = TypedDict(
+    "FormStyleConfigTypeDef",
     {
-        "provider": Literal["figma"],
-        "request": "ExchangeCodeForTokenRequestBodyTypeDef",
+        "tokenReference": str,
+        "value": str,
     },
+    total=False,
 )
 
-ExchangeCodeForTokenResponseTypeDef = TypedDict(
-    "ExchangeCodeForTokenResponseTypeDef",
+GetCodegenJobRequestRequestTypeDef = TypedDict(
+    "GetCodegenJobRequestRequestTypeDef",
     {
-        "accessToken": str,
-        "expiresIn": int,
-        "refreshToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
 )
 
-_RequiredExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
-    "_RequiredExportComponentsRequestExportComponentsPaginateTypeDef",
+GetComponentRequestRequestTypeDef = TypedDict(
+    "GetComponentRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
+        "id": str,
     },
 )
-_OptionalExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
-    "_OptionalExportComponentsRequestExportComponentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
-
-class ExportComponentsRequestExportComponentsPaginateTypeDef(
-    _RequiredExportComponentsRequestExportComponentsPaginateTypeDef,
-    _OptionalExportComponentsRequestExportComponentsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredExportComponentsRequestRequestTypeDef = TypedDict(
-    "_RequiredExportComponentsRequestRequestTypeDef",
+GetFormRequestRequestTypeDef = TypedDict(
+    "GetFormRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
+        "id": str,
     },
 )
-_OptionalExportComponentsRequestRequestTypeDef = TypedDict(
-    "_OptionalExportComponentsRequestRequestTypeDef",
+
+GetMetadataRequestRequestTypeDef = TypedDict(
+    "GetMetadataRequestRequestTypeDef",
     {
-        "nextToken": str,
+        "appId": str,
+        "environmentName": str,
     },
-    total=False,
 )
 
-
-class ExportComponentsRequestRequestTypeDef(
-    _RequiredExportComponentsRequestRequestTypeDef, _OptionalExportComponentsRequestRequestTypeDef
-):
-    pass
-
-
-ExportComponentsResponseTypeDef = TypedDict(
-    "ExportComponentsResponseTypeDef",
+GetThemeRequestRequestTypeDef = TypedDict(
+    "GetThemeRequestRequestTypeDef",
     {
-        "entities": List["ComponentTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
 )
 
-_RequiredExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
-    "_RequiredExportFormsRequestExportFormsPaginateTypeDef",
+_RequiredListCodegenJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListCodegenJobsRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
-    "_OptionalExportFormsRequestExportFormsPaginateTypeDef",
+_OptionalListCodegenJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListCodegenJobsRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 
-class ExportFormsRequestExportFormsPaginateTypeDef(
-    _RequiredExportFormsRequestExportFormsPaginateTypeDef,
-    _OptionalExportFormsRequestExportFormsPaginateTypeDef,
+class ListCodegenJobsRequestRequestTypeDef(
+    _RequiredListCodegenJobsRequestRequestTypeDef, _OptionalListCodegenJobsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredExportFormsRequestRequestTypeDef = TypedDict(
-    "_RequiredExportFormsRequestRequestTypeDef",
+_RequiredListComponentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListComponentsRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalExportFormsRequestRequestTypeDef = TypedDict(
-    "_OptionalExportFormsRequestRequestTypeDef",
+_OptionalListComponentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListComponentsRequestRequestTypeDef",
     {
         "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 
-class ExportFormsRequestRequestTypeDef(
-    _RequiredExportFormsRequestRequestTypeDef, _OptionalExportFormsRequestRequestTypeDef
+class ListComponentsRequestRequestTypeDef(
+    _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
 ):
     pass
 
 
-ExportFormsResponseTypeDef = TypedDict(
-    "ExportFormsResponseTypeDef",
-    {
-        "entities": List["FormTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
-    "_RequiredExportThemesRequestExportThemesPaginateTypeDef",
+_RequiredListFormsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFormsRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
-    "_OptionalExportThemesRequestExportThemesPaginateTypeDef",
+_OptionalListFormsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFormsRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 
-class ExportThemesRequestExportThemesPaginateTypeDef(
-    _RequiredExportThemesRequestExportThemesPaginateTypeDef,
-    _OptionalExportThemesRequestExportThemesPaginateTypeDef,
+class ListFormsRequestRequestTypeDef(
+    _RequiredListFormsRequestRequestTypeDef, _OptionalListFormsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredExportThemesRequestRequestTypeDef = TypedDict(
-    "_RequiredExportThemesRequestRequestTypeDef",
+_RequiredListThemesRequestRequestTypeDef = TypedDict(
+    "_RequiredListThemesRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalExportThemesRequestRequestTypeDef = TypedDict(
-    "_OptionalExportThemesRequestRequestTypeDef",
+_OptionalListThemesRequestRequestTypeDef = TypedDict(
+    "_OptionalListThemesRequestRequestTypeDef",
     {
         "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 
-class ExportThemesRequestRequestTypeDef(
-    _RequiredExportThemesRequestRequestTypeDef, _OptionalExportThemesRequestRequestTypeDef
+class ListThemesRequestRequestTypeDef(
+    _RequiredListThemesRequestRequestTypeDef, _OptionalListThemesRequestRequestTypeDef
 ):
     pass
 
 
-ExportThemesResponseTypeDef = TypedDict(
-    "ExportThemesResponseTypeDef",
+ThemeSummaryTypeDef = TypedDict(
+    "ThemeSummaryTypeDef",
     {
-        "entities": List["ThemeTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "name": str,
     },
 )
 
-FieldConfigOutputTypeDef = TypedDict(
-    "FieldConfigOutputTypeDef",
+PredicateOutputTypeDef = TypedDict(
+    "PredicateOutputTypeDef",
     {
-        "label": str,
-        "position": "FieldPositionOutputTypeDef",
-        "excluded": bool,
-        "inputType": "FieldInputConfigOutputTypeDef",
-        "validations": List["FieldValidationConfigurationOutputTypeDef"],
+        "or": List[Dict[str, Any]],
+        "and": List[Dict[str, Any]],
+        "field": str,
+        "operator": str,
+        "operand": str,
+        "operandType": str,
     },
     total=False,
 )
 
-FieldConfigTypeDef = TypedDict(
-    "FieldConfigTypeDef",
+PredicateTypeDef = TypedDict(
+    "PredicateTypeDef",
     {
-        "label": str,
-        "position": "FieldPositionTypeDef",
-        "excluded": bool,
-        "inputType": "FieldInputConfigTypeDef",
-        "validations": Sequence["FieldValidationConfigurationTypeDef"],
+        "or": Sequence[Dict[str, Any]],
+        "and": Sequence[Dict[str, Any]],
+        "field": str,
+        "operator": str,
+        "operand": str,
+        "operandType": str,
     },
     total=False,
 )
 
-_RequiredFieldInputConfigOutputTypeDef = TypedDict(
-    "_RequiredFieldInputConfigOutputTypeDef",
+PutMetadataFlagBodyTypeDef = TypedDict(
+    "PutMetadataFlagBodyTypeDef",
     {
-        "type": str,
+        "newValue": str,
     },
 )
-_OptionalFieldInputConfigOutputTypeDef = TypedDict(
-    "_OptionalFieldInputConfigOutputTypeDef",
+
+_RequiredRefreshTokenRequestBodyTypeDef = TypedDict(
+    "_RequiredRefreshTokenRequestBodyTypeDef",
     {
-        "required": bool,
-        "readOnly": bool,
-        "placeholder": str,
-        "defaultValue": str,
-        "descriptiveText": str,
-        "defaultChecked": bool,
-        "defaultCountryCode": str,
-        "valueMappings": "ValueMappingsOutputTypeDef",
-        "name": str,
-        "minValue": float,
-        "maxValue": float,
-        "step": float,
-        "value": str,
-        "isArray": bool,
-        "fileUploaderConfig": "FileUploaderFieldConfigOutputTypeDef",
+        "token": str,
+    },
+)
+_OptionalRefreshTokenRequestBodyTypeDef = TypedDict(
+    "_OptionalRefreshTokenRequestBodyTypeDef",
+    {
+        "clientId": str,
     },
     total=False,
 )
 
 
-class FieldInputConfigOutputTypeDef(
-    _RequiredFieldInputConfigOutputTypeDef, _OptionalFieldInputConfigOutputTypeDef
+class RefreshTokenRequestBodyTypeDef(
+    _RequiredRefreshTokenRequestBodyTypeDef, _OptionalRefreshTokenRequestBodyTypeDef
 ):
     pass
 
 
-_RequiredFieldInputConfigTypeDef = TypedDict(
-    "_RequiredFieldInputConfigTypeDef",
+ThemeValueOutputTypeDef = TypedDict(
+    "ThemeValueOutputTypeDef",
     {
-        "type": str,
+        "value": str,
+        "children": List[Dict[str, Any]],
     },
+    total=False,
 )
-_OptionalFieldInputConfigTypeDef = TypedDict(
-    "_OptionalFieldInputConfigTypeDef",
+
+ThemeValueTypeDef = TypedDict(
+    "ThemeValueTypeDef",
     {
-        "required": bool,
-        "readOnly": bool,
-        "placeholder": str,
-        "defaultValue": str,
-        "descriptiveText": str,
-        "defaultChecked": bool,
-        "defaultCountryCode": str,
-        "valueMappings": "ValueMappingsTypeDef",
-        "name": str,
-        "minValue": float,
-        "maxValue": float,
-        "step": float,
         "value": str,
-        "isArray": bool,
-        "fileUploaderConfig": "FileUploaderFieldConfigTypeDef",
+        "children": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-
-class FieldInputConfigTypeDef(_RequiredFieldInputConfigTypeDef, _OptionalFieldInputConfigTypeDef):
-    pass
-
-
-FieldPositionOutputTypeDef = TypedDict(
-    "FieldPositionOutputTypeDef",
+ThemeValuesOutputTypeDef = TypedDict(
+    "ThemeValuesOutputTypeDef",
     {
-        "fixed": Literal["first"],
-        "rightOf": str,
-        "below": str,
+        "key": str,
+        "value": Dict[str, Any],
     },
     total=False,
 )
 
-FieldPositionTypeDef = TypedDict(
-    "FieldPositionTypeDef",
+ThemeValuesTypeDef = TypedDict(
+    "ThemeValuesTypeDef",
     {
-        "fixed": Literal["first"],
-        "rightOf": str,
-        "below": str,
+        "key": str,
+        "value": Dict[str, Any],
     },
     total=False,
 )
 
-_RequiredFieldValidationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFieldValidationConfigurationOutputTypeDef",
+_RequiredUpdateThemeDataTypeDef = TypedDict(
+    "_RequiredUpdateThemeDataTypeDef",
     {
-        "type": str,
+        "values": Sequence["ThemeValuesTypeDef"],
     },
 )
-_OptionalFieldValidationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFieldValidationConfigurationOutputTypeDef",
+_OptionalUpdateThemeDataTypeDef = TypedDict(
+    "_OptionalUpdateThemeDataTypeDef",
     {
-        "strValues": List[str],
-        "numValues": List[int],
-        "validationMessage": str,
+        "id": str,
+        "name": str,
+        "overrides": Sequence["ThemeValuesTypeDef"],
     },
     total=False,
 )
 
 
-class FieldValidationConfigurationOutputTypeDef(
-    _RequiredFieldValidationConfigurationOutputTypeDef,
-    _OptionalFieldValidationConfigurationOutputTypeDef,
-):
+class UpdateThemeDataTypeDef(_RequiredUpdateThemeDataTypeDef, _OptionalUpdateThemeDataTypeDef):
     pass
 
 
-_RequiredFieldValidationConfigurationTypeDef = TypedDict(
-    "_RequiredFieldValidationConfigurationTypeDef",
+_RequiredValueMappingTypeDef = TypedDict(
+    "_RequiredValueMappingTypeDef",
     {
-        "type": str,
+        "value": "FormInputValuePropertyTypeDef",
     },
 )
-_OptionalFieldValidationConfigurationTypeDef = TypedDict(
-    "_OptionalFieldValidationConfigurationTypeDef",
+_OptionalValueMappingTypeDef = TypedDict(
+    "_OptionalValueMappingTypeDef",
     {
-        "strValues": Sequence[str],
-        "numValues": Sequence[int],
-        "validationMessage": str,
+        "displayValue": "FormInputValuePropertyTypeDef",
     },
     total=False,
 )
 
 
-class FieldValidationConfigurationTypeDef(
-    _RequiredFieldValidationConfigurationTypeDef, _OptionalFieldValidationConfigurationTypeDef
-):
+class ValueMappingTypeDef(_RequiredValueMappingTypeDef, _OptionalValueMappingTypeDef):
     pass
 
 
-_RequiredFileUploaderFieldConfigOutputTypeDef = TypedDict(
-    "_RequiredFileUploaderFieldConfigOutputTypeDef",
+ActionParametersOutputTypeDef = TypedDict(
+    "ActionParametersOutputTypeDef",
     {
-        "accessLevel": StorageAccessLevelType,
-        "acceptedFileTypes": List[str],
+        "type": "ComponentPropertyOutputTypeDef",
+        "url": "ComponentPropertyOutputTypeDef",
+        "anchor": "ComponentPropertyOutputTypeDef",
+        "target": "ComponentPropertyOutputTypeDef",
+        "global": "ComponentPropertyOutputTypeDef",
+        "model": str,
+        "id": "ComponentPropertyOutputTypeDef",
+        "fields": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "state": MutationActionSetStateParameterTypeDef,
     },
+    total=False,
 )
-_OptionalFileUploaderFieldConfigOutputTypeDef = TypedDict(
-    "_OptionalFileUploaderFieldConfigOutputTypeDef",
+
+ActionParametersTypeDef = TypedDict(
+    "ActionParametersTypeDef",
     {
-        "showThumbnails": bool,
-        "isResumable": bool,
-        "maxFileCount": int,
-        "maxSize": int,
+        "type": "ComponentPropertyTypeDef",
+        "url": "ComponentPropertyTypeDef",
+        "anchor": "ComponentPropertyTypeDef",
+        "target": "ComponentPropertyTypeDef",
+        "global": "ComponentPropertyTypeDef",
+        "model": str,
+        "id": "ComponentPropertyTypeDef",
+        "fields": Mapping[str, "ComponentPropertyTypeDef"],
+        "state": MutationActionSetStateParameterTypeDef,
     },
     total=False,
 )
 
-
-class FileUploaderFieldConfigOutputTypeDef(
-    _RequiredFileUploaderFieldConfigOutputTypeDef, _OptionalFileUploaderFieldConfigOutputTypeDef
-):
-    pass
-
-
-_RequiredFileUploaderFieldConfigTypeDef = TypedDict(
-    "_RequiredFileUploaderFieldConfigTypeDef",
+_RequiredCodegenGenericDataFieldOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataFieldOutputTypeDef",
     {
-        "accessLevel": StorageAccessLevelType,
-        "acceptedFileTypes": Sequence[str],
+        "dataType": CodegenGenericDataFieldDataTypeType,
+        "dataTypeValue": str,
+        "required": bool,
+        "readOnly": bool,
+        "isArray": bool,
     },
 )
-_OptionalFileUploaderFieldConfigTypeDef = TypedDict(
-    "_OptionalFileUploaderFieldConfigTypeDef",
+_OptionalCodegenGenericDataFieldOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataFieldOutputTypeDef",
     {
-        "showThumbnails": bool,
-        "isResumable": bool,
-        "maxFileCount": int,
-        "maxSize": int,
+        "relationship": CodegenGenericDataRelationshipTypeOutputTypeDef,
     },
     total=False,
 )
 
 
-class FileUploaderFieldConfigTypeDef(
-    _RequiredFileUploaderFieldConfigTypeDef, _OptionalFileUploaderFieldConfigTypeDef
+class CodegenGenericDataFieldOutputTypeDef(
+    _RequiredCodegenGenericDataFieldOutputTypeDef, _OptionalCodegenGenericDataFieldOutputTypeDef
 ):
     pass
 
 
-FormBindingElementOutputTypeDef = TypedDict(
-    "FormBindingElementOutputTypeDef",
-    {
-        "element": str,
-        "property": str,
-    },
-)
-
-FormBindingElementTypeDef = TypedDict(
-    "FormBindingElementTypeDef",
-    {
-        "element": str,
-        "property": str,
-    },
-)
-
-FormButtonOutputTypeDef = TypedDict(
-    "FormButtonOutputTypeDef",
-    {
-        "excluded": bool,
-        "children": str,
-        "position": "FieldPositionOutputTypeDef",
-    },
-    total=False,
-)
-
-FormButtonTypeDef = TypedDict(
-    "FormButtonTypeDef",
-    {
-        "excluded": bool,
-        "children": str,
-        "position": "FieldPositionTypeDef",
-    },
-    total=False,
-)
-
-FormCTAOutputTypeDef = TypedDict(
-    "FormCTAOutputTypeDef",
+_RequiredCodegenGenericDataFieldTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataFieldTypeDef",
     {
-        "position": FormButtonsPositionType,
-        "clear": "FormButtonOutputTypeDef",
-        "cancel": "FormButtonOutputTypeDef",
-        "submit": "FormButtonOutputTypeDef",
+        "dataType": CodegenGenericDataFieldDataTypeType,
+        "dataTypeValue": str,
+        "required": bool,
+        "readOnly": bool,
+        "isArray": bool,
     },
-    total=False,
 )
-
-FormCTATypeDef = TypedDict(
-    "FormCTATypeDef",
+_OptionalCodegenGenericDataFieldTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataFieldTypeDef",
     {
-        "position": FormButtonsPositionType,
-        "clear": "FormButtonTypeDef",
-        "cancel": "FormButtonTypeDef",
-        "submit": "FormButtonTypeDef",
+        "relationship": CodegenGenericDataRelationshipTypeTypeDef,
     },
     total=False,
 )
 
-FormDataTypeConfigOutputTypeDef = TypedDict(
-    "FormDataTypeConfigOutputTypeDef",
-    {
-        "dataSourceType": FormDataSourceTypeType,
-        "dataTypeName": str,
-    },
-)
 
-FormDataTypeConfigTypeDef = TypedDict(
-    "FormDataTypeConfigTypeDef",
-    {
-        "dataSourceType": FormDataSourceTypeType,
-        "dataTypeName": str,
-    },
-)
+class CodegenGenericDataFieldTypeDef(
+    _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
+):
+    pass
 
-FormInputBindingPropertiesValueOutputTypeDef = TypedDict(
-    "FormInputBindingPropertiesValueOutputTypeDef",
-    {
-        "type": str,
-        "bindingProperties": "FormInputBindingPropertiesValuePropertiesOutputTypeDef",
-    },
-    total=False,
-)
 
-FormInputBindingPropertiesValuePropertiesOutputTypeDef = TypedDict(
-    "FormInputBindingPropertiesValuePropertiesOutputTypeDef",
+CodegenJobRenderConfigTypeDef = TypedDict(
+    "CodegenJobRenderConfigTypeDef",
     {
-        "model": str,
+        "react": ReactStartCodegenJobDataTypeDef,
     },
     total=False,
 )
 
-FormInputBindingPropertiesValuePropertiesTypeDef = TypedDict(
-    "FormInputBindingPropertiesValuePropertiesTypeDef",
+ComponentBindingPropertiesValueOutputTypeDef = TypedDict(
+    "ComponentBindingPropertiesValueOutputTypeDef",
     {
-        "model": str,
+        "type": str,
+        "bindingProperties": ComponentBindingPropertiesValuePropertiesOutputTypeDef,
+        "defaultValue": str,
     },
     total=False,
 )
 
-FormInputBindingPropertiesValueTypeDef = TypedDict(
-    "FormInputBindingPropertiesValueTypeDef",
+ComponentBindingPropertiesValueTypeDef = TypedDict(
+    "ComponentBindingPropertiesValueTypeDef",
     {
         "type": str,
-        "bindingProperties": "FormInputBindingPropertiesValuePropertiesTypeDef",
+        "bindingProperties": ComponentBindingPropertiesValuePropertiesTypeDef,
+        "defaultValue": str,
     },
     total=False,
 )
 
-_RequiredFormInputValuePropertyBindingPropertiesOutputTypeDef = TypedDict(
-    "_RequiredFormInputValuePropertyBindingPropertiesOutputTypeDef",
+_RequiredComponentDataConfigurationOutputTypeDef = TypedDict(
+    "_RequiredComponentDataConfigurationOutputTypeDef",
     {
-        "property": str,
+        "model": str,
     },
 )
-_OptionalFormInputValuePropertyBindingPropertiesOutputTypeDef = TypedDict(
-    "_OptionalFormInputValuePropertyBindingPropertiesOutputTypeDef",
+_OptionalComponentDataConfigurationOutputTypeDef = TypedDict(
+    "_OptionalComponentDataConfigurationOutputTypeDef",
     {
-        "field": str,
+        "sort": List[SortPropertyTypeDef],
+        "predicate": "PredicateOutputTypeDef",
+        "identifiers": List[str],
     },
     total=False,
 )
 
 
-class FormInputValuePropertyBindingPropertiesOutputTypeDef(
-    _RequiredFormInputValuePropertyBindingPropertiesOutputTypeDef,
-    _OptionalFormInputValuePropertyBindingPropertiesOutputTypeDef,
+class ComponentDataConfigurationOutputTypeDef(
+    _RequiredComponentDataConfigurationOutputTypeDef,
+    _OptionalComponentDataConfigurationOutputTypeDef,
 ):
     pass
 
 
-_RequiredFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
-    "_RequiredFormInputValuePropertyBindingPropertiesTypeDef",
+_RequiredComponentDataConfigurationTypeDef = TypedDict(
+    "_RequiredComponentDataConfigurationTypeDef",
     {
-        "property": str,
+        "model": str,
     },
 )
-_OptionalFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
-    "_OptionalFormInputValuePropertyBindingPropertiesTypeDef",
+_OptionalComponentDataConfigurationTypeDef = TypedDict(
+    "_OptionalComponentDataConfigurationTypeDef",
     {
-        "field": str,
+        "sort": Sequence[SortPropertyTypeDef],
+        "predicate": "PredicateTypeDef",
+        "identifiers": Sequence[str],
     },
     total=False,
 )
 
 
-class FormInputValuePropertyBindingPropertiesTypeDef(
-    _RequiredFormInputValuePropertyBindingPropertiesTypeDef,
-    _OptionalFormInputValuePropertyBindingPropertiesTypeDef,
+class ComponentDataConfigurationTypeDef(
+    _RequiredComponentDataConfigurationTypeDef, _OptionalComponentDataConfigurationTypeDef
 ):
     pass
 
 
-FormInputValuePropertyOutputTypeDef = TypedDict(
-    "FormInputValuePropertyOutputTypeDef",
+ComponentPropertyOutputTypeDef = TypedDict(
+    "ComponentPropertyOutputTypeDef",
     {
         "value": str,
-        "bindingProperties": "FormInputValuePropertyBindingPropertiesOutputTypeDef",
+        "bindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "collectionBindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "defaultValue": str,
+        "model": str,
+        "bindings": Dict[str, FormBindingElementTypeDef],
+        "event": str,
+        "userAttribute": str,
         "concat": List[Dict[str, Any]],
+        "condition": "ComponentConditionPropertyTypeDef",
+        "configured": bool,
+        "type": str,
+        "importedValue": str,
+        "componentName": str,
+        "property": str,
     },
     total=False,
 )
 
-FormInputValuePropertyTypeDef = TypedDict(
-    "FormInputValuePropertyTypeDef",
+ComponentPropertyTypeDef = TypedDict(
+    "ComponentPropertyTypeDef",
     {
         "value": str,
-        "bindingProperties": "FormInputValuePropertyBindingPropertiesTypeDef",
+        "bindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "collectionBindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "defaultValue": str,
+        "model": str,
+        "bindings": Mapping[str, FormBindingElementTypeDef],
+        "event": str,
+        "userAttribute": str,
         "concat": Sequence[Dict[str, Any]],
+        "condition": Dict[str, Any],
+        "configured": bool,
+        "type": str,
+        "importedValue": str,
+        "componentName": str,
+        "property": str,
     },
     total=False,
 )
 
-FormStyleConfigOutputTypeDef = TypedDict(
-    "FormStyleConfigOutputTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "tokenReference": str,
-        "value": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-FormStyleConfigTypeDef = TypedDict(
-    "FormStyleConfigTypeDef",
+ExchangeCodeForTokenResponseTypeDef = TypedDict(
+    "ExchangeCodeForTokenResponseTypeDef",
     {
-        "tokenReference": str,
-        "value": str,
+        "accessToken": str,
+        "expiresIn": int,
+        "refreshToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-FormStyleOutputTypeDef = TypedDict(
-    "FormStyleOutputTypeDef",
+GetMetadataResponseTypeDef = TypedDict(
+    "GetMetadataResponseTypeDef",
     {
-        "horizontalGap": "FormStyleConfigOutputTypeDef",
-        "verticalGap": "FormStyleConfigOutputTypeDef",
-        "outerPadding": "FormStyleConfigOutputTypeDef",
+        "features": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-FormStyleTypeDef = TypedDict(
-    "FormStyleTypeDef",
+ListCodegenJobsResponseTypeDef = TypedDict(
+    "ListCodegenJobsResponseTypeDef",
+    {
+        "entities": List[CodegenJobSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListComponentsResponseTypeDef = TypedDict(
+    "ListComponentsResponseTypeDef",
     {
-        "horizontalGap": "FormStyleConfigTypeDef",
-        "verticalGap": "FormStyleConfigTypeDef",
-        "outerPadding": "FormStyleConfigTypeDef",
+        "entities": List[ComponentSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RefreshTokenResponseTypeDef = TypedDict(
+    "RefreshTokenResponseTypeDef",
+    {
+        "accessToken": str,
+        "expiresIn": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 FormSummaryTypeDef = TypedDict(
     "FormSummaryTypeDef",
     {
         "appId": str,
-        "dataType": "FormDataTypeConfigOutputTypeDef",
+        "dataType": FormDataTypeConfigTypeDef,
         "environmentName": str,
         "formActionType": FormActionTypeType,
         "id": str,
         "name": str,
     },
 )
 
-_RequiredFormTypeDef = TypedDict(
-    "_RequiredFormTypeDef",
+_RequiredCreateThemeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateThemeRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
-        "id": str,
-        "name": str,
-        "formActionType": FormActionTypeType,
-        "style": "FormStyleOutputTypeDef",
-        "dataType": "FormDataTypeConfigOutputTypeDef",
-        "fields": Dict[str, "FieldConfigOutputTypeDef"],
-        "sectionalElements": Dict[str, "SectionalElementOutputTypeDef"],
-        "schemaVersion": str,
+        "themeToCreate": CreateThemeDataTypeDef,
     },
 )
-_OptionalFormTypeDef = TypedDict(
-    "_OptionalFormTypeDef",
+_OptionalCreateThemeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateThemeRequestRequestTypeDef",
     {
-        "tags": Dict[str, str],
-        "cta": "FormCTAOutputTypeDef",
-        "labelDecorator": LabelDecoratorType,
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
+class CreateThemeRequestRequestTypeDef(
+    _RequiredCreateThemeRequestRequestTypeDef, _OptionalCreateThemeRequestRequestTypeDef
+):
     pass
 
 
-GetCodegenJobRequestRequestTypeDef = TypedDict(
-    "GetCodegenJobRequestRequestTypeDef",
-    {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-    },
-)
-
-GetCodegenJobResponseTypeDef = TypedDict(
-    "GetCodegenJobResponseTypeDef",
+CreateThemeResponseTypeDef = TypedDict(
+    "CreateThemeResponseTypeDef",
     {
-        "job": "CodegenJobTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "entity": ThemeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetComponentRequestRequestTypeDef = TypedDict(
-    "GetComponentRequestRequestTypeDef",
+ExportThemesResponseTypeDef = TypedDict(
+    "ExportThemesResponseTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "entities": List[ThemeTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetComponentResponseTypeDef = TypedDict(
-    "GetComponentResponseTypeDef",
+GetThemeResponseTypeDef = TypedDict(
+    "GetThemeResponseTypeDef",
     {
-        "component": "ComponentTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "theme": ThemeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetFormRequestRequestTypeDef = TypedDict(
-    "GetFormRequestRequestTypeDef",
+UpdateThemeResponseTypeDef = TypedDict(
+    "UpdateThemeResponseTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "entity": ThemeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetFormResponseTypeDef = TypedDict(
-    "GetFormResponseTypeDef",
+ExchangeCodeForTokenRequestRequestTypeDef = TypedDict(
+    "ExchangeCodeForTokenRequestRequestTypeDef",
     {
-        "form": "FormTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "provider": Literal["figma"],
+        "request": ExchangeCodeForTokenRequestBodyTypeDef,
     },
 )
 
-GetMetadataRequestRequestTypeDef = TypedDict(
-    "GetMetadataRequestRequestTypeDef",
+_RequiredExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
+    "_RequiredExportComponentsRequestExportComponentsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-
-GetMetadataResponseTypeDef = TypedDict(
-    "GetMetadataResponseTypeDef",
+_OptionalExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
+    "_OptionalExportComponentsRequestExportComponentsPaginateTypeDef",
     {
-        "features": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-GetThemeRequestRequestTypeDef = TypedDict(
-    "GetThemeRequestRequestTypeDef",
-    {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-    },
-)
 
-GetThemeResponseTypeDef = TypedDict(
-    "GetThemeResponseTypeDef",
-    {
-        "theme": "ThemeTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class ExportComponentsRequestExportComponentsPaginateTypeDef(
+    _RequiredExportComponentsRequestExportComponentsPaginateTypeDef,
+    _OptionalExportComponentsRequestExportComponentsPaginateTypeDef,
+):
+    pass
 
-_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
-    "_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+
+_RequiredExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
+    "_RequiredExportFormsRequestExportFormsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
-    "_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+_OptionalExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
+    "_OptionalExportFormsRequestExportFormsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListCodegenJobsRequestListCodegenJobsPaginateTypeDef(
-    _RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
-    _OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+class ExportFormsRequestExportFormsPaginateTypeDef(
+    _RequiredExportFormsRequestExportFormsPaginateTypeDef,
+    _OptionalExportFormsRequestExportFormsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListCodegenJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListCodegenJobsRequestRequestTypeDef",
+_RequiredExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
+    "_RequiredExportThemesRequestExportThemesPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListCodegenJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListCodegenJobsRequestRequestTypeDef",
+_OptionalExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
+    "_OptionalExportThemesRequestExportThemesPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListCodegenJobsRequestRequestTypeDef(
-    _RequiredListCodegenJobsRequestRequestTypeDef, _OptionalListCodegenJobsRequestRequestTypeDef
+class ExportThemesRequestExportThemesPaginateTypeDef(
+    _RequiredExportThemesRequestExportThemesPaginateTypeDef,
+    _OptionalExportThemesRequestExportThemesPaginateTypeDef,
 ):
     pass
 
 
-ListCodegenJobsResponseTypeDef = TypedDict(
-    "ListCodegenJobsResponseTypeDef",
-    {
-        "entities": List["CodegenJobSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
-    "_RequiredListComponentsRequestListComponentsPaginateTypeDef",
+_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
+    "_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
-    "_OptionalListComponentsRequestListComponentsPaginateTypeDef",
+_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
+    "_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListComponentsRequestListComponentsPaginateTypeDef(
-    _RequiredListComponentsRequestListComponentsPaginateTypeDef,
-    _OptionalListComponentsRequestListComponentsPaginateTypeDef,
+class ListCodegenJobsRequestListCodegenJobsPaginateTypeDef(
+    _RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    _OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListComponentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListComponentsRequestRequestTypeDef",
+_RequiredListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
+    "_RequiredListComponentsRequestListComponentsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListComponentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListComponentsRequestRequestTypeDef",
+_OptionalListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
+    "_OptionalListComponentsRequestListComponentsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListComponentsRequestRequestTypeDef(
-    _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
+class ListComponentsRequestListComponentsPaginateTypeDef(
+    _RequiredListComponentsRequestListComponentsPaginateTypeDef,
+    _OptionalListComponentsRequestListComponentsPaginateTypeDef,
 ):
     pass
 
 
-ListComponentsResponseTypeDef = TypedDict(
-    "ListComponentsResponseTypeDef",
-    {
-        "entities": List["ComponentSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListFormsRequestListFormsPaginateTypeDef = TypedDict(
     "_RequiredListFormsRequestListFormsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
 _OptionalListFormsRequestListFormsPaginateTypeDef = TypedDict(
     "_OptionalListFormsRequestListFormsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListFormsRequestListFormsPaginateTypeDef(
     _RequiredListFormsRequestListFormsPaginateTypeDef,
     _OptionalListFormsRequestListFormsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListFormsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFormsRequestRequestTypeDef",
+_RequiredListThemesRequestListThemesPaginateTypeDef = TypedDict(
+    "_RequiredListThemesRequestListThemesPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListFormsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFormsRequestRequestTypeDef",
+_OptionalListThemesRequestListThemesPaginateTypeDef = TypedDict(
+    "_OptionalListThemesRequestListThemesPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListFormsRequestRequestTypeDef(
-    _RequiredListFormsRequestRequestTypeDef, _OptionalListFormsRequestRequestTypeDef
+class ListThemesRequestListThemesPaginateTypeDef(
+    _RequiredListThemesRequestListThemesPaginateTypeDef,
+    _OptionalListThemesRequestListThemesPaginateTypeDef,
 ):
     pass
 
 
-ListFormsResponseTypeDef = TypedDict(
-    "ListFormsResponseTypeDef",
+FormButtonTypeDef = TypedDict(
+    "FormButtonTypeDef",
     {
-        "entities": List["FormSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "excluded": bool,
+        "children": str,
+        "position": FieldPositionTypeDef,
     },
+    total=False,
 )
 
-_RequiredListThemesRequestListThemesPaginateTypeDef = TypedDict(
-    "_RequiredListThemesRequestListThemesPaginateTypeDef",
+_RequiredSectionalElementTypeDef = TypedDict(
+    "_RequiredSectionalElementTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "type": str,
     },
 )
-_OptionalListThemesRequestListThemesPaginateTypeDef = TypedDict(
-    "_OptionalListThemesRequestListThemesPaginateTypeDef",
+_OptionalSectionalElementTypeDef = TypedDict(
+    "_OptionalSectionalElementTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "position": FieldPositionTypeDef,
+        "text": str,
+        "level": int,
+        "orientation": str,
+        "excluded": bool,
     },
     total=False,
 )
 
 
-class ListThemesRequestListThemesPaginateTypeDef(
-    _RequiredListThemesRequestListThemesPaginateTypeDef,
-    _OptionalListThemesRequestListThemesPaginateTypeDef,
-):
+class SectionalElementTypeDef(_RequiredSectionalElementTypeDef, _OptionalSectionalElementTypeDef):
     pass
 
 
-_RequiredListThemesRequestRequestTypeDef = TypedDict(
-    "_RequiredListThemesRequestRequestTypeDef",
+FormInputBindingPropertiesValueTypeDef = TypedDict(
+    "FormInputBindingPropertiesValueTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "type": str,
+        "bindingProperties": FormInputBindingPropertiesValuePropertiesTypeDef,
     },
+    total=False,
 )
-_OptionalListThemesRequestRequestTypeDef = TypedDict(
-    "_OptionalListThemesRequestRequestTypeDef",
+
+FormInputValuePropertyTypeDef = TypedDict(
+    "FormInputValuePropertyTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "value": str,
+        "bindingProperties": FormInputValuePropertyBindingPropertiesTypeDef,
+        "concat": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-
-class ListThemesRequestRequestTypeDef(
-    _RequiredListThemesRequestRequestTypeDef, _OptionalListThemesRequestRequestTypeDef
-):
-    pass
-
+FormStyleTypeDef = TypedDict(
+    "FormStyleTypeDef",
+    {
+        "horizontalGap": FormStyleConfigTypeDef,
+        "verticalGap": FormStyleConfigTypeDef,
+        "outerPadding": FormStyleConfigTypeDef,
+    },
+    total=False,
+)
 
 ListThemesResponseTypeDef = TypedDict(
     "ListThemesResponseTypeDef",
     {
-        "entities": List["ThemeSummaryTypeDef"],
+        "entities": List[ThemeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MutationActionSetStateParameterOutputTypeDef = TypedDict(
-    "MutationActionSetStateParameterOutputTypeDef",
+PutMetadataFlagRequestRequestTypeDef = TypedDict(
+    "PutMetadataFlagRequestRequestTypeDef",
     {
-        "componentName": str,
-        "property": str,
-        "set": "ComponentPropertyOutputTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "featureName": str,
+        "body": PutMetadataFlagBodyTypeDef,
     },
 )
 
-MutationActionSetStateParameterTypeDef = TypedDict(
-    "MutationActionSetStateParameterTypeDef",
+RefreshTokenRequestRequestTypeDef = TypedDict(
+    "RefreshTokenRequestRequestTypeDef",
     {
-        "componentName": str,
-        "property": str,
-        "set": "ComponentPropertyTypeDef",
+        "provider": Literal["figma"],
+        "refreshTokenBody": RefreshTokenRequestBodyTypeDef,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredUpdateThemeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateThemeRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "updatedTheme": UpdateThemeDataTypeDef,
     },
-    total=False,
 )
-
-PredicateOutputTypeDef = TypedDict(
-    "PredicateOutputTypeDef",
+_OptionalUpdateThemeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateThemeRequestRequestTypeDef",
     {
-        "or": List[Dict[str, Any]],
-        "and": List[Dict[str, Any]],
-        "field": str,
-        "operator": str,
-        "operand": str,
-        "operandType": str,
+        "clientToken": str,
     },
     total=False,
 )
 
-PredicateTypeDef = TypedDict(
-    "PredicateTypeDef",
+
+class UpdateThemeRequestRequestTypeDef(
+    _RequiredUpdateThemeRequestRequestTypeDef, _OptionalUpdateThemeRequestRequestTypeDef
+):
+    pass
+
+
+ComponentEventOutputTypeDef = TypedDict(
+    "ComponentEventOutputTypeDef",
     {
-        "or": Sequence[Dict[str, Any]],
-        "and": Sequence[Dict[str, Any]],
-        "field": str,
-        "operator": str,
-        "operand": str,
-        "operandType": str,
+        "action": str,
+        "parameters": ActionParametersOutputTypeDef,
+        "bindingEvent": str,
     },
     total=False,
 )
 
-PutMetadataFlagBodyTypeDef = TypedDict(
-    "PutMetadataFlagBodyTypeDef",
+ComponentEventTypeDef = TypedDict(
+    "ComponentEventTypeDef",
     {
-        "newValue": str,
+        "action": str,
+        "parameters": ActionParametersTypeDef,
+        "bindingEvent": str,
     },
+    total=False,
 )
 
-PutMetadataFlagRequestRequestTypeDef = TypedDict(
-    "PutMetadataFlagRequestRequestTypeDef",
+_RequiredCodegenGenericDataModelOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataModelOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "featureName": str,
-        "body": "PutMetadataFlagBodyTypeDef",
+        "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
+        "primaryKeys": List[str],
     },
 )
-
-ReactStartCodegenJobDataOutputTypeDef = TypedDict(
-    "ReactStartCodegenJobDataOutputTypeDef",
+_OptionalCodegenGenericDataModelOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataModelOutputTypeDef",
     {
-        "module": JSModuleType,
-        "target": JSTargetType,
-        "script": JSScriptType,
-        "renderTypeDeclarations": bool,
-        "inlineSourceMap": bool,
+        "isJoinTable": bool,
     },
     total=False,
 )
 
-ReactStartCodegenJobDataTypeDef = TypedDict(
-    "ReactStartCodegenJobDataTypeDef",
+
+class CodegenGenericDataModelOutputTypeDef(
+    _RequiredCodegenGenericDataModelOutputTypeDef, _OptionalCodegenGenericDataModelOutputTypeDef
+):
+    pass
+
+
+CodegenGenericDataNonModelOutputTypeDef = TypedDict(
+    "CodegenGenericDataNonModelOutputTypeDef",
     {
-        "module": JSModuleType,
-        "target": JSTargetType,
-        "script": JSScriptType,
-        "renderTypeDeclarations": bool,
-        "inlineSourceMap": bool,
+        "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
     },
-    total=False,
 )
 
-_RequiredRefreshTokenRequestBodyTypeDef = TypedDict(
-    "_RequiredRefreshTokenRequestBodyTypeDef",
+_RequiredCodegenGenericDataModelTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataModelTypeDef",
     {
-        "token": str,
+        "fields": Mapping[str, CodegenGenericDataFieldTypeDef],
+        "primaryKeys": Sequence[str],
     },
 )
-_OptionalRefreshTokenRequestBodyTypeDef = TypedDict(
-    "_OptionalRefreshTokenRequestBodyTypeDef",
+_OptionalCodegenGenericDataModelTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataModelTypeDef",
     {
-        "clientId": str,
+        "isJoinTable": bool,
     },
     total=False,
 )
 
 
-class RefreshTokenRequestBodyTypeDef(
-    _RequiredRefreshTokenRequestBodyTypeDef, _OptionalRefreshTokenRequestBodyTypeDef
+class CodegenGenericDataModelTypeDef(
+    _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
 ):
     pass
 
 
-RefreshTokenRequestRequestTypeDef = TypedDict(
-    "RefreshTokenRequestRequestTypeDef",
+CodegenGenericDataNonModelTypeDef = TypedDict(
+    "CodegenGenericDataNonModelTypeDef",
     {
-        "provider": Literal["figma"],
-        "refreshTokenBody": "RefreshTokenRequestBodyTypeDef",
+        "fields": Mapping[str, CodegenGenericDataFieldTypeDef],
     },
 )
 
-RefreshTokenResponseTypeDef = TypedDict(
-    "RefreshTokenResponseTypeDef",
+ListFormsResponseTypeDef = TypedDict(
+    "ListFormsResponseTypeDef",
     {
-        "accessToken": str,
-        "expiresIn": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "entities": List[FormSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+FormCTATypeDef = TypedDict(
+    "FormCTATypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "position": FormButtonsPositionType,
+        "clear": FormButtonTypeDef,
+        "cancel": FormButtonTypeDef,
+        "submit": FormButtonTypeDef,
     },
+    total=False,
 )
 
-_RequiredSectionalElementOutputTypeDef = TypedDict(
-    "_RequiredSectionalElementOutputTypeDef",
+_RequiredValueMappingsOutputTypeDef = TypedDict(
+    "_RequiredValueMappingsOutputTypeDef",
     {
-        "type": str,
+        "values": List[ValueMappingTypeDef],
     },
 )
-_OptionalSectionalElementOutputTypeDef = TypedDict(
-    "_OptionalSectionalElementOutputTypeDef",
+_OptionalValueMappingsOutputTypeDef = TypedDict(
+    "_OptionalValueMappingsOutputTypeDef",
     {
-        "position": "FieldPositionOutputTypeDef",
-        "text": str,
-        "level": int,
-        "orientation": str,
-        "excluded": bool,
+        "bindingProperties": Dict[str, FormInputBindingPropertiesValueTypeDef],
     },
     total=False,
 )
 
 
-class SectionalElementOutputTypeDef(
-    _RequiredSectionalElementOutputTypeDef, _OptionalSectionalElementOutputTypeDef
+class ValueMappingsOutputTypeDef(
+    _RequiredValueMappingsOutputTypeDef, _OptionalValueMappingsOutputTypeDef
 ):
     pass
 
 
-_RequiredSectionalElementTypeDef = TypedDict(
-    "_RequiredSectionalElementTypeDef",
+_RequiredValueMappingsTypeDef = TypedDict(
+    "_RequiredValueMappingsTypeDef",
     {
-        "type": str,
+        "values": Sequence[ValueMappingTypeDef],
     },
 )
-_OptionalSectionalElementTypeDef = TypedDict(
-    "_OptionalSectionalElementTypeDef",
+_OptionalValueMappingsTypeDef = TypedDict(
+    "_OptionalValueMappingsTypeDef",
     {
-        "position": "FieldPositionTypeDef",
-        "text": str,
-        "level": int,
-        "orientation": str,
-        "excluded": bool,
+        "bindingProperties": Mapping[str, FormInputBindingPropertiesValueTypeDef],
     },
     total=False,
 )
 
 
-class SectionalElementTypeDef(_RequiredSectionalElementTypeDef, _OptionalSectionalElementTypeDef):
+class ValueMappingsTypeDef(_RequiredValueMappingsTypeDef, _OptionalValueMappingsTypeDef):
     pass
 
 
-SortPropertyOutputTypeDef = TypedDict(
-    "SortPropertyOutputTypeDef",
+_RequiredComponentChildOutputTypeDef = TypedDict(
+    "_RequiredComponentChildOutputTypeDef",
     {
-        "field": str,
-        "direction": SortDirectionType,
+        "componentType": str,
+        "name": str,
+        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
     },
 )
-
-SortPropertyTypeDef = TypedDict(
-    "SortPropertyTypeDef",
+_OptionalComponentChildOutputTypeDef = TypedDict(
+    "_OptionalComponentChildOutputTypeDef",
     {
-        "field": str,
-        "direction": SortDirectionType,
+        "children": List[Dict[str, Any]],
+        "events": Dict[str, ComponentEventOutputTypeDef],
+        "sourceId": str,
     },
+    total=False,
 )
 
-_RequiredStartCodegenJobDataTypeDef = TypedDict(
-    "_RequiredStartCodegenJobDataTypeDef",
+
+class ComponentChildOutputTypeDef(
+    _RequiredComponentChildOutputTypeDef, _OptionalComponentChildOutputTypeDef
+):
+    pass
+
+
+_RequiredComponentTypeDef = TypedDict(
+    "_RequiredComponentTypeDef",
     {
-        "renderConfig": "CodegenJobRenderConfigTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "name": str,
+        "componentType": str,
+        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "variants": List[ComponentVariantOutputTypeDef],
+        "overrides": Dict[str, Dict[str, str]],
+        "bindingProperties": Dict[str, ComponentBindingPropertiesValueOutputTypeDef],
+        "createdAt": datetime,
     },
 )
-_OptionalStartCodegenJobDataTypeDef = TypedDict(
-    "_OptionalStartCodegenJobDataTypeDef",
+_OptionalComponentTypeDef = TypedDict(
+    "_OptionalComponentTypeDef",
     {
-        "genericDataSchema": "CodegenJobGenericDataSchemaTypeDef",
-        "autoGenerateForms": bool,
-        "features": "CodegenFeatureFlagsTypeDef",
-        "tags": Mapping[str, str],
+        "sourceId": str,
+        "children": List["ComponentChildOutputTypeDef"],
+        "collectionProperties": Dict[str, ComponentDataConfigurationOutputTypeDef],
+        "modifiedAt": datetime,
+        "tags": Dict[str, str],
+        "events": Dict[str, ComponentEventOutputTypeDef],
+        "schemaVersion": str,
     },
     total=False,
 )
 
 
-class StartCodegenJobDataTypeDef(
-    _RequiredStartCodegenJobDataTypeDef, _OptionalStartCodegenJobDataTypeDef
-):
+class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
     pass
 
 
-_RequiredStartCodegenJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartCodegenJobRequestRequestTypeDef",
+_RequiredComponentChildTypeDef = TypedDict(
+    "_RequiredComponentChildTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "codegenJobToCreate": "StartCodegenJobDataTypeDef",
+        "componentType": str,
+        "name": str,
+        "properties": Mapping[str, "ComponentPropertyTypeDef"],
     },
 )
-_OptionalStartCodegenJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartCodegenJobRequestRequestTypeDef",
+_OptionalComponentChildTypeDef = TypedDict(
+    "_OptionalComponentChildTypeDef",
     {
-        "clientToken": str,
+        "children": Sequence[Dict[str, Any]],
+        "events": Mapping[str, ComponentEventTypeDef],
+        "sourceId": str,
     },
     total=False,
 )
 
 
-class StartCodegenJobRequestRequestTypeDef(
-    _RequiredStartCodegenJobRequestRequestTypeDef, _OptionalStartCodegenJobRequestRequestTypeDef
-):
+class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
     pass
 
 
-StartCodegenJobResponseTypeDef = TypedDict(
-    "StartCodegenJobResponseTypeDef",
+_RequiredCreateComponentDataTypeDef = TypedDict(
+    "_RequiredCreateComponentDataTypeDef",
     {
-        "entity": "CodegenJobTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "componentType": str,
+        "properties": Mapping[str, "ComponentPropertyTypeDef"],
+        "variants": Sequence[ComponentVariantTypeDef],
+        "overrides": Mapping[str, Mapping[str, str]],
+        "bindingProperties": Mapping[str, ComponentBindingPropertiesValueTypeDef],
     },
 )
+_OptionalCreateComponentDataTypeDef = TypedDict(
+    "_OptionalCreateComponentDataTypeDef",
+    {
+        "sourceId": str,
+        "children": Sequence["ComponentChildTypeDef"],
+        "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
+        "tags": Mapping[str, str],
+        "events": Mapping[str, ComponentEventTypeDef],
+        "schemaVersion": str,
+    },
+    total=False,
+)
 
-ThemeSummaryTypeDef = TypedDict(
-    "ThemeSummaryTypeDef",
+
+class CreateComponentDataTypeDef(
+    _RequiredCreateComponentDataTypeDef, _OptionalCreateComponentDataTypeDef
+):
+    pass
+
+
+UpdateComponentDataTypeDef = TypedDict(
+    "UpdateComponentDataTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
         "id": str,
         "name": str,
+        "sourceId": str,
+        "componentType": str,
+        "properties": Mapping[str, "ComponentPropertyTypeDef"],
+        "children": Sequence["ComponentChildTypeDef"],
+        "variants": Sequence[ComponentVariantTypeDef],
+        "overrides": Mapping[str, Mapping[str, str]],
+        "bindingProperties": Mapping[str, ComponentBindingPropertiesValueTypeDef],
+        "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
+        "events": Mapping[str, ComponentEventTypeDef],
+        "schemaVersion": str,
     },
+    total=False,
 )
 
-_RequiredThemeTypeDef = TypedDict(
-    "_RequiredThemeTypeDef",
+CodegenJobGenericDataSchemaOutputTypeDef = TypedDict(
+    "CodegenJobGenericDataSchemaOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "name": str,
-        "createdAt": datetime,
-        "values": List["ThemeValuesOutputTypeDef"],
+        "dataSourceType": Literal["DataStore"],
+        "models": Dict[str, CodegenGenericDataModelOutputTypeDef],
+        "enums": Dict[str, CodegenGenericDataEnumOutputTypeDef],
+        "nonModels": Dict[str, CodegenGenericDataNonModelOutputTypeDef],
     },
 )
-_OptionalThemeTypeDef = TypedDict(
-    "_OptionalThemeTypeDef",
+
+CodegenJobGenericDataSchemaTypeDef = TypedDict(
+    "CodegenJobGenericDataSchemaTypeDef",
     {
-        "modifiedAt": datetime,
-        "overrides": List["ThemeValuesOutputTypeDef"],
-        "tags": Dict[str, str],
+        "dataSourceType": Literal["DataStore"],
+        "models": Mapping[str, CodegenGenericDataModelTypeDef],
+        "enums": Mapping[str, CodegenGenericDataEnumTypeDef],
+        "nonModels": Mapping[str, CodegenGenericDataNonModelTypeDef],
+    },
+)
+
+_RequiredFieldInputConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldInputConfigOutputTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalFieldInputConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldInputConfigOutputTypeDef",
+    {
+        "required": bool,
+        "readOnly": bool,
+        "placeholder": str,
+        "defaultValue": str,
+        "descriptiveText": str,
+        "defaultChecked": bool,
+        "defaultCountryCode": str,
+        "valueMappings": ValueMappingsOutputTypeDef,
+        "name": str,
+        "minValue": float,
+        "maxValue": float,
+        "step": float,
+        "value": str,
+        "isArray": bool,
+        "fileUploaderConfig": FileUploaderFieldConfigOutputTypeDef,
     },
     total=False,
 )
 
 
-class ThemeTypeDef(_RequiredThemeTypeDef, _OptionalThemeTypeDef):
+class FieldInputConfigOutputTypeDef(
+    _RequiredFieldInputConfigOutputTypeDef, _OptionalFieldInputConfigOutputTypeDef
+):
     pass
 
 
-ThemeValueOutputTypeDef = TypedDict(
-    "ThemeValueOutputTypeDef",
+_RequiredFieldInputConfigTypeDef = TypedDict(
+    "_RequiredFieldInputConfigTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalFieldInputConfigTypeDef = TypedDict(
+    "_OptionalFieldInputConfigTypeDef",
     {
+        "required": bool,
+        "readOnly": bool,
+        "placeholder": str,
+        "defaultValue": str,
+        "descriptiveText": str,
+        "defaultChecked": bool,
+        "defaultCountryCode": str,
+        "valueMappings": ValueMappingsTypeDef,
+        "name": str,
+        "minValue": float,
+        "maxValue": float,
+        "step": float,
         "value": str,
-        "children": List[Dict[str, Any]],
+        "isArray": bool,
+        "fileUploaderConfig": FileUploaderFieldConfigTypeDef,
     },
     total=False,
 )
 
-ThemeValueTypeDef = TypedDict(
-    "ThemeValueTypeDef",
+
+class FieldInputConfigTypeDef(_RequiredFieldInputConfigTypeDef, _OptionalFieldInputConfigTypeDef):
+    pass
+
+
+CreateComponentResponseTypeDef = TypedDict(
+    "CreateComponentResponseTypeDef",
     {
-        "value": str,
-        "children": Sequence[Dict[str, Any]],
+        "entity": ComponentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ThemeValuesOutputTypeDef = TypedDict(
-    "ThemeValuesOutputTypeDef",
+ExportComponentsResponseTypeDef = TypedDict(
+    "ExportComponentsResponseTypeDef",
     {
-        "key": str,
-        "value": Dict[str, Any],
+        "entities": List[ComponentTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ThemeValuesTypeDef = TypedDict(
-    "ThemeValuesTypeDef",
+GetComponentResponseTypeDef = TypedDict(
+    "GetComponentResponseTypeDef",
     {
-        "key": str,
-        "value": Dict[str, Any],
+        "component": ComponentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateComponentDataTypeDef = TypedDict(
-    "UpdateComponentDataTypeDef",
+UpdateComponentResponseTypeDef = TypedDict(
+    "UpdateComponentResponseTypeDef",
     {
-        "id": str,
-        "name": str,
-        "sourceId": str,
-        "componentType": str,
-        "properties": Mapping[str, "ComponentPropertyTypeDef"],
-        "children": Sequence["ComponentChildTypeDef"],
-        "variants": Sequence["ComponentVariantTypeDef"],
-        "overrides": Mapping[str, Mapping[str, str]],
-        "bindingProperties": Mapping[str, "ComponentBindingPropertiesValueTypeDef"],
-        "collectionProperties": Mapping[str, "ComponentDataConfigurationTypeDef"],
-        "events": Mapping[str, "ComponentEventTypeDef"],
-        "schemaVersion": str,
+        "entity": ComponentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateComponentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateComponentRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "componentToCreate": CreateComponentDataTypeDef,
+    },
+)
+_OptionalCreateComponentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateComponentRequestRequestTypeDef",
+    {
+        "clientToken": str,
     },
     total=False,
 )
 
+
+class CreateComponentRequestRequestTypeDef(
+    _RequiredCreateComponentRequestRequestTypeDef, _OptionalCreateComponentRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateComponentRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
-        "updatedComponent": "UpdateComponentDataTypeDef",
+        "updatedComponent": UpdateComponentDataTypeDef,
     },
 )
 _OptionalUpdateComponentRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateComponentRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -2421,194 +2077,275 @@
 
 class UpdateComponentRequestRequestTypeDef(
     _RequiredUpdateComponentRequestRequestTypeDef, _OptionalUpdateComponentRequestRequestTypeDef
 ):
     pass
 
 
-UpdateComponentResponseTypeDef = TypedDict(
-    "UpdateComponentResponseTypeDef",
+_RequiredCodegenJobTypeDef = TypedDict(
+    "_RequiredCodegenJobTypeDef",
     {
-        "entity": "ComponentTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "id": str,
+        "appId": str,
+        "environmentName": str,
     },
 )
-
-UpdateFormDataTypeDef = TypedDict(
-    "UpdateFormDataTypeDef",
+_OptionalCodegenJobTypeDef = TypedDict(
+    "_OptionalCodegenJobTypeDef",
     {
-        "name": str,
-        "dataType": "FormDataTypeConfigTypeDef",
-        "formActionType": FormActionTypeType,
-        "fields": Mapping[str, "FieldConfigTypeDef"],
-        "style": "FormStyleTypeDef",
-        "sectionalElements": Mapping[str, "SectionalElementTypeDef"],
-        "schemaVersion": str,
-        "cta": "FormCTATypeDef",
-        "labelDecorator": LabelDecoratorType,
+        "renderConfig": CodegenJobRenderConfigTypeDef,
+        "genericDataSchema": CodegenJobGenericDataSchemaOutputTypeDef,
+        "autoGenerateForms": bool,
+        "features": CodegenFeatureFlagsTypeDef,
+        "status": CodegenJobStatusType,
+        "statusMessage": str,
+        "asset": CodegenJobAssetTypeDef,
+        "tags": Dict[str, str],
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
     total=False,
 )
 
-_RequiredUpdateFormRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFormRequestRequestTypeDef",
+
+class CodegenJobTypeDef(_RequiredCodegenJobTypeDef, _OptionalCodegenJobTypeDef):
+    pass
+
+
+_RequiredStartCodegenJobDataTypeDef = TypedDict(
+    "_RequiredStartCodegenJobDataTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "updatedForm": "UpdateFormDataTypeDef",
+        "renderConfig": CodegenJobRenderConfigTypeDef,
     },
 )
-_OptionalUpdateFormRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFormRequestRequestTypeDef",
+_OptionalStartCodegenJobDataTypeDef = TypedDict(
+    "_OptionalStartCodegenJobDataTypeDef",
     {
-        "clientToken": str,
+        "genericDataSchema": CodegenJobGenericDataSchemaTypeDef,
+        "autoGenerateForms": bool,
+        "features": CodegenFeatureFlagsTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class UpdateFormRequestRequestTypeDef(
-    _RequiredUpdateFormRequestRequestTypeDef, _OptionalUpdateFormRequestRequestTypeDef
+class StartCodegenJobDataTypeDef(
+    _RequiredStartCodegenJobDataTypeDef, _OptionalStartCodegenJobDataTypeDef
 ):
     pass
 
 
-UpdateFormResponseTypeDef = TypedDict(
-    "UpdateFormResponseTypeDef",
+FieldConfigOutputTypeDef = TypedDict(
+    "FieldConfigOutputTypeDef",
     {
-        "entity": "FormTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "label": str,
+        "position": FieldPositionTypeDef,
+        "excluded": bool,
+        "inputType": FieldInputConfigOutputTypeDef,
+        "validations": List[FieldValidationConfigurationOutputTypeDef],
     },
+    total=False,
 )
 
-_RequiredUpdateThemeDataTypeDef = TypedDict(
-    "_RequiredUpdateThemeDataTypeDef",
+FieldConfigTypeDef = TypedDict(
+    "FieldConfigTypeDef",
     {
-        "values": Sequence["ThemeValuesTypeDef"],
+        "label": str,
+        "position": FieldPositionTypeDef,
+        "excluded": bool,
+        "inputType": FieldInputConfigTypeDef,
+        "validations": Sequence[FieldValidationConfigurationTypeDef],
     },
+    total=False,
 )
-_OptionalUpdateThemeDataTypeDef = TypedDict(
-    "_OptionalUpdateThemeDataTypeDef",
+
+GetCodegenJobResponseTypeDef = TypedDict(
+    "GetCodegenJobResponseTypeDef",
     {
-        "id": str,
-        "name": str,
-        "overrides": Sequence["ThemeValuesTypeDef"],
+        "job": CodegenJobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+StartCodegenJobResponseTypeDef = TypedDict(
+    "StartCodegenJobResponseTypeDef",
+    {
+        "entity": CodegenJobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateThemeDataTypeDef(_RequiredUpdateThemeDataTypeDef, _OptionalUpdateThemeDataTypeDef):
-    pass
-
-
-_RequiredUpdateThemeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateThemeRequestRequestTypeDef",
+_RequiredStartCodegenJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartCodegenJobRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
-        "id": str,
-        "updatedTheme": "UpdateThemeDataTypeDef",
+        "codegenJobToCreate": StartCodegenJobDataTypeDef,
     },
 )
-_OptionalUpdateThemeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateThemeRequestRequestTypeDef",
+_OptionalStartCodegenJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartCodegenJobRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
 
-class UpdateThemeRequestRequestTypeDef(
-    _RequiredUpdateThemeRequestRequestTypeDef, _OptionalUpdateThemeRequestRequestTypeDef
+class StartCodegenJobRequestRequestTypeDef(
+    _RequiredStartCodegenJobRequestRequestTypeDef, _OptionalStartCodegenJobRequestRequestTypeDef
 ):
     pass
 
 
-UpdateThemeResponseTypeDef = TypedDict(
-    "UpdateThemeResponseTypeDef",
+_RequiredFormTypeDef = TypedDict(
+    "_RequiredFormTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "name": str,
+        "formActionType": FormActionTypeType,
+        "style": FormStyleTypeDef,
+        "dataType": FormDataTypeConfigTypeDef,
+        "fields": Dict[str, FieldConfigOutputTypeDef],
+        "sectionalElements": Dict[str, SectionalElementTypeDef],
+        "schemaVersion": str,
+    },
+)
+_OptionalFormTypeDef = TypedDict(
+    "_OptionalFormTypeDef",
     {
-        "entity": "ThemeTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "cta": FormCTATypeDef,
+        "labelDecorator": LabelDecoratorType,
     },
+    total=False,
 )
 
-_RequiredValueMappingOutputTypeDef = TypedDict(
-    "_RequiredValueMappingOutputTypeDef",
+
+class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
+    pass
+
+
+_RequiredCreateFormDataTypeDef = TypedDict(
+    "_RequiredCreateFormDataTypeDef",
     {
-        "value": "FormInputValuePropertyOutputTypeDef",
+        "name": str,
+        "dataType": FormDataTypeConfigTypeDef,
+        "formActionType": FormActionTypeType,
+        "fields": Mapping[str, FieldConfigTypeDef],
+        "style": FormStyleTypeDef,
+        "sectionalElements": Mapping[str, SectionalElementTypeDef],
+        "schemaVersion": str,
     },
 )
-_OptionalValueMappingOutputTypeDef = TypedDict(
-    "_OptionalValueMappingOutputTypeDef",
+_OptionalCreateFormDataTypeDef = TypedDict(
+    "_OptionalCreateFormDataTypeDef",
     {
-        "displayValue": "FormInputValuePropertyOutputTypeDef",
+        "cta": FormCTATypeDef,
+        "tags": Mapping[str, str],
+        "labelDecorator": LabelDecoratorType,
     },
     total=False,
 )
 
 
-class ValueMappingOutputTypeDef(
-    _RequiredValueMappingOutputTypeDef, _OptionalValueMappingOutputTypeDef
-):
+class CreateFormDataTypeDef(_RequiredCreateFormDataTypeDef, _OptionalCreateFormDataTypeDef):
     pass
 
 
-_RequiredValueMappingTypeDef = TypedDict(
-    "_RequiredValueMappingTypeDef",
+UpdateFormDataTypeDef = TypedDict(
+    "UpdateFormDataTypeDef",
     {
-        "value": "FormInputValuePropertyTypeDef",
+        "name": str,
+        "dataType": FormDataTypeConfigTypeDef,
+        "formActionType": FormActionTypeType,
+        "fields": Mapping[str, FieldConfigTypeDef],
+        "style": FormStyleTypeDef,
+        "sectionalElements": Mapping[str, SectionalElementTypeDef],
+        "schemaVersion": str,
+        "cta": FormCTATypeDef,
+        "labelDecorator": LabelDecoratorType,
     },
+    total=False,
 )
-_OptionalValueMappingTypeDef = TypedDict(
-    "_OptionalValueMappingTypeDef",
+
+CreateFormResponseTypeDef = TypedDict(
+    "CreateFormResponseTypeDef",
     {
-        "displayValue": "FormInputValuePropertyTypeDef",
+        "entity": FormTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ExportFormsResponseTypeDef = TypedDict(
+    "ExportFormsResponseTypeDef",
+    {
+        "entities": List[FormTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ValueMappingTypeDef(_RequiredValueMappingTypeDef, _OptionalValueMappingTypeDef):
-    pass
+GetFormResponseTypeDef = TypedDict(
+    "GetFormResponseTypeDef",
+    {
+        "form": FormTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateFormResponseTypeDef = TypedDict(
+    "UpdateFormResponseTypeDef",
+    {
+        "entity": FormTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredValueMappingsOutputTypeDef = TypedDict(
-    "_RequiredValueMappingsOutputTypeDef",
+_RequiredCreateFormRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFormRequestRequestTypeDef",
     {
-        "values": List["ValueMappingOutputTypeDef"],
+        "appId": str,
+        "environmentName": str,
+        "formToCreate": CreateFormDataTypeDef,
     },
 )
-_OptionalValueMappingsOutputTypeDef = TypedDict(
-    "_OptionalValueMappingsOutputTypeDef",
+_OptionalCreateFormRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFormRequestRequestTypeDef",
     {
-        "bindingProperties": Dict[str, "FormInputBindingPropertiesValueOutputTypeDef"],
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class ValueMappingsOutputTypeDef(
-    _RequiredValueMappingsOutputTypeDef, _OptionalValueMappingsOutputTypeDef
+class CreateFormRequestRequestTypeDef(
+    _RequiredCreateFormRequestRequestTypeDef, _OptionalCreateFormRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredValueMappingsTypeDef = TypedDict(
-    "_RequiredValueMappingsTypeDef",
+_RequiredUpdateFormRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFormRequestRequestTypeDef",
     {
-        "values": Sequence["ValueMappingTypeDef"],
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "updatedForm": UpdateFormDataTypeDef,
     },
 )
-_OptionalValueMappingsTypeDef = TypedDict(
-    "_OptionalValueMappingsTypeDef",
+_OptionalUpdateFormRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFormRequestRequestTypeDef",
     {
-        "bindingProperties": Mapping[str, "FormInputBindingPropertiesValueTypeDef"],
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class ValueMappingsTypeDef(_RequiredValueMappingsTypeDef, _OptionalValueMappingsTypeDef):
+class UpdateFormRequestRequestTypeDef(
+    _RequiredUpdateFormRequestRequestTypeDef, _OptionalUpdateFormRequestRequestTypeDef
+):
     pass
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder/type_defs.pyi` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplifyuibuilder service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplifyuibuilder.type_defs import ActionParametersOutputTypeDef
+    from mypy_boto3_amplifyuibuilder.type_defs import MutationActionSetStateParameterTypeDef
 
-    data: ActionParametersOutputTypeDef = {...}
+    data: MutationActionSetStateParameterTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -36,214 +36,162 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ActionParametersOutputTypeDef",
-    "ActionParametersTypeDef",
-    "CodegenFeatureFlagsOutputTypeDef",
+    "MutationActionSetStateParameterTypeDef",
     "CodegenFeatureFlagsTypeDef",
     "CodegenGenericDataEnumOutputTypeDef",
     "CodegenGenericDataEnumTypeDef",
-    "CodegenGenericDataFieldOutputTypeDef",
-    "CodegenGenericDataFieldTypeDef",
-    "CodegenGenericDataModelOutputTypeDef",
-    "CodegenGenericDataModelTypeDef",
-    "CodegenGenericDataNonModelOutputTypeDef",
-    "CodegenGenericDataNonModelTypeDef",
     "CodegenGenericDataRelationshipTypeOutputTypeDef",
     "CodegenGenericDataRelationshipTypeTypeDef",
     "CodegenJobAssetTypeDef",
-    "CodegenJobGenericDataSchemaOutputTypeDef",
-    "CodegenJobGenericDataSchemaTypeDef",
-    "CodegenJobRenderConfigOutputTypeDef",
-    "CodegenJobRenderConfigTypeDef",
+    "ReactStartCodegenJobDataTypeDef",
     "CodegenJobSummaryTypeDef",
-    "CodegenJobTypeDef",
-    "ComponentBindingPropertiesValueOutputTypeDef",
     "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
-    "ComponentBindingPropertiesValueTypeDef",
-    "ComponentChildOutputTypeDef",
-    "ComponentChildTypeDef",
-    "ComponentConditionPropertyOutputTypeDef",
     "ComponentConditionPropertyTypeDef",
-    "ComponentDataConfigurationOutputTypeDef",
-    "ComponentDataConfigurationTypeDef",
-    "ComponentEventOutputTypeDef",
-    "ComponentEventTypeDef",
-    "ComponentPropertyBindingPropertiesOutputTypeDef",
+    "SortPropertyTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
-    "ComponentPropertyOutputTypeDef",
-    "ComponentPropertyTypeDef",
+    "FormBindingElementTypeDef",
     "ComponentSummaryTypeDef",
-    "ComponentTypeDef",
     "ComponentVariantOutputTypeDef",
     "ComponentVariantTypeDef",
-    "CreateComponentDataTypeDef",
-    "CreateComponentRequestRequestTypeDef",
-    "CreateComponentResponseTypeDef",
-    "CreateFormDataTypeDef",
-    "CreateFormRequestRequestTypeDef",
-    "CreateFormResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "FormDataTypeConfigTypeDef",
     "CreateThemeDataTypeDef",
-    "CreateThemeRequestRequestTypeDef",
-    "CreateThemeResponseTypeDef",
+    "ThemeTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteFormRequestRequestTypeDef",
     "DeleteThemeRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExchangeCodeForTokenRequestBodyTypeDef",
-    "ExchangeCodeForTokenRequestRequestTypeDef",
-    "ExchangeCodeForTokenResponseTypeDef",
-    "ExportComponentsRequestExportComponentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ExportComponentsRequestRequestTypeDef",
-    "ExportComponentsResponseTypeDef",
-    "ExportFormsRequestExportFormsPaginateTypeDef",
     "ExportFormsRequestRequestTypeDef",
-    "ExportFormsResponseTypeDef",
-    "ExportThemesRequestExportThemesPaginateTypeDef",
     "ExportThemesRequestRequestTypeDef",
-    "ExportThemesResponseTypeDef",
-    "FieldConfigOutputTypeDef",
-    "FieldConfigTypeDef",
-    "FieldInputConfigOutputTypeDef",
-    "FieldInputConfigTypeDef",
-    "FieldPositionOutputTypeDef",
     "FieldPositionTypeDef",
     "FieldValidationConfigurationOutputTypeDef",
     "FieldValidationConfigurationTypeDef",
     "FileUploaderFieldConfigOutputTypeDef",
     "FileUploaderFieldConfigTypeDef",
-    "FormBindingElementOutputTypeDef",
-    "FormBindingElementTypeDef",
-    "FormButtonOutputTypeDef",
-    "FormButtonTypeDef",
-    "FormCTAOutputTypeDef",
-    "FormCTATypeDef",
-    "FormDataTypeConfigOutputTypeDef",
-    "FormDataTypeConfigTypeDef",
-    "FormInputBindingPropertiesValueOutputTypeDef",
-    "FormInputBindingPropertiesValuePropertiesOutputTypeDef",
     "FormInputBindingPropertiesValuePropertiesTypeDef",
-    "FormInputBindingPropertiesValueTypeDef",
-    "FormInputValuePropertyBindingPropertiesOutputTypeDef",
     "FormInputValuePropertyBindingPropertiesTypeDef",
-    "FormInputValuePropertyOutputTypeDef",
-    "FormInputValuePropertyTypeDef",
-    "FormStyleConfigOutputTypeDef",
     "FormStyleConfigTypeDef",
-    "FormStyleOutputTypeDef",
-    "FormStyleTypeDef",
-    "FormSummaryTypeDef",
-    "FormTypeDef",
     "GetCodegenJobRequestRequestTypeDef",
-    "GetCodegenJobResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
-    "GetComponentResponseTypeDef",
     "GetFormRequestRequestTypeDef",
-    "GetFormResponseTypeDef",
     "GetMetadataRequestRequestTypeDef",
-    "GetMetadataResponseTypeDef",
     "GetThemeRequestRequestTypeDef",
-    "GetThemeResponseTypeDef",
-    "ListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
     "ListCodegenJobsRequestRequestTypeDef",
-    "ListCodegenJobsResponseTypeDef",
-    "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListComponentsRequestRequestTypeDef",
-    "ListComponentsResponseTypeDef",
-    "ListFormsRequestListFormsPaginateTypeDef",
     "ListFormsRequestRequestTypeDef",
-    "ListFormsResponseTypeDef",
-    "ListThemesRequestListThemesPaginateTypeDef",
     "ListThemesRequestRequestTypeDef",
-    "ListThemesResponseTypeDef",
-    "MutationActionSetStateParameterOutputTypeDef",
-    "MutationActionSetStateParameterTypeDef",
-    "PaginatorConfigTypeDef",
+    "ThemeSummaryTypeDef",
     "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "PutMetadataFlagBodyTypeDef",
-    "PutMetadataFlagRequestRequestTypeDef",
-    "ReactStartCodegenJobDataOutputTypeDef",
-    "ReactStartCodegenJobDataTypeDef",
     "RefreshTokenRequestBodyTypeDef",
-    "RefreshTokenRequestRequestTypeDef",
-    "RefreshTokenResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "SectionalElementOutputTypeDef",
-    "SectionalElementTypeDef",
-    "SortPropertyOutputTypeDef",
-    "SortPropertyTypeDef",
-    "StartCodegenJobDataTypeDef",
-    "StartCodegenJobRequestRequestTypeDef",
-    "StartCodegenJobResponseTypeDef",
-    "ThemeSummaryTypeDef",
-    "ThemeTypeDef",
     "ThemeValueOutputTypeDef",
     "ThemeValueTypeDef",
     "ThemeValuesOutputTypeDef",
     "ThemeValuesTypeDef",
-    "UpdateComponentDataTypeDef",
-    "UpdateComponentRequestRequestTypeDef",
-    "UpdateComponentResponseTypeDef",
-    "UpdateFormDataTypeDef",
-    "UpdateFormRequestRequestTypeDef",
-    "UpdateFormResponseTypeDef",
     "UpdateThemeDataTypeDef",
-    "UpdateThemeRequestRequestTypeDef",
-    "UpdateThemeResponseTypeDef",
-    "ValueMappingOutputTypeDef",
     "ValueMappingTypeDef",
-    "ValueMappingsOutputTypeDef",
-    "ValueMappingsTypeDef",
-)
-
-ActionParametersOutputTypeDef = TypedDict(
     "ActionParametersOutputTypeDef",
-    {
-        "type": "ComponentPropertyOutputTypeDef",
-        "url": "ComponentPropertyOutputTypeDef",
-        "anchor": "ComponentPropertyOutputTypeDef",
-        "target": "ComponentPropertyOutputTypeDef",
-        "global": "ComponentPropertyOutputTypeDef",
-        "model": str,
-        "id": "ComponentPropertyOutputTypeDef",
-        "fields": Dict[str, "ComponentPropertyOutputTypeDef"],
-        "state": "MutationActionSetStateParameterOutputTypeDef",
-    },
-    total=False,
-)
-
-ActionParametersTypeDef = TypedDict(
     "ActionParametersTypeDef",
-    {
-        "type": "ComponentPropertyTypeDef",
-        "url": "ComponentPropertyTypeDef",
-        "anchor": "ComponentPropertyTypeDef",
-        "target": "ComponentPropertyTypeDef",
-        "global": "ComponentPropertyTypeDef",
-        "model": str,
-        "id": "ComponentPropertyTypeDef",
-        "fields": Mapping[str, "ComponentPropertyTypeDef"],
-        "state": "MutationActionSetStateParameterTypeDef",
-    },
-    total=False,
+    "CodegenGenericDataFieldOutputTypeDef",
+    "CodegenGenericDataFieldTypeDef",
+    "CodegenJobRenderConfigTypeDef",
+    "ComponentBindingPropertiesValueOutputTypeDef",
+    "ComponentBindingPropertiesValueTypeDef",
+    "ComponentDataConfigurationOutputTypeDef",
+    "ComponentDataConfigurationTypeDef",
+    "ComponentPropertyOutputTypeDef",
+    "ComponentPropertyTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExchangeCodeForTokenResponseTypeDef",
+    "GetMetadataResponseTypeDef",
+    "ListCodegenJobsResponseTypeDef",
+    "ListComponentsResponseTypeDef",
+    "RefreshTokenResponseTypeDef",
+    "FormSummaryTypeDef",
+    "CreateThemeRequestRequestTypeDef",
+    "CreateThemeResponseTypeDef",
+    "ExportThemesResponseTypeDef",
+    "GetThemeResponseTypeDef",
+    "UpdateThemeResponseTypeDef",
+    "ExchangeCodeForTokenRequestRequestTypeDef",
+    "ExportComponentsRequestExportComponentsPaginateTypeDef",
+    "ExportFormsRequestExportFormsPaginateTypeDef",
+    "ExportThemesRequestExportThemesPaginateTypeDef",
+    "ListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+    "ListComponentsRequestListComponentsPaginateTypeDef",
+    "ListFormsRequestListFormsPaginateTypeDef",
+    "ListThemesRequestListThemesPaginateTypeDef",
+    "FormButtonTypeDef",
+    "SectionalElementTypeDef",
+    "FormInputBindingPropertiesValueTypeDef",
+    "FormInputValuePropertyTypeDef",
+    "FormStyleTypeDef",
+    "ListThemesResponseTypeDef",
+    "PutMetadataFlagRequestRequestTypeDef",
+    "RefreshTokenRequestRequestTypeDef",
+    "UpdateThemeRequestRequestTypeDef",
+    "ComponentEventOutputTypeDef",
+    "ComponentEventTypeDef",
+    "CodegenGenericDataModelOutputTypeDef",
+    "CodegenGenericDataNonModelOutputTypeDef",
+    "CodegenGenericDataModelTypeDef",
+    "CodegenGenericDataNonModelTypeDef",
+    "ListFormsResponseTypeDef",
+    "FormCTATypeDef",
+    "ValueMappingsOutputTypeDef",
+    "ValueMappingsTypeDef",
+    "ComponentChildOutputTypeDef",
+    "ComponentTypeDef",
+    "ComponentChildTypeDef",
+    "CreateComponentDataTypeDef",
+    "UpdateComponentDataTypeDef",
+    "CodegenJobGenericDataSchemaOutputTypeDef",
+    "CodegenJobGenericDataSchemaTypeDef",
+    "FieldInputConfigOutputTypeDef",
+    "FieldInputConfigTypeDef",
+    "CreateComponentResponseTypeDef",
+    "ExportComponentsResponseTypeDef",
+    "GetComponentResponseTypeDef",
+    "UpdateComponentResponseTypeDef",
+    "CreateComponentRequestRequestTypeDef",
+    "UpdateComponentRequestRequestTypeDef",
+    "CodegenJobTypeDef",
+    "StartCodegenJobDataTypeDef",
+    "FieldConfigOutputTypeDef",
+    "FieldConfigTypeDef",
+    "GetCodegenJobResponseTypeDef",
+    "StartCodegenJobResponseTypeDef",
+    "StartCodegenJobRequestRequestTypeDef",
+    "FormTypeDef",
+    "CreateFormDataTypeDef",
+    "UpdateFormDataTypeDef",
+    "CreateFormResponseTypeDef",
+    "ExportFormsResponseTypeDef",
+    "GetFormResponseTypeDef",
+    "UpdateFormResponseTypeDef",
+    "CreateFormRequestRequestTypeDef",
+    "UpdateFormRequestRequestTypeDef",
 )
 
-CodegenFeatureFlagsOutputTypeDef = TypedDict(
-    "CodegenFeatureFlagsOutputTypeDef",
+MutationActionSetStateParameterTypeDef = TypedDict(
+    "MutationActionSetStateParameterTypeDef",
     {
-        "isRelationshipSupported": bool,
-        "isNonModelSupported": bool,
+        "componentName": str,
+        "property": str,
+        "set": "ComponentPropertyTypeDef",
     },
-    total=False,
 )
 
 CodegenFeatureFlagsTypeDef = TypedDict(
     "CodegenFeatureFlagsTypeDef",
     {
         "isRelationshipSupported": bool,
         "isNonModelSupported": bool,
@@ -261,114 +209,14 @@
 CodegenGenericDataEnumTypeDef = TypedDict(
     "CodegenGenericDataEnumTypeDef",
     {
         "values": Sequence[str],
     },
 )
 
-_RequiredCodegenGenericDataFieldOutputTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataFieldOutputTypeDef",
-    {
-        "dataType": CodegenGenericDataFieldDataTypeType,
-        "dataTypeValue": str,
-        "required": bool,
-        "readOnly": bool,
-        "isArray": bool,
-    },
-)
-_OptionalCodegenGenericDataFieldOutputTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataFieldOutputTypeDef",
-    {
-        "relationship": "CodegenGenericDataRelationshipTypeOutputTypeDef",
-    },
-    total=False,
-)
-
-class CodegenGenericDataFieldOutputTypeDef(
-    _RequiredCodegenGenericDataFieldOutputTypeDef, _OptionalCodegenGenericDataFieldOutputTypeDef
-):
-    pass
-
-_RequiredCodegenGenericDataFieldTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataFieldTypeDef",
-    {
-        "dataType": CodegenGenericDataFieldDataTypeType,
-        "dataTypeValue": str,
-        "required": bool,
-        "readOnly": bool,
-        "isArray": bool,
-    },
-)
-_OptionalCodegenGenericDataFieldTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataFieldTypeDef",
-    {
-        "relationship": "CodegenGenericDataRelationshipTypeTypeDef",
-    },
-    total=False,
-)
-
-class CodegenGenericDataFieldTypeDef(
-    _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
-):
-    pass
-
-_RequiredCodegenGenericDataModelOutputTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataModelOutputTypeDef",
-    {
-        "fields": Dict[str, "CodegenGenericDataFieldOutputTypeDef"],
-        "primaryKeys": List[str],
-    },
-)
-_OptionalCodegenGenericDataModelOutputTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataModelOutputTypeDef",
-    {
-        "isJoinTable": bool,
-    },
-    total=False,
-)
-
-class CodegenGenericDataModelOutputTypeDef(
-    _RequiredCodegenGenericDataModelOutputTypeDef, _OptionalCodegenGenericDataModelOutputTypeDef
-):
-    pass
-
-_RequiredCodegenGenericDataModelTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataModelTypeDef",
-    {
-        "fields": Mapping[str, "CodegenGenericDataFieldTypeDef"],
-        "primaryKeys": Sequence[str],
-    },
-)
-_OptionalCodegenGenericDataModelTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataModelTypeDef",
-    {
-        "isJoinTable": bool,
-    },
-    total=False,
-)
-
-class CodegenGenericDataModelTypeDef(
-    _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
-):
-    pass
-
-CodegenGenericDataNonModelOutputTypeDef = TypedDict(
-    "CodegenGenericDataNonModelOutputTypeDef",
-    {
-        "fields": Dict[str, "CodegenGenericDataFieldOutputTypeDef"],
-    },
-)
-
-CodegenGenericDataNonModelTypeDef = TypedDict(
-    "CodegenGenericDataNonModelTypeDef",
-    {
-        "fields": Mapping[str, "CodegenGenericDataFieldTypeDef"],
-    },
-)
-
 _RequiredCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
     "_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef",
     {
         "type": GenericDataRelationshipTypeType,
         "relatedModelName": str,
     },
 )
@@ -423,46 +271,22 @@
     "CodegenJobAssetTypeDef",
     {
         "downloadUrl": str,
     },
     total=False,
 )
 
-CodegenJobGenericDataSchemaOutputTypeDef = TypedDict(
-    "CodegenJobGenericDataSchemaOutputTypeDef",
-    {
-        "dataSourceType": Literal["DataStore"],
-        "models": Dict[str, "CodegenGenericDataModelOutputTypeDef"],
-        "enums": Dict[str, "CodegenGenericDataEnumOutputTypeDef"],
-        "nonModels": Dict[str, "CodegenGenericDataNonModelOutputTypeDef"],
-    },
-)
-
-CodegenJobGenericDataSchemaTypeDef = TypedDict(
-    "CodegenJobGenericDataSchemaTypeDef",
-    {
-        "dataSourceType": Literal["DataStore"],
-        "models": Mapping[str, "CodegenGenericDataModelTypeDef"],
-        "enums": Mapping[str, "CodegenGenericDataEnumTypeDef"],
-        "nonModels": Mapping[str, "CodegenGenericDataNonModelTypeDef"],
-    },
-)
-
-CodegenJobRenderConfigOutputTypeDef = TypedDict(
-    "CodegenJobRenderConfigOutputTypeDef",
-    {
-        "react": "ReactStartCodegenJobDataOutputTypeDef",
-    },
-    total=False,
-)
-
-CodegenJobRenderConfigTypeDef = TypedDict(
-    "CodegenJobRenderConfigTypeDef",
+ReactStartCodegenJobDataTypeDef = TypedDict(
+    "ReactStartCodegenJobDataTypeDef",
     {
-        "react": "ReactStartCodegenJobDataTypeDef",
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
     },
     total=False,
 )
 
 _RequiredCodegenJobSummaryTypeDef = TypedDict(
     "_RequiredCodegenJobSummaryTypeDef",
     {
@@ -481,52 +305,14 @@
 )
 
 class CodegenJobSummaryTypeDef(
     _RequiredCodegenJobSummaryTypeDef, _OptionalCodegenJobSummaryTypeDef
 ):
     pass
 
-_RequiredCodegenJobTypeDef = TypedDict(
-    "_RequiredCodegenJobTypeDef",
-    {
-        "id": str,
-        "appId": str,
-        "environmentName": str,
-    },
-)
-_OptionalCodegenJobTypeDef = TypedDict(
-    "_OptionalCodegenJobTypeDef",
-    {
-        "renderConfig": "CodegenJobRenderConfigOutputTypeDef",
-        "genericDataSchema": "CodegenJobGenericDataSchemaOutputTypeDef",
-        "autoGenerateForms": bool,
-        "features": "CodegenFeatureFlagsOutputTypeDef",
-        "status": CodegenJobStatusType,
-        "statusMessage": str,
-        "asset": "CodegenJobAssetTypeDef",
-        "tags": Dict[str, str],
-        "createdAt": datetime,
-        "modifiedAt": datetime,
-    },
-    total=False,
-)
-
-class CodegenJobTypeDef(_RequiredCodegenJobTypeDef, _OptionalCodegenJobTypeDef):
-    pass
-
-ComponentBindingPropertiesValueOutputTypeDef = TypedDict(
-    "ComponentBindingPropertiesValueOutputTypeDef",
-    {
-        "type": str,
-        "bindingProperties": "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
-        "defaultValue": str,
-    },
-    total=False,
-)
-
 ComponentBindingPropertiesValuePropertiesOutputTypeDef = TypedDict(
     "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     {
         "model": str,
         "field": str,
         "predicates": List["PredicateOutputTypeDef"],
         "userAttribute": str,
@@ -549,179 +335,36 @@
         "key": str,
         "defaultValue": str,
         "slotName": str,
     },
     total=False,
 )
 
-ComponentBindingPropertiesValueTypeDef = TypedDict(
-    "ComponentBindingPropertiesValueTypeDef",
-    {
-        "type": str,
-        "bindingProperties": "ComponentBindingPropertiesValuePropertiesTypeDef",
-        "defaultValue": str,
-    },
-    total=False,
-)
-
-_RequiredComponentChildOutputTypeDef = TypedDict(
-    "_RequiredComponentChildOutputTypeDef",
-    {
-        "componentType": str,
-        "name": str,
-        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
-    },
-)
-_OptionalComponentChildOutputTypeDef = TypedDict(
-    "_OptionalComponentChildOutputTypeDef",
-    {
-        "children": List[Dict[str, Any]],
-        "events": Dict[str, "ComponentEventOutputTypeDef"],
-        "sourceId": str,
-    },
-    total=False,
-)
-
-class ComponentChildOutputTypeDef(
-    _RequiredComponentChildOutputTypeDef, _OptionalComponentChildOutputTypeDef
-):
-    pass
-
-_RequiredComponentChildTypeDef = TypedDict(
-    "_RequiredComponentChildTypeDef",
-    {
-        "componentType": str,
-        "name": str,
-        "properties": Mapping[str, "ComponentPropertyTypeDef"],
-    },
-)
-_OptionalComponentChildTypeDef = TypedDict(
-    "_OptionalComponentChildTypeDef",
-    {
-        "children": Sequence[Dict[str, Any]],
-        "events": Mapping[str, "ComponentEventTypeDef"],
-        "sourceId": str,
-    },
-    total=False,
-)
-
-class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
-    pass
-
-ComponentConditionPropertyOutputTypeDef = TypedDict(
-    "ComponentConditionPropertyOutputTypeDef",
-    {
-        "property": str,
-        "field": str,
-        "operator": str,
-        "operand": str,
-        "then": Dict[str, Any],
-        "else": Dict[str, Any],
-        "operandType": str,
-    },
-    total=False,
-)
-
 ComponentConditionPropertyTypeDef = TypedDict(
     "ComponentConditionPropertyTypeDef",
     {
         "property": str,
         "field": str,
         "operator": str,
         "operand": str,
-        "then": Dict[str, Any],
-        "else": Dict[str, Any],
+        "then": "ComponentPropertyTypeDef",
+        "else": "ComponentPropertyTypeDef",
         "operandType": str,
     },
     total=False,
 )
 
-_RequiredComponentDataConfigurationOutputTypeDef = TypedDict(
-    "_RequiredComponentDataConfigurationOutputTypeDef",
-    {
-        "model": str,
-    },
-)
-_OptionalComponentDataConfigurationOutputTypeDef = TypedDict(
-    "_OptionalComponentDataConfigurationOutputTypeDef",
-    {
-        "sort": List["SortPropertyOutputTypeDef"],
-        "predicate": "PredicateOutputTypeDef",
-        "identifiers": List[str],
-    },
-    total=False,
-)
-
-class ComponentDataConfigurationOutputTypeDef(
-    _RequiredComponentDataConfigurationOutputTypeDef,
-    _OptionalComponentDataConfigurationOutputTypeDef,
-):
-    pass
-
-_RequiredComponentDataConfigurationTypeDef = TypedDict(
-    "_RequiredComponentDataConfigurationTypeDef",
-    {
-        "model": str,
-    },
-)
-_OptionalComponentDataConfigurationTypeDef = TypedDict(
-    "_OptionalComponentDataConfigurationTypeDef",
-    {
-        "sort": Sequence["SortPropertyTypeDef"],
-        "predicate": "PredicateTypeDef",
-        "identifiers": Sequence[str],
-    },
-    total=False,
-)
-
-class ComponentDataConfigurationTypeDef(
-    _RequiredComponentDataConfigurationTypeDef, _OptionalComponentDataConfigurationTypeDef
-):
-    pass
-
-ComponentEventOutputTypeDef = TypedDict(
-    "ComponentEventOutputTypeDef",
-    {
-        "action": str,
-        "parameters": "ActionParametersOutputTypeDef",
-        "bindingEvent": str,
-    },
-    total=False,
-)
-
-ComponentEventTypeDef = TypedDict(
-    "ComponentEventTypeDef",
-    {
-        "action": str,
-        "parameters": "ActionParametersTypeDef",
-        "bindingEvent": str,
-    },
-    total=False,
-)
-
-_RequiredComponentPropertyBindingPropertiesOutputTypeDef = TypedDict(
-    "_RequiredComponentPropertyBindingPropertiesOutputTypeDef",
-    {
-        "property": str,
-    },
-)
-_OptionalComponentPropertyBindingPropertiesOutputTypeDef = TypedDict(
-    "_OptionalComponentPropertyBindingPropertiesOutputTypeDef",
+SortPropertyTypeDef = TypedDict(
+    "SortPropertyTypeDef",
     {
         "field": str,
+        "direction": SortDirectionType,
     },
-    total=False,
 )
 
-class ComponentPropertyBindingPropertiesOutputTypeDef(
-    _RequiredComponentPropertyBindingPropertiesOutputTypeDef,
-    _OptionalComponentPropertyBindingPropertiesOutputTypeDef,
-):
-    pass
-
 _RequiredComponentPropertyBindingPropertiesTypeDef = TypedDict(
     "_RequiredComponentPropertyBindingPropertiesTypeDef",
     {
         "property": str,
     },
 )
 _OptionalComponentPropertyBindingPropertiesTypeDef = TypedDict(
@@ -734,101 +377,33 @@
 
 class ComponentPropertyBindingPropertiesTypeDef(
     _RequiredComponentPropertyBindingPropertiesTypeDef,
     _OptionalComponentPropertyBindingPropertiesTypeDef,
 ):
     pass
 
-ComponentPropertyOutputTypeDef = TypedDict(
-    "ComponentPropertyOutputTypeDef",
-    {
-        "value": str,
-        "bindingProperties": "ComponentPropertyBindingPropertiesOutputTypeDef",
-        "collectionBindingProperties": "ComponentPropertyBindingPropertiesOutputTypeDef",
-        "defaultValue": str,
-        "model": str,
-        "bindings": Dict[str, "FormBindingElementOutputTypeDef"],
-        "event": str,
-        "userAttribute": str,
-        "concat": List[Dict[str, Any]],
-        "condition": Dict[str, Any],
-        "configured": bool,
-        "type": str,
-        "importedValue": str,
-        "componentName": str,
-        "property": str,
-    },
-    total=False,
-)
-
-ComponentPropertyTypeDef = TypedDict(
-    "ComponentPropertyTypeDef",
+FormBindingElementTypeDef = TypedDict(
+    "FormBindingElementTypeDef",
     {
-        "value": str,
-        "bindingProperties": "ComponentPropertyBindingPropertiesTypeDef",
-        "collectionBindingProperties": "ComponentPropertyBindingPropertiesTypeDef",
-        "defaultValue": str,
-        "model": str,
-        "bindings": Mapping[str, "FormBindingElementTypeDef"],
-        "event": str,
-        "userAttribute": str,
-        "concat": Sequence[Dict[str, Any]],
-        "condition": Dict[str, Any],
-        "configured": bool,
-        "type": str,
-        "importedValue": str,
-        "componentName": str,
+        "element": str,
         "property": str,
     },
-    total=False,
 )
 
 ComponentSummaryTypeDef = TypedDict(
     "ComponentSummaryTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "componentType": str,
     },
 )
 
-_RequiredComponentTypeDef = TypedDict(
-    "_RequiredComponentTypeDef",
-    {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "name": str,
-        "componentType": str,
-        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
-        "variants": List["ComponentVariantOutputTypeDef"],
-        "overrides": Dict[str, Dict[str, str]],
-        "bindingProperties": Dict[str, "ComponentBindingPropertiesValueOutputTypeDef"],
-        "createdAt": datetime,
-    },
-)
-_OptionalComponentTypeDef = TypedDict(
-    "_OptionalComponentTypeDef",
-    {
-        "sourceId": str,
-        "children": List["ComponentChildOutputTypeDef"],
-        "collectionProperties": Dict[str, "ComponentDataConfigurationOutputTypeDef"],
-        "modifiedAt": datetime,
-        "tags": Dict[str, str],
-        "events": Dict[str, "ComponentEventOutputTypeDef"],
-        "schemaVersion": str,
-    },
-    total=False,
-)
-
-class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
-    pass
-
 ComponentVariantOutputTypeDef = TypedDict(
     "ComponentVariantOutputTypeDef",
     {
         "variantValues": Dict[str, str],
         "overrides": Dict[str, Dict[str, str]],
     },
     total=False,
@@ -839,123 +414,30 @@
     {
         "variantValues": Mapping[str, str],
         "overrides": Mapping[str, Mapping[str, str]],
     },
     total=False,
 )
 
-_RequiredCreateComponentDataTypeDef = TypedDict(
-    "_RequiredCreateComponentDataTypeDef",
-    {
-        "name": str,
-        "componentType": str,
-        "properties": Mapping[str, "ComponentPropertyTypeDef"],
-        "variants": Sequence["ComponentVariantTypeDef"],
-        "overrides": Mapping[str, Mapping[str, str]],
-        "bindingProperties": Mapping[str, "ComponentBindingPropertiesValueTypeDef"],
-    },
-)
-_OptionalCreateComponentDataTypeDef = TypedDict(
-    "_OptionalCreateComponentDataTypeDef",
-    {
-        "sourceId": str,
-        "children": Sequence["ComponentChildTypeDef"],
-        "collectionProperties": Mapping[str, "ComponentDataConfigurationTypeDef"],
-        "tags": Mapping[str, str],
-        "events": Mapping[str, "ComponentEventTypeDef"],
-        "schemaVersion": str,
-    },
-    total=False,
-)
-
-class CreateComponentDataTypeDef(
-    _RequiredCreateComponentDataTypeDef, _OptionalCreateComponentDataTypeDef
-):
-    pass
-
-_RequiredCreateComponentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateComponentRequestRequestTypeDef",
-    {
-        "appId": str,
-        "environmentName": str,
-        "componentToCreate": "CreateComponentDataTypeDef",
-    },
-)
-_OptionalCreateComponentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateComponentRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class CreateComponentRequestRequestTypeDef(
-    _RequiredCreateComponentRequestRequestTypeDef, _OptionalCreateComponentRequestRequestTypeDef
-):
-    pass
-
-CreateComponentResponseTypeDef = TypedDict(
-    "CreateComponentResponseTypeDef",
-    {
-        "entity": "ComponentTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateFormDataTypeDef = TypedDict(
-    "_RequiredCreateFormDataTypeDef",
-    {
-        "name": str,
-        "dataType": "FormDataTypeConfigTypeDef",
-        "formActionType": FormActionTypeType,
-        "fields": Mapping[str, "FieldConfigTypeDef"],
-        "style": "FormStyleTypeDef",
-        "sectionalElements": Mapping[str, "SectionalElementTypeDef"],
-        "schemaVersion": str,
-    },
-)
-_OptionalCreateFormDataTypeDef = TypedDict(
-    "_OptionalCreateFormDataTypeDef",
-    {
-        "cta": "FormCTATypeDef",
-        "tags": Mapping[str, str],
-        "labelDecorator": LabelDecoratorType,
-    },
-    total=False,
-)
-
-class CreateFormDataTypeDef(_RequiredCreateFormDataTypeDef, _OptionalCreateFormDataTypeDef):
-    pass
-
-_RequiredCreateFormRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFormRequestRequestTypeDef",
-    {
-        "appId": str,
-        "environmentName": str,
-        "formToCreate": "CreateFormDataTypeDef",
-    },
-)
-_OptionalCreateFormRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFormRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "clientToken": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class CreateFormRequestRequestTypeDef(
-    _RequiredCreateFormRequestRequestTypeDef, _OptionalCreateFormRequestRequestTypeDef
-):
-    pass
-
-CreateFormResponseTypeDef = TypedDict(
-    "CreateFormResponseTypeDef",
+FormDataTypeConfigTypeDef = TypedDict(
+    "FormDataTypeConfigTypeDef",
     {
-        "entity": "FormTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "dataSourceType": FormDataSourceTypeType,
+        "dataTypeName": str,
     },
 )
 
 _RequiredCreateThemeDataTypeDef = TypedDict(
     "_RequiredCreateThemeDataTypeDef",
     {
         "name": str,
@@ -970,43 +452,38 @@
     },
     total=False,
 )
 
 class CreateThemeDataTypeDef(_RequiredCreateThemeDataTypeDef, _OptionalCreateThemeDataTypeDef):
     pass
 
-_RequiredCreateThemeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateThemeRequestRequestTypeDef",
+_RequiredThemeTypeDef = TypedDict(
+    "_RequiredThemeTypeDef",
     {
         "appId": str,
         "environmentName": str,
-        "themeToCreate": "CreateThemeDataTypeDef",
+        "id": str,
+        "name": str,
+        "createdAt": datetime,
+        "values": List["ThemeValuesOutputTypeDef"],
     },
 )
-_OptionalCreateThemeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateThemeRequestRequestTypeDef",
+_OptionalThemeTypeDef = TypedDict(
+    "_OptionalThemeTypeDef",
     {
-        "clientToken": str,
+        "modifiedAt": datetime,
+        "overrides": List["ThemeValuesOutputTypeDef"],
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
-class CreateThemeRequestRequestTypeDef(
-    _RequiredCreateThemeRequestRequestTypeDef, _OptionalCreateThemeRequestRequestTypeDef
-):
+class ThemeTypeDef(_RequiredThemeTypeDef, _OptionalThemeTypeDef):
     pass
 
-CreateThemeResponseTypeDef = TypedDict(
-    "CreateThemeResponseTypeDef",
-    {
-        "entity": "ThemeTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteComponentRequestRequestTypeDef = TypedDict(
     "DeleteComponentRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
     },
@@ -1026,21 +503,14 @@
     {
         "appId": str,
         "environmentName": str,
         "id": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
     "_RequiredExchangeCodeForTokenRequestBodyTypeDef",
     {
         "code": str,
         "redirectUri": str,
     },
 )
@@ -1053,53 +523,24 @@
 )
 
 class ExchangeCodeForTokenRequestBodyTypeDef(
     _RequiredExchangeCodeForTokenRequestBodyTypeDef, _OptionalExchangeCodeForTokenRequestBodyTypeDef
 ):
     pass
 
-ExchangeCodeForTokenRequestRequestTypeDef = TypedDict(
-    "ExchangeCodeForTokenRequestRequestTypeDef",
-    {
-        "provider": Literal["figma"],
-        "request": "ExchangeCodeForTokenRequestBodyTypeDef",
-    },
-)
-
-ExchangeCodeForTokenResponseTypeDef = TypedDict(
-    "ExchangeCodeForTokenResponseTypeDef",
-    {
-        "accessToken": str,
-        "expiresIn": int,
-        "refreshToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
-    "_RequiredExportComponentsRequestExportComponentsPaginateTypeDef",
-    {
-        "appId": str,
-        "environmentName": str,
-    },
-)
-_OptionalExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
-    "_OptionalExportComponentsRequestExportComponentsPaginateTypeDef",
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
 
-class ExportComponentsRequestExportComponentsPaginateTypeDef(
-    _RequiredExportComponentsRequestExportComponentsPaginateTypeDef,
-    _OptionalExportComponentsRequestExportComponentsPaginateTypeDef,
-):
-    pass
-
 _RequiredExportComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredExportComponentsRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
@@ -1112,44 +553,14 @@
 )
 
 class ExportComponentsRequestRequestTypeDef(
     _RequiredExportComponentsRequestRequestTypeDef, _OptionalExportComponentsRequestRequestTypeDef
 ):
     pass
 
-ExportComponentsResponseTypeDef = TypedDict(
-    "ExportComponentsResponseTypeDef",
-    {
-        "entities": List["ComponentTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
-    "_RequiredExportFormsRequestExportFormsPaginateTypeDef",
-    {
-        "appId": str,
-        "environmentName": str,
-    },
-)
-_OptionalExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
-    "_OptionalExportFormsRequestExportFormsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ExportFormsRequestExportFormsPaginateTypeDef(
-    _RequiredExportFormsRequestExportFormsPaginateTypeDef,
-    _OptionalExportFormsRequestExportFormsPaginateTypeDef,
-):
-    pass
-
 _RequiredExportFormsRequestRequestTypeDef = TypedDict(
     "_RequiredExportFormsRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
@@ -1162,44 +573,14 @@
 )
 
 class ExportFormsRequestRequestTypeDef(
     _RequiredExportFormsRequestRequestTypeDef, _OptionalExportFormsRequestRequestTypeDef
 ):
     pass
 
-ExportFormsResponseTypeDef = TypedDict(
-    "ExportFormsResponseTypeDef",
-    {
-        "entities": List["FormTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
-    "_RequiredExportThemesRequestExportThemesPaginateTypeDef",
-    {
-        "appId": str,
-        "environmentName": str,
-    },
-)
-_OptionalExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
-    "_OptionalExportThemesRequestExportThemesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ExportThemesRequestExportThemesPaginateTypeDef(
-    _RequiredExportThemesRequestExportThemesPaginateTypeDef,
-    _OptionalExportThemesRequestExportThemesPaginateTypeDef,
-):
-    pass
-
 _RequiredExportThemesRequestRequestTypeDef = TypedDict(
     "_RequiredExportThemesRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
@@ -1212,121 +593,14 @@
 )
 
 class ExportThemesRequestRequestTypeDef(
     _RequiredExportThemesRequestRequestTypeDef, _OptionalExportThemesRequestRequestTypeDef
 ):
     pass
 
-ExportThemesResponseTypeDef = TypedDict(
-    "ExportThemesResponseTypeDef",
-    {
-        "entities": List["ThemeTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-FieldConfigOutputTypeDef = TypedDict(
-    "FieldConfigOutputTypeDef",
-    {
-        "label": str,
-        "position": "FieldPositionOutputTypeDef",
-        "excluded": bool,
-        "inputType": "FieldInputConfigOutputTypeDef",
-        "validations": List["FieldValidationConfigurationOutputTypeDef"],
-    },
-    total=False,
-)
-
-FieldConfigTypeDef = TypedDict(
-    "FieldConfigTypeDef",
-    {
-        "label": str,
-        "position": "FieldPositionTypeDef",
-        "excluded": bool,
-        "inputType": "FieldInputConfigTypeDef",
-        "validations": Sequence["FieldValidationConfigurationTypeDef"],
-    },
-    total=False,
-)
-
-_RequiredFieldInputConfigOutputTypeDef = TypedDict(
-    "_RequiredFieldInputConfigOutputTypeDef",
-    {
-        "type": str,
-    },
-)
-_OptionalFieldInputConfigOutputTypeDef = TypedDict(
-    "_OptionalFieldInputConfigOutputTypeDef",
-    {
-        "required": bool,
-        "readOnly": bool,
-        "placeholder": str,
-        "defaultValue": str,
-        "descriptiveText": str,
-        "defaultChecked": bool,
-        "defaultCountryCode": str,
-        "valueMappings": "ValueMappingsOutputTypeDef",
-        "name": str,
-        "minValue": float,
-        "maxValue": float,
-        "step": float,
-        "value": str,
-        "isArray": bool,
-        "fileUploaderConfig": "FileUploaderFieldConfigOutputTypeDef",
-    },
-    total=False,
-)
-
-class FieldInputConfigOutputTypeDef(
-    _RequiredFieldInputConfigOutputTypeDef, _OptionalFieldInputConfigOutputTypeDef
-):
-    pass
-
-_RequiredFieldInputConfigTypeDef = TypedDict(
-    "_RequiredFieldInputConfigTypeDef",
-    {
-        "type": str,
-    },
-)
-_OptionalFieldInputConfigTypeDef = TypedDict(
-    "_OptionalFieldInputConfigTypeDef",
-    {
-        "required": bool,
-        "readOnly": bool,
-        "placeholder": str,
-        "defaultValue": str,
-        "descriptiveText": str,
-        "defaultChecked": bool,
-        "defaultCountryCode": str,
-        "valueMappings": "ValueMappingsTypeDef",
-        "name": str,
-        "minValue": float,
-        "maxValue": float,
-        "step": float,
-        "value": str,
-        "isArray": bool,
-        "fileUploaderConfig": "FileUploaderFieldConfigTypeDef",
-    },
-    total=False,
-)
-
-class FieldInputConfigTypeDef(_RequiredFieldInputConfigTypeDef, _OptionalFieldInputConfigTypeDef):
-    pass
-
-FieldPositionOutputTypeDef = TypedDict(
-    "FieldPositionOutputTypeDef",
-    {
-        "fixed": Literal["first"],
-        "rightOf": str,
-        "below": str,
-    },
-    total=False,
-)
-
 FieldPositionTypeDef = TypedDict(
     "FieldPositionTypeDef",
     {
         "fixed": Literal["first"],
         "rightOf": str,
         "below": str,
     },
@@ -1418,897 +692,1287 @@
 )
 
 class FileUploaderFieldConfigTypeDef(
     _RequiredFileUploaderFieldConfigTypeDef, _OptionalFileUploaderFieldConfigTypeDef
 ):
     pass
 
-FormBindingElementOutputTypeDef = TypedDict(
-    "FormBindingElementOutputTypeDef",
+FormInputBindingPropertiesValuePropertiesTypeDef = TypedDict(
+    "FormInputBindingPropertiesValuePropertiesTypeDef",
     {
-        "element": str,
-        "property": str,
+        "model": str,
     },
+    total=False,
 )
 
-FormBindingElementTypeDef = TypedDict(
-    "FormBindingElementTypeDef",
+_RequiredFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
+    "_RequiredFormInputValuePropertyBindingPropertiesTypeDef",
     {
-        "element": str,
         "property": str,
     },
 )
-
-FormButtonOutputTypeDef = TypedDict(
-    "FormButtonOutputTypeDef",
+_OptionalFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
+    "_OptionalFormInputValuePropertyBindingPropertiesTypeDef",
     {
-        "excluded": bool,
-        "children": str,
-        "position": "FieldPositionOutputTypeDef",
+        "field": str,
     },
     total=False,
 )
 
-FormButtonTypeDef = TypedDict(
-    "FormButtonTypeDef",
+class FormInputValuePropertyBindingPropertiesTypeDef(
+    _RequiredFormInputValuePropertyBindingPropertiesTypeDef,
+    _OptionalFormInputValuePropertyBindingPropertiesTypeDef,
+):
+    pass
+
+FormStyleConfigTypeDef = TypedDict(
+    "FormStyleConfigTypeDef",
     {
-        "excluded": bool,
-        "children": str,
-        "position": "FieldPositionTypeDef",
+        "tokenReference": str,
+        "value": str,
     },
     total=False,
 )
 
-FormCTAOutputTypeDef = TypedDict(
-    "FormCTAOutputTypeDef",
+GetCodegenJobRequestRequestTypeDef = TypedDict(
+    "GetCodegenJobRequestRequestTypeDef",
     {
-        "position": FormButtonsPositionType,
-        "clear": "FormButtonOutputTypeDef",
-        "cancel": "FormButtonOutputTypeDef",
-        "submit": "FormButtonOutputTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
-    total=False,
 )
 
-FormCTATypeDef = TypedDict(
-    "FormCTATypeDef",
+GetComponentRequestRequestTypeDef = TypedDict(
+    "GetComponentRequestRequestTypeDef",
     {
-        "position": FormButtonsPositionType,
-        "clear": "FormButtonTypeDef",
-        "cancel": "FormButtonTypeDef",
-        "submit": "FormButtonTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
-    total=False,
 )
 
-FormDataTypeConfigOutputTypeDef = TypedDict(
-    "FormDataTypeConfigOutputTypeDef",
+GetFormRequestRequestTypeDef = TypedDict(
+    "GetFormRequestRequestTypeDef",
     {
-        "dataSourceType": FormDataSourceTypeType,
-        "dataTypeName": str,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
 )
 
-FormDataTypeConfigTypeDef = TypedDict(
-    "FormDataTypeConfigTypeDef",
+GetMetadataRequestRequestTypeDef = TypedDict(
+    "GetMetadataRequestRequestTypeDef",
     {
-        "dataSourceType": FormDataSourceTypeType,
-        "dataTypeName": str,
+        "appId": str,
+        "environmentName": str,
     },
 )
 
-FormInputBindingPropertiesValueOutputTypeDef = TypedDict(
-    "FormInputBindingPropertiesValueOutputTypeDef",
+GetThemeRequestRequestTypeDef = TypedDict(
+    "GetThemeRequestRequestTypeDef",
     {
-        "type": str,
-        "bindingProperties": "FormInputBindingPropertiesValuePropertiesOutputTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
-    total=False,
 )
 
-FormInputBindingPropertiesValuePropertiesOutputTypeDef = TypedDict(
-    "FormInputBindingPropertiesValuePropertiesOutputTypeDef",
+_RequiredListCodegenJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListCodegenJobsRequestRequestTypeDef",
     {
-        "model": str,
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalListCodegenJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListCodegenJobsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-FormInputBindingPropertiesValuePropertiesTypeDef = TypedDict(
-    "FormInputBindingPropertiesValuePropertiesTypeDef",
+class ListCodegenJobsRequestRequestTypeDef(
+    _RequiredListCodegenJobsRequestRequestTypeDef, _OptionalListCodegenJobsRequestRequestTypeDef
+):
+    pass
+
+_RequiredListComponentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListComponentsRequestRequestTypeDef",
     {
-        "model": str,
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalListComponentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListComponentsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-FormInputBindingPropertiesValueTypeDef = TypedDict(
-    "FormInputBindingPropertiesValueTypeDef",
+class ListComponentsRequestRequestTypeDef(
+    _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
+):
+    pass
+
+_RequiredListFormsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFormsRequestRequestTypeDef",
     {
-        "type": str,
-        "bindingProperties": "FormInputBindingPropertiesValuePropertiesTypeDef",
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalListFormsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFormsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-_RequiredFormInputValuePropertyBindingPropertiesOutputTypeDef = TypedDict(
-    "_RequiredFormInputValuePropertyBindingPropertiesOutputTypeDef",
+class ListFormsRequestRequestTypeDef(
+    _RequiredListFormsRequestRequestTypeDef, _OptionalListFormsRequestRequestTypeDef
+):
+    pass
+
+_RequiredListThemesRequestRequestTypeDef = TypedDict(
+    "_RequiredListThemesRequestRequestTypeDef",
     {
-        "property": str,
+        "appId": str,
+        "environmentName": str,
     },
 )
-_OptionalFormInputValuePropertyBindingPropertiesOutputTypeDef = TypedDict(
-    "_OptionalFormInputValuePropertyBindingPropertiesOutputTypeDef",
+_OptionalListThemesRequestRequestTypeDef = TypedDict(
+    "_OptionalListThemesRequestRequestTypeDef",
     {
-        "field": str,
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-class FormInputValuePropertyBindingPropertiesOutputTypeDef(
-    _RequiredFormInputValuePropertyBindingPropertiesOutputTypeDef,
-    _OptionalFormInputValuePropertyBindingPropertiesOutputTypeDef,
+class ListThemesRequestRequestTypeDef(
+    _RequiredListThemesRequestRequestTypeDef, _OptionalListThemesRequestRequestTypeDef
 ):
     pass
 
-_RequiredFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
-    "_RequiredFormInputValuePropertyBindingPropertiesTypeDef",
+ThemeSummaryTypeDef = TypedDict(
+    "ThemeSummaryTypeDef",
     {
-        "property": str,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "name": str,
     },
 )
-_OptionalFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
-    "_OptionalFormInputValuePropertyBindingPropertiesTypeDef",
+
+PredicateOutputTypeDef = TypedDict(
+    "PredicateOutputTypeDef",
+    {
+        "or": List[Dict[str, Any]],
+        "and": List[Dict[str, Any]],
+        "field": str,
+        "operator": str,
+        "operand": str,
+        "operandType": str,
+    },
+    total=False,
+)
+
+PredicateTypeDef = TypedDict(
+    "PredicateTypeDef",
     {
+        "or": Sequence[Dict[str, Any]],
+        "and": Sequence[Dict[str, Any]],
         "field": str,
+        "operator": str,
+        "operand": str,
+        "operandType": str,
     },
     total=False,
 )
 
-class FormInputValuePropertyBindingPropertiesTypeDef(
-    _RequiredFormInputValuePropertyBindingPropertiesTypeDef,
-    _OptionalFormInputValuePropertyBindingPropertiesTypeDef,
+PutMetadataFlagBodyTypeDef = TypedDict(
+    "PutMetadataFlagBodyTypeDef",
+    {
+        "newValue": str,
+    },
+)
+
+_RequiredRefreshTokenRequestBodyTypeDef = TypedDict(
+    "_RequiredRefreshTokenRequestBodyTypeDef",
+    {
+        "token": str,
+    },
+)
+_OptionalRefreshTokenRequestBodyTypeDef = TypedDict(
+    "_OptionalRefreshTokenRequestBodyTypeDef",
+    {
+        "clientId": str,
+    },
+    total=False,
+)
+
+class RefreshTokenRequestBodyTypeDef(
+    _RequiredRefreshTokenRequestBodyTypeDef, _OptionalRefreshTokenRequestBodyTypeDef
 ):
     pass
 
-FormInputValuePropertyOutputTypeDef = TypedDict(
-    "FormInputValuePropertyOutputTypeDef",
+ThemeValueOutputTypeDef = TypedDict(
+    "ThemeValueOutputTypeDef",
     {
         "value": str,
-        "bindingProperties": "FormInputValuePropertyBindingPropertiesOutputTypeDef",
-        "concat": List[Dict[str, Any]],
+        "children": List[Dict[str, Any]],
     },
     total=False,
 )
 
-FormInputValuePropertyTypeDef = TypedDict(
-    "FormInputValuePropertyTypeDef",
+ThemeValueTypeDef = TypedDict(
+    "ThemeValueTypeDef",
     {
         "value": str,
-        "bindingProperties": "FormInputValuePropertyBindingPropertiesTypeDef",
-        "concat": Sequence[Dict[str, Any]],
+        "children": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-FormStyleConfigOutputTypeDef = TypedDict(
-    "FormStyleConfigOutputTypeDef",
+ThemeValuesOutputTypeDef = TypedDict(
+    "ThemeValuesOutputTypeDef",
     {
-        "tokenReference": str,
-        "value": str,
+        "key": str,
+        "value": Dict[str, Any],
     },
     total=False,
 )
 
-FormStyleConfigTypeDef = TypedDict(
-    "FormStyleConfigTypeDef",
+ThemeValuesTypeDef = TypedDict(
+    "ThemeValuesTypeDef",
     {
-        "tokenReference": str,
-        "value": str,
+        "key": str,
+        "value": Dict[str, Any],
     },
     total=False,
 )
 
-FormStyleOutputTypeDef = TypedDict(
-    "FormStyleOutputTypeDef",
+_RequiredUpdateThemeDataTypeDef = TypedDict(
+    "_RequiredUpdateThemeDataTypeDef",
     {
-        "horizontalGap": "FormStyleConfigOutputTypeDef",
-        "verticalGap": "FormStyleConfigOutputTypeDef",
-        "outerPadding": "FormStyleConfigOutputTypeDef",
+        "values": Sequence["ThemeValuesTypeDef"],
+    },
+)
+_OptionalUpdateThemeDataTypeDef = TypedDict(
+    "_OptionalUpdateThemeDataTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "overrides": Sequence["ThemeValuesTypeDef"],
     },
     total=False,
 )
 
-FormStyleTypeDef = TypedDict(
-    "FormStyleTypeDef",
+class UpdateThemeDataTypeDef(_RequiredUpdateThemeDataTypeDef, _OptionalUpdateThemeDataTypeDef):
+    pass
+
+_RequiredValueMappingTypeDef = TypedDict(
+    "_RequiredValueMappingTypeDef",
+    {
+        "value": "FormInputValuePropertyTypeDef",
+    },
+)
+_OptionalValueMappingTypeDef = TypedDict(
+    "_OptionalValueMappingTypeDef",
     {
-        "horizontalGap": "FormStyleConfigTypeDef",
-        "verticalGap": "FormStyleConfigTypeDef",
-        "outerPadding": "FormStyleConfigTypeDef",
+        "displayValue": "FormInputValuePropertyTypeDef",
     },
     total=False,
 )
 
-FormSummaryTypeDef = TypedDict(
-    "FormSummaryTypeDef",
+class ValueMappingTypeDef(_RequiredValueMappingTypeDef, _OptionalValueMappingTypeDef):
+    pass
+
+ActionParametersOutputTypeDef = TypedDict(
+    "ActionParametersOutputTypeDef",
     {
-        "appId": str,
-        "dataType": "FormDataTypeConfigOutputTypeDef",
-        "environmentName": str,
-        "formActionType": FormActionTypeType,
-        "id": str,
-        "name": str,
+        "type": "ComponentPropertyOutputTypeDef",
+        "url": "ComponentPropertyOutputTypeDef",
+        "anchor": "ComponentPropertyOutputTypeDef",
+        "target": "ComponentPropertyOutputTypeDef",
+        "global": "ComponentPropertyOutputTypeDef",
+        "model": str,
+        "id": "ComponentPropertyOutputTypeDef",
+        "fields": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "state": MutationActionSetStateParameterTypeDef,
     },
+    total=False,
 )
 
-_RequiredFormTypeDef = TypedDict(
-    "_RequiredFormTypeDef",
+ActionParametersTypeDef = TypedDict(
+    "ActionParametersTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "name": str,
-        "formActionType": FormActionTypeType,
-        "style": "FormStyleOutputTypeDef",
-        "dataType": "FormDataTypeConfigOutputTypeDef",
-        "fields": Dict[str, "FieldConfigOutputTypeDef"],
-        "sectionalElements": Dict[str, "SectionalElementOutputTypeDef"],
-        "schemaVersion": str,
+        "type": "ComponentPropertyTypeDef",
+        "url": "ComponentPropertyTypeDef",
+        "anchor": "ComponentPropertyTypeDef",
+        "target": "ComponentPropertyTypeDef",
+        "global": "ComponentPropertyTypeDef",
+        "model": str,
+        "id": "ComponentPropertyTypeDef",
+        "fields": Mapping[str, "ComponentPropertyTypeDef"],
+        "state": MutationActionSetStateParameterTypeDef,
     },
+    total=False,
 )
-_OptionalFormTypeDef = TypedDict(
-    "_OptionalFormTypeDef",
+
+_RequiredCodegenGenericDataFieldOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataFieldOutputTypeDef",
     {
-        "tags": Dict[str, str],
-        "cta": "FormCTAOutputTypeDef",
-        "labelDecorator": LabelDecoratorType,
+        "dataType": CodegenGenericDataFieldDataTypeType,
+        "dataTypeValue": str,
+        "required": bool,
+        "readOnly": bool,
+        "isArray": bool,
+    },
+)
+_OptionalCodegenGenericDataFieldOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataFieldOutputTypeDef",
+    {
+        "relationship": CodegenGenericDataRelationshipTypeOutputTypeDef,
     },
     total=False,
 )
 
-class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
+class CodegenGenericDataFieldOutputTypeDef(
+    _RequiredCodegenGenericDataFieldOutputTypeDef, _OptionalCodegenGenericDataFieldOutputTypeDef
+):
     pass
 
-GetCodegenJobRequestRequestTypeDef = TypedDict(
-    "GetCodegenJobRequestRequestTypeDef",
+_RequiredCodegenGenericDataFieldTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataFieldTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "dataType": CodegenGenericDataFieldDataTypeType,
+        "dataTypeValue": str,
+        "required": bool,
+        "readOnly": bool,
+        "isArray": bool,
+    },
+)
+_OptionalCodegenGenericDataFieldTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataFieldTypeDef",
+    {
+        "relationship": CodegenGenericDataRelationshipTypeTypeDef,
     },
+    total=False,
 )
 
-GetCodegenJobResponseTypeDef = TypedDict(
-    "GetCodegenJobResponseTypeDef",
+class CodegenGenericDataFieldTypeDef(
+    _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
+):
+    pass
+
+CodegenJobRenderConfigTypeDef = TypedDict(
+    "CodegenJobRenderConfigTypeDef",
     {
-        "job": "CodegenJobTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "react": ReactStartCodegenJobDataTypeDef,
     },
+    total=False,
 )
 
-GetComponentRequestRequestTypeDef = TypedDict(
-    "GetComponentRequestRequestTypeDef",
+ComponentBindingPropertiesValueOutputTypeDef = TypedDict(
+    "ComponentBindingPropertiesValueOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "type": str,
+        "bindingProperties": ComponentBindingPropertiesValuePropertiesOutputTypeDef,
+        "defaultValue": str,
     },
+    total=False,
 )
 
-GetComponentResponseTypeDef = TypedDict(
-    "GetComponentResponseTypeDef",
+ComponentBindingPropertiesValueTypeDef = TypedDict(
+    "ComponentBindingPropertiesValueTypeDef",
     {
-        "component": "ComponentTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "type": str,
+        "bindingProperties": ComponentBindingPropertiesValuePropertiesTypeDef,
+        "defaultValue": str,
     },
+    total=False,
 )
 
-GetFormRequestRequestTypeDef = TypedDict(
-    "GetFormRequestRequestTypeDef",
+_RequiredComponentDataConfigurationOutputTypeDef = TypedDict(
+    "_RequiredComponentDataConfigurationOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "model": str,
     },
 )
+_OptionalComponentDataConfigurationOutputTypeDef = TypedDict(
+    "_OptionalComponentDataConfigurationOutputTypeDef",
+    {
+        "sort": List[SortPropertyTypeDef],
+        "predicate": "PredicateOutputTypeDef",
+        "identifiers": List[str],
+    },
+    total=False,
+)
 
-GetFormResponseTypeDef = TypedDict(
-    "GetFormResponseTypeDef",
+class ComponentDataConfigurationOutputTypeDef(
+    _RequiredComponentDataConfigurationOutputTypeDef,
+    _OptionalComponentDataConfigurationOutputTypeDef,
+):
+    pass
+
+_RequiredComponentDataConfigurationTypeDef = TypedDict(
+    "_RequiredComponentDataConfigurationTypeDef",
+    {
+        "model": str,
+    },
+)
+_OptionalComponentDataConfigurationTypeDef = TypedDict(
+    "_OptionalComponentDataConfigurationTypeDef",
     {
-        "form": "FormTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sort": Sequence[SortPropertyTypeDef],
+        "predicate": "PredicateTypeDef",
+        "identifiers": Sequence[str],
     },
+    total=False,
 )
 
-GetMetadataRequestRequestTypeDef = TypedDict(
-    "GetMetadataRequestRequestTypeDef",
+class ComponentDataConfigurationTypeDef(
+    _RequiredComponentDataConfigurationTypeDef, _OptionalComponentDataConfigurationTypeDef
+):
+    pass
+
+ComponentPropertyOutputTypeDef = TypedDict(
+    "ComponentPropertyOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "value": str,
+        "bindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "collectionBindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "defaultValue": str,
+        "model": str,
+        "bindings": Dict[str, FormBindingElementTypeDef],
+        "event": str,
+        "userAttribute": str,
+        "concat": List[Dict[str, Any]],
+        "condition": "ComponentConditionPropertyTypeDef",
+        "configured": bool,
+        "type": str,
+        "importedValue": str,
+        "componentName": str,
+        "property": str,
+    },
+    total=False,
+)
+
+ComponentPropertyTypeDef = TypedDict(
+    "ComponentPropertyTypeDef",
+    {
+        "value": str,
+        "bindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "collectionBindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "defaultValue": str,
+        "model": str,
+        "bindings": Mapping[str, FormBindingElementTypeDef],
+        "event": str,
+        "userAttribute": str,
+        "concat": Sequence[Dict[str, Any]],
+        "condition": Dict[str, Any],
+        "configured": bool,
+        "type": str,
+        "importedValue": str,
+        "componentName": str,
+        "property": str,
+    },
+    total=False,
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExchangeCodeForTokenResponseTypeDef = TypedDict(
+    "ExchangeCodeForTokenResponseTypeDef",
+    {
+        "accessToken": str,
+        "expiresIn": int,
+        "refreshToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMetadataResponseTypeDef = TypedDict(
     "GetMetadataResponseTypeDef",
     {
         "features": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetThemeRequestRequestTypeDef = TypedDict(
-    "GetThemeRequestRequestTypeDef",
+ListCodegenJobsResponseTypeDef = TypedDict(
+    "ListCodegenJobsResponseTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "entities": List[CodegenJobSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetThemeResponseTypeDef = TypedDict(
-    "GetThemeResponseTypeDef",
+ListComponentsResponseTypeDef = TypedDict(
+    "ListComponentsResponseTypeDef",
     {
-        "theme": "ThemeTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "entities": List[ComponentSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
-    "_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+RefreshTokenResponseTypeDef = TypedDict(
+    "RefreshTokenResponseTypeDef",
+    {
+        "accessToken": str,
+        "expiresIn": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FormSummaryTypeDef = TypedDict(
+    "FormSummaryTypeDef",
+    {
+        "appId": str,
+        "dataType": FormDataTypeConfigTypeDef,
+        "environmentName": str,
+        "formActionType": FormActionTypeType,
+        "id": str,
+        "name": str,
+    },
+)
+
+_RequiredCreateThemeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateThemeRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
+        "themeToCreate": CreateThemeDataTypeDef,
     },
 )
-_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
-    "_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+_OptionalCreateThemeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateThemeRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "clientToken": str,
     },
     total=False,
 )
 
-class ListCodegenJobsRequestListCodegenJobsPaginateTypeDef(
-    _RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
-    _OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+class CreateThemeRequestRequestTypeDef(
+    _RequiredCreateThemeRequestRequestTypeDef, _OptionalCreateThemeRequestRequestTypeDef
 ):
     pass
 
-_RequiredListCodegenJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListCodegenJobsRequestRequestTypeDef",
+CreateThemeResponseTypeDef = TypedDict(
+    "CreateThemeResponseTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "entity": ThemeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListCodegenJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListCodegenJobsRequestRequestTypeDef",
+
+ExportThemesResponseTypeDef = TypedDict(
+    "ExportThemesResponseTypeDef",
     {
+        "entities": List[ThemeTypeDef],
         "nextToken": str,
-        "maxResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ListCodegenJobsRequestRequestTypeDef(
-    _RequiredListCodegenJobsRequestRequestTypeDef, _OptionalListCodegenJobsRequestRequestTypeDef
-):
-    pass
+GetThemeResponseTypeDef = TypedDict(
+    "GetThemeResponseTypeDef",
+    {
+        "theme": ThemeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-ListCodegenJobsResponseTypeDef = TypedDict(
-    "ListCodegenJobsResponseTypeDef",
+UpdateThemeResponseTypeDef = TypedDict(
+    "UpdateThemeResponseTypeDef",
     {
-        "entities": List["CodegenJobSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "entity": ThemeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
-    "_RequiredListComponentsRequestListComponentsPaginateTypeDef",
+ExchangeCodeForTokenRequestRequestTypeDef = TypedDict(
+    "ExchangeCodeForTokenRequestRequestTypeDef",
+    {
+        "provider": Literal["figma"],
+        "request": ExchangeCodeForTokenRequestBodyTypeDef,
+    },
+)
+
+_RequiredExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
+    "_RequiredExportComponentsRequestExportComponentsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
-    "_OptionalListComponentsRequestListComponentsPaginateTypeDef",
+_OptionalExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
+    "_OptionalExportComponentsRequestExportComponentsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListComponentsRequestListComponentsPaginateTypeDef(
-    _RequiredListComponentsRequestListComponentsPaginateTypeDef,
-    _OptionalListComponentsRequestListComponentsPaginateTypeDef,
+class ExportComponentsRequestExportComponentsPaginateTypeDef(
+    _RequiredExportComponentsRequestExportComponentsPaginateTypeDef,
+    _OptionalExportComponentsRequestExportComponentsPaginateTypeDef,
 ):
     pass
 
-_RequiredListComponentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListComponentsRequestRequestTypeDef",
+_RequiredExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
+    "_RequiredExportFormsRequestExportFormsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListComponentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListComponentsRequestRequestTypeDef",
+_OptionalExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
+    "_OptionalExportFormsRequestExportFormsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListComponentsRequestRequestTypeDef(
-    _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
+class ExportFormsRequestExportFormsPaginateTypeDef(
+    _RequiredExportFormsRequestExportFormsPaginateTypeDef,
+    _OptionalExportFormsRequestExportFormsPaginateTypeDef,
 ):
     pass
 
-ListComponentsResponseTypeDef = TypedDict(
-    "ListComponentsResponseTypeDef",
-    {
-        "entities": List["ComponentSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFormsRequestListFormsPaginateTypeDef = TypedDict(
-    "_RequiredListFormsRequestListFormsPaginateTypeDef",
+_RequiredExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
+    "_RequiredExportThemesRequestExportThemesPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListFormsRequestListFormsPaginateTypeDef = TypedDict(
-    "_OptionalListFormsRequestListFormsPaginateTypeDef",
+_OptionalExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
+    "_OptionalExportThemesRequestExportThemesPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListFormsRequestListFormsPaginateTypeDef(
-    _RequiredListFormsRequestListFormsPaginateTypeDef,
-    _OptionalListFormsRequestListFormsPaginateTypeDef,
+class ExportThemesRequestExportThemesPaginateTypeDef(
+    _RequiredExportThemesRequestExportThemesPaginateTypeDef,
+    _OptionalExportThemesRequestExportThemesPaginateTypeDef,
 ):
     pass
 
-_RequiredListFormsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFormsRequestRequestTypeDef",
+_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
+    "_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListFormsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFormsRequestRequestTypeDef",
+_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
+    "_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListFormsRequestRequestTypeDef(
-    _RequiredListFormsRequestRequestTypeDef, _OptionalListFormsRequestRequestTypeDef
+class ListCodegenJobsRequestListCodegenJobsPaginateTypeDef(
+    _RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    _OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
 ):
     pass
 
-ListFormsResponseTypeDef = TypedDict(
-    "ListFormsResponseTypeDef",
+_RequiredListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
+    "_RequiredListComponentsRequestListComponentsPaginateTypeDef",
     {
-        "entities": List["FormSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
+    "_OptionalListComponentsRequestListComponentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredListThemesRequestListThemesPaginateTypeDef = TypedDict(
-    "_RequiredListThemesRequestListThemesPaginateTypeDef",
+class ListComponentsRequestListComponentsPaginateTypeDef(
+    _RequiredListComponentsRequestListComponentsPaginateTypeDef,
+    _OptionalListComponentsRequestListComponentsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFormsRequestListFormsPaginateTypeDef = TypedDict(
+    "_RequiredListFormsRequestListFormsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListThemesRequestListThemesPaginateTypeDef = TypedDict(
-    "_OptionalListThemesRequestListThemesPaginateTypeDef",
+_OptionalListFormsRequestListFormsPaginateTypeDef = TypedDict(
+    "_OptionalListFormsRequestListFormsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListThemesRequestListThemesPaginateTypeDef(
-    _RequiredListThemesRequestListThemesPaginateTypeDef,
-    _OptionalListThemesRequestListThemesPaginateTypeDef,
+class ListFormsRequestListFormsPaginateTypeDef(
+    _RequiredListFormsRequestListFormsPaginateTypeDef,
+    _OptionalListFormsRequestListFormsPaginateTypeDef,
 ):
     pass
 
-_RequiredListThemesRequestRequestTypeDef = TypedDict(
-    "_RequiredListThemesRequestRequestTypeDef",
+_RequiredListThemesRequestListThemesPaginateTypeDef = TypedDict(
+    "_RequiredListThemesRequestListThemesPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListThemesRequestRequestTypeDef = TypedDict(
-    "_OptionalListThemesRequestRequestTypeDef",
+_OptionalListThemesRequestListThemesPaginateTypeDef = TypedDict(
+    "_OptionalListThemesRequestListThemesPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListThemesRequestRequestTypeDef(
-    _RequiredListThemesRequestRequestTypeDef, _OptionalListThemesRequestRequestTypeDef
+class ListThemesRequestListThemesPaginateTypeDef(
+    _RequiredListThemesRequestListThemesPaginateTypeDef,
+    _OptionalListThemesRequestListThemesPaginateTypeDef,
 ):
     pass
 
-ListThemesResponseTypeDef = TypedDict(
-    "ListThemesResponseTypeDef",
+FormButtonTypeDef = TypedDict(
+    "FormButtonTypeDef",
     {
-        "entities": List["ThemeSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "excluded": bool,
+        "children": str,
+        "position": FieldPositionTypeDef,
     },
+    total=False,
 )
 
-MutationActionSetStateParameterOutputTypeDef = TypedDict(
-    "MutationActionSetStateParameterOutputTypeDef",
+_RequiredSectionalElementTypeDef = TypedDict(
+    "_RequiredSectionalElementTypeDef",
     {
-        "componentName": str,
-        "property": str,
-        "set": "ComponentPropertyOutputTypeDef",
+        "type": str,
     },
 )
-
-MutationActionSetStateParameterTypeDef = TypedDict(
-    "MutationActionSetStateParameterTypeDef",
+_OptionalSectionalElementTypeDef = TypedDict(
+    "_OptionalSectionalElementTypeDef",
     {
-        "componentName": str,
-        "property": str,
-        "set": "ComponentPropertyTypeDef",
+        "position": FieldPositionTypeDef,
+        "text": str,
+        "level": int,
+        "orientation": str,
+        "excluded": bool,
     },
+    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+class SectionalElementTypeDef(_RequiredSectionalElementTypeDef, _OptionalSectionalElementTypeDef):
+    pass
+
+FormInputBindingPropertiesValueTypeDef = TypedDict(
+    "FormInputBindingPropertiesValueTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "type": str,
+        "bindingProperties": FormInputBindingPropertiesValuePropertiesTypeDef,
     },
     total=False,
 )
 
-PredicateOutputTypeDef = TypedDict(
-    "PredicateOutputTypeDef",
+FormInputValuePropertyTypeDef = TypedDict(
+    "FormInputValuePropertyTypeDef",
     {
-        "or": List[Dict[str, Any]],
-        "and": List[Dict[str, Any]],
-        "field": str,
-        "operator": str,
-        "operand": str,
-        "operandType": str,
+        "value": str,
+        "bindingProperties": FormInputValuePropertyBindingPropertiesTypeDef,
+        "concat": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-PredicateTypeDef = TypedDict(
-    "PredicateTypeDef",
+FormStyleTypeDef = TypedDict(
+    "FormStyleTypeDef",
     {
-        "or": Sequence[Dict[str, Any]],
-        "and": Sequence[Dict[str, Any]],
-        "field": str,
-        "operator": str,
-        "operand": str,
-        "operandType": str,
+        "horizontalGap": FormStyleConfigTypeDef,
+        "verticalGap": FormStyleConfigTypeDef,
+        "outerPadding": FormStyleConfigTypeDef,
     },
     total=False,
 )
 
-PutMetadataFlagBodyTypeDef = TypedDict(
-    "PutMetadataFlagBodyTypeDef",
+ListThemesResponseTypeDef = TypedDict(
+    "ListThemesResponseTypeDef",
     {
-        "newValue": str,
+        "entities": List[ThemeSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutMetadataFlagRequestRequestTypeDef = TypedDict(
     "PutMetadataFlagRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "featureName": str,
-        "body": "PutMetadataFlagBodyTypeDef",
+        "body": PutMetadataFlagBodyTypeDef,
     },
 )
 
-ReactStartCodegenJobDataOutputTypeDef = TypedDict(
-    "ReactStartCodegenJobDataOutputTypeDef",
-    {
-        "module": JSModuleType,
-        "target": JSTargetType,
-        "script": JSScriptType,
-        "renderTypeDeclarations": bool,
-        "inlineSourceMap": bool,
-    },
-    total=False,
-)
-
-ReactStartCodegenJobDataTypeDef = TypedDict(
-    "ReactStartCodegenJobDataTypeDef",
+RefreshTokenRequestRequestTypeDef = TypedDict(
+    "RefreshTokenRequestRequestTypeDef",
     {
-        "module": JSModuleType,
-        "target": JSTargetType,
-        "script": JSScriptType,
-        "renderTypeDeclarations": bool,
-        "inlineSourceMap": bool,
+        "provider": Literal["figma"],
+        "refreshTokenBody": RefreshTokenRequestBodyTypeDef,
     },
-    total=False,
 )
 
-_RequiredRefreshTokenRequestBodyTypeDef = TypedDict(
-    "_RequiredRefreshTokenRequestBodyTypeDef",
+_RequiredUpdateThemeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateThemeRequestRequestTypeDef",
     {
-        "token": str,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "updatedTheme": UpdateThemeDataTypeDef,
     },
 )
-_OptionalRefreshTokenRequestBodyTypeDef = TypedDict(
-    "_OptionalRefreshTokenRequestBodyTypeDef",
+_OptionalUpdateThemeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateThemeRequestRequestTypeDef",
     {
-        "clientId": str,
+        "clientToken": str,
     },
     total=False,
 )
 
-class RefreshTokenRequestBodyTypeDef(
-    _RequiredRefreshTokenRequestBodyTypeDef, _OptionalRefreshTokenRequestBodyTypeDef
+class UpdateThemeRequestRequestTypeDef(
+    _RequiredUpdateThemeRequestRequestTypeDef, _OptionalUpdateThemeRequestRequestTypeDef
 ):
     pass
 
-RefreshTokenRequestRequestTypeDef = TypedDict(
-    "RefreshTokenRequestRequestTypeDef",
-    {
-        "provider": Literal["figma"],
-        "refreshTokenBody": "RefreshTokenRequestBodyTypeDef",
-    },
-)
-
-RefreshTokenResponseTypeDef = TypedDict(
-    "RefreshTokenResponseTypeDef",
+ComponentEventOutputTypeDef = TypedDict(
+    "ComponentEventOutputTypeDef",
     {
-        "accessToken": str,
-        "expiresIn": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "action": str,
+        "parameters": ActionParametersOutputTypeDef,
+        "bindingEvent": str,
     },
+    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ComponentEventTypeDef = TypedDict(
+    "ComponentEventTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "action": str,
+        "parameters": ActionParametersTypeDef,
+        "bindingEvent": str,
     },
+    total=False,
 )
 
-_RequiredSectionalElementOutputTypeDef = TypedDict(
-    "_RequiredSectionalElementOutputTypeDef",
+_RequiredCodegenGenericDataModelOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataModelOutputTypeDef",
     {
-        "type": str,
+        "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
+        "primaryKeys": List[str],
     },
 )
-_OptionalSectionalElementOutputTypeDef = TypedDict(
-    "_OptionalSectionalElementOutputTypeDef",
+_OptionalCodegenGenericDataModelOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataModelOutputTypeDef",
     {
-        "position": "FieldPositionOutputTypeDef",
-        "text": str,
-        "level": int,
-        "orientation": str,
-        "excluded": bool,
+        "isJoinTable": bool,
     },
     total=False,
 )
 
-class SectionalElementOutputTypeDef(
-    _RequiredSectionalElementOutputTypeDef, _OptionalSectionalElementOutputTypeDef
+class CodegenGenericDataModelOutputTypeDef(
+    _RequiredCodegenGenericDataModelOutputTypeDef, _OptionalCodegenGenericDataModelOutputTypeDef
 ):
     pass
 
-_RequiredSectionalElementTypeDef = TypedDict(
-    "_RequiredSectionalElementTypeDef",
+CodegenGenericDataNonModelOutputTypeDef = TypedDict(
+    "CodegenGenericDataNonModelOutputTypeDef",
     {
-        "type": str,
+        "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
     },
 )
-_OptionalSectionalElementTypeDef = TypedDict(
-    "_OptionalSectionalElementTypeDef",
+
+_RequiredCodegenGenericDataModelTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataModelTypeDef",
     {
-        "position": "FieldPositionTypeDef",
-        "text": str,
-        "level": int,
-        "orientation": str,
-        "excluded": bool,
+        "fields": Mapping[str, CodegenGenericDataFieldTypeDef],
+        "primaryKeys": Sequence[str],
+    },
+)
+_OptionalCodegenGenericDataModelTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataModelTypeDef",
+    {
+        "isJoinTable": bool,
     },
     total=False,
 )
 
-class SectionalElementTypeDef(_RequiredSectionalElementTypeDef, _OptionalSectionalElementTypeDef):
+class CodegenGenericDataModelTypeDef(
+    _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
+):
     pass
 
-SortPropertyOutputTypeDef = TypedDict(
-    "SortPropertyOutputTypeDef",
+CodegenGenericDataNonModelTypeDef = TypedDict(
+    "CodegenGenericDataNonModelTypeDef",
     {
-        "field": str,
-        "direction": SortDirectionType,
+        "fields": Mapping[str, CodegenGenericDataFieldTypeDef],
     },
 )
 
-SortPropertyTypeDef = TypedDict(
-    "SortPropertyTypeDef",
+ListFormsResponseTypeDef = TypedDict(
+    "ListFormsResponseTypeDef",
     {
-        "field": str,
-        "direction": SortDirectionType,
+        "entities": List[FormSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartCodegenJobDataTypeDef = TypedDict(
-    "_RequiredStartCodegenJobDataTypeDef",
+FormCTATypeDef = TypedDict(
+    "FormCTATypeDef",
     {
-        "renderConfig": "CodegenJobRenderConfigTypeDef",
+        "position": FormButtonsPositionType,
+        "clear": FormButtonTypeDef,
+        "cancel": FormButtonTypeDef,
+        "submit": FormButtonTypeDef,
     },
+    total=False,
 )
-_OptionalStartCodegenJobDataTypeDef = TypedDict(
-    "_OptionalStartCodegenJobDataTypeDef",
+
+_RequiredValueMappingsOutputTypeDef = TypedDict(
+    "_RequiredValueMappingsOutputTypeDef",
     {
-        "genericDataSchema": "CodegenJobGenericDataSchemaTypeDef",
-        "autoGenerateForms": bool,
-        "features": "CodegenFeatureFlagsTypeDef",
-        "tags": Mapping[str, str],
+        "values": List[ValueMappingTypeDef],
+    },
+)
+_OptionalValueMappingsOutputTypeDef = TypedDict(
+    "_OptionalValueMappingsOutputTypeDef",
+    {
+        "bindingProperties": Dict[str, FormInputBindingPropertiesValueTypeDef],
     },
     total=False,
 )
 
-class StartCodegenJobDataTypeDef(
-    _RequiredStartCodegenJobDataTypeDef, _OptionalStartCodegenJobDataTypeDef
+class ValueMappingsOutputTypeDef(
+    _RequiredValueMappingsOutputTypeDef, _OptionalValueMappingsOutputTypeDef
 ):
     pass
 
-_RequiredStartCodegenJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartCodegenJobRequestRequestTypeDef",
+_RequiredValueMappingsTypeDef = TypedDict(
+    "_RequiredValueMappingsTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "codegenJobToCreate": "StartCodegenJobDataTypeDef",
+        "values": Sequence[ValueMappingTypeDef],
     },
 )
-_OptionalStartCodegenJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartCodegenJobRequestRequestTypeDef",
+_OptionalValueMappingsTypeDef = TypedDict(
+    "_OptionalValueMappingsTypeDef",
     {
-        "clientToken": str,
+        "bindingProperties": Mapping[str, FormInputBindingPropertiesValueTypeDef],
     },
     total=False,
 )
 
-class StartCodegenJobRequestRequestTypeDef(
-    _RequiredStartCodegenJobRequestRequestTypeDef, _OptionalStartCodegenJobRequestRequestTypeDef
-):
+class ValueMappingsTypeDef(_RequiredValueMappingsTypeDef, _OptionalValueMappingsTypeDef):
     pass
 
-StartCodegenJobResponseTypeDef = TypedDict(
-    "StartCodegenJobResponseTypeDef",
+_RequiredComponentChildOutputTypeDef = TypedDict(
+    "_RequiredComponentChildOutputTypeDef",
     {
-        "entity": "CodegenJobTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "componentType": str,
+        "name": str,
+        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
     },
 )
-
-ThemeSummaryTypeDef = TypedDict(
-    "ThemeSummaryTypeDef",
+_OptionalComponentChildOutputTypeDef = TypedDict(
+    "_OptionalComponentChildOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "name": str,
+        "children": List[Dict[str, Any]],
+        "events": Dict[str, ComponentEventOutputTypeDef],
+        "sourceId": str,
     },
+    total=False,
 )
 
-_RequiredThemeTypeDef = TypedDict(
-    "_RequiredThemeTypeDef",
+class ComponentChildOutputTypeDef(
+    _RequiredComponentChildOutputTypeDef, _OptionalComponentChildOutputTypeDef
+):
+    pass
+
+_RequiredComponentTypeDef = TypedDict(
+    "_RequiredComponentTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
+        "componentType": str,
+        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "variants": List[ComponentVariantOutputTypeDef],
+        "overrides": Dict[str, Dict[str, str]],
+        "bindingProperties": Dict[str, ComponentBindingPropertiesValueOutputTypeDef],
         "createdAt": datetime,
-        "values": List["ThemeValuesOutputTypeDef"],
     },
 )
-_OptionalThemeTypeDef = TypedDict(
-    "_OptionalThemeTypeDef",
+_OptionalComponentTypeDef = TypedDict(
+    "_OptionalComponentTypeDef",
     {
+        "sourceId": str,
+        "children": List["ComponentChildOutputTypeDef"],
+        "collectionProperties": Dict[str, ComponentDataConfigurationOutputTypeDef],
         "modifiedAt": datetime,
-        "overrides": List["ThemeValuesOutputTypeDef"],
         "tags": Dict[str, str],
+        "events": Dict[str, ComponentEventOutputTypeDef],
+        "schemaVersion": str,
     },
     total=False,
 )
 
-class ThemeTypeDef(_RequiredThemeTypeDef, _OptionalThemeTypeDef):
+class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
     pass
 
-ThemeValueOutputTypeDef = TypedDict(
-    "ThemeValueOutputTypeDef",
+_RequiredComponentChildTypeDef = TypedDict(
+    "_RequiredComponentChildTypeDef",
     {
-        "value": str,
-        "children": List[Dict[str, Any]],
+        "componentType": str,
+        "name": str,
+        "properties": Mapping[str, "ComponentPropertyTypeDef"],
     },
-    total=False,
 )
-
-ThemeValueTypeDef = TypedDict(
-    "ThemeValueTypeDef",
+_OptionalComponentChildTypeDef = TypedDict(
+    "_OptionalComponentChildTypeDef",
     {
-        "value": str,
         "children": Sequence[Dict[str, Any]],
+        "events": Mapping[str, ComponentEventTypeDef],
+        "sourceId": str,
     },
     total=False,
 )
 
-ThemeValuesOutputTypeDef = TypedDict(
-    "ThemeValuesOutputTypeDef",
+class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
+    pass
+
+_RequiredCreateComponentDataTypeDef = TypedDict(
+    "_RequiredCreateComponentDataTypeDef",
     {
-        "key": str,
-        "value": Dict[str, Any],
+        "name": str,
+        "componentType": str,
+        "properties": Mapping[str, "ComponentPropertyTypeDef"],
+        "variants": Sequence[ComponentVariantTypeDef],
+        "overrides": Mapping[str, Mapping[str, str]],
+        "bindingProperties": Mapping[str, ComponentBindingPropertiesValueTypeDef],
     },
-    total=False,
 )
-
-ThemeValuesTypeDef = TypedDict(
-    "ThemeValuesTypeDef",
+_OptionalCreateComponentDataTypeDef = TypedDict(
+    "_OptionalCreateComponentDataTypeDef",
     {
-        "key": str,
-        "value": Dict[str, Any],
+        "sourceId": str,
+        "children": Sequence["ComponentChildTypeDef"],
+        "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
+        "tags": Mapping[str, str],
+        "events": Mapping[str, ComponentEventTypeDef],
+        "schemaVersion": str,
     },
     total=False,
 )
 
+class CreateComponentDataTypeDef(
+    _RequiredCreateComponentDataTypeDef, _OptionalCreateComponentDataTypeDef
+):
+    pass
+
 UpdateComponentDataTypeDef = TypedDict(
     "UpdateComponentDataTypeDef",
     {
         "id": str,
         "name": str,
         "sourceId": str,
         "componentType": str,
         "properties": Mapping[str, "ComponentPropertyTypeDef"],
         "children": Sequence["ComponentChildTypeDef"],
-        "variants": Sequence["ComponentVariantTypeDef"],
+        "variants": Sequence[ComponentVariantTypeDef],
         "overrides": Mapping[str, Mapping[str, str]],
-        "bindingProperties": Mapping[str, "ComponentBindingPropertiesValueTypeDef"],
-        "collectionProperties": Mapping[str, "ComponentDataConfigurationTypeDef"],
-        "events": Mapping[str, "ComponentEventTypeDef"],
+        "bindingProperties": Mapping[str, ComponentBindingPropertiesValueTypeDef],
+        "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
+        "events": Mapping[str, ComponentEventTypeDef],
         "schemaVersion": str,
     },
     total=False,
 )
 
+CodegenJobGenericDataSchemaOutputTypeDef = TypedDict(
+    "CodegenJobGenericDataSchemaOutputTypeDef",
+    {
+        "dataSourceType": Literal["DataStore"],
+        "models": Dict[str, CodegenGenericDataModelOutputTypeDef],
+        "enums": Dict[str, CodegenGenericDataEnumOutputTypeDef],
+        "nonModels": Dict[str, CodegenGenericDataNonModelOutputTypeDef],
+    },
+)
+
+CodegenJobGenericDataSchemaTypeDef = TypedDict(
+    "CodegenJobGenericDataSchemaTypeDef",
+    {
+        "dataSourceType": Literal["DataStore"],
+        "models": Mapping[str, CodegenGenericDataModelTypeDef],
+        "enums": Mapping[str, CodegenGenericDataEnumTypeDef],
+        "nonModels": Mapping[str, CodegenGenericDataNonModelTypeDef],
+    },
+)
+
+_RequiredFieldInputConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldInputConfigOutputTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalFieldInputConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldInputConfigOutputTypeDef",
+    {
+        "required": bool,
+        "readOnly": bool,
+        "placeholder": str,
+        "defaultValue": str,
+        "descriptiveText": str,
+        "defaultChecked": bool,
+        "defaultCountryCode": str,
+        "valueMappings": ValueMappingsOutputTypeDef,
+        "name": str,
+        "minValue": float,
+        "maxValue": float,
+        "step": float,
+        "value": str,
+        "isArray": bool,
+        "fileUploaderConfig": FileUploaderFieldConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class FieldInputConfigOutputTypeDef(
+    _RequiredFieldInputConfigOutputTypeDef, _OptionalFieldInputConfigOutputTypeDef
+):
+    pass
+
+_RequiredFieldInputConfigTypeDef = TypedDict(
+    "_RequiredFieldInputConfigTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalFieldInputConfigTypeDef = TypedDict(
+    "_OptionalFieldInputConfigTypeDef",
+    {
+        "required": bool,
+        "readOnly": bool,
+        "placeholder": str,
+        "defaultValue": str,
+        "descriptiveText": str,
+        "defaultChecked": bool,
+        "defaultCountryCode": str,
+        "valueMappings": ValueMappingsTypeDef,
+        "name": str,
+        "minValue": float,
+        "maxValue": float,
+        "step": float,
+        "value": str,
+        "isArray": bool,
+        "fileUploaderConfig": FileUploaderFieldConfigTypeDef,
+    },
+    total=False,
+)
+
+class FieldInputConfigTypeDef(_RequiredFieldInputConfigTypeDef, _OptionalFieldInputConfigTypeDef):
+    pass
+
+CreateComponentResponseTypeDef = TypedDict(
+    "CreateComponentResponseTypeDef",
+    {
+        "entity": ComponentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportComponentsResponseTypeDef = TypedDict(
+    "ExportComponentsResponseTypeDef",
+    {
+        "entities": List[ComponentTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComponentResponseTypeDef = TypedDict(
+    "GetComponentResponseTypeDef",
+    {
+        "component": ComponentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateComponentResponseTypeDef = TypedDict(
+    "UpdateComponentResponseTypeDef",
+    {
+        "entity": ComponentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateComponentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateComponentRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "componentToCreate": CreateComponentDataTypeDef,
+    },
+)
+_OptionalCreateComponentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateComponentRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class CreateComponentRequestRequestTypeDef(
+    _RequiredCreateComponentRequestRequestTypeDef, _OptionalCreateComponentRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateComponentRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
-        "updatedComponent": "UpdateComponentDataTypeDef",
+        "updatedComponent": UpdateComponentDataTypeDef,
     },
 )
 _OptionalUpdateComponentRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateComponentRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -2316,181 +1980,262 @@
 )
 
 class UpdateComponentRequestRequestTypeDef(
     _RequiredUpdateComponentRequestRequestTypeDef, _OptionalUpdateComponentRequestRequestTypeDef
 ):
     pass
 
-UpdateComponentResponseTypeDef = TypedDict(
-    "UpdateComponentResponseTypeDef",
+_RequiredCodegenJobTypeDef = TypedDict(
+    "_RequiredCodegenJobTypeDef",
     {
-        "entity": "ComponentTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "id": str,
+        "appId": str,
+        "environmentName": str,
     },
 )
-
-UpdateFormDataTypeDef = TypedDict(
-    "UpdateFormDataTypeDef",
+_OptionalCodegenJobTypeDef = TypedDict(
+    "_OptionalCodegenJobTypeDef",
     {
-        "name": str,
-        "dataType": "FormDataTypeConfigTypeDef",
-        "formActionType": FormActionTypeType,
-        "fields": Mapping[str, "FieldConfigTypeDef"],
-        "style": "FormStyleTypeDef",
-        "sectionalElements": Mapping[str, "SectionalElementTypeDef"],
-        "schemaVersion": str,
-        "cta": "FormCTATypeDef",
-        "labelDecorator": LabelDecoratorType,
+        "renderConfig": CodegenJobRenderConfigTypeDef,
+        "genericDataSchema": CodegenJobGenericDataSchemaOutputTypeDef,
+        "autoGenerateForms": bool,
+        "features": CodegenFeatureFlagsTypeDef,
+        "status": CodegenJobStatusType,
+        "statusMessage": str,
+        "asset": CodegenJobAssetTypeDef,
+        "tags": Dict[str, str],
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
     total=False,
 )
 
-_RequiredUpdateFormRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFormRequestRequestTypeDef",
+class CodegenJobTypeDef(_RequiredCodegenJobTypeDef, _OptionalCodegenJobTypeDef):
+    pass
+
+_RequiredStartCodegenJobDataTypeDef = TypedDict(
+    "_RequiredStartCodegenJobDataTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "updatedForm": "UpdateFormDataTypeDef",
+        "renderConfig": CodegenJobRenderConfigTypeDef,
     },
 )
-_OptionalUpdateFormRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFormRequestRequestTypeDef",
+_OptionalStartCodegenJobDataTypeDef = TypedDict(
+    "_OptionalStartCodegenJobDataTypeDef",
     {
-        "clientToken": str,
+        "genericDataSchema": CodegenJobGenericDataSchemaTypeDef,
+        "autoGenerateForms": bool,
+        "features": CodegenFeatureFlagsTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class UpdateFormRequestRequestTypeDef(
-    _RequiredUpdateFormRequestRequestTypeDef, _OptionalUpdateFormRequestRequestTypeDef
+class StartCodegenJobDataTypeDef(
+    _RequiredStartCodegenJobDataTypeDef, _OptionalStartCodegenJobDataTypeDef
 ):
     pass
 
-UpdateFormResponseTypeDef = TypedDict(
-    "UpdateFormResponseTypeDef",
+FieldConfigOutputTypeDef = TypedDict(
+    "FieldConfigOutputTypeDef",
     {
-        "entity": "FormTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "label": str,
+        "position": FieldPositionTypeDef,
+        "excluded": bool,
+        "inputType": FieldInputConfigOutputTypeDef,
+        "validations": List[FieldValidationConfigurationOutputTypeDef],
     },
+    total=False,
 )
 
-_RequiredUpdateThemeDataTypeDef = TypedDict(
-    "_RequiredUpdateThemeDataTypeDef",
+FieldConfigTypeDef = TypedDict(
+    "FieldConfigTypeDef",
     {
-        "values": Sequence["ThemeValuesTypeDef"],
+        "label": str,
+        "position": FieldPositionTypeDef,
+        "excluded": bool,
+        "inputType": FieldInputConfigTypeDef,
+        "validations": Sequence[FieldValidationConfigurationTypeDef],
     },
+    total=False,
 )
-_OptionalUpdateThemeDataTypeDef = TypedDict(
-    "_OptionalUpdateThemeDataTypeDef",
+
+GetCodegenJobResponseTypeDef = TypedDict(
+    "GetCodegenJobResponseTypeDef",
     {
-        "id": str,
-        "name": str,
-        "overrides": Sequence["ThemeValuesTypeDef"],
+        "job": CodegenJobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateThemeDataTypeDef(_RequiredUpdateThemeDataTypeDef, _OptionalUpdateThemeDataTypeDef):
-    pass
+StartCodegenJobResponseTypeDef = TypedDict(
+    "StartCodegenJobResponseTypeDef",
+    {
+        "entity": CodegenJobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredUpdateThemeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateThemeRequestRequestTypeDef",
+_RequiredStartCodegenJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartCodegenJobRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
-        "id": str,
-        "updatedTheme": "UpdateThemeDataTypeDef",
+        "codegenJobToCreate": StartCodegenJobDataTypeDef,
     },
 )
-_OptionalUpdateThemeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateThemeRequestRequestTypeDef",
+_OptionalStartCodegenJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartCodegenJobRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-class UpdateThemeRequestRequestTypeDef(
-    _RequiredUpdateThemeRequestRequestTypeDef, _OptionalUpdateThemeRequestRequestTypeDef
+class StartCodegenJobRequestRequestTypeDef(
+    _RequiredStartCodegenJobRequestRequestTypeDef, _OptionalStartCodegenJobRequestRequestTypeDef
 ):
     pass
 
-UpdateThemeResponseTypeDef = TypedDict(
-    "UpdateThemeResponseTypeDef",
+_RequiredFormTypeDef = TypedDict(
+    "_RequiredFormTypeDef",
     {
-        "entity": "ThemeTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "name": str,
+        "formActionType": FormActionTypeType,
+        "style": FormStyleTypeDef,
+        "dataType": FormDataTypeConfigTypeDef,
+        "fields": Dict[str, FieldConfigOutputTypeDef],
+        "sectionalElements": Dict[str, SectionalElementTypeDef],
+        "schemaVersion": str,
     },
 )
+_OptionalFormTypeDef = TypedDict(
+    "_OptionalFormTypeDef",
+    {
+        "tags": Dict[str, str],
+        "cta": FormCTATypeDef,
+        "labelDecorator": LabelDecoratorType,
+    },
+    total=False,
+)
 
-_RequiredValueMappingOutputTypeDef = TypedDict(
-    "_RequiredValueMappingOutputTypeDef",
+class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
+    pass
+
+_RequiredCreateFormDataTypeDef = TypedDict(
+    "_RequiredCreateFormDataTypeDef",
     {
-        "value": "FormInputValuePropertyOutputTypeDef",
+        "name": str,
+        "dataType": FormDataTypeConfigTypeDef,
+        "formActionType": FormActionTypeType,
+        "fields": Mapping[str, FieldConfigTypeDef],
+        "style": FormStyleTypeDef,
+        "sectionalElements": Mapping[str, SectionalElementTypeDef],
+        "schemaVersion": str,
     },
 )
-_OptionalValueMappingOutputTypeDef = TypedDict(
-    "_OptionalValueMappingOutputTypeDef",
+_OptionalCreateFormDataTypeDef = TypedDict(
+    "_OptionalCreateFormDataTypeDef",
     {
-        "displayValue": "FormInputValuePropertyOutputTypeDef",
+        "cta": FormCTATypeDef,
+        "tags": Mapping[str, str],
+        "labelDecorator": LabelDecoratorType,
     },
     total=False,
 )
 
-class ValueMappingOutputTypeDef(
-    _RequiredValueMappingOutputTypeDef, _OptionalValueMappingOutputTypeDef
-):
+class CreateFormDataTypeDef(_RequiredCreateFormDataTypeDef, _OptionalCreateFormDataTypeDef):
     pass
 
-_RequiredValueMappingTypeDef = TypedDict(
-    "_RequiredValueMappingTypeDef",
+UpdateFormDataTypeDef = TypedDict(
+    "UpdateFormDataTypeDef",
     {
-        "value": "FormInputValuePropertyTypeDef",
+        "name": str,
+        "dataType": FormDataTypeConfigTypeDef,
+        "formActionType": FormActionTypeType,
+        "fields": Mapping[str, FieldConfigTypeDef],
+        "style": FormStyleTypeDef,
+        "sectionalElements": Mapping[str, SectionalElementTypeDef],
+        "schemaVersion": str,
+        "cta": FormCTATypeDef,
+        "labelDecorator": LabelDecoratorType,
     },
+    total=False,
 )
-_OptionalValueMappingTypeDef = TypedDict(
-    "_OptionalValueMappingTypeDef",
+
+CreateFormResponseTypeDef = TypedDict(
+    "CreateFormResponseTypeDef",
     {
-        "displayValue": "FormInputValuePropertyTypeDef",
+        "entity": FormTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ValueMappingTypeDef(_RequiredValueMappingTypeDef, _OptionalValueMappingTypeDef):
-    pass
+ExportFormsResponseTypeDef = TypedDict(
+    "ExportFormsResponseTypeDef",
+    {
+        "entities": List[FormTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredValueMappingsOutputTypeDef = TypedDict(
-    "_RequiredValueMappingsOutputTypeDef",
+GetFormResponseTypeDef = TypedDict(
+    "GetFormResponseTypeDef",
     {
-        "values": List["ValueMappingOutputTypeDef"],
+        "form": FormTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalValueMappingsOutputTypeDef = TypedDict(
-    "_OptionalValueMappingsOutputTypeDef",
+
+UpdateFormResponseTypeDef = TypedDict(
+    "UpdateFormResponseTypeDef",
+    {
+        "entity": FormTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateFormRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFormRequestRequestTypeDef",
     {
-        "bindingProperties": Dict[str, "FormInputBindingPropertiesValueOutputTypeDef"],
+        "appId": str,
+        "environmentName": str,
+        "formToCreate": CreateFormDataTypeDef,
+    },
+)
+_OptionalCreateFormRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFormRequestRequestTypeDef",
+    {
+        "clientToken": str,
     },
     total=False,
 )
 
-class ValueMappingsOutputTypeDef(
-    _RequiredValueMappingsOutputTypeDef, _OptionalValueMappingsOutputTypeDef
+class CreateFormRequestRequestTypeDef(
+    _RequiredCreateFormRequestRequestTypeDef, _OptionalCreateFormRequestRequestTypeDef
 ):
     pass
 
-_RequiredValueMappingsTypeDef = TypedDict(
-    "_RequiredValueMappingsTypeDef",
+_RequiredUpdateFormRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFormRequestRequestTypeDef",
     {
-        "values": Sequence["ValueMappingTypeDef"],
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "updatedForm": UpdateFormDataTypeDef,
     },
 )
-_OptionalValueMappingsTypeDef = TypedDict(
-    "_OptionalValueMappingsTypeDef",
+_OptionalUpdateFormRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFormRequestRequestTypeDef",
     {
-        "bindingProperties": Mapping[str, "FormInputBindingPropertiesValueTypeDef"],
+        "clientToken": str,
     },
     total=False,
 )
 
-class ValueMappingsTypeDef(_RequiredValueMappingsTypeDef, _OptionalValueMappingsTypeDef):
+class UpdateFormRequestRequestTypeDef(
+    _RequiredUpdateFormRequestRequestTypeDef, _OptionalUpdateFormRequestRequestTypeDef
+):
     pass
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifyuibuilder
-Version: 1.28.12
-Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifyuibuilder)](https://pepy.tech/project/mypy-boto3-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyUIBuilder 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[boto3.AmplifyUIBuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
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
 [mypy-boto3-amplifyuibuilder docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,177 +355,157 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
-    ActionParametersOutputTypeDef,
-    ActionParametersTypeDef,
-    CodegenFeatureFlagsOutputTypeDef,
+    MutationActionSetStateParameterTypeDef,
     CodegenFeatureFlagsTypeDef,
     CodegenGenericDataEnumOutputTypeDef,
     CodegenGenericDataEnumTypeDef,
-    CodegenGenericDataFieldOutputTypeDef,
-    CodegenGenericDataFieldTypeDef,
-    CodegenGenericDataModelOutputTypeDef,
-    CodegenGenericDataModelTypeDef,
-    CodegenGenericDataNonModelOutputTypeDef,
-    CodegenGenericDataNonModelTypeDef,
     CodegenGenericDataRelationshipTypeOutputTypeDef,
     CodegenGenericDataRelationshipTypeTypeDef,
     CodegenJobAssetTypeDef,
-    CodegenJobGenericDataSchemaOutputTypeDef,
-    CodegenJobGenericDataSchemaTypeDef,
-    CodegenJobRenderConfigOutputTypeDef,
-    CodegenJobRenderConfigTypeDef,
+    ReactStartCodegenJobDataTypeDef,
     CodegenJobSummaryTypeDef,
-    CodegenJobTypeDef,
-    ComponentBindingPropertiesValueOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
-    ComponentBindingPropertiesValueTypeDef,
-    ComponentChildOutputTypeDef,
-    ComponentChildTypeDef,
-    ComponentConditionPropertyOutputTypeDef,
     ComponentConditionPropertyTypeDef,
-    ComponentDataConfigurationOutputTypeDef,
-    ComponentDataConfigurationTypeDef,
-    ComponentEventOutputTypeDef,
-    ComponentEventTypeDef,
-    ComponentPropertyBindingPropertiesOutputTypeDef,
+    SortPropertyTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
-    ComponentPropertyOutputTypeDef,
-    ComponentPropertyTypeDef,
+    FormBindingElementTypeDef,
     ComponentSummaryTypeDef,
-    ComponentTypeDef,
     ComponentVariantOutputTypeDef,
     ComponentVariantTypeDef,
-    CreateComponentDataTypeDef,
-    CreateComponentRequestRequestTypeDef,
-    CreateComponentResponseTypeDef,
-    CreateFormDataTypeDef,
-    CreateFormRequestRequestTypeDef,
-    CreateFormResponseTypeDef,
+    ResponseMetadataTypeDef,
+    FormDataTypeConfigTypeDef,
     CreateThemeDataTypeDef,
-    CreateThemeRequestRequestTypeDef,
-    CreateThemeResponseTypeDef,
+    ThemeTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteFormRequestRequestTypeDef,
     DeleteThemeRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExchangeCodeForTokenRequestBodyTypeDef,
-    ExchangeCodeForTokenRequestRequestTypeDef,
-    ExchangeCodeForTokenResponseTypeDef,
-    ExportComponentsRequestExportComponentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ExportComponentsRequestRequestTypeDef,
-    ExportComponentsResponseTypeDef,
-    ExportFormsRequestExportFormsPaginateTypeDef,
     ExportFormsRequestRequestTypeDef,
-    ExportFormsResponseTypeDef,
-    ExportThemesRequestExportThemesPaginateTypeDef,
     ExportThemesRequestRequestTypeDef,
-    ExportThemesResponseTypeDef,
-    FieldConfigOutputTypeDef,
-    FieldConfigTypeDef,
-    FieldInputConfigOutputTypeDef,
-    FieldInputConfigTypeDef,
-    FieldPositionOutputTypeDef,
     FieldPositionTypeDef,
     FieldValidationConfigurationOutputTypeDef,
     FieldValidationConfigurationTypeDef,
     FileUploaderFieldConfigOutputTypeDef,
     FileUploaderFieldConfigTypeDef,
-    FormBindingElementOutputTypeDef,
-    FormBindingElementTypeDef,
-    FormButtonOutputTypeDef,
-    FormButtonTypeDef,
-    FormCTAOutputTypeDef,
-    FormCTATypeDef,
-    FormDataTypeConfigOutputTypeDef,
-    FormDataTypeConfigTypeDef,
-    FormInputBindingPropertiesValueOutputTypeDef,
-    FormInputBindingPropertiesValuePropertiesOutputTypeDef,
     FormInputBindingPropertiesValuePropertiesTypeDef,
-    FormInputBindingPropertiesValueTypeDef,
-    FormInputValuePropertyBindingPropertiesOutputTypeDef,
     FormInputValuePropertyBindingPropertiesTypeDef,
-    FormInputValuePropertyOutputTypeDef,
-    FormInputValuePropertyTypeDef,
-    FormStyleConfigOutputTypeDef,
     FormStyleConfigTypeDef,
-    FormStyleOutputTypeDef,
-    FormStyleTypeDef,
-    FormSummaryTypeDef,
-    FormTypeDef,
     GetCodegenJobRequestRequestTypeDef,
-    GetCodegenJobResponseTypeDef,
     GetComponentRequestRequestTypeDef,
-    GetComponentResponseTypeDef,
     GetFormRequestRequestTypeDef,
-    GetFormResponseTypeDef,
     GetMetadataRequestRequestTypeDef,
-    GetMetadataResponseTypeDef,
     GetThemeRequestRequestTypeDef,
-    GetThemeResponseTypeDef,
-    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
     ListCodegenJobsRequestRequestTypeDef,
-    ListCodegenJobsResponseTypeDef,
-    ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListComponentsResponseTypeDef,
-    ListFormsRequestListFormsPaginateTypeDef,
     ListFormsRequestRequestTypeDef,
-    ListFormsResponseTypeDef,
-    ListThemesRequestListThemesPaginateTypeDef,
     ListThemesRequestRequestTypeDef,
-    ListThemesResponseTypeDef,
-    MutationActionSetStateParameterOutputTypeDef,
-    MutationActionSetStateParameterTypeDef,
-    PaginatorConfigTypeDef,
+    ThemeSummaryTypeDef,
     PredicateOutputTypeDef,
     PredicateTypeDef,
     PutMetadataFlagBodyTypeDef,
-    PutMetadataFlagRequestRequestTypeDef,
-    ReactStartCodegenJobDataOutputTypeDef,
-    ReactStartCodegenJobDataTypeDef,
     RefreshTokenRequestBodyTypeDef,
-    RefreshTokenRequestRequestTypeDef,
-    RefreshTokenResponseTypeDef,
-    ResponseMetadataTypeDef,
-    SectionalElementOutputTypeDef,
-    SectionalElementTypeDef,
-    SortPropertyOutputTypeDef,
-    SortPropertyTypeDef,
-    StartCodegenJobDataTypeDef,
-    StartCodegenJobRequestRequestTypeDef,
-    StartCodegenJobResponseTypeDef,
-    ThemeSummaryTypeDef,
-    ThemeTypeDef,
     ThemeValueOutputTypeDef,
     ThemeValueTypeDef,
     ThemeValuesOutputTypeDef,
     ThemeValuesTypeDef,
-    UpdateComponentDataTypeDef,
-    UpdateComponentRequestRequestTypeDef,
-    UpdateComponentResponseTypeDef,
-    UpdateFormDataTypeDef,
-    UpdateFormRequestRequestTypeDef,
-    UpdateFormResponseTypeDef,
     UpdateThemeDataTypeDef,
-    UpdateThemeRequestRequestTypeDef,
-    UpdateThemeResponseTypeDef,
-    ValueMappingOutputTypeDef,
     ValueMappingTypeDef,
+    ActionParametersOutputTypeDef,
+    ActionParametersTypeDef,
+    CodegenGenericDataFieldOutputTypeDef,
+    CodegenGenericDataFieldTypeDef,
+    CodegenJobRenderConfigTypeDef,
+    ComponentBindingPropertiesValueOutputTypeDef,
+    ComponentBindingPropertiesValueTypeDef,
+    ComponentDataConfigurationOutputTypeDef,
+    ComponentDataConfigurationTypeDef,
+    ComponentPropertyOutputTypeDef,
+    ComponentPropertyTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExchangeCodeForTokenResponseTypeDef,
+    GetMetadataResponseTypeDef,
+    ListCodegenJobsResponseTypeDef,
+    ListComponentsResponseTypeDef,
+    RefreshTokenResponseTypeDef,
+    FormSummaryTypeDef,
+    CreateThemeRequestRequestTypeDef,
+    CreateThemeResponseTypeDef,
+    ExportThemesResponseTypeDef,
+    GetThemeResponseTypeDef,
+    UpdateThemeResponseTypeDef,
+    ExchangeCodeForTokenRequestRequestTypeDef,
+    ExportComponentsRequestExportComponentsPaginateTypeDef,
+    ExportFormsRequestExportFormsPaginateTypeDef,
+    ExportThemesRequestExportThemesPaginateTypeDef,
+    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    ListComponentsRequestListComponentsPaginateTypeDef,
+    ListFormsRequestListFormsPaginateTypeDef,
+    ListThemesRequestListThemesPaginateTypeDef,
+    FormButtonTypeDef,
+    SectionalElementTypeDef,
+    FormInputBindingPropertiesValueTypeDef,
+    FormInputValuePropertyTypeDef,
+    FormStyleTypeDef,
+    ListThemesResponseTypeDef,
+    PutMetadataFlagRequestRequestTypeDef,
+    RefreshTokenRequestRequestTypeDef,
+    UpdateThemeRequestRequestTypeDef,
+    ComponentEventOutputTypeDef,
+    ComponentEventTypeDef,
+    CodegenGenericDataModelOutputTypeDef,
+    CodegenGenericDataNonModelOutputTypeDef,
+    CodegenGenericDataModelTypeDef,
+    CodegenGenericDataNonModelTypeDef,
+    ListFormsResponseTypeDef,
+    FormCTATypeDef,
     ValueMappingsOutputTypeDef,
     ValueMappingsTypeDef,
+    ComponentChildOutputTypeDef,
+    ComponentTypeDef,
+    ComponentChildTypeDef,
+    CreateComponentDataTypeDef,
+    UpdateComponentDataTypeDef,
+    CodegenJobGenericDataSchemaOutputTypeDef,
+    CodegenJobGenericDataSchemaTypeDef,
+    FieldInputConfigOutputTypeDef,
+    FieldInputConfigTypeDef,
+    CreateComponentResponseTypeDef,
+    ExportComponentsResponseTypeDef,
+    GetComponentResponseTypeDef,
+    UpdateComponentResponseTypeDef,
+    CreateComponentRequestRequestTypeDef,
+    UpdateComponentRequestRequestTypeDef,
+    CodegenJobTypeDef,
+    StartCodegenJobDataTypeDef,
+    FieldConfigOutputTypeDef,
+    FieldConfigTypeDef,
+    GetCodegenJobResponseTypeDef,
+    StartCodegenJobResponseTypeDef,
+    StartCodegenJobRequestRequestTypeDef,
+    FormTypeDef,
+    CreateFormDataTypeDef,
+    UpdateFormDataTypeDef,
+    CreateFormResponseTypeDef,
+    ExportFormsResponseTypeDef,
+    GetFormResponseTypeDef,
+    UpdateFormResponseTypeDef,
+    CreateFormRequestRequestTypeDef,
+    UpdateFormRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActionParametersOutputTypeDef:
+def get_structure() -> MutationActionSetStateParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt` & `mypy-boto3-amplifyuibuilder-1.28.15/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.12/setup.py` & `mypy-boto3-amplifyuibuilder-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplifyuibuilder",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_amplifyuibuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AmplifyUIBuilder 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.AmplifyUIBuilder 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

