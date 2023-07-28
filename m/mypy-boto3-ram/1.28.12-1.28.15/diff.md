# Comparing `tmp/mypy-boto3-ram-1.28.12.tar.gz` & `tmp/mypy-boto3-ram-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ram-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
+gzip compressed data, was "mypy-boto3-ram-1.28.15.tar", last modified: Fri Jul 28 20:43:30 2023, max compression
```

## Comparing `mypy-boto3-ram-1.28.12.tar` & `mypy-boto3-ram-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.593188 mypy-boto3-ram-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17668 2023-07-27 11:49:27.581188 mypy-boto3-ram-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.577188 mypy-boto3-ram-1.28.12/mypy_boto3_ram/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-07-27 11:43:55.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31821 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-07-27 11:43:56.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-27 11:43:56.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-07-27 11:43:55.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-27 11:43:55.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41268 2023-07-27 11:43:57.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41203 2023-07-27 11:43:56.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.581188 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17668 2023-07-27 11:49:27.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:27.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:27.000000 mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.593188 mypy-boto3-ram-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:43:54.000000 mypy-boto3-ram-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.953689 mypy-boto3-ram-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:36:06.000000 mypy-boto3-ram-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-07-28 20:43:30.949689 mypy-boto3-ram-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-07-28 20:36:06.000000 mypy-boto3-ram-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.941689 mypy-boto3-ram-1.28.15/mypy_boto3_ram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-28 20:36:06.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-28 20:36:06.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:36:06.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-07-28 20:36:07.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31821 2023-07-28 20:36:06.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-07-28 20:36:07.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-28 20:36:07.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-07-28 20:36:07.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-28 20:36:07.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:36:06.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41097 2023-07-28 20:36:12.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41032 2023-07-28 20:36:11.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:36:06.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.949689 mypy-boto3-ram-1.28.15/mypy_boto3_ram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-07-28 20:43:30.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:43:30.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:30.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:30.000000 mypy-boto3-ram-1.28.15/mypy_boto3_ram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:30.953689 mypy-boto3-ram-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:36:06.000000 mypy-boto3-ram-1.28.15/setup.py
```

### Comparing `mypy-boto3-ram-1.28.12/LICENSE` & `mypy-boto3-ram-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.12/PKG-INFO` & `mypy-boto3-ram-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ram
-Version: 1.28.12
-Summary: Type annotations for boto3.RAM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.RAM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ram)](https://pepy.tech/project/mypy-boto3-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RAM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[boto3.RAM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
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
 [mypy-boto3-ram docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/).
 
 See how it helps to find and fix potential bugs:
 
@@ -392,15 +392,14 @@
     ListResourceTypesRequestRequestTypeDef,
     ServiceNameAndResourceTypeTypeDef,
     ListResourcesRequestRequestTypeDef,
     PromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef,
     RejectResourceShareInvitationRequestRequestTypeDef,
     ReplacePermissionAssociationsRequestRequestTypeDef,
-    TagOutputTypeDef,
     SetDefaultPermissionVersionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateResourceShareRequestRequestTypeDef,
     AssociateResourceSharePermissionResponseTypeDef,
     DeletePermissionResponseTypeDef,
     DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareResponseTypeDef,
@@ -412,31 +411,31 @@
     AssociateResourceShareResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     ResourceShareInvitationTypeDef,
     ListPermissionAssociationsResponseTypeDef,
     CreatePermissionRequestRequestTypeDef,
     CreateResourceShareRequestRequestTypeDef,
+    ResourceSharePermissionDetailTypeDef,
+    ResourceSharePermissionSummaryTypeDef,
+    ResourceShareTypeDef,
     TagResourceRequestRequestTypeDef,
     GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
     GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
     ListPrincipalsRequestListPrincipalsPaginateTypeDef,
     ListResourcesRequestListResourcesPaginateTypeDef,
     GetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     GetResourceSharesRequestRequestTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListPrincipalsResponseTypeDef,
     ListReplacePermissionAssociationsWorkResponseTypeDef,
     ReplacePermissionAssociationsResponseTypeDef,
     ListResourceTypesResponseTypeDef,
-    ResourceSharePermissionDetailTypeDef,
-    ResourceSharePermissionSummaryTypeDef,
-    ResourceShareTypeDef,
     AcceptResourceShareInvitationResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
     CreatePermissionVersionResponseTypeDef,
     GetPermissionResponseTypeDef,
     CreatePermissionResponseTypeDef,
     ListPermissionVersionsResponseTypeDef,
```

### Comparing `mypy-boto3-ram-1.28.12/README.md` & `mypy-boto3-ram-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ram)](https://pepy.tech/project/mypy-boto3-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RAM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[boto3.RAM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
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
 [mypy-boto3-ram docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,15 +360,14 @@
     ListResourceTypesRequestRequestTypeDef,
     ServiceNameAndResourceTypeTypeDef,
     ListResourcesRequestRequestTypeDef,
     PromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef,
     RejectResourceShareInvitationRequestRequestTypeDef,
     ReplacePermissionAssociationsRequestRequestTypeDef,
-    TagOutputTypeDef,
     SetDefaultPermissionVersionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateResourceShareRequestRequestTypeDef,
     AssociateResourceSharePermissionResponseTypeDef,
     DeletePermissionResponseTypeDef,
     DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareResponseTypeDef,
@@ -380,31 +379,31 @@
     AssociateResourceShareResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     ResourceShareInvitationTypeDef,
     ListPermissionAssociationsResponseTypeDef,
     CreatePermissionRequestRequestTypeDef,
     CreateResourceShareRequestRequestTypeDef,
+    ResourceSharePermissionDetailTypeDef,
+    ResourceSharePermissionSummaryTypeDef,
+    ResourceShareTypeDef,
     TagResourceRequestRequestTypeDef,
     GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
     GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
     ListPrincipalsRequestListPrincipalsPaginateTypeDef,
     ListResourcesRequestListResourcesPaginateTypeDef,
     GetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     GetResourceSharesRequestRequestTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListPrincipalsResponseTypeDef,
     ListReplacePermissionAssociationsWorkResponseTypeDef,
     ReplacePermissionAssociationsResponseTypeDef,
     ListResourceTypesResponseTypeDef,
-    ResourceSharePermissionDetailTypeDef,
-    ResourceSharePermissionSummaryTypeDef,
-    ResourceShareTypeDef,
     AcceptResourceShareInvitationResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
     CreatePermissionVersionResponseTypeDef,
     GetPermissionResponseTypeDef,
     CreatePermissionResponseTypeDef,
     ListPermissionVersionsResponseTypeDef,
```

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram/__init__.py` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram/__init__.pyi` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram/__main__.py` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RAM 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.RAM 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM\nOther"
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

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram/client.py` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram/client.pyi` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram/literals.py` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram/literals.pyi` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram/paginator.py` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram/paginator.pyi` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram/type_defs.py` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     "ListResourceTypesRequestRequestTypeDef",
     "ServiceNameAndResourceTypeTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "PromotePermissionCreatedFromPolicyRequestRequestTypeDef",
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
     "RejectResourceShareInvitationRequestRequestTypeDef",
     "ReplacePermissionAssociationsRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "SetDefaultPermissionVersionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateResourceShareRequestRequestTypeDef",
     "AssociateResourceSharePermissionResponseTypeDef",
     "DeletePermissionResponseTypeDef",
     "DeletePermissionVersionResponseTypeDef",
     "DeleteResourceShareResponseTypeDef",
@@ -91,31 +90,31 @@
     "AssociateResourceShareResponseTypeDef",
     "DisassociateResourceShareResponseTypeDef",
     "GetResourceShareAssociationsResponseTypeDef",
     "ResourceShareInvitationTypeDef",
     "ListPermissionAssociationsResponseTypeDef",
     "CreatePermissionRequestRequestTypeDef",
     "CreateResourceShareRequestRequestTypeDef",
+    "ResourceSharePermissionDetailTypeDef",
+    "ResourceSharePermissionSummaryTypeDef",
+    "ResourceShareTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
     "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
     "ListPrincipalsRequestListPrincipalsPaginateTypeDef",
     "ListResourcesRequestListResourcesPaginateTypeDef",
     "GetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     "GetResourceSharesRequestRequestTypeDef",
     "ListPendingInvitationResourcesResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "ListPrincipalsResponseTypeDef",
     "ListReplacePermissionAssociationsWorkResponseTypeDef",
     "ReplacePermissionAssociationsResponseTypeDef",
     "ListResourceTypesResponseTypeDef",
-    "ResourceSharePermissionDetailTypeDef",
-    "ResourceSharePermissionSummaryTypeDef",
-    "ResourceShareTypeDef",
     "AcceptResourceShareInvitationResponseTypeDef",
     "GetResourceShareInvitationsResponseTypeDef",
     "RejectResourceShareInvitationResponseTypeDef",
     "CreatePermissionVersionResponseTypeDef",
     "GetPermissionResponseTypeDef",
     "CreatePermissionResponseTypeDef",
     "ListPermissionVersionsResponseTypeDef",
@@ -785,23 +784,14 @@
 class ReplacePermissionAssociationsRequestRequestTypeDef(
     _RequiredReplacePermissionAssociationsRequestRequestTypeDef,
     _OptionalReplacePermissionAssociationsRequestRequestTypeDef,
 ):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
 _RequiredSetDefaultPermissionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredSetDefaultPermissionVersionRequestRequestTypeDef",
     {
         "permissionArn": str,
         "permissionVersion": int,
     },
 )
@@ -1048,14 +1038,70 @@
 class CreateResourceShareRequestRequestTypeDef(
     _RequiredCreateResourceShareRequestRequestTypeDef,
     _OptionalCreateResourceShareRequestRequestTypeDef,
 ):
     pass
 
 
+ResourceSharePermissionDetailTypeDef = TypedDict(
+    "ResourceSharePermissionDetailTypeDef",
+    {
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "permission": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+        "permissionType": PermissionTypeType,
+        "featureSet": PermissionFeatureSetType,
+        "status": PermissionStatusType,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+ResourceSharePermissionSummaryTypeDef = TypedDict(
+    "ResourceSharePermissionSummaryTypeDef",
+    {
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "status": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+        "permissionType": PermissionTypeType,
+        "featureSet": PermissionFeatureSetType,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+ResourceShareTypeDef = TypedDict(
+    "ResourceShareTypeDef",
+    {
+        "resourceShareArn": str,
+        "name": str,
+        "owningAccountId": str,
+        "allowExternalPrincipals": bool,
+        "status": ResourceShareStatusType,
+        "statusMessage": str,
+        "tags": List[TagTypeDef],
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "featureSet": ResourceShareFeatureSetType,
+    },
+    total=False,
+)
+
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
@@ -1292,70 +1338,14 @@
     {
         "resourceTypes": List[ServiceNameAndResourceTypeTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResourceSharePermissionDetailTypeDef = TypedDict(
-    "ResourceSharePermissionDetailTypeDef",
-    {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "permission": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
-        "permissionType": PermissionTypeType,
-        "featureSet": PermissionFeatureSetType,
-        "status": PermissionStatusType,
-        "tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-ResourceSharePermissionSummaryTypeDef = TypedDict(
-    "ResourceSharePermissionSummaryTypeDef",
-    {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "status": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
-        "permissionType": PermissionTypeType,
-        "featureSet": PermissionFeatureSetType,
-        "tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-ResourceShareTypeDef = TypedDict(
-    "ResourceShareTypeDef",
-    {
-        "resourceShareArn": str,
-        "name": str,
-        "owningAccountId": str,
-        "allowExternalPrincipals": bool,
-        "status": ResourceShareStatusType,
-        "statusMessage": str,
-        "tags": List[TagOutputTypeDef],
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "featureSet": ResourceShareFeatureSetType,
-    },
-    total=False,
-)
-
 AcceptResourceShareInvitationResponseTypeDef = TypedDict(
     "AcceptResourceShareInvitationResponseTypeDef",
     {
         "resourceShareInvitation": ResourceShareInvitationTypeDef,
         "clientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram/type_defs.pyi` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     "ListResourceTypesRequestRequestTypeDef",
     "ServiceNameAndResourceTypeTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "PromotePermissionCreatedFromPolicyRequestRequestTypeDef",
     "PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef",
     "RejectResourceShareInvitationRequestRequestTypeDef",
     "ReplacePermissionAssociationsRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "SetDefaultPermissionVersionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateResourceShareRequestRequestTypeDef",
     "AssociateResourceSharePermissionResponseTypeDef",
     "DeletePermissionResponseTypeDef",
     "DeletePermissionVersionResponseTypeDef",
     "DeleteResourceShareResponseTypeDef",
@@ -90,31 +89,31 @@
     "AssociateResourceShareResponseTypeDef",
     "DisassociateResourceShareResponseTypeDef",
     "GetResourceShareAssociationsResponseTypeDef",
     "ResourceShareInvitationTypeDef",
     "ListPermissionAssociationsResponseTypeDef",
     "CreatePermissionRequestRequestTypeDef",
     "CreateResourceShareRequestRequestTypeDef",
+    "ResourceSharePermissionDetailTypeDef",
+    "ResourceSharePermissionSummaryTypeDef",
+    "ResourceShareTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     "GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef",
     "GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef",
     "ListPrincipalsRequestListPrincipalsPaginateTypeDef",
     "ListResourcesRequestListResourcesPaginateTypeDef",
     "GetResourceSharesRequestGetResourceSharesPaginateTypeDef",
     "GetResourceSharesRequestRequestTypeDef",
     "ListPendingInvitationResourcesResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "ListPrincipalsResponseTypeDef",
     "ListReplacePermissionAssociationsWorkResponseTypeDef",
     "ReplacePermissionAssociationsResponseTypeDef",
     "ListResourceTypesResponseTypeDef",
-    "ResourceSharePermissionDetailTypeDef",
-    "ResourceSharePermissionSummaryTypeDef",
-    "ResourceShareTypeDef",
     "AcceptResourceShareInvitationResponseTypeDef",
     "GetResourceShareInvitationsResponseTypeDef",
     "RejectResourceShareInvitationResponseTypeDef",
     "CreatePermissionVersionResponseTypeDef",
     "GetPermissionResponseTypeDef",
     "CreatePermissionResponseTypeDef",
     "ListPermissionVersionsResponseTypeDef",
@@ -744,23 +743,14 @@
 
 class ReplacePermissionAssociationsRequestRequestTypeDef(
     _RequiredReplacePermissionAssociationsRequestRequestTypeDef,
     _OptionalReplacePermissionAssociationsRequestRequestTypeDef,
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
 _RequiredSetDefaultPermissionVersionRequestRequestTypeDef = TypedDict(
     "_RequiredSetDefaultPermissionVersionRequestRequestTypeDef",
     {
         "permissionArn": str,
         "permissionVersion": int,
     },
 )
@@ -997,14 +987,70 @@
 
 class CreateResourceShareRequestRequestTypeDef(
     _RequiredCreateResourceShareRequestRequestTypeDef,
     _OptionalCreateResourceShareRequestRequestTypeDef,
 ):
     pass
 
+ResourceSharePermissionDetailTypeDef = TypedDict(
+    "ResourceSharePermissionDetailTypeDef",
+    {
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "permission": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+        "permissionType": PermissionTypeType,
+        "featureSet": PermissionFeatureSetType,
+        "status": PermissionStatusType,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+ResourceSharePermissionSummaryTypeDef = TypedDict(
+    "ResourceSharePermissionSummaryTypeDef",
+    {
+        "arn": str,
+        "version": str,
+        "defaultVersion": bool,
+        "name": str,
+        "resourceType": str,
+        "status": str,
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "isResourceTypeDefault": bool,
+        "permissionType": PermissionTypeType,
+        "featureSet": PermissionFeatureSetType,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+ResourceShareTypeDef = TypedDict(
+    "ResourceShareTypeDef",
+    {
+        "resourceShareArn": str,
+        "name": str,
+        "owningAccountId": str,
+        "allowExternalPrincipals": bool,
+        "status": ResourceShareStatusType,
+        "statusMessage": str,
+        "tags": List[TagTypeDef],
+        "creationTime": datetime,
+        "lastUpdatedTime": datetime,
+        "featureSet": ResourceShareFeatureSetType,
+    },
+    total=False,
+)
+
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
@@ -1227,70 +1273,14 @@
     {
         "resourceTypes": List[ServiceNameAndResourceTypeTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResourceSharePermissionDetailTypeDef = TypedDict(
-    "ResourceSharePermissionDetailTypeDef",
-    {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "permission": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
-        "permissionType": PermissionTypeType,
-        "featureSet": PermissionFeatureSetType,
-        "status": PermissionStatusType,
-        "tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-ResourceSharePermissionSummaryTypeDef = TypedDict(
-    "ResourceSharePermissionSummaryTypeDef",
-    {
-        "arn": str,
-        "version": str,
-        "defaultVersion": bool,
-        "name": str,
-        "resourceType": str,
-        "status": str,
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "isResourceTypeDefault": bool,
-        "permissionType": PermissionTypeType,
-        "featureSet": PermissionFeatureSetType,
-        "tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-ResourceShareTypeDef = TypedDict(
-    "ResourceShareTypeDef",
-    {
-        "resourceShareArn": str,
-        "name": str,
-        "owningAccountId": str,
-        "allowExternalPrincipals": bool,
-        "status": ResourceShareStatusType,
-        "statusMessage": str,
-        "tags": List[TagOutputTypeDef],
-        "creationTime": datetime,
-        "lastUpdatedTime": datetime,
-        "featureSet": ResourceShareFeatureSetType,
-    },
-    total=False,
-)
-
 AcceptResourceShareInvitationResponseTypeDef = TypedDict(
     "AcceptResourceShareInvitationResponseTypeDef",
     {
         "resourceShareInvitation": ResourceShareInvitationTypeDef,
         "clientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/PKG-INFO` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ram
-Version: 1.28.12
-Summary: Type annotations for boto3.RAM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.RAM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ram.svg?color=blue)](https://pypi.org/project/mypy-boto3-ram)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ram)](https://pepy.tech/project/mypy-boto3-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RAM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[boto3.RAM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
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
 [mypy-boto3-ram docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ram/).
 
 See how it helps to find and fix potential bugs:
 
@@ -392,15 +392,14 @@
     ListResourceTypesRequestRequestTypeDef,
     ServiceNameAndResourceTypeTypeDef,
     ListResourcesRequestRequestTypeDef,
     PromotePermissionCreatedFromPolicyRequestRequestTypeDef,
     PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef,
     RejectResourceShareInvitationRequestRequestTypeDef,
     ReplacePermissionAssociationsRequestRequestTypeDef,
-    TagOutputTypeDef,
     SetDefaultPermissionVersionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateResourceShareRequestRequestTypeDef,
     AssociateResourceSharePermissionResponseTypeDef,
     DeletePermissionResponseTypeDef,
     DeletePermissionVersionResponseTypeDef,
     DeleteResourceShareResponseTypeDef,
@@ -412,31 +411,31 @@
     AssociateResourceShareResponseTypeDef,
     DisassociateResourceShareResponseTypeDef,
     GetResourceShareAssociationsResponseTypeDef,
     ResourceShareInvitationTypeDef,
     ListPermissionAssociationsResponseTypeDef,
     CreatePermissionRequestRequestTypeDef,
     CreateResourceShareRequestRequestTypeDef,
+    ResourceSharePermissionDetailTypeDef,
+    ResourceSharePermissionSummaryTypeDef,
+    ResourceShareTypeDef,
     TagResourceRequestRequestTypeDef,
     GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef,
     GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef,
     GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef,
     ListPrincipalsRequestListPrincipalsPaginateTypeDef,
     ListResourcesRequestListResourcesPaginateTypeDef,
     GetResourceSharesRequestGetResourceSharesPaginateTypeDef,
     GetResourceSharesRequestRequestTypeDef,
     ListPendingInvitationResourcesResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListPrincipalsResponseTypeDef,
     ListReplacePermissionAssociationsWorkResponseTypeDef,
     ReplacePermissionAssociationsResponseTypeDef,
     ListResourceTypesResponseTypeDef,
-    ResourceSharePermissionDetailTypeDef,
-    ResourceSharePermissionSummaryTypeDef,
-    ResourceShareTypeDef,
     AcceptResourceShareInvitationResponseTypeDef,
     GetResourceShareInvitationsResponseTypeDef,
     RejectResourceShareInvitationResponseTypeDef,
     CreatePermissionVersionResponseTypeDef,
     GetPermissionResponseTypeDef,
     CreatePermissionResponseTypeDef,
     ListPermissionVersionsResponseTypeDef,
```

### Comparing `mypy-boto3-ram-1.28.12/mypy_boto3_ram.egg-info/SOURCES.txt` & `mypy-boto3-ram-1.28.15/mypy_boto3_ram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ram-1.28.12/setup.py` & `mypy-boto3-ram-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ram",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ram"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RAM 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.RAM 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

