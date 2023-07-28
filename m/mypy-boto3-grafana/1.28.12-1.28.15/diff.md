# Comparing `tmp/mypy-boto3-grafana-1.28.12.tar.gz` & `tmp/mypy-boto3-grafana-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-grafana-1.28.12.tar", last modified: Thu Jul 27 05:34:44 2023, max compression
+gzip compressed data, was "mypy-boto3-grafana-1.28.15.tar", last modified: Fri Jul 28 20:42:53 2023, max compression
```

## Comparing `mypy-boto3-grafana-1.28.12.tar` & `mypy-boto3-grafana-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.632500 mypy-boto3-grafana-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-07-27 05:34:44.632500 mypy-boto3-grafana-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.632500 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-07-27 05:23:03.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-07-27 05:23:03.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-27 05:23:03.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-27 05:23:03.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22786 2023-07-27 05:23:03.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22759 2023-07-27 05:23:03.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.632500 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-07-27 05:34:44.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 05:34:44.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:44.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:44.000000 mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:44.632500 mypy-boto3-grafana-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:23:02.000000 mypy-boto3-grafana-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.089169 mypy-boto3-grafana-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-07-28 20:42:53.089169 mypy-boto3-grafana-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.085169 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22103 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22076 2023-07-28 20:26:58.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.089169 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-07-28 20:42:52.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-28 20:42:52.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:52.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:52.000000 mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:53.089169 mypy-boto3-grafana-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:26:57.000000 mypy-boto3-grafana-1.28.15/setup.py
```

### Comparing `mypy-boto3-grafana-1.28.12/LICENSE` & `mypy-boto3-grafana-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.12/PKG-INFO` & `mypy-boto3-grafana-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-grafana
-Version: 1.28.12
-Summary: Type annotations for boto3.ManagedGrafana 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ManagedGrafana 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-grafana)](https://pepy.tech/project/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,82 +337,79 @@
 ### Typed dictionaries
 
 `mypy_boto3_grafana.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_grafana.type_defs import (
-    AssertionAttributesOutputTypeDef,
     AssertionAttributesTypeDef,
     AssociateLicenseRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AwsSsoAuthenticationTypeDef,
     AuthenticationSummaryTypeDef,
     CreateWorkspaceApiKeyRequestRequestTypeDef,
-    CreateWorkspaceApiKeyResponseTypeDef,
     NetworkAccessConfigurationTypeDef,
     VpcConfigurationTypeDef,
     DeleteWorkspaceApiKeyRequestRequestTypeDef,
-    DeleteWorkspaceApiKeyResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
     DescribeWorkspaceAuthenticationRequestRequestTypeDef,
     DescribeWorkspaceConfigurationRequestRequestTypeDef,
-    DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceRequestRequestTypeDef,
     DisassociateLicenseRequestRequestTypeDef,
-    IdpMetadataOutputTypeDef,
     IdpMetadataTypeDef,
-    ListPermissionsRequestListPermissionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPermissionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVersionsRequestListVersionsPaginateTypeDef,
     ListVersionsRequestRequestTypeDef,
-    ListVersionsResponseTypeDef,
-    ListWorkspacesRequestListWorkspacesPaginateTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     NetworkAccessConfigurationOutputTypeDef,
-    PaginatorConfigTypeDef,
-    UserOutputTypeDef,
-    ResponseMetadataTypeDef,
+    UserTypeDef,
     RoleValuesOutputTypeDef,
     RoleValuesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UserTypeDef,
     UpdateWorkspaceConfigurationRequestRequestTypeDef,
     VpcConfigurationOutputTypeDef,
+    CreateWorkspaceApiKeyResponseTypeDef,
+    DeleteWorkspaceApiKeyResponseTypeDef,
+    DescribeWorkspaceConfigurationResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVersionsResponseTypeDef,
     WorkspaceSummaryTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
+    ListPermissionsRequestListPermissionsPaginateTypeDef,
+    ListVersionsRequestListVersionsPaginateTypeDef,
+    ListWorkspacesRequestListWorkspacesPaginateTypeDef,
     PermissionEntryTypeDef,
     UpdateInstructionOutputTypeDef,
+    UpdateInstructionTypeDef,
     SamlConfigurationOutputTypeDef,
     SamlConfigurationTypeDef,
-    UpdateInstructionTypeDef,
     WorkspaceDescriptionTypeDef,
     ListWorkspacesResponseTypeDef,
     ListPermissionsResponseTypeDef,
     UpdateErrorTypeDef,
+    UpdatePermissionsRequestRequestTypeDef,
     SamlAuthenticationTypeDef,
     UpdateWorkspaceAuthenticationRequestRequestTypeDef,
-    UpdatePermissionsRequestRequestTypeDef,
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
     UpdatePermissionsResponseTypeDef,
     AuthenticationDescriptionTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
 )
 
 
-def get_structure() -> AssertionAttributesOutputTypeDef:
+def get_structure() -> AssertionAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-grafana-1.28.12/README.md` & `mypy-boto3-grafana-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-grafana)](https://pepy.tech/project/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,82 +305,79 @@
 ### Typed dictionaries
 
 `mypy_boto3_grafana.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_grafana.type_defs import (
-    AssertionAttributesOutputTypeDef,
     AssertionAttributesTypeDef,
     AssociateLicenseRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AwsSsoAuthenticationTypeDef,
     AuthenticationSummaryTypeDef,
     CreateWorkspaceApiKeyRequestRequestTypeDef,
-    CreateWorkspaceApiKeyResponseTypeDef,
     NetworkAccessConfigurationTypeDef,
     VpcConfigurationTypeDef,
     DeleteWorkspaceApiKeyRequestRequestTypeDef,
-    DeleteWorkspaceApiKeyResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
     DescribeWorkspaceAuthenticationRequestRequestTypeDef,
     DescribeWorkspaceConfigurationRequestRequestTypeDef,
-    DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceRequestRequestTypeDef,
     DisassociateLicenseRequestRequestTypeDef,
-    IdpMetadataOutputTypeDef,
     IdpMetadataTypeDef,
-    ListPermissionsRequestListPermissionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPermissionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVersionsRequestListVersionsPaginateTypeDef,
     ListVersionsRequestRequestTypeDef,
-    ListVersionsResponseTypeDef,
-    ListWorkspacesRequestListWorkspacesPaginateTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     NetworkAccessConfigurationOutputTypeDef,
-    PaginatorConfigTypeDef,
-    UserOutputTypeDef,
-    ResponseMetadataTypeDef,
+    UserTypeDef,
     RoleValuesOutputTypeDef,
     RoleValuesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UserTypeDef,
     UpdateWorkspaceConfigurationRequestRequestTypeDef,
     VpcConfigurationOutputTypeDef,
+    CreateWorkspaceApiKeyResponseTypeDef,
+    DeleteWorkspaceApiKeyResponseTypeDef,
+    DescribeWorkspaceConfigurationResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVersionsResponseTypeDef,
     WorkspaceSummaryTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
+    ListPermissionsRequestListPermissionsPaginateTypeDef,
+    ListVersionsRequestListVersionsPaginateTypeDef,
+    ListWorkspacesRequestListWorkspacesPaginateTypeDef,
     PermissionEntryTypeDef,
     UpdateInstructionOutputTypeDef,
+    UpdateInstructionTypeDef,
     SamlConfigurationOutputTypeDef,
     SamlConfigurationTypeDef,
-    UpdateInstructionTypeDef,
     WorkspaceDescriptionTypeDef,
     ListWorkspacesResponseTypeDef,
     ListPermissionsResponseTypeDef,
     UpdateErrorTypeDef,
+    UpdatePermissionsRequestRequestTypeDef,
     SamlAuthenticationTypeDef,
     UpdateWorkspaceAuthenticationRequestRequestTypeDef,
-    UpdatePermissionsRequestRequestTypeDef,
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
     UpdatePermissionsResponseTypeDef,
     AuthenticationDescriptionTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
 )
 
 
-def get_structure() -> AssertionAttributesOutputTypeDef:
+def get_structure() -> AssertionAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/__init__.py` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/__init__.pyi` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/__main__.py` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ManagedGrafana 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ManagedGrafana 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana\nOther"
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

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/client.py` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/client.pyi` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/literals.py` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/literals.pyi` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/paginator.py` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,43 +57,43 @@
     def paginate(
         self,
         *,
         workspaceId: str,
         groupId: str = ...,
         userId: str = ...,
         userType: UserTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listpermissionspaginator)
         """
 
 
 class ListVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listversionspaginator)
     """
 
     def paginate(
-        self, *, workspaceId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workspaceId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listversionspaginator)
         """
 
 
 class ListWorkspacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listworkspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkspacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listworkspacespaginator)
         """
```

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/paginator.pyi` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -54,41 +54,41 @@
     def paginate(
         self,
         *,
         workspaceId: str,
         groupId: str = ...,
         userId: str = ...,
         userType: UserTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listpermissionspaginator)
         """
 
 class ListVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listversionspaginator)
     """
 
     def paginate(
-        self, *, workspaceId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workspaceId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listversionspaginator)
         """
 
 class ListWorkspacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listworkspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkspacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana.Paginator.ListWorkspaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/paginators/#listworkspacespaginator)
         """
```

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/type_defs.py` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for grafana service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_grafana.type_defs import AssertionAttributesOutputTypeDef
+    from mypy_boto3_grafana.type_defs import AssertionAttributesTypeDef
 
-    data: AssertionAttributesOutputTypeDef = {...}
+    data: AssertionAttributesTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -35,93 +35,77 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AssertionAttributesOutputTypeDef",
     "AssertionAttributesTypeDef",
     "AssociateLicenseRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AwsSsoAuthenticationTypeDef",
     "AuthenticationSummaryTypeDef",
     "CreateWorkspaceApiKeyRequestRequestTypeDef",
-    "CreateWorkspaceApiKeyResponseTypeDef",
     "NetworkAccessConfigurationTypeDef",
     "VpcConfigurationTypeDef",
     "DeleteWorkspaceApiKeyRequestRequestTypeDef",
-    "DeleteWorkspaceApiKeyResponseTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
     "DescribeWorkspaceAuthenticationRequestRequestTypeDef",
     "DescribeWorkspaceConfigurationRequestRequestTypeDef",
-    "DescribeWorkspaceConfigurationResponseTypeDef",
     "DescribeWorkspaceRequestRequestTypeDef",
     "DisassociateLicenseRequestRequestTypeDef",
-    "IdpMetadataOutputTypeDef",
     "IdpMetadataTypeDef",
-    "ListPermissionsRequestListPermissionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListVersionsRequestListVersionsPaginateTypeDef",
     "ListVersionsRequestRequestTypeDef",
-    "ListVersionsResponseTypeDef",
-    "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "NetworkAccessConfigurationOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "UserOutputTypeDef",
-    "ResponseMetadataTypeDef",
+    "UserTypeDef",
     "RoleValuesOutputTypeDef",
     "RoleValuesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UserTypeDef",
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
     "VpcConfigurationOutputTypeDef",
+    "CreateWorkspaceApiKeyResponseTypeDef",
+    "DeleteWorkspaceApiKeyResponseTypeDef",
+    "DescribeWorkspaceConfigurationResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListVersionsResponseTypeDef",
     "WorkspaceSummaryTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
+    "ListPermissionsRequestListPermissionsPaginateTypeDef",
+    "ListVersionsRequestListVersionsPaginateTypeDef",
+    "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     "PermissionEntryTypeDef",
     "UpdateInstructionOutputTypeDef",
+    "UpdateInstructionTypeDef",
     "SamlConfigurationOutputTypeDef",
     "SamlConfigurationTypeDef",
-    "UpdateInstructionTypeDef",
     "WorkspaceDescriptionTypeDef",
     "ListWorkspacesResponseTypeDef",
     "ListPermissionsResponseTypeDef",
     "UpdateErrorTypeDef",
+    "UpdatePermissionsRequestRequestTypeDef",
     "SamlAuthenticationTypeDef",
     "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
-    "UpdatePermissionsRequestRequestTypeDef",
     "AssociateLicenseResponseTypeDef",
     "CreateWorkspaceResponseTypeDef",
     "DeleteWorkspaceResponseTypeDef",
     "DescribeWorkspaceResponseTypeDef",
     "DisassociateLicenseResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "UpdatePermissionsResponseTypeDef",
     "AuthenticationDescriptionTypeDef",
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     "UpdateWorkspaceAuthenticationResponseTypeDef",
 )
 
-AssertionAttributesOutputTypeDef = TypedDict(
-    "AssertionAttributesOutputTypeDef",
-    {
-        "email": str,
-        "groups": str,
-        "login": str,
-        "name": str,
-        "org": str,
-        "role": str,
-    },
-    total=False,
-)
-
 AssertionAttributesTypeDef = TypedDict(
     "AssertionAttributesTypeDef",
     {
         "email": str,
         "groups": str,
         "login": str,
         "name": str,
@@ -135,14 +119,25 @@
     "AssociateLicenseRequestRequestTypeDef",
     {
         "licenseType": LicenseTypeType,
         "workspaceId": str,
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
 AwsSsoAuthenticationTypeDef = TypedDict(
     "AwsSsoAuthenticationTypeDef",
     {
         "ssoClientId": str,
     },
     total=False,
 )
@@ -174,24 +169,14 @@
         "keyName": str,
         "keyRole": str,
         "secondsToLive": int,
         "workspaceId": str,
     },
 )
 
-CreateWorkspaceApiKeyResponseTypeDef = TypedDict(
-    "CreateWorkspaceApiKeyResponseTypeDef",
-    {
-        "key": str,
-        "keyName": str,
-        "workspaceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NetworkAccessConfigurationTypeDef = TypedDict(
     "NetworkAccessConfigurationTypeDef",
     {
         "prefixListIds": Sequence[str],
         "vpceIds": Sequence[str],
     },
 )
@@ -208,23 +193,14 @@
     "DeleteWorkspaceApiKeyRequestRequestTypeDef",
     {
         "keyName": str,
         "workspaceId": str,
     },
 )
 
-DeleteWorkspaceApiKeyResponseTypeDef = TypedDict(
-    "DeleteWorkspaceApiKeyResponseTypeDef",
-    {
-        "keyName": str,
-        "workspaceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkspaceRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
@@ -238,23 +214,14 @@
 DescribeWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceConfigurationRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
-DescribeWorkspaceConfigurationResponseTypeDef = TypedDict(
-    "DescribeWorkspaceConfigurationResponseTypeDef",
-    {
-        "configuration": str,
-        "grafanaVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeWorkspaceRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
@@ -262,57 +229,33 @@
     "DisassociateLicenseRequestRequestTypeDef",
     {
         "licenseType": LicenseTypeType,
         "workspaceId": str,
     },
 )
 
-IdpMetadataOutputTypeDef = TypedDict(
-    "IdpMetadataOutputTypeDef",
-    {
-        "url": str,
-        "xml": str,
-    },
-    total=False,
-)
-
 IdpMetadataTypeDef = TypedDict(
     "IdpMetadataTypeDef",
     {
         "url": str,
         "xml": str,
     },
     total=False,
 )
 
-_RequiredListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
-    "_RequiredListPermissionsRequestListPermissionsPaginateTypeDef",
-    {
-        "workspaceId": str,
-    },
-)
-_OptionalListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
-    "_OptionalListPermissionsRequestListPermissionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "groupId": str,
-        "userId": str,
-        "userType": UserTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListPermissionsRequestListPermissionsPaginateTypeDef(
-    _RequiredListPermissionsRequestListPermissionsPaginateTypeDef,
-    _OptionalListPermissionsRequestListPermissionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionsRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalListPermissionsRequestRequestTypeDef = TypedDict(
@@ -337,58 +280,24 @@
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
-ListVersionsRequestListVersionsPaginateTypeDef = TypedDict(
-    "ListVersionsRequestListVersionsPaginateTypeDef",
-    {
-        "workspaceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVersionsRequestRequestTypeDef = TypedDict(
     "ListVersionsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "workspaceId": str,
     },
     total=False,
 )
 
-ListVersionsResponseTypeDef = TypedDict(
-    "ListVersionsResponseTypeDef",
-    {
-        "grafanaVersions": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListWorkspacesRequestListWorkspacesPaginateTypeDef = TypedDict(
-    "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -398,43 +307,22 @@
     "NetworkAccessConfigurationOutputTypeDef",
     {
         "prefixListIds": List[str],
         "vpceIds": List[str],
     },
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
-UserOutputTypeDef = TypedDict(
-    "UserOutputTypeDef",
+UserTypeDef = TypedDict(
+    "UserTypeDef",
     {
         "id": str,
         "type": UserTypeType,
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
 RoleValuesOutputTypeDef = TypedDict(
     "RoleValuesOutputTypeDef",
     {
         "admin": List[str],
         "editor": List[str],
     },
     total=False,
@@ -461,22 +349,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UserTypeDef = TypedDict(
-    "UserTypeDef",
-    {
-        "id": str,
-        "type": UserTypeType,
-    },
-)
-
 _RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef",
     {
         "configuration": str,
         "workspaceId": str,
     },
 )
@@ -500,14 +380,59 @@
     "VpcConfigurationOutputTypeDef",
     {
         "securityGroupIds": List[str],
         "subnetIds": List[str],
     },
 )
 
+CreateWorkspaceApiKeyResponseTypeDef = TypedDict(
+    "CreateWorkspaceApiKeyResponseTypeDef",
+    {
+        "key": str,
+        "keyName": str,
+        "workspaceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteWorkspaceApiKeyResponseTypeDef = TypedDict(
+    "DeleteWorkspaceApiKeyResponseTypeDef",
+    {
+        "keyName": str,
+        "workspaceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorkspaceConfigurationResponseTypeDef = TypedDict(
+    "DescribeWorkspaceConfigurationResponseTypeDef",
+    {
+        "configuration": str,
+        "grafanaVersion": str,
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
+ListVersionsResponseTypeDef = TypedDict(
+    "ListVersionsResponseTypeDef",
+    {
+        "grafanaVersions": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredWorkspaceSummaryTypeDef = TypedDict(
     "_RequiredWorkspaceSummaryTypeDef",
     {
         "authentication": AuthenticationSummaryTypeDef,
         "created": datetime,
         "endpoint": str,
         "grafanaVersion": str,
@@ -598,42 +523,93 @@
 
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
+    "_RequiredListPermissionsRequestListPermissionsPaginateTypeDef",
+    {
+        "workspaceId": str,
+    },
+)
+_OptionalListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
+    "_OptionalListPermissionsRequestListPermissionsPaginateTypeDef",
+    {
+        "groupId": str,
+        "userId": str,
+        "userType": UserTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPermissionsRequestListPermissionsPaginateTypeDef(
+    _RequiredListPermissionsRequestListPermissionsPaginateTypeDef,
+    _OptionalListPermissionsRequestListPermissionsPaginateTypeDef,
+):
+    pass
+
+
+ListVersionsRequestListVersionsPaginateTypeDef = TypedDict(
+    "ListVersionsRequestListVersionsPaginateTypeDef",
+    {
+        "workspaceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkspacesRequestListWorkspacesPaginateTypeDef = TypedDict(
+    "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 PermissionEntryTypeDef = TypedDict(
     "PermissionEntryTypeDef",
     {
         "role": RoleType,
-        "user": UserOutputTypeDef,
+        "user": UserTypeDef,
     },
 )
 
 UpdateInstructionOutputTypeDef = TypedDict(
     "UpdateInstructionOutputTypeDef",
     {
         "action": UpdateActionType,
         "role": RoleType,
-        "users": List[UserOutputTypeDef],
+        "users": List[UserTypeDef],
+    },
+)
+
+UpdateInstructionTypeDef = TypedDict(
+    "UpdateInstructionTypeDef",
+    {
+        "action": UpdateActionType,
+        "role": RoleType,
+        "users": Sequence[UserTypeDef],
     },
 )
 
 _RequiredSamlConfigurationOutputTypeDef = TypedDict(
     "_RequiredSamlConfigurationOutputTypeDef",
     {
-        "idpMetadata": IdpMetadataOutputTypeDef,
+        "idpMetadata": IdpMetadataTypeDef,
     },
 )
 _OptionalSamlConfigurationOutputTypeDef = TypedDict(
     "_OptionalSamlConfigurationOutputTypeDef",
     {
         "allowedOrganizations": List[str],
-        "assertionAttributes": AssertionAttributesOutputTypeDef,
+        "assertionAttributes": AssertionAttributesTypeDef,
         "loginValidityDuration": int,
         "roleValues": RoleValuesOutputTypeDef,
     },
     total=False,
 )
 
 
@@ -663,23 +639,14 @@
 
 class SamlConfigurationTypeDef(
     _RequiredSamlConfigurationTypeDef, _OptionalSamlConfigurationTypeDef
 ):
     pass
 
 
-UpdateInstructionTypeDef = TypedDict(
-    "UpdateInstructionTypeDef",
-    {
-        "action": UpdateActionType,
-        "role": RoleType,
-        "users": Sequence[UserTypeDef],
-    },
-)
-
 _RequiredWorkspaceDescriptionTypeDef = TypedDict(
     "_RequiredWorkspaceDescriptionTypeDef",
     {
         "authentication": AuthenticationSummaryTypeDef,
         "created": datetime,
         "dataSources": List[DataSourceTypeType],
         "endpoint": str,
@@ -720,36 +687,44 @@
 
 
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
         "nextToken": str,
         "workspaces": List[WorkspaceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "nextToken": str,
         "permissions": List[PermissionEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateErrorTypeDef = TypedDict(
     "UpdateErrorTypeDef",
     {
         "causedBy": UpdateInstructionOutputTypeDef,
         "code": int,
         "message": str,
     },
 )
 
+UpdatePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdatePermissionsRequestRequestTypeDef",
+    {
+        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
+        "workspaceId": str,
+    },
+)
+
 _RequiredSamlAuthenticationTypeDef = TypedDict(
     "_RequiredSamlAuthenticationTypeDef",
     {
         "status": SamlConfigurationStatusType,
     },
 )
 _OptionalSamlAuthenticationTypeDef = TypedDict(
@@ -786,75 +761,67 @@
 class UpdateWorkspaceAuthenticationRequestRequestTypeDef(
     _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef,
     _OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef,
 ):
     pass
 
 
-UpdatePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdatePermissionsRequestRequestTypeDef",
-    {
-        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
-        "workspaceId": str,
-    },
-)
-
 AssociateLicenseResponseTypeDef = TypedDict(
     "AssociateLicenseResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkspaceResponseTypeDef = TypedDict(
     "CreateWorkspaceResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteWorkspaceResponseTypeDef = TypedDict(
     "DeleteWorkspaceResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspaceResponseTypeDef = TypedDict(
     "DescribeWorkspaceResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateLicenseResponseTypeDef = TypedDict(
     "DisassociateLicenseResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkspaceResponseTypeDef = TypedDict(
     "UpdateWorkspaceResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePermissionsResponseTypeDef = TypedDict(
     "UpdatePermissionsResponseTypeDef",
     {
         "errors": List[UpdateErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAuthenticationDescriptionTypeDef = TypedDict(
     "_RequiredAuthenticationDescriptionTypeDef",
     {
         "providers": List[AuthenticationProviderTypesType],
@@ -876,18 +843,18 @@
     pass
 
 
 DescribeWorkspaceAuthenticationResponseTypeDef = TypedDict(
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     {
         "authentication": AuthenticationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkspaceAuthenticationResponseTypeDef = TypedDict(
     "UpdateWorkspaceAuthenticationResponseTypeDef",
     {
         "authentication": AuthenticationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana/type_defs.pyi` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for grafana service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_grafana.type_defs import AssertionAttributesOutputTypeDef
+    from mypy_boto3_grafana.type_defs import AssertionAttributesTypeDef
 
-    data: AssertionAttributesOutputTypeDef = {...}
+    data: AssertionAttributesTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -34,93 +34,77 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AssertionAttributesOutputTypeDef",
     "AssertionAttributesTypeDef",
     "AssociateLicenseRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AwsSsoAuthenticationTypeDef",
     "AuthenticationSummaryTypeDef",
     "CreateWorkspaceApiKeyRequestRequestTypeDef",
-    "CreateWorkspaceApiKeyResponseTypeDef",
     "NetworkAccessConfigurationTypeDef",
     "VpcConfigurationTypeDef",
     "DeleteWorkspaceApiKeyRequestRequestTypeDef",
-    "DeleteWorkspaceApiKeyResponseTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
     "DescribeWorkspaceAuthenticationRequestRequestTypeDef",
     "DescribeWorkspaceConfigurationRequestRequestTypeDef",
-    "DescribeWorkspaceConfigurationResponseTypeDef",
     "DescribeWorkspaceRequestRequestTypeDef",
     "DisassociateLicenseRequestRequestTypeDef",
-    "IdpMetadataOutputTypeDef",
     "IdpMetadataTypeDef",
-    "ListPermissionsRequestListPermissionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListVersionsRequestListVersionsPaginateTypeDef",
     "ListVersionsRequestRequestTypeDef",
-    "ListVersionsResponseTypeDef",
-    "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "NetworkAccessConfigurationOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "UserOutputTypeDef",
-    "ResponseMetadataTypeDef",
+    "UserTypeDef",
     "RoleValuesOutputTypeDef",
     "RoleValuesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UserTypeDef",
     "UpdateWorkspaceConfigurationRequestRequestTypeDef",
     "VpcConfigurationOutputTypeDef",
+    "CreateWorkspaceApiKeyResponseTypeDef",
+    "DeleteWorkspaceApiKeyResponseTypeDef",
+    "DescribeWorkspaceConfigurationResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListVersionsResponseTypeDef",
     "WorkspaceSummaryTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
+    "ListPermissionsRequestListPermissionsPaginateTypeDef",
+    "ListVersionsRequestListVersionsPaginateTypeDef",
+    "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
     "PermissionEntryTypeDef",
     "UpdateInstructionOutputTypeDef",
+    "UpdateInstructionTypeDef",
     "SamlConfigurationOutputTypeDef",
     "SamlConfigurationTypeDef",
-    "UpdateInstructionTypeDef",
     "WorkspaceDescriptionTypeDef",
     "ListWorkspacesResponseTypeDef",
     "ListPermissionsResponseTypeDef",
     "UpdateErrorTypeDef",
+    "UpdatePermissionsRequestRequestTypeDef",
     "SamlAuthenticationTypeDef",
     "UpdateWorkspaceAuthenticationRequestRequestTypeDef",
-    "UpdatePermissionsRequestRequestTypeDef",
     "AssociateLicenseResponseTypeDef",
     "CreateWorkspaceResponseTypeDef",
     "DeleteWorkspaceResponseTypeDef",
     "DescribeWorkspaceResponseTypeDef",
     "DisassociateLicenseResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "UpdatePermissionsResponseTypeDef",
     "AuthenticationDescriptionTypeDef",
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     "UpdateWorkspaceAuthenticationResponseTypeDef",
 )
 
-AssertionAttributesOutputTypeDef = TypedDict(
-    "AssertionAttributesOutputTypeDef",
-    {
-        "email": str,
-        "groups": str,
-        "login": str,
-        "name": str,
-        "org": str,
-        "role": str,
-    },
-    total=False,
-)
-
 AssertionAttributesTypeDef = TypedDict(
     "AssertionAttributesTypeDef",
     {
         "email": str,
         "groups": str,
         "login": str,
         "name": str,
@@ -134,14 +118,25 @@
     "AssociateLicenseRequestRequestTypeDef",
     {
         "licenseType": LicenseTypeType,
         "workspaceId": str,
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
 AwsSsoAuthenticationTypeDef = TypedDict(
     "AwsSsoAuthenticationTypeDef",
     {
         "ssoClientId": str,
     },
     total=False,
 )
@@ -171,24 +166,14 @@
         "keyName": str,
         "keyRole": str,
         "secondsToLive": int,
         "workspaceId": str,
     },
 )
 
-CreateWorkspaceApiKeyResponseTypeDef = TypedDict(
-    "CreateWorkspaceApiKeyResponseTypeDef",
-    {
-        "key": str,
-        "keyName": str,
-        "workspaceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NetworkAccessConfigurationTypeDef = TypedDict(
     "NetworkAccessConfigurationTypeDef",
     {
         "prefixListIds": Sequence[str],
         "vpceIds": Sequence[str],
     },
 )
@@ -205,23 +190,14 @@
     "DeleteWorkspaceApiKeyRequestRequestTypeDef",
     {
         "keyName": str,
         "workspaceId": str,
     },
 )
 
-DeleteWorkspaceApiKeyResponseTypeDef = TypedDict(
-    "DeleteWorkspaceApiKeyResponseTypeDef",
-    {
-        "keyName": str,
-        "workspaceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkspaceRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
@@ -235,23 +211,14 @@
 DescribeWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceConfigurationRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
-DescribeWorkspaceConfigurationResponseTypeDef = TypedDict(
-    "DescribeWorkspaceConfigurationResponseTypeDef",
-    {
-        "configuration": str,
-        "grafanaVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeWorkspaceRequestRequestTypeDef = TypedDict(
     "DescribeWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
@@ -259,55 +226,33 @@
     "DisassociateLicenseRequestRequestTypeDef",
     {
         "licenseType": LicenseTypeType,
         "workspaceId": str,
     },
 )
 
-IdpMetadataOutputTypeDef = TypedDict(
-    "IdpMetadataOutputTypeDef",
-    {
-        "url": str,
-        "xml": str,
-    },
-    total=False,
-)
-
 IdpMetadataTypeDef = TypedDict(
     "IdpMetadataTypeDef",
     {
         "url": str,
         "xml": str,
     },
     total=False,
 )
 
-_RequiredListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
-    "_RequiredListPermissionsRequestListPermissionsPaginateTypeDef",
-    {
-        "workspaceId": str,
-    },
-)
-_OptionalListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
-    "_OptionalListPermissionsRequestListPermissionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "groupId": str,
-        "userId": str,
-        "userType": UserTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListPermissionsRequestListPermissionsPaginateTypeDef(
-    _RequiredListPermissionsRequestListPermissionsPaginateTypeDef,
-    _OptionalListPermissionsRequestListPermissionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionsRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalListPermissionsRequestRequestTypeDef = TypedDict(
@@ -330,58 +275,24 @@
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
-ListVersionsRequestListVersionsPaginateTypeDef = TypedDict(
-    "ListVersionsRequestListVersionsPaginateTypeDef",
-    {
-        "workspaceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVersionsRequestRequestTypeDef = TypedDict(
     "ListVersionsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "workspaceId": str,
     },
     total=False,
 )
 
-ListVersionsResponseTypeDef = TypedDict(
-    "ListVersionsResponseTypeDef",
-    {
-        "grafanaVersions": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListWorkspacesRequestListWorkspacesPaginateTypeDef = TypedDict(
-    "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -391,43 +302,22 @@
     "NetworkAccessConfigurationOutputTypeDef",
     {
         "prefixListIds": List[str],
         "vpceIds": List[str],
     },
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
-UserOutputTypeDef = TypedDict(
-    "UserOutputTypeDef",
+UserTypeDef = TypedDict(
+    "UserTypeDef",
     {
         "id": str,
         "type": UserTypeType,
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
 RoleValuesOutputTypeDef = TypedDict(
     "RoleValuesOutputTypeDef",
     {
         "admin": List[str],
         "editor": List[str],
     },
     total=False,
@@ -454,22 +344,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UserTypeDef = TypedDict(
-    "UserTypeDef",
-    {
-        "id": str,
-        "type": UserTypeType,
-    },
-)
-
 _RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceConfigurationRequestRequestTypeDef",
     {
         "configuration": str,
         "workspaceId": str,
     },
 )
@@ -491,14 +373,59 @@
     "VpcConfigurationOutputTypeDef",
     {
         "securityGroupIds": List[str],
         "subnetIds": List[str],
     },
 )
 
+CreateWorkspaceApiKeyResponseTypeDef = TypedDict(
+    "CreateWorkspaceApiKeyResponseTypeDef",
+    {
+        "key": str,
+        "keyName": str,
+        "workspaceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteWorkspaceApiKeyResponseTypeDef = TypedDict(
+    "DeleteWorkspaceApiKeyResponseTypeDef",
+    {
+        "keyName": str,
+        "workspaceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorkspaceConfigurationResponseTypeDef = TypedDict(
+    "DescribeWorkspaceConfigurationResponseTypeDef",
+    {
+        "configuration": str,
+        "grafanaVersion": str,
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
+ListVersionsResponseTypeDef = TypedDict(
+    "ListVersionsResponseTypeDef",
+    {
+        "grafanaVersions": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredWorkspaceSummaryTypeDef = TypedDict(
     "_RequiredWorkspaceSummaryTypeDef",
     {
         "authentication": AuthenticationSummaryTypeDef,
         "created": datetime,
         "endpoint": str,
         "grafanaVersion": str,
@@ -583,42 +510,91 @@
 )
 
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
+_RequiredListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
+    "_RequiredListPermissionsRequestListPermissionsPaginateTypeDef",
+    {
+        "workspaceId": str,
+    },
+)
+_OptionalListPermissionsRequestListPermissionsPaginateTypeDef = TypedDict(
+    "_OptionalListPermissionsRequestListPermissionsPaginateTypeDef",
+    {
+        "groupId": str,
+        "userId": str,
+        "userType": UserTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPermissionsRequestListPermissionsPaginateTypeDef(
+    _RequiredListPermissionsRequestListPermissionsPaginateTypeDef,
+    _OptionalListPermissionsRequestListPermissionsPaginateTypeDef,
+):
+    pass
+
+ListVersionsRequestListVersionsPaginateTypeDef = TypedDict(
+    "ListVersionsRequestListVersionsPaginateTypeDef",
+    {
+        "workspaceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkspacesRequestListWorkspacesPaginateTypeDef = TypedDict(
+    "ListWorkspacesRequestListWorkspacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 PermissionEntryTypeDef = TypedDict(
     "PermissionEntryTypeDef",
     {
         "role": RoleType,
-        "user": UserOutputTypeDef,
+        "user": UserTypeDef,
     },
 )
 
 UpdateInstructionOutputTypeDef = TypedDict(
     "UpdateInstructionOutputTypeDef",
     {
         "action": UpdateActionType,
         "role": RoleType,
-        "users": List[UserOutputTypeDef],
+        "users": List[UserTypeDef],
+    },
+)
+
+UpdateInstructionTypeDef = TypedDict(
+    "UpdateInstructionTypeDef",
+    {
+        "action": UpdateActionType,
+        "role": RoleType,
+        "users": Sequence[UserTypeDef],
     },
 )
 
 _RequiredSamlConfigurationOutputTypeDef = TypedDict(
     "_RequiredSamlConfigurationOutputTypeDef",
     {
-        "idpMetadata": IdpMetadataOutputTypeDef,
+        "idpMetadata": IdpMetadataTypeDef,
     },
 )
 _OptionalSamlConfigurationOutputTypeDef = TypedDict(
     "_OptionalSamlConfigurationOutputTypeDef",
     {
         "allowedOrganizations": List[str],
-        "assertionAttributes": AssertionAttributesOutputTypeDef,
+        "assertionAttributes": AssertionAttributesTypeDef,
         "loginValidityDuration": int,
         "roleValues": RoleValuesOutputTypeDef,
     },
     total=False,
 )
 
 class SamlConfigurationOutputTypeDef(
@@ -644,23 +620,14 @@
 )
 
 class SamlConfigurationTypeDef(
     _RequiredSamlConfigurationTypeDef, _OptionalSamlConfigurationTypeDef
 ):
     pass
 
-UpdateInstructionTypeDef = TypedDict(
-    "UpdateInstructionTypeDef",
-    {
-        "action": UpdateActionType,
-        "role": RoleType,
-        "users": Sequence[UserTypeDef],
-    },
-)
-
 _RequiredWorkspaceDescriptionTypeDef = TypedDict(
     "_RequiredWorkspaceDescriptionTypeDef",
     {
         "authentication": AuthenticationSummaryTypeDef,
         "created": datetime,
         "dataSources": List[DataSourceTypeType],
         "endpoint": str,
@@ -699,36 +666,44 @@
     pass
 
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
         "nextToken": str,
         "workspaces": List[WorkspaceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "nextToken": str,
         "permissions": List[PermissionEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateErrorTypeDef = TypedDict(
     "UpdateErrorTypeDef",
     {
         "causedBy": UpdateInstructionOutputTypeDef,
         "code": int,
         "message": str,
     },
 )
 
+UpdatePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdatePermissionsRequestRequestTypeDef",
+    {
+        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
+        "workspaceId": str,
+    },
+)
+
 _RequiredSamlAuthenticationTypeDef = TypedDict(
     "_RequiredSamlAuthenticationTypeDef",
     {
         "status": SamlConfigurationStatusType,
     },
 )
 _OptionalSamlAuthenticationTypeDef = TypedDict(
@@ -761,75 +736,67 @@
 
 class UpdateWorkspaceAuthenticationRequestRequestTypeDef(
     _RequiredUpdateWorkspaceAuthenticationRequestRequestTypeDef,
     _OptionalUpdateWorkspaceAuthenticationRequestRequestTypeDef,
 ):
     pass
 
-UpdatePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdatePermissionsRequestRequestTypeDef",
-    {
-        "updateInstructionBatch": Sequence[UpdateInstructionTypeDef],
-        "workspaceId": str,
-    },
-)
-
 AssociateLicenseResponseTypeDef = TypedDict(
     "AssociateLicenseResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkspaceResponseTypeDef = TypedDict(
     "CreateWorkspaceResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteWorkspaceResponseTypeDef = TypedDict(
     "DeleteWorkspaceResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkspaceResponseTypeDef = TypedDict(
     "DescribeWorkspaceResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateLicenseResponseTypeDef = TypedDict(
     "DisassociateLicenseResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkspaceResponseTypeDef = TypedDict(
     "UpdateWorkspaceResponseTypeDef",
     {
         "workspace": WorkspaceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePermissionsResponseTypeDef = TypedDict(
     "UpdatePermissionsResponseTypeDef",
     {
         "errors": List[UpdateErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAuthenticationDescriptionTypeDef = TypedDict(
     "_RequiredAuthenticationDescriptionTypeDef",
     {
         "providers": List[AuthenticationProviderTypesType],
@@ -849,18 +816,18 @@
 ):
     pass
 
 DescribeWorkspaceAuthenticationResponseTypeDef = TypedDict(
     "DescribeWorkspaceAuthenticationResponseTypeDef",
     {
         "authentication": AuthenticationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkspaceAuthenticationResponseTypeDef = TypedDict(
     "UpdateWorkspaceAuthenticationResponseTypeDef",
     {
         "authentication": AuthenticationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/PKG-INFO` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-grafana
-Version: 1.28.12
-Summary: Type annotations for boto3.ManagedGrafana 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ManagedGrafana 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-grafana.svg?color=blue)](https://pypi.org/project/mypy-boto3-grafana)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-grafana)](https://pepy.tech/project/mypy-boto3-grafana)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ManagedGrafana 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
+[boto3.ManagedGrafana 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
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
 [mypy-boto3-grafana docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_grafana/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,82 +337,79 @@
 ### Typed dictionaries
 
 `mypy_boto3_grafana.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_grafana.type_defs import (
-    AssertionAttributesOutputTypeDef,
     AssertionAttributesTypeDef,
     AssociateLicenseRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AwsSsoAuthenticationTypeDef,
     AuthenticationSummaryTypeDef,
     CreateWorkspaceApiKeyRequestRequestTypeDef,
-    CreateWorkspaceApiKeyResponseTypeDef,
     NetworkAccessConfigurationTypeDef,
     VpcConfigurationTypeDef,
     DeleteWorkspaceApiKeyRequestRequestTypeDef,
-    DeleteWorkspaceApiKeyResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
     DescribeWorkspaceAuthenticationRequestRequestTypeDef,
     DescribeWorkspaceConfigurationRequestRequestTypeDef,
-    DescribeWorkspaceConfigurationResponseTypeDef,
     DescribeWorkspaceRequestRequestTypeDef,
     DisassociateLicenseRequestRequestTypeDef,
-    IdpMetadataOutputTypeDef,
     IdpMetadataTypeDef,
-    ListPermissionsRequestListPermissionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPermissionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVersionsRequestListVersionsPaginateTypeDef,
     ListVersionsRequestRequestTypeDef,
-    ListVersionsResponseTypeDef,
-    ListWorkspacesRequestListWorkspacesPaginateTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     NetworkAccessConfigurationOutputTypeDef,
-    PaginatorConfigTypeDef,
-    UserOutputTypeDef,
-    ResponseMetadataTypeDef,
+    UserTypeDef,
     RoleValuesOutputTypeDef,
     RoleValuesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UserTypeDef,
     UpdateWorkspaceConfigurationRequestRequestTypeDef,
     VpcConfigurationOutputTypeDef,
+    CreateWorkspaceApiKeyResponseTypeDef,
+    DeleteWorkspaceApiKeyResponseTypeDef,
+    DescribeWorkspaceConfigurationResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListVersionsResponseTypeDef,
     WorkspaceSummaryTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
+    ListPermissionsRequestListPermissionsPaginateTypeDef,
+    ListVersionsRequestListVersionsPaginateTypeDef,
+    ListWorkspacesRequestListWorkspacesPaginateTypeDef,
     PermissionEntryTypeDef,
     UpdateInstructionOutputTypeDef,
+    UpdateInstructionTypeDef,
     SamlConfigurationOutputTypeDef,
     SamlConfigurationTypeDef,
-    UpdateInstructionTypeDef,
     WorkspaceDescriptionTypeDef,
     ListWorkspacesResponseTypeDef,
     ListPermissionsResponseTypeDef,
     UpdateErrorTypeDef,
+    UpdatePermissionsRequestRequestTypeDef,
     SamlAuthenticationTypeDef,
     UpdateWorkspaceAuthenticationRequestRequestTypeDef,
-    UpdatePermissionsRequestRequestTypeDef,
     AssociateLicenseResponseTypeDef,
     CreateWorkspaceResponseTypeDef,
     DeleteWorkspaceResponseTypeDef,
     DescribeWorkspaceResponseTypeDef,
     DisassociateLicenseResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
     UpdatePermissionsResponseTypeDef,
     AuthenticationDescriptionTypeDef,
     DescribeWorkspaceAuthenticationResponseTypeDef,
     UpdateWorkspaceAuthenticationResponseTypeDef,
 )
 
 
-def get_structure() -> AssertionAttributesOutputTypeDef:
+def get_structure() -> AssertionAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-grafana-1.28.12/mypy_boto3_grafana.egg-info/SOURCES.txt` & `mypy-boto3-grafana-1.28.15/mypy_boto3_grafana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-grafana-1.28.12/setup.py` & `mypy-boto3-grafana-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-grafana",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_grafana"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ManagedGrafana 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ManagedGrafana 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

