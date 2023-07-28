# Comparing `tmp/mypy-boto3-organizations-1.28.12.tar.gz` & `tmp/mypy-boto3-organizations-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-organizations-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
+gzip compressed data, was "mypy-boto3-organizations-1.28.15.tar", last modified: Fri Jul 28 20:43:24 2023, max compression
```

## Comparing `mypy-boto3-organizations-1.28.12.tar` & `mypy-boto3-organizations-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.793132 mypy-boto3-organizations-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21949 2023-07-27 11:49:21.793132 mypy-boto3-organizations-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20438 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.785132 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46983 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46905 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19645 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44616 2023-07-27 11:41:07.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44561 2023-07-27 11:41:06.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.785132 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21949 2023-07-27 11:49:21.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 11:49:21.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:49:21.000000 mypy-boto3-organizations-1.28.12/mypy_boto3_organizations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.793132 mypy-boto3-organizations-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 11:41:05.000000 mypy-boto3-organizations-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.657603 mypy-boto3-organizations-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:01.000000 mypy-boto3-organizations-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21894 2023-07-28 20:43:24.657603 mypy-boto3-organizations-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20383 2023-07-28 20:33:01.000000 mypy-boto3-organizations-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.657603 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-28 20:33:01.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-28 20:33:01.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:33:01.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46983 2023-07-28 20:33:04.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46905 2023-07-28 20:33:02.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-28 20:33:05.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-07-28 20:33:04.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-07-28 20:33:04.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19645 2023-07-28 20:33:04.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:01.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44282 2023-07-28 20:33:06.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44227 2023-07-28 20:33:05.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:01.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.657603 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21894 2023-07-28 20:43:24.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:43:24.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:24.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:43:24.000000 mypy-boto3-organizations-1.28.15/mypy_boto3_organizations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:24.657603 mypy-boto3-organizations-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 20:33:01.000000 mypy-boto3-organizations-1.28.15/setup.py
```

### Comparing `mypy-boto3-organizations-1.28.12/LICENSE` & `mypy-boto3-organizations-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-organizations-1.28.12/PKG-INFO` & `mypy-boto3-organizations-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-organizations
-Version: 1.28.12
-Summary: Type annotations for boto3.Organizations 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Organizations 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_organizations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-organizations.svg?color=blue)](https://pypi.org/project/mypy-boto3-organizations)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_organizations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-organizations)](https://pepy.tech/project/mypy-boto3-organizations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Organizations 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
+[boto3.Organizations 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
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
 [mypy-boto3-organizations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_organizations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -434,15 +434,14 @@
     DetachPolicyRequestRequestTypeDef,
     DisableAWSServiceAccessRequestRequestTypeDef,
     DisablePolicyTypeRequestRequestTypeDef,
     EnableAWSServiceAccessRequestRequestTypeDef,
     EnablePolicyTypeRequestRequestTypeDef,
     EnabledServicePrincipalTypeDef,
     HandshakeFilterTypeDef,
-    HandshakePartyOutputTypeDef,
     HandshakePartyTypeDef,
     HandshakeResourceTypeDef,
     PaginatorConfigTypeDef,
     ListAWSServiceAccessForOrganizationRequestRequestTypeDef,
     ListAccountsForParentRequestRequestTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListChildrenRequestRequestTypeDef,
@@ -453,15 +452,14 @@
     ListParentsRequestRequestTypeDef,
     ParentTypeDef,
     ListPoliciesForTargetRequestRequestTypeDef,
     PolicySummaryTypeDef,
     ListPoliciesRequestRequestTypeDef,
     ListRootsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListTargetsForPolicyRequestRequestTypeDef,
     PolicyTargetSummaryTypeDef,
     MoveAccountRequestRequestTypeDef,
     PolicyTypeSummaryTypeDef,
     RegisterDelegatedAdministratorRequestRequestTypeDef,
     RemoveAccountFromOrganizationRequestRequestTypeDef,
     ResourcePolicySummaryTypeDef,
@@ -473,14 +471,15 @@
     ListAccountsForParentResponseTypeDef,
     ListAccountsResponseTypeDef,
     ListChildrenResponseTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateGovCloudAccountRequestRequestTypeDef,
     CreateOrganizationalUnitRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateAccountResponseTypeDef,
     CreateGovCloudAccountResponseTypeDef,
     DescribeCreateAccountStatusResponseTypeDef,
     ListCreateAccountStatusResponseTypeDef,
     CreateOrganizationalUnitResponseTypeDef,
@@ -511,15 +510,14 @@
     ListRootsRequestListRootsPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
     ListParentsResponseTypeDef,
     ListPoliciesForTargetResponseTypeDef,
     ListPoliciesResponseTypeDef,
     PolicyTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTargetsForPolicyResponseTypeDef,
     OrganizationTypeDef,
     RootTypeDef,
     ResourcePolicyTypeDef,
     AcceptHandshakeResponseTypeDef,
     CancelHandshakeResponseTypeDef,
     DeclineHandshakeResponseTypeDef,
```

### Comparing `mypy-boto3-organizations-1.28.12/README.md` & `mypy-boto3-organizations-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-organizations.svg?color=blue)](https://pypi.org/project/mypy-boto3-organizations)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_organizations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-organizations)](https://pepy.tech/project/mypy-boto3-organizations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Organizations 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
+[boto3.Organizations 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
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
 [mypy-boto3-organizations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_organizations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -402,15 +402,14 @@
     DetachPolicyRequestRequestTypeDef,
     DisableAWSServiceAccessRequestRequestTypeDef,
     DisablePolicyTypeRequestRequestTypeDef,
     EnableAWSServiceAccessRequestRequestTypeDef,
     EnablePolicyTypeRequestRequestTypeDef,
     EnabledServicePrincipalTypeDef,
     HandshakeFilterTypeDef,
-    HandshakePartyOutputTypeDef,
     HandshakePartyTypeDef,
     HandshakeResourceTypeDef,
     PaginatorConfigTypeDef,
     ListAWSServiceAccessForOrganizationRequestRequestTypeDef,
     ListAccountsForParentRequestRequestTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListChildrenRequestRequestTypeDef,
@@ -421,15 +420,14 @@
     ListParentsRequestRequestTypeDef,
     ParentTypeDef,
     ListPoliciesForTargetRequestRequestTypeDef,
     PolicySummaryTypeDef,
     ListPoliciesRequestRequestTypeDef,
     ListRootsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListTargetsForPolicyRequestRequestTypeDef,
     PolicyTargetSummaryTypeDef,
     MoveAccountRequestRequestTypeDef,
     PolicyTypeSummaryTypeDef,
     RegisterDelegatedAdministratorRequestRequestTypeDef,
     RemoveAccountFromOrganizationRequestRequestTypeDef,
     ResourcePolicySummaryTypeDef,
@@ -441,14 +439,15 @@
     ListAccountsForParentResponseTypeDef,
     ListAccountsResponseTypeDef,
     ListChildrenResponseTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateGovCloudAccountRequestRequestTypeDef,
     CreateOrganizationalUnitRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateAccountResponseTypeDef,
     CreateGovCloudAccountResponseTypeDef,
     DescribeCreateAccountStatusResponseTypeDef,
     ListCreateAccountStatusResponseTypeDef,
     CreateOrganizationalUnitResponseTypeDef,
@@ -479,15 +478,14 @@
     ListRootsRequestListRootsPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
     ListParentsResponseTypeDef,
     ListPoliciesForTargetResponseTypeDef,
     ListPoliciesResponseTypeDef,
     PolicyTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTargetsForPolicyResponseTypeDef,
     OrganizationTypeDef,
     RootTypeDef,
     ResourcePolicyTypeDef,
     AcceptHandshakeResponseTypeDef,
     CancelHandshakeResponseTypeDef,
     DeclineHandshakeResponseTypeDef,
```

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/__init__.py` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/__init__.pyi` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/__main__.py` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Organizations 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.Organizations 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_organizations//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations\nOther"
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

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/client.py` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/client.pyi` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/literals.py` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/literals.pyi` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/paginator.py` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/paginator.pyi` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/type_defs.py` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     "DetachPolicyRequestRequestTypeDef",
     "DisableAWSServiceAccessRequestRequestTypeDef",
     "DisablePolicyTypeRequestRequestTypeDef",
     "EnableAWSServiceAccessRequestRequestTypeDef",
     "EnablePolicyTypeRequestRequestTypeDef",
     "EnabledServicePrincipalTypeDef",
     "HandshakeFilterTypeDef",
-    "HandshakePartyOutputTypeDef",
     "HandshakePartyTypeDef",
     "HandshakeResourceTypeDef",
     "PaginatorConfigTypeDef",
     "ListAWSServiceAccessForOrganizationRequestRequestTypeDef",
     "ListAccountsForParentRequestRequestTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "ListChildrenRequestRequestTypeDef",
@@ -87,15 +86,14 @@
     "ListParentsRequestRequestTypeDef",
     "ParentTypeDef",
     "ListPoliciesForTargetRequestRequestTypeDef",
     "PolicySummaryTypeDef",
     "ListPoliciesRequestRequestTypeDef",
     "ListRootsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListTargetsForPolicyRequestRequestTypeDef",
     "PolicyTargetSummaryTypeDef",
     "MoveAccountRequestRequestTypeDef",
     "PolicyTypeSummaryTypeDef",
     "RegisterDelegatedAdministratorRequestRequestTypeDef",
     "RemoveAccountFromOrganizationRequestRequestTypeDef",
     "ResourcePolicySummaryTypeDef",
@@ -107,14 +105,15 @@
     "ListAccountsForParentResponseTypeDef",
     "ListAccountsResponseTypeDef",
     "ListChildrenResponseTypeDef",
     "CreateAccountRequestRequestTypeDef",
     "CreateGovCloudAccountRequestRequestTypeDef",
     "CreateOrganizationalUnitRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateAccountResponseTypeDef",
     "CreateGovCloudAccountResponseTypeDef",
     "DescribeCreateAccountStatusResponseTypeDef",
     "ListCreateAccountStatusResponseTypeDef",
     "CreateOrganizationalUnitResponseTypeDef",
@@ -145,15 +144,14 @@
     "ListRootsRequestListRootsPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
     "ListParentsResponseTypeDef",
     "ListPoliciesForTargetResponseTypeDef",
     "ListPoliciesResponseTypeDef",
     "PolicyTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTargetsForPolicyResponseTypeDef",
     "OrganizationTypeDef",
     "RootTypeDef",
     "ResourcePolicyTypeDef",
     "AcceptHandshakeResponseTypeDef",
     "CancelHandshakeResponseTypeDef",
     "DeclineHandshakeResponseTypeDef",
@@ -451,22 +449,14 @@
     {
         "ActionType": ActionTypeType,
         "ParentHandshakeId": str,
     },
     total=False,
 )
 
-HandshakePartyOutputTypeDef = TypedDict(
-    "HandshakePartyOutputTypeDef",
-    {
-        "Id": str,
-        "Type": HandshakePartyTypeType,
-    },
-)
-
 HandshakePartyTypeDef = TypedDict(
     "HandshakePartyTypeDef",
     {
         "Id": str,
         "Type": HandshakePartyTypeType,
     },
 )
@@ -738,22 +728,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredListTargetsForPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsForPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalListTargetsForPolicyRequestRequestTypeDef = TypedDict(
@@ -1013,14 +995,23 @@
 
 class CreatePolicyRequestRequestTypeDef(
     _RequiredCreatePolicyRequestRequestTypeDef, _OptionalCreatePolicyRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "Content": str,
     },
 )
 _OptionalPutResourcePolicyRequestRequestTypeDef = TypedDict(
@@ -1168,15 +1159,15 @@
 )
 
 HandshakeTypeDef = TypedDict(
     "HandshakeTypeDef",
     {
         "Id": str,
         "Arn": str,
-        "Parties": List[HandshakePartyOutputTypeDef],
+        "Parties": List[HandshakePartyTypeDef],
         "State": HandshakeStateType,
         "RequestedTimestamp": datetime,
         "ExpirationTimestamp": datetime,
         "Action": ActionTypeType,
         "Resources": List["HandshakeResourceTypeDef"],
     },
     total=False,
@@ -1497,23 +1488,14 @@
     {
         "PolicySummary": PolicySummaryTypeDef,
         "Content": str,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTargetsForPolicyResponseTypeDef = TypedDict(
     "ListTargetsForPolicyResponseTypeDef",
     {
         "Targets": List[PolicyTargetSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations/type_defs.pyi` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     "DetachPolicyRequestRequestTypeDef",
     "DisableAWSServiceAccessRequestRequestTypeDef",
     "DisablePolicyTypeRequestRequestTypeDef",
     "EnableAWSServiceAccessRequestRequestTypeDef",
     "EnablePolicyTypeRequestRequestTypeDef",
     "EnabledServicePrincipalTypeDef",
     "HandshakeFilterTypeDef",
-    "HandshakePartyOutputTypeDef",
     "HandshakePartyTypeDef",
     "HandshakeResourceTypeDef",
     "PaginatorConfigTypeDef",
     "ListAWSServiceAccessForOrganizationRequestRequestTypeDef",
     "ListAccountsForParentRequestRequestTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "ListChildrenRequestRequestTypeDef",
@@ -86,15 +85,14 @@
     "ListParentsRequestRequestTypeDef",
     "ParentTypeDef",
     "ListPoliciesForTargetRequestRequestTypeDef",
     "PolicySummaryTypeDef",
     "ListPoliciesRequestRequestTypeDef",
     "ListRootsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListTargetsForPolicyRequestRequestTypeDef",
     "PolicyTargetSummaryTypeDef",
     "MoveAccountRequestRequestTypeDef",
     "PolicyTypeSummaryTypeDef",
     "RegisterDelegatedAdministratorRequestRequestTypeDef",
     "RemoveAccountFromOrganizationRequestRequestTypeDef",
     "ResourcePolicySummaryTypeDef",
@@ -106,14 +104,15 @@
     "ListAccountsForParentResponseTypeDef",
     "ListAccountsResponseTypeDef",
     "ListChildrenResponseTypeDef",
     "CreateAccountRequestRequestTypeDef",
     "CreateGovCloudAccountRequestRequestTypeDef",
     "CreateOrganizationalUnitRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateAccountResponseTypeDef",
     "CreateGovCloudAccountResponseTypeDef",
     "DescribeCreateAccountStatusResponseTypeDef",
     "ListCreateAccountStatusResponseTypeDef",
     "CreateOrganizationalUnitResponseTypeDef",
@@ -144,15 +143,14 @@
     "ListRootsRequestListRootsPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
     "ListParentsResponseTypeDef",
     "ListPoliciesForTargetResponseTypeDef",
     "ListPoliciesResponseTypeDef",
     "PolicyTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTargetsForPolicyResponseTypeDef",
     "OrganizationTypeDef",
     "RootTypeDef",
     "ResourcePolicyTypeDef",
     "AcceptHandshakeResponseTypeDef",
     "CancelHandshakeResponseTypeDef",
     "DeclineHandshakeResponseTypeDef",
@@ -448,22 +446,14 @@
     {
         "ActionType": ActionTypeType,
         "ParentHandshakeId": str,
     },
     total=False,
 )
 
-HandshakePartyOutputTypeDef = TypedDict(
-    "HandshakePartyOutputTypeDef",
-    {
-        "Id": str,
-        "Type": HandshakePartyTypeType,
-    },
-)
-
 HandshakePartyTypeDef = TypedDict(
     "HandshakePartyTypeDef",
     {
         "Id": str,
         "Type": HandshakePartyTypeType,
     },
 )
@@ -719,22 +709,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredListTargetsForPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsForPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalListTargetsForPolicyRequestRequestTypeDef = TypedDict(
@@ -980,14 +962,23 @@
 )
 
 class CreatePolicyRequestRequestTypeDef(
     _RequiredCreatePolicyRequestRequestTypeDef, _OptionalCreatePolicyRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "Content": str,
     },
 )
 _OptionalPutResourcePolicyRequestRequestTypeDef = TypedDict(
@@ -1133,15 +1124,15 @@
 )
 
 HandshakeTypeDef = TypedDict(
     "HandshakeTypeDef",
     {
         "Id": str,
         "Arn": str,
-        "Parties": List[HandshakePartyOutputTypeDef],
+        "Parties": List[HandshakePartyTypeDef],
         "State": HandshakeStateType,
         "RequestedTimestamp": datetime,
         "ExpirationTimestamp": datetime,
         "Action": ActionTypeType,
         "Resources": List["HandshakeResourceTypeDef"],
     },
     total=False,
@@ -1442,23 +1433,14 @@
     {
         "PolicySummary": PolicySummaryTypeDef,
         "Content": str,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTargetsForPolicyResponseTypeDef = TypedDict(
     "ListTargetsForPolicyResponseTypeDef",
     {
         "Targets": List[PolicyTargetSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations.egg-info/PKG-INFO` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-organizations
-Version: 1.28.12
-Summary: Type annotations for boto3.Organizations 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Organizations 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_organizations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-organizations.svg?color=blue)](https://pypi.org/project/mypy-boto3-organizations)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_organizations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-organizations)](https://pepy.tech/project/mypy-boto3-organizations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Organizations 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
+[boto3.Organizations 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
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
 [mypy-boto3-organizations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_organizations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -434,15 +434,14 @@
     DetachPolicyRequestRequestTypeDef,
     DisableAWSServiceAccessRequestRequestTypeDef,
     DisablePolicyTypeRequestRequestTypeDef,
     EnableAWSServiceAccessRequestRequestTypeDef,
     EnablePolicyTypeRequestRequestTypeDef,
     EnabledServicePrincipalTypeDef,
     HandshakeFilterTypeDef,
-    HandshakePartyOutputTypeDef,
     HandshakePartyTypeDef,
     HandshakeResourceTypeDef,
     PaginatorConfigTypeDef,
     ListAWSServiceAccessForOrganizationRequestRequestTypeDef,
     ListAccountsForParentRequestRequestTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListChildrenRequestRequestTypeDef,
@@ -453,15 +452,14 @@
     ListParentsRequestRequestTypeDef,
     ParentTypeDef,
     ListPoliciesForTargetRequestRequestTypeDef,
     PolicySummaryTypeDef,
     ListPoliciesRequestRequestTypeDef,
     ListRootsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListTargetsForPolicyRequestRequestTypeDef,
     PolicyTargetSummaryTypeDef,
     MoveAccountRequestRequestTypeDef,
     PolicyTypeSummaryTypeDef,
     RegisterDelegatedAdministratorRequestRequestTypeDef,
     RemoveAccountFromOrganizationRequestRequestTypeDef,
     ResourcePolicySummaryTypeDef,
@@ -473,14 +471,15 @@
     ListAccountsForParentResponseTypeDef,
     ListAccountsResponseTypeDef,
     ListChildrenResponseTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateGovCloudAccountRequestRequestTypeDef,
     CreateOrganizationalUnitRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateAccountResponseTypeDef,
     CreateGovCloudAccountResponseTypeDef,
     DescribeCreateAccountStatusResponseTypeDef,
     ListCreateAccountStatusResponseTypeDef,
     CreateOrganizationalUnitResponseTypeDef,
@@ -511,15 +510,14 @@
     ListRootsRequestListRootsPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
     ListParentsResponseTypeDef,
     ListPoliciesForTargetResponseTypeDef,
     ListPoliciesResponseTypeDef,
     PolicyTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTargetsForPolicyResponseTypeDef,
     OrganizationTypeDef,
     RootTypeDef,
     ResourcePolicyTypeDef,
     AcceptHandshakeResponseTypeDef,
     CancelHandshakeResponseTypeDef,
     DeclineHandshakeResponseTypeDef,
```

### Comparing `mypy-boto3-organizations-1.28.12/mypy_boto3_organizations.egg-info/SOURCES.txt` & `mypy-boto3-organizations-1.28.15/mypy_boto3_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-organizations-1.28.12/setup.py` & `mypy-boto3-organizations-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-organizations",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_organizations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Organizations 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Organizations 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

