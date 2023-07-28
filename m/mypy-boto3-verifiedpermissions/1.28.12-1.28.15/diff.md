# Comparing `tmp/mypy-boto3-verifiedpermissions-1.28.12.tar.gz` & `tmp/mypy-boto3-verifiedpermissions-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-verifiedpermissions-1.28.12.tar", last modified: Thu Jul 27 11:49:47 2023, max compression
+gzip compressed data, was "mypy-boto3-verifiedpermissions-1.28.15.tar", last modified: Fri Jul 28 20:43:54 2023, max compression
```

## Comparing `mypy-boto3-verifiedpermissions-1.28.12.tar` & `mypy-boto3-verifiedpermissions-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.529473 mypy-boto3-verifiedpermissions-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16930 2023-07-27 11:49:47.525473 mypy-boto3-verifiedpermissions-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.517473 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21090 2023-07-27 11:48:14.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21055 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-07-27 11:48:16.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-27 11:48:16.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-27 11:48:14.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-27 11:48:14.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31636 2023-07-27 11:48:17.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31585 2023-07-27 11:48:16.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:47.525473 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16930 2023-07-27 11:49:47.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-27 11:49:47.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:47.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:47.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:47.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 11:49:47.000000 mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:47.529473 mypy-boto3-verifiedpermissions-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-27 11:48:13.000000 mypy-boto3-verifiedpermissions-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:54.866017 mypy-boto3-verifiedpermissions-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-07-28 20:43:54.862017 mypy-boto3-verifiedpermissions-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:54.850016 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21090 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21055 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31198 2023-07-28 20:40:54.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31147 2023-07-28 20:40:54.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:54.862017 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-07-28 20:43:54.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-28 20:43:54.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:54.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:54.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:54.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 20:43:54.000000 mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:54.866017 mypy-boto3-verifiedpermissions-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-28 20:40:53.000000 mypy-boto3-verifiedpermissions-1.28.15/setup.py
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/LICENSE` & `mypy-boto3-verifiedpermissions-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/PKG-INFO` & `mypy-boto3-verifiedpermissions-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-verifiedpermissions
-Version: 1.28.12
-Summary: Type annotations for boto3.VerifiedPermissions 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.VerifiedPermissions 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-verifiedpermissions)](https://pepy.tech/project/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
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
 [mypy-boto3-verifiedpermissions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,28 +344,26 @@
 ```python
 from mypy_boto3_verifiedpermissions.type_defs import (
     ActionIdentifierTypeDef,
     EntityIdentifierTypeDef,
     CognitoUserPoolConfigurationTypeDef,
     ContextDefinitionTypeDef,
     ResponseMetadataTypeDef,
-    EntityIdentifierOutputTypeDef,
     ValidationSettingsTypeDef,
     CreatePolicyTemplateInputRequestTypeDef,
     DeleteIdentitySourceInputRequestTypeDef,
     DeletePolicyInputRequestTypeDef,
     DeletePolicyStoreInputRequestTypeDef,
     DeletePolicyTemplateInputRequestTypeDef,
     DeterminingPolicyItemTypeDef,
     EvaluationErrorItemTypeDef,
     GetIdentitySourceInputRequestTypeDef,
     IdentitySourceDetailsTypeDef,
     GetPolicyInputRequestTypeDef,
     GetPolicyStoreInputRequestTypeDef,
-    ValidationSettingsOutputTypeDef,
     GetPolicyTemplateInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     IdentitySourceFilterTypeDef,
     IdentitySourceItemDetailsTypeDef,
     PaginatorConfigTypeDef,
     ListPolicyStoresInputRequestTypeDef,
     PolicyStoreItemTypeDef,
@@ -377,61 +375,61 @@
     SchemaDefinitionTypeDef,
     UpdateCognitoUserPoolConfigurationTypeDef,
     UpdateStaticPolicyDefinitionTypeDef,
     UpdatePolicyTemplateInputRequestTypeDef,
     AttributeValueTypeDef,
     EntityItemTypeDef,
     EntityReferenceTypeDef,
+    TemplateLinkedPolicyDefinitionDetailTypeDef,
+    TemplateLinkedPolicyDefinitionItemTypeDef,
     TemplateLinkedPolicyDefinitionTypeDef,
     ConfigurationTypeDef,
     CreateIdentitySourceOutputTypeDef,
+    CreatePolicyOutputTypeDef,
     CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateOutputTypeDef,
     GetPolicyTemplateOutputTypeDef,
     GetSchemaOutputTypeDef,
     PutSchemaOutputTypeDef,
     UpdateIdentitySourceOutputTypeDef,
+    UpdatePolicyOutputTypeDef,
     UpdatePolicyStoreOutputTypeDef,
     UpdatePolicyTemplateOutputTypeDef,
-    CreatePolicyOutputTypeDef,
-    TemplateLinkedPolicyDefinitionDetailTypeDef,
-    TemplateLinkedPolicyDefinitionItemTypeDef,
-    UpdatePolicyOutputTypeDef,
     CreatePolicyStoreInputRequestTypeDef,
+    GetPolicyStoreOutputTypeDef,
     UpdatePolicyStoreInputRequestTypeDef,
     IsAuthorizedOutputTypeDef,
     IsAuthorizedWithTokenOutputTypeDef,
     GetIdentitySourceOutputTypeDef,
-    GetPolicyStoreOutputTypeDef,
     ListIdentitySourcesInputRequestTypeDef,
     IdentitySourceItemTypeDef,
     ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
     ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
     ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyStoresOutputTypeDef,
     ListPolicyTemplatesOutputTypeDef,
     PutSchemaInputRequestTypeDef,
     UpdateConfigurationTypeDef,
     UpdatePolicyDefinitionTypeDef,
     EntitiesDefinitionTypeDef,
     PolicyFilterTypeDef,
-    PolicyDefinitionTypeDef,
-    CreateIdentitySourceInputRequestTypeDef,
     PolicyDefinitionDetailTypeDef,
     PolicyDefinitionItemTypeDef,
+    PolicyDefinitionTypeDef,
+    CreateIdentitySourceInputRequestTypeDef,
     ListIdentitySourcesOutputTypeDef,
     UpdateIdentitySourceInputRequestTypeDef,
     UpdatePolicyInputRequestTypeDef,
     IsAuthorizedInputRequestTypeDef,
     IsAuthorizedWithTokenInputRequestTypeDef,
     ListPoliciesInputListPoliciesPaginateTypeDef,
     ListPoliciesInputRequestTypeDef,
-    CreatePolicyInputRequestTypeDef,
     GetPolicyOutputTypeDef,
     PolicyItemTypeDef,
+    CreatePolicyInputRequestTypeDef,
     ListPoliciesOutputTypeDef,
 )
 
 
 def get_structure() -> ActionIdentifierTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/README.md` & `mypy-boto3-verifiedpermissions-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-verifiedpermissions)](https://pepy.tech/project/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
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
 [mypy-boto3-verifiedpermissions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,28 +312,26 @@
 ```python
 from mypy_boto3_verifiedpermissions.type_defs import (
     ActionIdentifierTypeDef,
     EntityIdentifierTypeDef,
     CognitoUserPoolConfigurationTypeDef,
     ContextDefinitionTypeDef,
     ResponseMetadataTypeDef,
-    EntityIdentifierOutputTypeDef,
     ValidationSettingsTypeDef,
     CreatePolicyTemplateInputRequestTypeDef,
     DeleteIdentitySourceInputRequestTypeDef,
     DeletePolicyInputRequestTypeDef,
     DeletePolicyStoreInputRequestTypeDef,
     DeletePolicyTemplateInputRequestTypeDef,
     DeterminingPolicyItemTypeDef,
     EvaluationErrorItemTypeDef,
     GetIdentitySourceInputRequestTypeDef,
     IdentitySourceDetailsTypeDef,
     GetPolicyInputRequestTypeDef,
     GetPolicyStoreInputRequestTypeDef,
-    ValidationSettingsOutputTypeDef,
     GetPolicyTemplateInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     IdentitySourceFilterTypeDef,
     IdentitySourceItemDetailsTypeDef,
     PaginatorConfigTypeDef,
     ListPolicyStoresInputRequestTypeDef,
     PolicyStoreItemTypeDef,
@@ -345,61 +343,61 @@
     SchemaDefinitionTypeDef,
     UpdateCognitoUserPoolConfigurationTypeDef,
     UpdateStaticPolicyDefinitionTypeDef,
     UpdatePolicyTemplateInputRequestTypeDef,
     AttributeValueTypeDef,
     EntityItemTypeDef,
     EntityReferenceTypeDef,
+    TemplateLinkedPolicyDefinitionDetailTypeDef,
+    TemplateLinkedPolicyDefinitionItemTypeDef,
     TemplateLinkedPolicyDefinitionTypeDef,
     ConfigurationTypeDef,
     CreateIdentitySourceOutputTypeDef,
+    CreatePolicyOutputTypeDef,
     CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateOutputTypeDef,
     GetPolicyTemplateOutputTypeDef,
     GetSchemaOutputTypeDef,
     PutSchemaOutputTypeDef,
     UpdateIdentitySourceOutputTypeDef,
+    UpdatePolicyOutputTypeDef,
     UpdatePolicyStoreOutputTypeDef,
     UpdatePolicyTemplateOutputTypeDef,
-    CreatePolicyOutputTypeDef,
-    TemplateLinkedPolicyDefinitionDetailTypeDef,
-    TemplateLinkedPolicyDefinitionItemTypeDef,
-    UpdatePolicyOutputTypeDef,
     CreatePolicyStoreInputRequestTypeDef,
+    GetPolicyStoreOutputTypeDef,
     UpdatePolicyStoreInputRequestTypeDef,
     IsAuthorizedOutputTypeDef,
     IsAuthorizedWithTokenOutputTypeDef,
     GetIdentitySourceOutputTypeDef,
-    GetPolicyStoreOutputTypeDef,
     ListIdentitySourcesInputRequestTypeDef,
     IdentitySourceItemTypeDef,
     ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
     ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
     ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyStoresOutputTypeDef,
     ListPolicyTemplatesOutputTypeDef,
     PutSchemaInputRequestTypeDef,
     UpdateConfigurationTypeDef,
     UpdatePolicyDefinitionTypeDef,
     EntitiesDefinitionTypeDef,
     PolicyFilterTypeDef,
-    PolicyDefinitionTypeDef,
-    CreateIdentitySourceInputRequestTypeDef,
     PolicyDefinitionDetailTypeDef,
     PolicyDefinitionItemTypeDef,
+    PolicyDefinitionTypeDef,
+    CreateIdentitySourceInputRequestTypeDef,
     ListIdentitySourcesOutputTypeDef,
     UpdateIdentitySourceInputRequestTypeDef,
     UpdatePolicyInputRequestTypeDef,
     IsAuthorizedInputRequestTypeDef,
     IsAuthorizedWithTokenInputRequestTypeDef,
     ListPoliciesInputListPoliciesPaginateTypeDef,
     ListPoliciesInputRequestTypeDef,
-    CreatePolicyInputRequestTypeDef,
     GetPolicyOutputTypeDef,
     PolicyItemTypeDef,
+    CreatePolicyInputRequestTypeDef,
     ListPoliciesOutputTypeDef,
 )
 
 
 def get_structure() -> ActionIdentifierTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/__init__.py` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/__init__.pyi` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/__main__.py` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VerifiedPermissions 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.VerifiedPermissions 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions\nOther"
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

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/client.py` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/client.pyi` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/literals.py` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/literals.pyi` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/paginator.py` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/paginator.pyi` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/type_defs.py` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,28 +29,26 @@
 
 __all__ = (
     "ActionIdentifierTypeDef",
     "EntityIdentifierTypeDef",
     "CognitoUserPoolConfigurationTypeDef",
     "ContextDefinitionTypeDef",
     "ResponseMetadataTypeDef",
-    "EntityIdentifierOutputTypeDef",
     "ValidationSettingsTypeDef",
     "CreatePolicyTemplateInputRequestTypeDef",
     "DeleteIdentitySourceInputRequestTypeDef",
     "DeletePolicyInputRequestTypeDef",
     "DeletePolicyStoreInputRequestTypeDef",
     "DeletePolicyTemplateInputRequestTypeDef",
     "DeterminingPolicyItemTypeDef",
     "EvaluationErrorItemTypeDef",
     "GetIdentitySourceInputRequestTypeDef",
     "IdentitySourceDetailsTypeDef",
     "GetPolicyInputRequestTypeDef",
     "GetPolicyStoreInputRequestTypeDef",
-    "ValidationSettingsOutputTypeDef",
     "GetPolicyTemplateInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "IdentitySourceFilterTypeDef",
     "IdentitySourceItemDetailsTypeDef",
     "PaginatorConfigTypeDef",
     "ListPolicyStoresInputRequestTypeDef",
     "PolicyStoreItemTypeDef",
@@ -62,61 +60,61 @@
     "SchemaDefinitionTypeDef",
     "UpdateCognitoUserPoolConfigurationTypeDef",
     "UpdateStaticPolicyDefinitionTypeDef",
     "UpdatePolicyTemplateInputRequestTypeDef",
     "AttributeValueTypeDef",
     "EntityItemTypeDef",
     "EntityReferenceTypeDef",
+    "TemplateLinkedPolicyDefinitionDetailTypeDef",
+    "TemplateLinkedPolicyDefinitionItemTypeDef",
     "TemplateLinkedPolicyDefinitionTypeDef",
     "ConfigurationTypeDef",
     "CreateIdentitySourceOutputTypeDef",
+    "CreatePolicyOutputTypeDef",
     "CreatePolicyStoreOutputTypeDef",
     "CreatePolicyTemplateOutputTypeDef",
     "GetPolicyTemplateOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "PutSchemaOutputTypeDef",
     "UpdateIdentitySourceOutputTypeDef",
+    "UpdatePolicyOutputTypeDef",
     "UpdatePolicyStoreOutputTypeDef",
     "UpdatePolicyTemplateOutputTypeDef",
-    "CreatePolicyOutputTypeDef",
-    "TemplateLinkedPolicyDefinitionDetailTypeDef",
-    "TemplateLinkedPolicyDefinitionItemTypeDef",
-    "UpdatePolicyOutputTypeDef",
     "CreatePolicyStoreInputRequestTypeDef",
+    "GetPolicyStoreOutputTypeDef",
     "UpdatePolicyStoreInputRequestTypeDef",
     "IsAuthorizedOutputTypeDef",
     "IsAuthorizedWithTokenOutputTypeDef",
     "GetIdentitySourceOutputTypeDef",
-    "GetPolicyStoreOutputTypeDef",
     "ListIdentitySourcesInputRequestTypeDef",
     "IdentitySourceItemTypeDef",
     "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
     "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
     "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyStoresOutputTypeDef",
     "ListPolicyTemplatesOutputTypeDef",
     "PutSchemaInputRequestTypeDef",
     "UpdateConfigurationTypeDef",
     "UpdatePolicyDefinitionTypeDef",
     "EntitiesDefinitionTypeDef",
     "PolicyFilterTypeDef",
-    "PolicyDefinitionTypeDef",
-    "CreateIdentitySourceInputRequestTypeDef",
     "PolicyDefinitionDetailTypeDef",
     "PolicyDefinitionItemTypeDef",
+    "PolicyDefinitionTypeDef",
+    "CreateIdentitySourceInputRequestTypeDef",
     "ListIdentitySourcesOutputTypeDef",
     "UpdateIdentitySourceInputRequestTypeDef",
     "UpdatePolicyInputRequestTypeDef",
     "IsAuthorizedInputRequestTypeDef",
     "IsAuthorizedWithTokenInputRequestTypeDef",
     "ListPoliciesInputListPoliciesPaginateTypeDef",
     "ListPoliciesInputRequestTypeDef",
-    "CreatePolicyInputRequestTypeDef",
     "GetPolicyOutputTypeDef",
     "PolicyItemTypeDef",
+    "CreatePolicyInputRequestTypeDef",
     "ListPoliciesOutputTypeDef",
 )
 
 ActionIdentifierTypeDef = TypedDict(
     "ActionIdentifierTypeDef",
     {
         "actionType": str,
@@ -168,22 +166,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-EntityIdentifierOutputTypeDef = TypedDict(
-    "EntityIdentifierOutputTypeDef",
-    {
-        "entityType": str,
-        "entityId": str,
-    },
-)
-
 ValidationSettingsTypeDef = TypedDict(
     "ValidationSettingsTypeDef",
     {
         "mode": ValidationModeType,
     },
 )
 
@@ -286,21 +276,14 @@
 GetPolicyStoreInputRequestTypeDef = TypedDict(
     "GetPolicyStoreInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 
-ValidationSettingsOutputTypeDef = TypedDict(
-    "ValidationSettingsOutputTypeDef",
-    {
-        "mode": ValidationModeType,
-    },
-)
-
 GetPolicyTemplateInputRequestTypeDef = TypedDict(
     "GetPolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
     },
 )
@@ -568,14 +551,60 @@
     {
         "unspecified": bool,
         "identifier": EntityIdentifierTypeDef,
     },
     total=False,
 )
 
+_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
+    "_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef",
+    {
+        "policyTemplateId": str,
+    },
+)
+_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
+    "_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef",
+    {
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
+    },
+    total=False,
+)
+
+
+class TemplateLinkedPolicyDefinitionDetailTypeDef(
+    _RequiredTemplateLinkedPolicyDefinitionDetailTypeDef,
+    _OptionalTemplateLinkedPolicyDefinitionDetailTypeDef,
+):
+    pass
+
+
+_RequiredTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
+    "_RequiredTemplateLinkedPolicyDefinitionItemTypeDef",
+    {
+        "policyTemplateId": str,
+    },
+)
+_OptionalTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
+    "_OptionalTemplateLinkedPolicyDefinitionItemTypeDef",
+    {
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
+    },
+    total=False,
+)
+
+
+class TemplateLinkedPolicyDefinitionItemTypeDef(
+    _RequiredTemplateLinkedPolicyDefinitionItemTypeDef,
+    _OptionalTemplateLinkedPolicyDefinitionItemTypeDef,
+):
+    pass
+
+
 _RequiredTemplateLinkedPolicyDefinitionTypeDef = TypedDict(
     "_RequiredTemplateLinkedPolicyDefinitionTypeDef",
     {
         "policyTemplateId": str,
     },
 )
 _OptionalTemplateLinkedPolicyDefinitionTypeDef = TypedDict(
@@ -609,14 +638,28 @@
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreatePolicyOutputTypeDef = TypedDict(
+    "CreatePolicyOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyId": str,
+        "policyType": PolicyTypeType,
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreatePolicyStoreOutputTypeDef = TypedDict(
     "CreatePolicyStoreOutputTypeDef",
     {
         "policyStoreId": str,
         "arn": str,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
@@ -677,104 +720,44 @@
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePolicyStoreOutputTypeDef = TypedDict(
-    "UpdatePolicyStoreOutputTypeDef",
+UpdatePolicyOutputTypeDef = TypedDict(
+    "UpdatePolicyOutputTypeDef",
     {
         "policyStoreId": str,
-        "arn": str,
+        "policyId": str,
+        "policyType": PolicyTypeType,
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePolicyTemplateOutputTypeDef = TypedDict(
-    "UpdatePolicyTemplateOutputTypeDef",
+UpdatePolicyStoreOutputTypeDef = TypedDict(
+    "UpdatePolicyStoreOutputTypeDef",
     {
         "policyStoreId": str,
-        "policyTemplateId": str,
+        "arn": str,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreatePolicyOutputTypeDef = TypedDict(
-    "CreatePolicyOutputTypeDef",
+UpdatePolicyTemplateOutputTypeDef = TypedDict(
+    "UpdatePolicyTemplateOutputTypeDef",
     {
         "policyStoreId": str,
-        "policyId": str,
-        "policyType": PolicyTypeType,
-        "principal": EntityIdentifierOutputTypeDef,
-        "resource": EntityIdentifierOutputTypeDef,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
-    "_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef",
-    {
-        "policyTemplateId": str,
-    },
-)
-_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
-    "_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef",
-    {
-        "principal": EntityIdentifierOutputTypeDef,
-        "resource": EntityIdentifierOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class TemplateLinkedPolicyDefinitionDetailTypeDef(
-    _RequiredTemplateLinkedPolicyDefinitionDetailTypeDef,
-    _OptionalTemplateLinkedPolicyDefinitionDetailTypeDef,
-):
-    pass
-
-
-_RequiredTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
-    "_RequiredTemplateLinkedPolicyDefinitionItemTypeDef",
-    {
         "policyTemplateId": str,
-    },
-)
-_OptionalTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
-    "_OptionalTemplateLinkedPolicyDefinitionItemTypeDef",
-    {
-        "principal": EntityIdentifierOutputTypeDef,
-        "resource": EntityIdentifierOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class TemplateLinkedPolicyDefinitionItemTypeDef(
-    _RequiredTemplateLinkedPolicyDefinitionItemTypeDef,
-    _OptionalTemplateLinkedPolicyDefinitionItemTypeDef,
-):
-    pass
-
-
-UpdatePolicyOutputTypeDef = TypedDict(
-    "UpdatePolicyOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyId": str,
-        "policyType": PolicyTypeType,
-        "principal": EntityIdentifierOutputTypeDef,
-        "resource": EntityIdentifierOutputTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePolicyStoreInputRequestTypeDef = TypedDict(
@@ -794,14 +777,26 @@
 
 class CreatePolicyStoreInputRequestTypeDef(
     _RequiredCreatePolicyStoreInputRequestTypeDef, _OptionalCreatePolicyStoreInputRequestTypeDef
 ):
     pass
 
 
+GetPolicyStoreOutputTypeDef = TypedDict(
+    "GetPolicyStoreOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "arn": str,
+        "validationSettings": ValidationSettingsTypeDef,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdatePolicyStoreInputRequestTypeDef = TypedDict(
     "UpdatePolicyStoreInputRequestTypeDef",
     {
         "policyStoreId": str,
         "validationSettings": ValidationSettingsTypeDef,
     },
 )
@@ -835,26 +830,14 @@
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "principalEntityType": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetPolicyStoreOutputTypeDef = TypedDict(
-    "GetPolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "validationSettings": ValidationSettingsOutputTypeDef,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredListIdentitySourcesInputRequestTypeDef = TypedDict(
     "_RequiredListIdentitySourcesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListIdentitySourcesInputRequestTypeDef = TypedDict(
@@ -996,14 +979,32 @@
         "resource": EntityReferenceTypeDef,
         "policyType": PolicyTypeType,
         "policyTemplateId": str,
     },
     total=False,
 )
 
+PolicyDefinitionDetailTypeDef = TypedDict(
+    "PolicyDefinitionDetailTypeDef",
+    {
+        "static": StaticPolicyDefinitionDetailTypeDef,
+        "templateLinked": TemplateLinkedPolicyDefinitionDetailTypeDef,
+    },
+    total=False,
+)
+
+PolicyDefinitionItemTypeDef = TypedDict(
+    "PolicyDefinitionItemTypeDef",
+    {
+        "static": StaticPolicyDefinitionItemTypeDef,
+        "templateLinked": TemplateLinkedPolicyDefinitionItemTypeDef,
+    },
+    total=False,
+)
+
 PolicyDefinitionTypeDef = TypedDict(
     "PolicyDefinitionTypeDef",
     {
         "static": StaticPolicyDefinitionTypeDef,
         "templateLinked": TemplateLinkedPolicyDefinitionTypeDef,
     },
     total=False,
@@ -1029,32 +1030,14 @@
 class CreateIdentitySourceInputRequestTypeDef(
     _RequiredCreateIdentitySourceInputRequestTypeDef,
     _OptionalCreateIdentitySourceInputRequestTypeDef,
 ):
     pass
 
 
-PolicyDefinitionDetailTypeDef = TypedDict(
-    "PolicyDefinitionDetailTypeDef",
-    {
-        "static": StaticPolicyDefinitionDetailTypeDef,
-        "templateLinked": TemplateLinkedPolicyDefinitionDetailTypeDef,
-    },
-    total=False,
-)
-
-PolicyDefinitionItemTypeDef = TypedDict(
-    "PolicyDefinitionItemTypeDef",
-    {
-        "static": StaticPolicyDefinitionItemTypeDef,
-        "templateLinked": TemplateLinkedPolicyDefinitionItemTypeDef,
-    },
-    total=False,
-)
-
 ListIdentitySourcesOutputTypeDef = TypedDict(
     "ListIdentitySourcesOutputTypeDef",
     {
         "nextToken": str,
         "identitySources": List[IdentitySourceItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1187,44 +1170,22 @@
 
 class ListPoliciesInputRequestTypeDef(
     _RequiredListPoliciesInputRequestTypeDef, _OptionalListPoliciesInputRequestTypeDef
 ):
     pass
 
 
-_RequiredCreatePolicyInputRequestTypeDef = TypedDict(
-    "_RequiredCreatePolicyInputRequestTypeDef",
-    {
-        "policyStoreId": str,
-        "definition": PolicyDefinitionTypeDef,
-    },
-)
-_OptionalCreatePolicyInputRequestTypeDef = TypedDict(
-    "_OptionalCreatePolicyInputRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class CreatePolicyInputRequestTypeDef(
-    _RequiredCreatePolicyInputRequestTypeDef, _OptionalCreatePolicyInputRequestTypeDef
-):
-    pass
-
-
 GetPolicyOutputTypeDef = TypedDict(
     "GetPolicyOutputTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
         "policyType": PolicyTypeType,
-        "principal": EntityIdentifierOutputTypeDef,
-        "resource": EntityIdentifierOutputTypeDef,
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
         "definition": PolicyDefinitionDetailTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1238,25 +1199,47 @@
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
     },
 )
 _OptionalPolicyItemTypeDef = TypedDict(
     "_OptionalPolicyItemTypeDef",
     {
-        "principal": EntityIdentifierOutputTypeDef,
-        "resource": EntityIdentifierOutputTypeDef,
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
     },
     total=False,
 )
 
 
 class PolicyItemTypeDef(_RequiredPolicyItemTypeDef, _OptionalPolicyItemTypeDef):
     pass
 
 
+_RequiredCreatePolicyInputRequestTypeDef = TypedDict(
+    "_RequiredCreatePolicyInputRequestTypeDef",
+    {
+        "policyStoreId": str,
+        "definition": PolicyDefinitionTypeDef,
+    },
+)
+_OptionalCreatePolicyInputRequestTypeDef = TypedDict(
+    "_OptionalCreatePolicyInputRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class CreatePolicyInputRequestTypeDef(
+    _RequiredCreatePolicyInputRequestTypeDef, _OptionalCreatePolicyInputRequestTypeDef
+):
+    pass
+
+
 ListPoliciesOutputTypeDef = TypedDict(
     "ListPoliciesOutputTypeDef",
     {
         "nextToken": str,
         "policies": List[PolicyItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions/type_defs.pyi` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -28,28 +28,26 @@
 
 __all__ = (
     "ActionIdentifierTypeDef",
     "EntityIdentifierTypeDef",
     "CognitoUserPoolConfigurationTypeDef",
     "ContextDefinitionTypeDef",
     "ResponseMetadataTypeDef",
-    "EntityIdentifierOutputTypeDef",
     "ValidationSettingsTypeDef",
     "CreatePolicyTemplateInputRequestTypeDef",
     "DeleteIdentitySourceInputRequestTypeDef",
     "DeletePolicyInputRequestTypeDef",
     "DeletePolicyStoreInputRequestTypeDef",
     "DeletePolicyTemplateInputRequestTypeDef",
     "DeterminingPolicyItemTypeDef",
     "EvaluationErrorItemTypeDef",
     "GetIdentitySourceInputRequestTypeDef",
     "IdentitySourceDetailsTypeDef",
     "GetPolicyInputRequestTypeDef",
     "GetPolicyStoreInputRequestTypeDef",
-    "ValidationSettingsOutputTypeDef",
     "GetPolicyTemplateInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "IdentitySourceFilterTypeDef",
     "IdentitySourceItemDetailsTypeDef",
     "PaginatorConfigTypeDef",
     "ListPolicyStoresInputRequestTypeDef",
     "PolicyStoreItemTypeDef",
@@ -61,61 +59,61 @@
     "SchemaDefinitionTypeDef",
     "UpdateCognitoUserPoolConfigurationTypeDef",
     "UpdateStaticPolicyDefinitionTypeDef",
     "UpdatePolicyTemplateInputRequestTypeDef",
     "AttributeValueTypeDef",
     "EntityItemTypeDef",
     "EntityReferenceTypeDef",
+    "TemplateLinkedPolicyDefinitionDetailTypeDef",
+    "TemplateLinkedPolicyDefinitionItemTypeDef",
     "TemplateLinkedPolicyDefinitionTypeDef",
     "ConfigurationTypeDef",
     "CreateIdentitySourceOutputTypeDef",
+    "CreatePolicyOutputTypeDef",
     "CreatePolicyStoreOutputTypeDef",
     "CreatePolicyTemplateOutputTypeDef",
     "GetPolicyTemplateOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "PutSchemaOutputTypeDef",
     "UpdateIdentitySourceOutputTypeDef",
+    "UpdatePolicyOutputTypeDef",
     "UpdatePolicyStoreOutputTypeDef",
     "UpdatePolicyTemplateOutputTypeDef",
-    "CreatePolicyOutputTypeDef",
-    "TemplateLinkedPolicyDefinitionDetailTypeDef",
-    "TemplateLinkedPolicyDefinitionItemTypeDef",
-    "UpdatePolicyOutputTypeDef",
     "CreatePolicyStoreInputRequestTypeDef",
+    "GetPolicyStoreOutputTypeDef",
     "UpdatePolicyStoreInputRequestTypeDef",
     "IsAuthorizedOutputTypeDef",
     "IsAuthorizedWithTokenOutputTypeDef",
     "GetIdentitySourceOutputTypeDef",
-    "GetPolicyStoreOutputTypeDef",
     "ListIdentitySourcesInputRequestTypeDef",
     "IdentitySourceItemTypeDef",
     "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
     "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
     "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyStoresOutputTypeDef",
     "ListPolicyTemplatesOutputTypeDef",
     "PutSchemaInputRequestTypeDef",
     "UpdateConfigurationTypeDef",
     "UpdatePolicyDefinitionTypeDef",
     "EntitiesDefinitionTypeDef",
     "PolicyFilterTypeDef",
-    "PolicyDefinitionTypeDef",
-    "CreateIdentitySourceInputRequestTypeDef",
     "PolicyDefinitionDetailTypeDef",
     "PolicyDefinitionItemTypeDef",
+    "PolicyDefinitionTypeDef",
+    "CreateIdentitySourceInputRequestTypeDef",
     "ListIdentitySourcesOutputTypeDef",
     "UpdateIdentitySourceInputRequestTypeDef",
     "UpdatePolicyInputRequestTypeDef",
     "IsAuthorizedInputRequestTypeDef",
     "IsAuthorizedWithTokenInputRequestTypeDef",
     "ListPoliciesInputListPoliciesPaginateTypeDef",
     "ListPoliciesInputRequestTypeDef",
-    "CreatePolicyInputRequestTypeDef",
     "GetPolicyOutputTypeDef",
     "PolicyItemTypeDef",
+    "CreatePolicyInputRequestTypeDef",
     "ListPoliciesOutputTypeDef",
 )
 
 ActionIdentifierTypeDef = TypedDict(
     "ActionIdentifierTypeDef",
     {
         "actionType": str,
@@ -165,22 +163,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-EntityIdentifierOutputTypeDef = TypedDict(
-    "EntityIdentifierOutputTypeDef",
-    {
-        "entityType": str,
-        "entityId": str,
-    },
-)
-
 ValidationSettingsTypeDef = TypedDict(
     "ValidationSettingsTypeDef",
     {
         "mode": ValidationModeType,
     },
 )
 
@@ -281,21 +271,14 @@
 GetPolicyStoreInputRequestTypeDef = TypedDict(
     "GetPolicyStoreInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 
-ValidationSettingsOutputTypeDef = TypedDict(
-    "ValidationSettingsOutputTypeDef",
-    {
-        "mode": ValidationModeType,
-    },
-)
-
 GetPolicyTemplateInputRequestTypeDef = TypedDict(
     "GetPolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
     },
 )
@@ -547,14 +530,56 @@
     {
         "unspecified": bool,
         "identifier": EntityIdentifierTypeDef,
     },
     total=False,
 )
 
+_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
+    "_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef",
+    {
+        "policyTemplateId": str,
+    },
+)
+_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
+    "_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef",
+    {
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
+    },
+    total=False,
+)
+
+class TemplateLinkedPolicyDefinitionDetailTypeDef(
+    _RequiredTemplateLinkedPolicyDefinitionDetailTypeDef,
+    _OptionalTemplateLinkedPolicyDefinitionDetailTypeDef,
+):
+    pass
+
+_RequiredTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
+    "_RequiredTemplateLinkedPolicyDefinitionItemTypeDef",
+    {
+        "policyTemplateId": str,
+    },
+)
+_OptionalTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
+    "_OptionalTemplateLinkedPolicyDefinitionItemTypeDef",
+    {
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
+    },
+    total=False,
+)
+
+class TemplateLinkedPolicyDefinitionItemTypeDef(
+    _RequiredTemplateLinkedPolicyDefinitionItemTypeDef,
+    _OptionalTemplateLinkedPolicyDefinitionItemTypeDef,
+):
+    pass
+
 _RequiredTemplateLinkedPolicyDefinitionTypeDef = TypedDict(
     "_RequiredTemplateLinkedPolicyDefinitionTypeDef",
     {
         "policyTemplateId": str,
     },
 )
 _OptionalTemplateLinkedPolicyDefinitionTypeDef = TypedDict(
@@ -586,14 +611,28 @@
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreatePolicyOutputTypeDef = TypedDict(
+    "CreatePolicyOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyId": str,
+        "policyType": PolicyTypeType,
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreatePolicyStoreOutputTypeDef = TypedDict(
     "CreatePolicyStoreOutputTypeDef",
     {
         "policyStoreId": str,
         "arn": str,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
@@ -654,100 +693,44 @@
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePolicyStoreOutputTypeDef = TypedDict(
-    "UpdatePolicyStoreOutputTypeDef",
+UpdatePolicyOutputTypeDef = TypedDict(
+    "UpdatePolicyOutputTypeDef",
     {
         "policyStoreId": str,
-        "arn": str,
+        "policyId": str,
+        "policyType": PolicyTypeType,
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdatePolicyTemplateOutputTypeDef = TypedDict(
-    "UpdatePolicyTemplateOutputTypeDef",
+UpdatePolicyStoreOutputTypeDef = TypedDict(
+    "UpdatePolicyStoreOutputTypeDef",
     {
         "policyStoreId": str,
-        "policyTemplateId": str,
+        "arn": str,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreatePolicyOutputTypeDef = TypedDict(
-    "CreatePolicyOutputTypeDef",
+UpdatePolicyTemplateOutputTypeDef = TypedDict(
+    "UpdatePolicyTemplateOutputTypeDef",
     {
         "policyStoreId": str,
-        "policyId": str,
-        "policyType": PolicyTypeType,
-        "principal": EntityIdentifierOutputTypeDef,
-        "resource": EntityIdentifierOutputTypeDef,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
-    "_RequiredTemplateLinkedPolicyDefinitionDetailTypeDef",
-    {
-        "policyTemplateId": str,
-    },
-)
-_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef = TypedDict(
-    "_OptionalTemplateLinkedPolicyDefinitionDetailTypeDef",
-    {
-        "principal": EntityIdentifierOutputTypeDef,
-        "resource": EntityIdentifierOutputTypeDef,
-    },
-    total=False,
-)
-
-class TemplateLinkedPolicyDefinitionDetailTypeDef(
-    _RequiredTemplateLinkedPolicyDefinitionDetailTypeDef,
-    _OptionalTemplateLinkedPolicyDefinitionDetailTypeDef,
-):
-    pass
-
-_RequiredTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
-    "_RequiredTemplateLinkedPolicyDefinitionItemTypeDef",
-    {
         "policyTemplateId": str,
-    },
-)
-_OptionalTemplateLinkedPolicyDefinitionItemTypeDef = TypedDict(
-    "_OptionalTemplateLinkedPolicyDefinitionItemTypeDef",
-    {
-        "principal": EntityIdentifierOutputTypeDef,
-        "resource": EntityIdentifierOutputTypeDef,
-    },
-    total=False,
-)
-
-class TemplateLinkedPolicyDefinitionItemTypeDef(
-    _RequiredTemplateLinkedPolicyDefinitionItemTypeDef,
-    _OptionalTemplateLinkedPolicyDefinitionItemTypeDef,
-):
-    pass
-
-UpdatePolicyOutputTypeDef = TypedDict(
-    "UpdatePolicyOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyId": str,
-        "policyType": PolicyTypeType,
-        "principal": EntityIdentifierOutputTypeDef,
-        "resource": EntityIdentifierOutputTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePolicyStoreInputRequestTypeDef = TypedDict(
@@ -765,14 +748,26 @@
 )
 
 class CreatePolicyStoreInputRequestTypeDef(
     _RequiredCreatePolicyStoreInputRequestTypeDef, _OptionalCreatePolicyStoreInputRequestTypeDef
 ):
     pass
 
+GetPolicyStoreOutputTypeDef = TypedDict(
+    "GetPolicyStoreOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "arn": str,
+        "validationSettings": ValidationSettingsTypeDef,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdatePolicyStoreInputRequestTypeDef = TypedDict(
     "UpdatePolicyStoreInputRequestTypeDef",
     {
         "policyStoreId": str,
         "validationSettings": ValidationSettingsTypeDef,
     },
 )
@@ -806,26 +801,14 @@
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "principalEntityType": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetPolicyStoreOutputTypeDef = TypedDict(
-    "GetPolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "validationSettings": ValidationSettingsOutputTypeDef,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredListIdentitySourcesInputRequestTypeDef = TypedDict(
     "_RequiredListIdentitySourcesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListIdentitySourcesInputRequestTypeDef = TypedDict(
@@ -961,14 +944,32 @@
         "resource": EntityReferenceTypeDef,
         "policyType": PolicyTypeType,
         "policyTemplateId": str,
     },
     total=False,
 )
 
+PolicyDefinitionDetailTypeDef = TypedDict(
+    "PolicyDefinitionDetailTypeDef",
+    {
+        "static": StaticPolicyDefinitionDetailTypeDef,
+        "templateLinked": TemplateLinkedPolicyDefinitionDetailTypeDef,
+    },
+    total=False,
+)
+
+PolicyDefinitionItemTypeDef = TypedDict(
+    "PolicyDefinitionItemTypeDef",
+    {
+        "static": StaticPolicyDefinitionItemTypeDef,
+        "templateLinked": TemplateLinkedPolicyDefinitionItemTypeDef,
+    },
+    total=False,
+)
+
 PolicyDefinitionTypeDef = TypedDict(
     "PolicyDefinitionTypeDef",
     {
         "static": StaticPolicyDefinitionTypeDef,
         "templateLinked": TemplateLinkedPolicyDefinitionTypeDef,
     },
     total=False,
@@ -992,32 +993,14 @@
 
 class CreateIdentitySourceInputRequestTypeDef(
     _RequiredCreateIdentitySourceInputRequestTypeDef,
     _OptionalCreateIdentitySourceInputRequestTypeDef,
 ):
     pass
 
-PolicyDefinitionDetailTypeDef = TypedDict(
-    "PolicyDefinitionDetailTypeDef",
-    {
-        "static": StaticPolicyDefinitionDetailTypeDef,
-        "templateLinked": TemplateLinkedPolicyDefinitionDetailTypeDef,
-    },
-    total=False,
-)
-
-PolicyDefinitionItemTypeDef = TypedDict(
-    "PolicyDefinitionItemTypeDef",
-    {
-        "static": StaticPolicyDefinitionItemTypeDef,
-        "templateLinked": TemplateLinkedPolicyDefinitionItemTypeDef,
-    },
-    total=False,
-)
-
 ListIdentitySourcesOutputTypeDef = TypedDict(
     "ListIdentitySourcesOutputTypeDef",
     {
         "nextToken": str,
         "identitySources": List[IdentitySourceItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1140,42 +1123,22 @@
 )
 
 class ListPoliciesInputRequestTypeDef(
     _RequiredListPoliciesInputRequestTypeDef, _OptionalListPoliciesInputRequestTypeDef
 ):
     pass
 
-_RequiredCreatePolicyInputRequestTypeDef = TypedDict(
-    "_RequiredCreatePolicyInputRequestTypeDef",
-    {
-        "policyStoreId": str,
-        "definition": PolicyDefinitionTypeDef,
-    },
-)
-_OptionalCreatePolicyInputRequestTypeDef = TypedDict(
-    "_OptionalCreatePolicyInputRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class CreatePolicyInputRequestTypeDef(
-    _RequiredCreatePolicyInputRequestTypeDef, _OptionalCreatePolicyInputRequestTypeDef
-):
-    pass
-
 GetPolicyOutputTypeDef = TypedDict(
     "GetPolicyOutputTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
         "policyType": PolicyTypeType,
-        "principal": EntityIdentifierOutputTypeDef,
-        "resource": EntityIdentifierOutputTypeDef,
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
         "definition": PolicyDefinitionDetailTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1189,23 +1152,43 @@
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
     },
 )
 _OptionalPolicyItemTypeDef = TypedDict(
     "_OptionalPolicyItemTypeDef",
     {
-        "principal": EntityIdentifierOutputTypeDef,
-        "resource": EntityIdentifierOutputTypeDef,
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
     },
     total=False,
 )
 
 class PolicyItemTypeDef(_RequiredPolicyItemTypeDef, _OptionalPolicyItemTypeDef):
     pass
 
+_RequiredCreatePolicyInputRequestTypeDef = TypedDict(
+    "_RequiredCreatePolicyInputRequestTypeDef",
+    {
+        "policyStoreId": str,
+        "definition": PolicyDefinitionTypeDef,
+    },
+)
+_OptionalCreatePolicyInputRequestTypeDef = TypedDict(
+    "_OptionalCreatePolicyInputRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class CreatePolicyInputRequestTypeDef(
+    _RequiredCreatePolicyInputRequestTypeDef, _OptionalCreatePolicyInputRequestTypeDef
+):
+    pass
+
 ListPoliciesOutputTypeDef = TypedDict(
     "ListPoliciesOutputTypeDef",
     {
         "nextToken": str,
         "policies": List[PolicyItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-verifiedpermissions
-Version: 1.28.12
-Summary: Type annotations for boto3.VerifiedPermissions 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.VerifiedPermissions 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-verifiedpermissions.svg?color=blue)](https://pypi.org/project/mypy-boto3-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-verifiedpermissions)](https://pepy.tech/project/mypy-boto3-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VerifiedPermissions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
+[boto3.VerifiedPermissions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
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
 [mypy-boto3-verifiedpermissions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -344,28 +344,26 @@
 ```python
 from mypy_boto3_verifiedpermissions.type_defs import (
     ActionIdentifierTypeDef,
     EntityIdentifierTypeDef,
     CognitoUserPoolConfigurationTypeDef,
     ContextDefinitionTypeDef,
     ResponseMetadataTypeDef,
-    EntityIdentifierOutputTypeDef,
     ValidationSettingsTypeDef,
     CreatePolicyTemplateInputRequestTypeDef,
     DeleteIdentitySourceInputRequestTypeDef,
     DeletePolicyInputRequestTypeDef,
     DeletePolicyStoreInputRequestTypeDef,
     DeletePolicyTemplateInputRequestTypeDef,
     DeterminingPolicyItemTypeDef,
     EvaluationErrorItemTypeDef,
     GetIdentitySourceInputRequestTypeDef,
     IdentitySourceDetailsTypeDef,
     GetPolicyInputRequestTypeDef,
     GetPolicyStoreInputRequestTypeDef,
-    ValidationSettingsOutputTypeDef,
     GetPolicyTemplateInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     IdentitySourceFilterTypeDef,
     IdentitySourceItemDetailsTypeDef,
     PaginatorConfigTypeDef,
     ListPolicyStoresInputRequestTypeDef,
     PolicyStoreItemTypeDef,
@@ -377,61 +375,61 @@
     SchemaDefinitionTypeDef,
     UpdateCognitoUserPoolConfigurationTypeDef,
     UpdateStaticPolicyDefinitionTypeDef,
     UpdatePolicyTemplateInputRequestTypeDef,
     AttributeValueTypeDef,
     EntityItemTypeDef,
     EntityReferenceTypeDef,
+    TemplateLinkedPolicyDefinitionDetailTypeDef,
+    TemplateLinkedPolicyDefinitionItemTypeDef,
     TemplateLinkedPolicyDefinitionTypeDef,
     ConfigurationTypeDef,
     CreateIdentitySourceOutputTypeDef,
+    CreatePolicyOutputTypeDef,
     CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateOutputTypeDef,
     GetPolicyTemplateOutputTypeDef,
     GetSchemaOutputTypeDef,
     PutSchemaOutputTypeDef,
     UpdateIdentitySourceOutputTypeDef,
+    UpdatePolicyOutputTypeDef,
     UpdatePolicyStoreOutputTypeDef,
     UpdatePolicyTemplateOutputTypeDef,
-    CreatePolicyOutputTypeDef,
-    TemplateLinkedPolicyDefinitionDetailTypeDef,
-    TemplateLinkedPolicyDefinitionItemTypeDef,
-    UpdatePolicyOutputTypeDef,
     CreatePolicyStoreInputRequestTypeDef,
+    GetPolicyStoreOutputTypeDef,
     UpdatePolicyStoreInputRequestTypeDef,
     IsAuthorizedOutputTypeDef,
     IsAuthorizedWithTokenOutputTypeDef,
     GetIdentitySourceOutputTypeDef,
-    GetPolicyStoreOutputTypeDef,
     ListIdentitySourcesInputRequestTypeDef,
     IdentitySourceItemTypeDef,
     ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
     ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
     ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyStoresOutputTypeDef,
     ListPolicyTemplatesOutputTypeDef,
     PutSchemaInputRequestTypeDef,
     UpdateConfigurationTypeDef,
     UpdatePolicyDefinitionTypeDef,
     EntitiesDefinitionTypeDef,
     PolicyFilterTypeDef,
-    PolicyDefinitionTypeDef,
-    CreateIdentitySourceInputRequestTypeDef,
     PolicyDefinitionDetailTypeDef,
     PolicyDefinitionItemTypeDef,
+    PolicyDefinitionTypeDef,
+    CreateIdentitySourceInputRequestTypeDef,
     ListIdentitySourcesOutputTypeDef,
     UpdateIdentitySourceInputRequestTypeDef,
     UpdatePolicyInputRequestTypeDef,
     IsAuthorizedInputRequestTypeDef,
     IsAuthorizedWithTokenInputRequestTypeDef,
     ListPoliciesInputListPoliciesPaginateTypeDef,
     ListPoliciesInputRequestTypeDef,
-    CreatePolicyInputRequestTypeDef,
     GetPolicyOutputTypeDef,
     PolicyItemTypeDef,
+    CreatePolicyInputRequestTypeDef,
     ListPoliciesOutputTypeDef,
 )
 
 
 def get_structure() -> ActionIdentifierTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt` & `mypy-boto3-verifiedpermissions-1.28.15/mypy_boto3_verifiedpermissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-verifiedpermissions-1.28.12/setup.py` & `mypy-boto3-verifiedpermissions-1.28.15/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-verifiedpermissions",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_verifiedpermissions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VerifiedPermissions 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.VerifiedPermissions 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

