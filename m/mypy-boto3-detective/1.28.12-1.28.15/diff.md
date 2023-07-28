# Comparing `tmp/mypy-boto3-detective-1.28.12.tar.gz` & `tmp/mypy-boto3-detective-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-detective-1.28.12.tar", last modified: Thu Jul 27 05:34:33 2023, max compression
+gzip compressed data, was "mypy-boto3-detective-1.28.15.tar", last modified: Fri Jul 28 20:42:37 2023, max compression
```

## Comparing `mypy-boto3-detective-1.28.12.tar` & `mypy-boto3-detective-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.800535 mypy-boto3-detective-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-07-27 05:34:33.800535 mypy-boto3-detective-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.796535 mypy-boto3-detective-1.28.12/mypy_boto3_detective/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16651 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.800535 mypy-boto3-detective-1.28.12/mypy_boto3_detective.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-07-27 05:34:33.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 05:34:33.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:33.000000 mypy-boto3-detective-1.28.12/mypy_boto3_detective.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:33.800535 mypy-boto3-detective-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:20:06.000000 mypy-boto3-detective-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.700956 mypy-boto3-detective-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:43.000000 mypy-boto3-detective-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-07-28 20:42:37.700956 mypy-boto3-detective-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-07-28 20:22:43.000000 mypy-boto3-detective-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.684956 mypy-boto3-detective-1.28.15/mypy_boto3_detective/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-28 20:22:43.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-28 20:22:43.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:22:43.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16651 2023-07-28 20:22:44.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-28 20:22:44.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-07-28 20:22:44.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-28 20:22:44.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:43.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14268 2023-07-28 20:22:44.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-07-28 20:22:44.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:43.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.700956 mypy-boto3-detective-1.28.15/mypy_boto3_detective.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-07-28 20:42:37.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-28 20:42:37.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:37.000000 mypy-boto3-detective-1.28.15/mypy_boto3_detective.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:37.700956 mypy-boto3-detective-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:22:43.000000 mypy-boto3-detective-1.28.15/setup.py
```

### Comparing `mypy-boto3-detective-1.28.12/LICENSE` & `mypy-boto3-detective-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-detective-1.28.12/PKG-INFO` & `mypy-boto3-detective-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-detective
-Version: 1.28.12
-Summary: Type annotations for boto3.Detective 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Detective 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-detective.svg?color=blue)](https://pypi.org/project/mypy-boto3-detective)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-detective)](https://pepy.tech/project/mypy-boto3-detective)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Detective 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
+[boto3.Detective 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
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
 [mypy-boto3-detective docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,46 +304,46 @@
 
 ```python
 from mypy_boto3_detective.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccountTypeDef,
     AdministratorTypeDef,
     BatchGetGraphMemberDatasourcesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedAccountTypeDef,
     BatchGetMembershipDatasourcesRequestRequestTypeDef,
     UnprocessedGraphTypeDef,
     CreateGraphRequestRequestTypeDef,
-    CreateGraphResponseTypeDef,
     TimestampForCollectionTypeDef,
     DatasourcePackageUsageInfoTypeDef,
     DeleteGraphRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
     DisassociateMembershipRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     GraphTypeDef,
     ListDatasourcePackagesRequestRequestTypeDef,
     ListGraphsRequestRequestTypeDef,
     ListInvitationsRequestRequestTypeDef,
     ListMembersRequestRequestTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RejectInvitationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartMonitoringMemberRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasourcePackagesRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
+    CreateGraphResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DatasourcePackageIngestDetailTypeDef,
     MembershipDatasourcesTypeDef,
     MemberDetailTypeDef,
     ListGraphsResponseTypeDef,
     ListDatasourcePackagesResponseTypeDef,
     BatchGetGraphMemberDatasourcesResponseTypeDef,
```

### Comparing `mypy-boto3-detective-1.28.12/README.md` & `mypy-boto3-detective-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-detective.svg?color=blue)](https://pypi.org/project/mypy-boto3-detective)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-detective)](https://pepy.tech/project/mypy-boto3-detective)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Detective 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
+[boto3.Detective 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
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
 [mypy-boto3-detective docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,46 +272,46 @@
 
 ```python
 from mypy_boto3_detective.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccountTypeDef,
     AdministratorTypeDef,
     BatchGetGraphMemberDatasourcesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedAccountTypeDef,
     BatchGetMembershipDatasourcesRequestRequestTypeDef,
     UnprocessedGraphTypeDef,
     CreateGraphRequestRequestTypeDef,
-    CreateGraphResponseTypeDef,
     TimestampForCollectionTypeDef,
     DatasourcePackageUsageInfoTypeDef,
     DeleteGraphRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
     DisassociateMembershipRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     GraphTypeDef,
     ListDatasourcePackagesRequestRequestTypeDef,
     ListGraphsRequestRequestTypeDef,
     ListInvitationsRequestRequestTypeDef,
     ListMembersRequestRequestTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RejectInvitationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartMonitoringMemberRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasourcePackagesRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
+    CreateGraphResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DatasourcePackageIngestDetailTypeDef,
     MembershipDatasourcesTypeDef,
     MemberDetailTypeDef,
     ListGraphsResponseTypeDef,
     ListDatasourcePackagesResponseTypeDef,
     BatchGetGraphMemberDatasourcesResponseTypeDef,
```

### Comparing `mypy-boto3-detective-1.28.12/mypy_boto3_detective/__main__.py` & `mypy-boto3-detective-1.28.15/mypy_boto3_detective/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Detective 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Detective 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective\nOther"
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

### Comparing `mypy-boto3-detective-1.28.12/mypy_boto3_detective/client.py` & `mypy-boto3-detective-1.28.15/mypy_boto3_detective/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-detective-1.28.12/mypy_boto3_detective/client.pyi` & `mypy-boto3-detective-1.28.15/mypy_boto3_detective/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-detective-1.28.12/mypy_boto3_detective/literals.py` & `mypy-boto3-detective-1.28.15/mypy_boto3_detective/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-detective-1.28.12/mypy_boto3_detective/literals.pyi` & `mypy-boto3-detective-1.28.15/mypy_boto3_detective/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-detective-1.28.12/mypy_boto3_detective/type_defs.py` & `mypy-boto3-detective-1.28.15/mypy_boto3_detective/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,52 +24,51 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptInvitationRequestRequestTypeDef",
     "AccountTypeDef",
     "AdministratorTypeDef",
     "BatchGetGraphMemberDatasourcesRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedAccountTypeDef",
     "BatchGetMembershipDatasourcesRequestRequestTypeDef",
     "UnprocessedGraphTypeDef",
     "CreateGraphRequestRequestTypeDef",
-    "CreateGraphResponseTypeDef",
     "TimestampForCollectionTypeDef",
     "DatasourcePackageUsageInfoTypeDef",
     "DeleteGraphRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
     "DescribeOrganizationConfigurationRequestRequestTypeDef",
-    "DescribeOrganizationConfigurationResponseTypeDef",
     "DisassociateMembershipRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "GetMembersRequestRequestTypeDef",
     "GraphTypeDef",
     "ListDatasourcePackagesRequestRequestTypeDef",
     "ListGraphsRequestRequestTypeDef",
     "ListInvitationsRequestRequestTypeDef",
     "ListMembersRequestRequestTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RejectInvitationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartMonitoringMemberRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasourcePackagesRequestRequestTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "CreateMembersRequestRequestTypeDef",
+    "CreateGraphResponseTypeDef",
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListOrganizationAdminAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "DatasourcePackageIngestDetailTypeDef",
     "MembershipDatasourcesTypeDef",
     "MemberDetailTypeDef",
     "ListGraphsResponseTypeDef",
     "ListDatasourcePackagesResponseTypeDef",
     "BatchGetGraphMemberDatasourcesResponseTypeDef",
@@ -109,14 +108,25 @@
     "BatchGetGraphMemberDatasourcesRequestRequestTypeDef",
     {
         "GraphArn": str,
         "AccountIds": Sequence[str],
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
 UnprocessedAccountTypeDef = TypedDict(
     "UnprocessedAccountTypeDef",
     {
         "AccountId": str,
         "Reason": str,
     },
     total=False,
@@ -142,22 +152,14 @@
     "CreateGraphRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateGraphResponseTypeDef = TypedDict(
-    "CreateGraphResponseTypeDef",
-    {
-        "GraphArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TimestampForCollectionTypeDef = TypedDict(
     "TimestampForCollectionTypeDef",
     {
         "Timestamp": datetime,
     },
     total=False,
 )
@@ -189,36 +191,21 @@
 DescribeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConfigurationRequestRequestTypeDef",
     {
         "GraphArn": str,
     },
 )
 
-DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
-    "DescribeOrganizationConfigurationResponseTypeDef",
-    {
-        "AutoEnable": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateMembershipRequestRequestTypeDef = TypedDict(
     "DisassociateMembershipRequestRequestTypeDef",
     {
         "GraphArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 
@@ -250,22 +237,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDatasourcePackagesRequestRequestTypeDef(
     _RequiredListDatasourcePackagesRequestRequestTypeDef,
     _OptionalListDatasourcePackagesRequestRequestTypeDef,
 ):
     pass
 
-
 ListGraphsRequestRequestTypeDef = TypedDict(
     "ListGraphsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -291,21 +276,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListMembersRequestRequestTypeDef(
     _RequiredListMembersRequestRequestTypeDef, _OptionalListMembersRequestRequestTypeDef
 ):
     pass
 
-
 ListOrganizationAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -314,40 +297,21 @@
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
 RejectInvitationRequestRequestTypeDef = TypedDict(
     "RejectInvitationRequestRequestTypeDef",
     {
         "GraphArn": str,
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
 StartMonitoringMemberRequestRequestTypeDef = TypedDict(
     "StartMonitoringMemberRequestRequestTypeDef",
     {
         "GraphArn": str,
         "AccountId": str,
     },
 )
@@ -386,22 +350,20 @@
     "_OptionalUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "AutoEnable": bool,
     },
     total=False,
 )
 
-
 class UpdateOrganizationConfigurationRequestRequestTypeDef(
     _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef,
     _OptionalUpdateOrganizationConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateMembersRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMembersRequestRequestTypeDef",
     {
         "GraphArn": str,
         "Accounts": Sequence[AccountTypeDef],
     },
 )
@@ -410,36 +372,65 @@
     {
         "Message": str,
         "DisableEmailNotification": bool,
     },
     total=False,
 )
 
-
 class CreateMembersRequestRequestTypeDef(
     _RequiredCreateMembersRequestRequestTypeDef, _OptionalCreateMembersRequestRequestTypeDef
 ):
     pass
 
+CreateGraphResponseTypeDef = TypedDict(
+    "CreateGraphResponseTypeDef",
+    {
+        "GraphArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    {
+        "AutoEnable": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
     "ListOrganizationAdminAccountsResponseTypeDef",
     {
         "Administrators": List[AdministratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMembersResponseTypeDef = TypedDict(
     "DeleteMembersResponseTypeDef",
     {
         "AccountIds": List[str],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasourcePackageIngestDetailTypeDef = TypedDict(
     "DatasourcePackageIngestDetailTypeDef",
     {
         "DatasourcePackageIngestState": DatasourcePackageIngestStateType,
@@ -491,73 +482,73 @@
 )
 
 ListGraphsResponseTypeDef = TypedDict(
     "ListGraphsResponseTypeDef",
     {
         "GraphList": List[GraphTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasourcePackagesResponseTypeDef = TypedDict(
     "ListDatasourcePackagesResponseTypeDef",
     {
         "DatasourcePackages": Dict[DatasourcePackageType, DatasourcePackageIngestDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetGraphMemberDatasourcesResponseTypeDef = TypedDict(
     "BatchGetGraphMemberDatasourcesResponseTypeDef",
     {
         "MemberDatasources": List[MembershipDatasourcesTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetMembershipDatasourcesResponseTypeDef = TypedDict(
     "BatchGetMembershipDatasourcesResponseTypeDef",
     {
         "MembershipDatasources": List[MembershipDatasourcesTypeDef],
         "UnprocessedGraphs": List[UnprocessedGraphTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMembersResponseTypeDef = TypedDict(
     "CreateMembersResponseTypeDef",
     {
         "Members": List[MemberDetailTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "MemberDetails": List[MemberDetailTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "Invitations": List[MemberDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "MemberDetails": List[MemberDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-detective-1.28.12/mypy_boto3_detective/type_defs.pyi` & `mypy-boto3-detective-1.28.15/mypy_boto3_detective/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,51 +24,52 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptInvitationRequestRequestTypeDef",
     "AccountTypeDef",
     "AdministratorTypeDef",
     "BatchGetGraphMemberDatasourcesRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedAccountTypeDef",
     "BatchGetMembershipDatasourcesRequestRequestTypeDef",
     "UnprocessedGraphTypeDef",
     "CreateGraphRequestRequestTypeDef",
-    "CreateGraphResponseTypeDef",
     "TimestampForCollectionTypeDef",
     "DatasourcePackageUsageInfoTypeDef",
     "DeleteGraphRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
     "DescribeOrganizationConfigurationRequestRequestTypeDef",
-    "DescribeOrganizationConfigurationResponseTypeDef",
     "DisassociateMembershipRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "GetMembersRequestRequestTypeDef",
     "GraphTypeDef",
     "ListDatasourcePackagesRequestRequestTypeDef",
     "ListGraphsRequestRequestTypeDef",
     "ListInvitationsRequestRequestTypeDef",
     "ListMembersRequestRequestTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RejectInvitationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartMonitoringMemberRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasourcePackagesRequestRequestTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "CreateMembersRequestRequestTypeDef",
+    "CreateGraphResponseTypeDef",
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListOrganizationAdminAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "DatasourcePackageIngestDetailTypeDef",
     "MembershipDatasourcesTypeDef",
     "MemberDetailTypeDef",
     "ListGraphsResponseTypeDef",
     "ListDatasourcePackagesResponseTypeDef",
     "BatchGetGraphMemberDatasourcesResponseTypeDef",
@@ -108,14 +109,25 @@
     "BatchGetGraphMemberDatasourcesRequestRequestTypeDef",
     {
         "GraphArn": str,
         "AccountIds": Sequence[str],
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
 UnprocessedAccountTypeDef = TypedDict(
     "UnprocessedAccountTypeDef",
     {
         "AccountId": str,
         "Reason": str,
     },
     total=False,
@@ -141,22 +153,14 @@
     "CreateGraphRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateGraphResponseTypeDef = TypedDict(
-    "CreateGraphResponseTypeDef",
-    {
-        "GraphArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TimestampForCollectionTypeDef = TypedDict(
     "TimestampForCollectionTypeDef",
     {
         "Timestamp": datetime,
     },
     total=False,
 )
@@ -188,36 +192,21 @@
 DescribeOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConfigurationRequestRequestTypeDef",
     {
         "GraphArn": str,
     },
 )
 
-DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
-    "DescribeOrganizationConfigurationResponseTypeDef",
-    {
-        "AutoEnable": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateMembershipRequestRequestTypeDef = TypedDict(
     "DisassociateMembershipRequestRequestTypeDef",
     {
         "GraphArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 
@@ -249,20 +238,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDatasourcePackagesRequestRequestTypeDef(
     _RequiredListDatasourcePackagesRequestRequestTypeDef,
     _OptionalListDatasourcePackagesRequestRequestTypeDef,
 ):
     pass
 
+
 ListGraphsRequestRequestTypeDef = TypedDict(
     "ListGraphsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -288,19 +279,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListMembersRequestRequestTypeDef(
     _RequiredListMembersRequestRequestTypeDef, _OptionalListMembersRequestRequestTypeDef
 ):
     pass
 
+
 ListOrganizationAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -309,40 +302,21 @@
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
 RejectInvitationRequestRequestTypeDef = TypedDict(
     "RejectInvitationRequestRequestTypeDef",
     {
         "GraphArn": str,
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
 StartMonitoringMemberRequestRequestTypeDef = TypedDict(
     "StartMonitoringMemberRequestRequestTypeDef",
     {
         "GraphArn": str,
         "AccountId": str,
     },
 )
@@ -381,20 +355,22 @@
     "_OptionalUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "AutoEnable": bool,
     },
     total=False,
 )
 
+
 class UpdateOrganizationConfigurationRequestRequestTypeDef(
     _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef,
     _OptionalUpdateOrganizationConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateMembersRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMembersRequestRequestTypeDef",
     {
         "GraphArn": str,
         "Accounts": Sequence[AccountTypeDef],
     },
 )
@@ -403,34 +379,67 @@
     {
         "Message": str,
         "DisableEmailNotification": bool,
     },
     total=False,
 )
 
+
 class CreateMembersRequestRequestTypeDef(
     _RequiredCreateMembersRequestRequestTypeDef, _OptionalCreateMembersRequestRequestTypeDef
 ):
     pass
 
+
+CreateGraphResponseTypeDef = TypedDict(
+    "CreateGraphResponseTypeDef",
+    {
+        "GraphArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    {
+        "AutoEnable": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
     "ListOrganizationAdminAccountsResponseTypeDef",
     {
         "Administrators": List[AdministratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMembersResponseTypeDef = TypedDict(
     "DeleteMembersResponseTypeDef",
     {
         "AccountIds": List[str],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasourcePackageIngestDetailTypeDef = TypedDict(
     "DatasourcePackageIngestDetailTypeDef",
     {
         "DatasourcePackageIngestState": DatasourcePackageIngestStateType,
@@ -482,73 +491,73 @@
 )
 
 ListGraphsResponseTypeDef = TypedDict(
     "ListGraphsResponseTypeDef",
     {
         "GraphList": List[GraphTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasourcePackagesResponseTypeDef = TypedDict(
     "ListDatasourcePackagesResponseTypeDef",
     {
         "DatasourcePackages": Dict[DatasourcePackageType, DatasourcePackageIngestDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetGraphMemberDatasourcesResponseTypeDef = TypedDict(
     "BatchGetGraphMemberDatasourcesResponseTypeDef",
     {
         "MemberDatasources": List[MembershipDatasourcesTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetMembershipDatasourcesResponseTypeDef = TypedDict(
     "BatchGetMembershipDatasourcesResponseTypeDef",
     {
         "MembershipDatasources": List[MembershipDatasourcesTypeDef],
         "UnprocessedGraphs": List[UnprocessedGraphTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMembersResponseTypeDef = TypedDict(
     "CreateMembersResponseTypeDef",
     {
         "Members": List[MemberDetailTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "MemberDetails": List[MemberDetailTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "Invitations": List[MemberDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "MemberDetails": List[MemberDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-detective-1.28.12/mypy_boto3_detective.egg-info/PKG-INFO` & `mypy-boto3-detective-1.28.15/mypy_boto3_detective.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-detective
-Version: 1.28.12
-Summary: Type annotations for boto3.Detective 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Detective 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-detective.svg?color=blue)](https://pypi.org/project/mypy-boto3-detective)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-detective)](https://pepy.tech/project/mypy-boto3-detective)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Detective 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
+[boto3.Detective 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
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
 [mypy-boto3-detective docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_detective/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,46 +304,46 @@
 
 ```python
 from mypy_boto3_detective.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccountTypeDef,
     AdministratorTypeDef,
     BatchGetGraphMemberDatasourcesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedAccountTypeDef,
     BatchGetMembershipDatasourcesRequestRequestTypeDef,
     UnprocessedGraphTypeDef,
     CreateGraphRequestRequestTypeDef,
-    CreateGraphResponseTypeDef,
     TimestampForCollectionTypeDef,
     DatasourcePackageUsageInfoTypeDef,
     DeleteGraphRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
     DisassociateMembershipRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     GraphTypeDef,
     ListDatasourcePackagesRequestRequestTypeDef,
     ListGraphsRequestRequestTypeDef,
     ListInvitationsRequestRequestTypeDef,
     ListMembersRequestRequestTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RejectInvitationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartMonitoringMemberRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasourcePackagesRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
+    CreateGraphResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DatasourcePackageIngestDetailTypeDef,
     MembershipDatasourcesTypeDef,
     MemberDetailTypeDef,
     ListGraphsResponseTypeDef,
     ListDatasourcePackagesResponseTypeDef,
     BatchGetGraphMemberDatasourcesResponseTypeDef,
```

### Comparing `mypy-boto3-detective-1.28.12/mypy_boto3_detective.egg-info/SOURCES.txt` & `mypy-boto3-detective-1.28.15/mypy_boto3_detective.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-detective-1.28.12/setup.py` & `mypy-boto3-detective-1.28.15/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-detective",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_detective"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Detective 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Detective 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

