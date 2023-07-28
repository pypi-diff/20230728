# Comparing `tmp/mypy-boto3-amplify-1.28.12.tar.gz` & `tmp/mypy-boto3-amplify-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplify-1.28.12.tar", last modified: Thu Jul 27 05:34:13 2023, max compression
+gzip compressed data, was "mypy-boto3-amplify-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
```

## Comparing `mypy-boto3-amplify-1.28.12.tar` & `mypy-boto3-amplify-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.844594 mypy-boto3-amplify-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16422 2023-07-27 05:34:13.844594 mypy-boto3-amplify-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.840594 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27948 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27900 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36465 2023-07-27 05:17:01.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36404 2023-07-27 05:17:01.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.844594 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16422 2023-07-27 05:34:13.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 05:34:13.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:13.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:13.000000 mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:13.844594 mypy-boto3-amplify-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:17:00.000000 mypy-boto3-amplify-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.632608 mypy-boto3-amplify-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-07-28 20:42:12.632608 mypy-boto3-amplify-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.616608 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27948 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27900 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9175 2023-07-28 20:18:50.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-07-28 20:18:50.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35813 2023-07-28 20:18:51.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35754 2023-07-28 20:18:50.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.632608 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-07-28 20:42:12.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-28 20:42:12.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:12.000000 mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.632608 mypy-boto3-amplify-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:18:49.000000 mypy-boto3-amplify-1.28.15/setup.py
```

### Comparing `mypy-boto3-amplify-1.28.12/LICENSE` & `mypy-boto3-amplify-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.12/PKG-INFO` & `mypy-boto3-amplify-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplify
-Version: 1.28.12
-Summary: Type annotations for boto3.Amplify 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Amplify 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplify)](https://pepy.tech/project/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,21 +338,20 @@
 
 `mypy_boto3_amplify.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplify.type_defs import (
     AutoBranchCreationConfigOutputTypeDef,
-    CustomRuleOutputTypeDef,
+    CustomRuleTypeDef,
     ProductionBranchTypeDef,
     ArtifactTypeDef,
     AutoBranchCreationConfigTypeDef,
     BackendEnvironmentTypeDef,
     BranchTypeDef,
-    CustomRuleTypeDef,
     ResponseMetadataTypeDef,
     CreateBackendEnvironmentRequestRequestTypeDef,
     CreateBranchRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     SubDomainSettingTypeDef,
     CreateWebhookRequestRequestTypeDef,
     WebhookTypeDef,
@@ -380,15 +379,14 @@
     ListDomainAssociationsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebhooksRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StartJobRequestRequestTypeDef,
     StopJobRequestRequestTypeDef,
-    SubDomainSettingOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBranchRequestRequestTypeDef,
     UpdateWebhookRequestRequestTypeDef,
     AppTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
@@ -403,14 +401,15 @@
     GetBranchResultTypeDef,
     ListArtifactsResultTypeDef,
     ListBackendEnvironmentsResultTypeDef,
     ListBranchesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateBranchResultTypeDef,
     CreateDomainAssociationRequestRequestTypeDef,
+    SubDomainTypeDef,
     UpdateDomainAssociationRequestRequestTypeDef,
     CreateWebhookResultTypeDef,
     DeleteWebhookResultTypeDef,
     GetWebhookResultTypeDef,
     ListWebhooksResultTypeDef,
     UpdateWebhookResultTypeDef,
     DeleteJobResultTypeDef,
@@ -419,22 +418,21 @@
     StartJobResultTypeDef,
     StopJobResultTypeDef,
     JobTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     ListBranchesRequestListBranchesPaginateTypeDef,
     ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
-    SubDomainTypeDef,
     CreateAppResultTypeDef,
     DeleteAppResultTypeDef,
     GetAppResultTypeDef,
     ListAppsResultTypeDef,
     UpdateAppResultTypeDef,
-    GetJobResultTypeDef,
     DomainAssociationTypeDef,
+    GetJobResultTypeDef,
     CreateDomainAssociationResultTypeDef,
     DeleteDomainAssociationResultTypeDef,
     GetDomainAssociationResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
 )
```

### Comparing `mypy-boto3-amplify-1.28.12/README.md` & `mypy-boto3-amplify-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplify)](https://pepy.tech/project/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,21 +306,20 @@
 
 `mypy_boto3_amplify.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplify.type_defs import (
     AutoBranchCreationConfigOutputTypeDef,
-    CustomRuleOutputTypeDef,
+    CustomRuleTypeDef,
     ProductionBranchTypeDef,
     ArtifactTypeDef,
     AutoBranchCreationConfigTypeDef,
     BackendEnvironmentTypeDef,
     BranchTypeDef,
-    CustomRuleTypeDef,
     ResponseMetadataTypeDef,
     CreateBackendEnvironmentRequestRequestTypeDef,
     CreateBranchRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     SubDomainSettingTypeDef,
     CreateWebhookRequestRequestTypeDef,
     WebhookTypeDef,
@@ -348,15 +347,14 @@
     ListDomainAssociationsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebhooksRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StartJobRequestRequestTypeDef,
     StopJobRequestRequestTypeDef,
-    SubDomainSettingOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBranchRequestRequestTypeDef,
     UpdateWebhookRequestRequestTypeDef,
     AppTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
@@ -371,14 +369,15 @@
     GetBranchResultTypeDef,
     ListArtifactsResultTypeDef,
     ListBackendEnvironmentsResultTypeDef,
     ListBranchesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateBranchResultTypeDef,
     CreateDomainAssociationRequestRequestTypeDef,
+    SubDomainTypeDef,
     UpdateDomainAssociationRequestRequestTypeDef,
     CreateWebhookResultTypeDef,
     DeleteWebhookResultTypeDef,
     GetWebhookResultTypeDef,
     ListWebhooksResultTypeDef,
     UpdateWebhookResultTypeDef,
     DeleteJobResultTypeDef,
@@ -387,22 +386,21 @@
     StartJobResultTypeDef,
     StopJobResultTypeDef,
     JobTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     ListBranchesRequestListBranchesPaginateTypeDef,
     ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
-    SubDomainTypeDef,
     CreateAppResultTypeDef,
     DeleteAppResultTypeDef,
     GetAppResultTypeDef,
     ListAppsResultTypeDef,
     UpdateAppResultTypeDef,
-    GetJobResultTypeDef,
     DomainAssociationTypeDef,
+    GetJobResultTypeDef,
     CreateDomainAssociationResultTypeDef,
     DeleteDomainAssociationResultTypeDef,
     GetDomainAssociationResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
 )
```

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/__init__.py` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/__init__.pyi` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/__main__.py` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Amplify 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Amplify 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify\nOther"
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

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/client.py` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/client.pyi` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/literals.py` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/literals.pyi` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/paginator.py` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/paginator.pyi` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/type_defs.py` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,21 +28,20 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AutoBranchCreationConfigOutputTypeDef",
-    "CustomRuleOutputTypeDef",
+    "CustomRuleTypeDef",
     "ProductionBranchTypeDef",
     "ArtifactTypeDef",
     "AutoBranchCreationConfigTypeDef",
     "BackendEnvironmentTypeDef",
     "BranchTypeDef",
-    "CustomRuleTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackendEnvironmentRequestRequestTypeDef",
     "CreateBranchRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "SubDomainSettingTypeDef",
     "CreateWebhookRequestRequestTypeDef",
     "WebhookTypeDef",
@@ -70,15 +69,14 @@
     "ListDomainAssociationsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebhooksRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StartJobRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
-    "SubDomainSettingOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBranchRequestRequestTypeDef",
     "UpdateWebhookRequestRequestTypeDef",
     "AppTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
@@ -93,14 +91,15 @@
     "GetBranchResultTypeDef",
     "ListArtifactsResultTypeDef",
     "ListBackendEnvironmentsResultTypeDef",
     "ListBranchesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateBranchResultTypeDef",
     "CreateDomainAssociationRequestRequestTypeDef",
+    "SubDomainTypeDef",
     "UpdateDomainAssociationRequestRequestTypeDef",
     "CreateWebhookResultTypeDef",
     "DeleteWebhookResultTypeDef",
     "GetWebhookResultTypeDef",
     "ListWebhooksResultTypeDef",
     "UpdateWebhookResultTypeDef",
     "DeleteJobResultTypeDef",
@@ -109,22 +108,21 @@
     "StartJobResultTypeDef",
     "StopJobResultTypeDef",
     "JobTypeDef",
     "ListAppsRequestListAppsPaginateTypeDef",
     "ListBranchesRequestListBranchesPaginateTypeDef",
     "ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
-    "SubDomainTypeDef",
     "CreateAppResultTypeDef",
     "DeleteAppResultTypeDef",
     "GetAppResultTypeDef",
     "ListAppsResultTypeDef",
     "UpdateAppResultTypeDef",
-    "GetJobResultTypeDef",
     "DomainAssociationTypeDef",
+    "GetJobResultTypeDef",
     "CreateDomainAssociationResultTypeDef",
     "DeleteDomainAssociationResultTypeDef",
     "GetDomainAssociationResultTypeDef",
     "ListDomainAssociationsResultTypeDef",
     "UpdateDomainAssociationResultTypeDef",
 )
 
@@ -141,32 +139,32 @@
         "buildSpec": str,
         "enablePullRequestPreview": bool,
         "pullRequestEnvironmentName": str,
     },
     total=False,
 )
 
-_RequiredCustomRuleOutputTypeDef = TypedDict(
-    "_RequiredCustomRuleOutputTypeDef",
+_RequiredCustomRuleTypeDef = TypedDict(
+    "_RequiredCustomRuleTypeDef",
     {
         "source": str,
         "target": str,
     },
 )
-_OptionalCustomRuleOutputTypeDef = TypedDict(
-    "_OptionalCustomRuleOutputTypeDef",
+_OptionalCustomRuleTypeDef = TypedDict(
+    "_OptionalCustomRuleTypeDef",
     {
         "status": str,
         "condition": str,
     },
     total=False,
 )
 
 
-class CustomRuleOutputTypeDef(_RequiredCustomRuleOutputTypeDef, _OptionalCustomRuleOutputTypeDef):
+class CustomRuleTypeDef(_RequiredCustomRuleTypeDef, _OptionalCustomRuleTypeDef):
     pass
 
 
 ProductionBranchTypeDef = TypedDict(
     "ProductionBranchTypeDef",
     {
         "lastDeployTime": datetime,
@@ -267,35 +265,14 @@
 )
 
 
 class BranchTypeDef(_RequiredBranchTypeDef, _OptionalBranchTypeDef):
     pass
 
 
-_RequiredCustomRuleTypeDef = TypedDict(
-    "_RequiredCustomRuleTypeDef",
-    {
-        "source": str,
-        "target": str,
-    },
-)
-_OptionalCustomRuleTypeDef = TypedDict(
-    "_OptionalCustomRuleTypeDef",
-    {
-        "status": str,
-        "condition": str,
-    },
-    total=False,
-)
-
-
-class CustomRuleTypeDef(_RequiredCustomRuleTypeDef, _OptionalCustomRuleTypeDef):
-    pass
-
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -827,22 +804,14 @@
     {
         "appId": str,
         "branchName": str,
         "jobId": str,
     },
 )
 
-SubDomainSettingOutputTypeDef = TypedDict(
-    "SubDomainSettingOutputTypeDef",
-    {
-        "prefix": str,
-        "branchName": str,
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
@@ -933,15 +902,15 @@
 _OptionalAppTypeDef = TypedDict(
     "_OptionalAppTypeDef",
     {
         "tags": Dict[str, str],
         "iamServiceRoleArn": str,
         "enableBranchAutoDeletion": bool,
         "basicAuthCredentials": str,
-        "customRules": List[CustomRuleOutputTypeDef],
+        "customRules": List[CustomRuleTypeDef],
         "productionBranch": ProductionBranchTypeDef,
         "buildSpec": str,
         "customHeaders": str,
         "enableAutoBranchCreation": bool,
         "autoBranchCreationPatterns": List[str],
         "autoBranchCreationConfig": AutoBranchCreationConfigOutputTypeDef,
         "repositoryCloneMethod": RepositoryCloneMethodType,
@@ -1170,14 +1139,23 @@
 class CreateDomainAssociationRequestRequestTypeDef(
     _RequiredCreateDomainAssociationRequestRequestTypeDef,
     _OptionalCreateDomainAssociationRequestRequestTypeDef,
 ):
     pass
 
 
+SubDomainTypeDef = TypedDict(
+    "SubDomainTypeDef",
+    {
+        "subDomainSetting": SubDomainSettingTypeDef,
+        "verified": bool,
+        "dnsRecord": str,
+    },
+)
+
 _RequiredUpdateDomainAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainAssociationRequestRequestTypeDef",
     {
         "appId": str,
         "domainName": str,
     },
 )
@@ -1360,23 +1338,14 @@
 
 class ListJobsRequestListJobsPaginateTypeDef(
     _RequiredListJobsRequestListJobsPaginateTypeDef, _OptionalListJobsRequestListJobsPaginateTypeDef
 ):
     pass
 
 
-SubDomainTypeDef = TypedDict(
-    "SubDomainTypeDef",
-    {
-        "subDomainSetting": SubDomainSettingOutputTypeDef,
-        "verified": bool,
-        "dnsRecord": str,
-    },
-)
-
 CreateAppResultTypeDef = TypedDict(
     "CreateAppResultTypeDef",
     {
         "app": AppTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1410,22 +1379,14 @@
     "UpdateAppResultTypeDef",
     {
         "app": AppTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetJobResultTypeDef = TypedDict(
-    "GetJobResultTypeDef",
-    {
-        "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredDomainAssociationTypeDef = TypedDict(
     "_RequiredDomainAssociationTypeDef",
     {
         "domainAssociationArn": str,
         "domainName": str,
         "enableAutoSubDomain": bool,
         "domainStatus": DomainStatusType,
@@ -1446,14 +1407,22 @@
 
 class DomainAssociationTypeDef(
     _RequiredDomainAssociationTypeDef, _OptionalDomainAssociationTypeDef
 ):
     pass
 
 
+GetJobResultTypeDef = TypedDict(
+    "GetJobResultTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateDomainAssociationResultTypeDef = TypedDict(
     "CreateDomainAssociationResultTypeDef",
     {
         "domainAssociation": DomainAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify/type_defs.pyi` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,20 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AutoBranchCreationConfigOutputTypeDef",
-    "CustomRuleOutputTypeDef",
+    "CustomRuleTypeDef",
     "ProductionBranchTypeDef",
     "ArtifactTypeDef",
     "AutoBranchCreationConfigTypeDef",
     "BackendEnvironmentTypeDef",
     "BranchTypeDef",
-    "CustomRuleTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackendEnvironmentRequestRequestTypeDef",
     "CreateBranchRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "SubDomainSettingTypeDef",
     "CreateWebhookRequestRequestTypeDef",
     "WebhookTypeDef",
@@ -69,15 +68,14 @@
     "ListDomainAssociationsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWebhooksRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StartJobRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
-    "SubDomainSettingOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBranchRequestRequestTypeDef",
     "UpdateWebhookRequestRequestTypeDef",
     "AppTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
@@ -92,14 +90,15 @@
     "GetBranchResultTypeDef",
     "ListArtifactsResultTypeDef",
     "ListBackendEnvironmentsResultTypeDef",
     "ListBranchesResultTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "UpdateBranchResultTypeDef",
     "CreateDomainAssociationRequestRequestTypeDef",
+    "SubDomainTypeDef",
     "UpdateDomainAssociationRequestRequestTypeDef",
     "CreateWebhookResultTypeDef",
     "DeleteWebhookResultTypeDef",
     "GetWebhookResultTypeDef",
     "ListWebhooksResultTypeDef",
     "UpdateWebhookResultTypeDef",
     "DeleteJobResultTypeDef",
@@ -108,22 +107,21 @@
     "StartJobResultTypeDef",
     "StopJobResultTypeDef",
     "JobTypeDef",
     "ListAppsRequestListAppsPaginateTypeDef",
     "ListBranchesRequestListBranchesPaginateTypeDef",
     "ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
-    "SubDomainTypeDef",
     "CreateAppResultTypeDef",
     "DeleteAppResultTypeDef",
     "GetAppResultTypeDef",
     "ListAppsResultTypeDef",
     "UpdateAppResultTypeDef",
-    "GetJobResultTypeDef",
     "DomainAssociationTypeDef",
+    "GetJobResultTypeDef",
     "CreateDomainAssociationResultTypeDef",
     "DeleteDomainAssociationResultTypeDef",
     "GetDomainAssociationResultTypeDef",
     "ListDomainAssociationsResultTypeDef",
     "UpdateDomainAssociationResultTypeDef",
 )
 
@@ -140,31 +138,31 @@
         "buildSpec": str,
         "enablePullRequestPreview": bool,
         "pullRequestEnvironmentName": str,
     },
     total=False,
 )
 
-_RequiredCustomRuleOutputTypeDef = TypedDict(
-    "_RequiredCustomRuleOutputTypeDef",
+_RequiredCustomRuleTypeDef = TypedDict(
+    "_RequiredCustomRuleTypeDef",
     {
         "source": str,
         "target": str,
     },
 )
-_OptionalCustomRuleOutputTypeDef = TypedDict(
-    "_OptionalCustomRuleOutputTypeDef",
+_OptionalCustomRuleTypeDef = TypedDict(
+    "_OptionalCustomRuleTypeDef",
     {
         "status": str,
         "condition": str,
     },
     total=False,
 )
 
-class CustomRuleOutputTypeDef(_RequiredCustomRuleOutputTypeDef, _OptionalCustomRuleOutputTypeDef):
+class CustomRuleTypeDef(_RequiredCustomRuleTypeDef, _OptionalCustomRuleTypeDef):
     pass
 
 ProductionBranchTypeDef = TypedDict(
     "ProductionBranchTypeDef",
     {
         "lastDeployTime": datetime,
         "status": str,
@@ -260,33 +258,14 @@
     },
     total=False,
 )
 
 class BranchTypeDef(_RequiredBranchTypeDef, _OptionalBranchTypeDef):
     pass
 
-_RequiredCustomRuleTypeDef = TypedDict(
-    "_RequiredCustomRuleTypeDef",
-    {
-        "source": str,
-        "target": str,
-    },
-)
-_OptionalCustomRuleTypeDef = TypedDict(
-    "_OptionalCustomRuleTypeDef",
-    {
-        "status": str,
-        "condition": str,
-    },
-    total=False,
-)
-
-class CustomRuleTypeDef(_RequiredCustomRuleTypeDef, _OptionalCustomRuleTypeDef):
-    pass
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -788,22 +767,14 @@
     {
         "appId": str,
         "branchName": str,
         "jobId": str,
     },
 )
 
-SubDomainSettingOutputTypeDef = TypedDict(
-    "SubDomainSettingOutputTypeDef",
-    {
-        "prefix": str,
-        "branchName": str,
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
@@ -890,15 +861,15 @@
 _OptionalAppTypeDef = TypedDict(
     "_OptionalAppTypeDef",
     {
         "tags": Dict[str, str],
         "iamServiceRoleArn": str,
         "enableBranchAutoDeletion": bool,
         "basicAuthCredentials": str,
-        "customRules": List[CustomRuleOutputTypeDef],
+        "customRules": List[CustomRuleTypeDef],
         "productionBranch": ProductionBranchTypeDef,
         "buildSpec": str,
         "customHeaders": str,
         "enableAutoBranchCreation": bool,
         "autoBranchCreationPatterns": List[str],
         "autoBranchCreationConfig": AutoBranchCreationConfigOutputTypeDef,
         "repositoryCloneMethod": RepositoryCloneMethodType,
@@ -1119,14 +1090,23 @@
 
 class CreateDomainAssociationRequestRequestTypeDef(
     _RequiredCreateDomainAssociationRequestRequestTypeDef,
     _OptionalCreateDomainAssociationRequestRequestTypeDef,
 ):
     pass
 
+SubDomainTypeDef = TypedDict(
+    "SubDomainTypeDef",
+    {
+        "subDomainSetting": SubDomainSettingTypeDef,
+        "verified": bool,
+        "dnsRecord": str,
+    },
+)
+
 _RequiredUpdateDomainAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainAssociationRequestRequestTypeDef",
     {
         "appId": str,
         "domainName": str,
     },
 )
@@ -1301,23 +1281,14 @@
 )
 
 class ListJobsRequestListJobsPaginateTypeDef(
     _RequiredListJobsRequestListJobsPaginateTypeDef, _OptionalListJobsRequestListJobsPaginateTypeDef
 ):
     pass
 
-SubDomainTypeDef = TypedDict(
-    "SubDomainTypeDef",
-    {
-        "subDomainSetting": SubDomainSettingOutputTypeDef,
-        "verified": bool,
-        "dnsRecord": str,
-    },
-)
-
 CreateAppResultTypeDef = TypedDict(
     "CreateAppResultTypeDef",
     {
         "app": AppTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1351,22 +1322,14 @@
     "UpdateAppResultTypeDef",
     {
         "app": AppTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetJobResultTypeDef = TypedDict(
-    "GetJobResultTypeDef",
-    {
-        "job": JobTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredDomainAssociationTypeDef = TypedDict(
     "_RequiredDomainAssociationTypeDef",
     {
         "domainAssociationArn": str,
         "domainName": str,
         "enableAutoSubDomain": bool,
         "domainStatus": DomainStatusType,
@@ -1385,14 +1348,22 @@
 )
 
 class DomainAssociationTypeDef(
     _RequiredDomainAssociationTypeDef, _OptionalDomainAssociationTypeDef
 ):
     pass
 
+GetJobResultTypeDef = TypedDict(
+    "GetJobResultTypeDef",
+    {
+        "job": JobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateDomainAssociationResultTypeDef = TypedDict(
     "CreateDomainAssociationResultTypeDef",
     {
         "domainAssociation": DomainAssociationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/PKG-INFO` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplify
-Version: 1.28.12
-Summary: Type annotations for boto3.Amplify 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Amplify 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplify.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplify)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplify)](https://pepy.tech/project/mypy-boto3-amplify)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Amplify 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
+[boto3.Amplify 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
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
 [mypy-boto3-amplify docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplify/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,21 +338,20 @@
 
 `mypy_boto3_amplify.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplify.type_defs import (
     AutoBranchCreationConfigOutputTypeDef,
-    CustomRuleOutputTypeDef,
+    CustomRuleTypeDef,
     ProductionBranchTypeDef,
     ArtifactTypeDef,
     AutoBranchCreationConfigTypeDef,
     BackendEnvironmentTypeDef,
     BranchTypeDef,
-    CustomRuleTypeDef,
     ResponseMetadataTypeDef,
     CreateBackendEnvironmentRequestRequestTypeDef,
     CreateBranchRequestRequestTypeDef,
     CreateDeploymentRequestRequestTypeDef,
     SubDomainSettingTypeDef,
     CreateWebhookRequestRequestTypeDef,
     WebhookTypeDef,
@@ -380,15 +379,14 @@
     ListDomainAssociationsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListWebhooksRequestRequestTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StartJobRequestRequestTypeDef,
     StopJobRequestRequestTypeDef,
-    SubDomainSettingOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBranchRequestRequestTypeDef,
     UpdateWebhookRequestRequestTypeDef,
     AppTypeDef,
     CreateAppRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
@@ -403,14 +401,15 @@
     GetBranchResultTypeDef,
     ListArtifactsResultTypeDef,
     ListBackendEnvironmentsResultTypeDef,
     ListBranchesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     UpdateBranchResultTypeDef,
     CreateDomainAssociationRequestRequestTypeDef,
+    SubDomainTypeDef,
     UpdateDomainAssociationRequestRequestTypeDef,
     CreateWebhookResultTypeDef,
     DeleteWebhookResultTypeDef,
     GetWebhookResultTypeDef,
     ListWebhooksResultTypeDef,
     UpdateWebhookResultTypeDef,
     DeleteJobResultTypeDef,
@@ -419,22 +418,21 @@
     StartJobResultTypeDef,
     StopJobResultTypeDef,
     JobTypeDef,
     ListAppsRequestListAppsPaginateTypeDef,
     ListBranchesRequestListBranchesPaginateTypeDef,
     ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
-    SubDomainTypeDef,
     CreateAppResultTypeDef,
     DeleteAppResultTypeDef,
     GetAppResultTypeDef,
     ListAppsResultTypeDef,
     UpdateAppResultTypeDef,
-    GetJobResultTypeDef,
     DomainAssociationTypeDef,
+    GetJobResultTypeDef,
     CreateDomainAssociationResultTypeDef,
     DeleteDomainAssociationResultTypeDef,
     GetDomainAssociationResultTypeDef,
     ListDomainAssociationsResultTypeDef,
     UpdateDomainAssociationResultTypeDef,
 )
```

### Comparing `mypy-boto3-amplify-1.28.12/mypy_boto3_amplify.egg-info/SOURCES.txt` & `mypy-boto3-amplify-1.28.15/mypy_boto3_amplify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplify-1.28.12/setup.py` & `mypy-boto3-amplify-1.28.15/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplify",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_amplify"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Amplify 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Amplify 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

