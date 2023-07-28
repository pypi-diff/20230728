# Comparing `tmp/mypy-boto3-codestar-1.28.12.tar.gz` & `tmp/mypy-boto3-codestar-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codestar-1.28.12.tar", last modified: Thu Jul 27 05:34:29 2023, max compression
+gzip compressed data, was "mypy-boto3-codestar-1.28.15.tar", last modified: Fri Jul 28 20:42:31 2023, max compression
```

## Comparing `mypy-boto3-codestar-1.28.12.tar` & `mypy-boto3-codestar-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.412549 mypy-boto3-codestar-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-07-27 05:34:29.408549 mypy-boto3-codestar-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.408549 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15728 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-27 05:19:14.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18008 2023-07-27 05:19:14.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17976 2023-07-27 05:19:14.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.408549 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-07-27 05:34:29.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:34:29.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:29.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:29.000000 mypy-boto3-codestar-1.28.12/mypy_boto3_codestar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:29.412549 mypy-boto3-codestar-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:19:13.000000 mypy-boto3-codestar-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.632868 mypy-boto3-codestar-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:21:42.000000 mypy-boto3-codestar-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-07-28 20:42:31.624868 mypy-boto3-codestar-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-28 20:21:42.000000 mypy-boto3-codestar-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.616868 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-28 20:21:43.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-28 20:21:43.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:21:43.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15728 2023-07-28 20:21:43.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-28 20:21:43.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-28 20:21:43.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-28 20:21:43.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-28 20:21:43.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-28 20:21:43.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:21:43.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-07-28 20:21:43.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17938 2023-07-28 20:21:43.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:21:42.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:31.624868 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-07-28 20:42:31.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:42:31.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:31.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:31.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:42:31.000000 mypy-boto3-codestar-1.28.15/mypy_boto3_codestar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:31.632868 mypy-boto3-codestar-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:21:42.000000 mypy-boto3-codestar-1.28.15/setup.py
```

### Comparing `mypy-boto3-codestar-1.28.12/LICENSE` & `mypy-boto3-codestar-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.28.12/PKG-INFO` & `mypy-boto3-codestar-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeStar 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeStar 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar)](https://pepy.tech/project/mypy-boto3-codestar)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStar 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
+[boto3.CodeStar 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
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
 [mypy-boto3-codestar docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,58 +330,58 @@
 
 `mypy_boto3_codestar.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar.type_defs import (
     AssociateTeamMemberRequestRequestTypeDef,
-    AssociateTeamMemberResultTypeDef,
+    ResponseMetadataTypeDef,
     CodeCommitCodeDestinationTypeDef,
     GitHubCodeDestinationTypeDef,
     S3LocationTypeDef,
-    CreateProjectResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
-    CreateUserProfileResultTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResultTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
-    DeleteUserProfileResultTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ProjectStatusTypeDef,
     DescribeUserProfileRequestRequestTypeDef,
-    DescribeUserProfileResultTypeDef,
     DisassociateTeamMemberRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForProjectRequestRequestTypeDef,
-    ListTagsForProjectResultTypeDef,
-    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
     ListTeamMembersRequestRequestTypeDef,
     TeamMemberTypeDef,
-    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListUserProfilesRequestRequestTypeDef,
     UserProfileSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagProjectRequestRequestTypeDef,
-    TagProjectResultTypeDef,
     UntagProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     UpdateTeamMemberRequestRequestTypeDef,
-    UpdateTeamMemberResultTypeDef,
     UpdateUserProfileRequestRequestTypeDef,
+    AssociateTeamMemberResultTypeDef,
+    CreateProjectResultTypeDef,
+    CreateUserProfileResultTypeDef,
+    DeleteProjectResultTypeDef,
+    DeleteUserProfileResultTypeDef,
+    DescribeUserProfileResultTypeDef,
+    ListTagsForProjectResultTypeDef,
+    TagProjectResultTypeDef,
+    UpdateTeamMemberResultTypeDef,
     UpdateUserProfileResultTypeDef,
     CodeDestinationTypeDef,
     CodeSourceTypeDef,
     ToolchainSourceTypeDef,
     DescribeProjectResultTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
+    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
+    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListProjectsResultTypeDef,
     ListResourcesResultTypeDef,
     ListTeamMembersResultTypeDef,
     ListUserProfilesResultTypeDef,
     CodeTypeDef,
     ToolchainTypeDef,
     CreateProjectRequestRequestTypeDef,
```

### Comparing `mypy-boto3-codestar-1.28.12/README.md` & `mypy-boto3-codestar-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar)](https://pepy.tech/project/mypy-boto3-codestar)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStar 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
+[boto3.CodeStar 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
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
 [mypy-boto3-codestar docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,58 +298,58 @@
 
 `mypy_boto3_codestar.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar.type_defs import (
     AssociateTeamMemberRequestRequestTypeDef,
-    AssociateTeamMemberResultTypeDef,
+    ResponseMetadataTypeDef,
     CodeCommitCodeDestinationTypeDef,
     GitHubCodeDestinationTypeDef,
     S3LocationTypeDef,
-    CreateProjectResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
-    CreateUserProfileResultTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResultTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
-    DeleteUserProfileResultTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ProjectStatusTypeDef,
     DescribeUserProfileRequestRequestTypeDef,
-    DescribeUserProfileResultTypeDef,
     DisassociateTeamMemberRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForProjectRequestRequestTypeDef,
-    ListTagsForProjectResultTypeDef,
-    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
     ListTeamMembersRequestRequestTypeDef,
     TeamMemberTypeDef,
-    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListUserProfilesRequestRequestTypeDef,
     UserProfileSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagProjectRequestRequestTypeDef,
-    TagProjectResultTypeDef,
     UntagProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     UpdateTeamMemberRequestRequestTypeDef,
-    UpdateTeamMemberResultTypeDef,
     UpdateUserProfileRequestRequestTypeDef,
+    AssociateTeamMemberResultTypeDef,
+    CreateProjectResultTypeDef,
+    CreateUserProfileResultTypeDef,
+    DeleteProjectResultTypeDef,
+    DeleteUserProfileResultTypeDef,
+    DescribeUserProfileResultTypeDef,
+    ListTagsForProjectResultTypeDef,
+    TagProjectResultTypeDef,
+    UpdateTeamMemberResultTypeDef,
     UpdateUserProfileResultTypeDef,
     CodeDestinationTypeDef,
     CodeSourceTypeDef,
     ToolchainSourceTypeDef,
     DescribeProjectResultTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
+    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
+    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListProjectsResultTypeDef,
     ListResourcesResultTypeDef,
     ListTeamMembersResultTypeDef,
     ListUserProfilesResultTypeDef,
     CodeTypeDef,
     ToolchainTypeDef,
     CreateProjectRequestRequestTypeDef,
```

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/__init__.py` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/__init__.pyi` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/__main__.py` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeStar 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.CodeStar 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar\nOther"
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

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/client.py` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/client.pyi` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/literals.py` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/literals.pyi` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/paginator.py` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,76 +40,70 @@
 __all__ = (
     "ListProjectsPaginator",
     "ListResourcesPaginator",
     "ListTeamMembersPaginator",
     "ListUserProfilesPaginator",
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
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listprojectspaginator)
         """
 
-
 class ListResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listresourcespaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listresourcespaginator)
         """
 
-
 class ListTeamMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listteammemberspaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTeamMembersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listteammemberspaginator)
         """
 
-
 class ListUserProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listuserprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUserProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listuserprofilespaginator)
         """
```

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/paginator.pyi` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,70 +40,76 @@
 __all__ = (
     "ListProjectsPaginator",
     "ListResourcesPaginator",
     "ListTeamMembersPaginator",
     "ListUserProfilesPaginator",
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
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listprojectspaginator)
         """
 
+
 class ListResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listresourcespaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listresourcespaginator)
         """
 
+
 class ListTeamMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listteammemberspaginator)
     """
 
     def paginate(
-        self, *, projectId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTeamMembersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListTeamMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listteammemberspaginator)
         """
 
+
 class ListUserProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listuserprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUserProfilesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar.Paginator.ListUserProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/paginators/#listuserprofilespaginator)
         """
```

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/type_defs.py` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,58 +19,58 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateTeamMemberRequestRequestTypeDef",
-    "AssociateTeamMemberResultTypeDef",
+    "ResponseMetadataTypeDef",
     "CodeCommitCodeDestinationTypeDef",
     "GitHubCodeDestinationTypeDef",
     "S3LocationTypeDef",
-    "CreateProjectResultTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
-    "CreateUserProfileResultTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResultTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
-    "DeleteUserProfileResultTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "ProjectStatusTypeDef",
     "DescribeUserProfileRequestRequestTypeDef",
-    "DescribeUserProfileResultTypeDef",
     "DisassociateTeamMemberRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
-    "ListResourcesRequestListResourcesPaginateTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListTagsForProjectRequestRequestTypeDef",
-    "ListTagsForProjectResultTypeDef",
-    "ListTeamMembersRequestListTeamMembersPaginateTypeDef",
     "ListTeamMembersRequestRequestTypeDef",
     "TeamMemberTypeDef",
-    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
     "ListUserProfilesRequestRequestTypeDef",
     "UserProfileSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagProjectRequestRequestTypeDef",
-    "TagProjectResultTypeDef",
     "UntagProjectRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "UpdateTeamMemberRequestRequestTypeDef",
-    "UpdateTeamMemberResultTypeDef",
     "UpdateUserProfileRequestRequestTypeDef",
+    "AssociateTeamMemberResultTypeDef",
+    "CreateProjectResultTypeDef",
+    "CreateUserProfileResultTypeDef",
+    "DeleteProjectResultTypeDef",
+    "DeleteUserProfileResultTypeDef",
+    "DescribeUserProfileResultTypeDef",
+    "ListTagsForProjectResultTypeDef",
+    "TagProjectResultTypeDef",
+    "UpdateTeamMemberResultTypeDef",
     "UpdateUserProfileResultTypeDef",
     "CodeDestinationTypeDef",
     "CodeSourceTypeDef",
     "ToolchainSourceTypeDef",
     "DescribeProjectResultTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListResourcesRequestListResourcesPaginateTypeDef",
+    "ListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
     "ListProjectsResultTypeDef",
     "ListResourcesResultTypeDef",
     "ListTeamMembersResultTypeDef",
     "ListUserProfilesResultTypeDef",
     "CodeTypeDef",
     "ToolchainTypeDef",
     "CreateProjectRequestRequestTypeDef",
@@ -97,19 +97,22 @@
 class AssociateTeamMemberRequestRequestTypeDef(
     _RequiredAssociateTeamMemberRequestRequestTypeDef,
     _OptionalAssociateTeamMemberRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateTeamMemberResultTypeDef = TypedDict(
-    "AssociateTeamMemberResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "clientRequestToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CodeCommitCodeDestinationTypeDef = TypedDict(
     "CodeCommitCodeDestinationTypeDef",
     {
         "name": str,
@@ -147,25 +150,14 @@
     {
         "bucketName": str,
         "bucketKey": str,
     },
     total=False,
 )
 
-CreateProjectResultTypeDef = TypedDict(
-    "CreateProjectResultTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "clientRequestToken": str,
-        "projectTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
         "displayName": str,
         "emailAddress": str,
     },
@@ -181,27 +173,14 @@
 
 class CreateUserProfileRequestRequestTypeDef(
     _RequiredCreateUserProfileRequestRequestTypeDef, _OptionalCreateUserProfileRequestRequestTypeDef
 ):
     pass
 
 
-CreateUserProfileResultTypeDef = TypedDict(
-    "CreateUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "displayName": str,
-        "emailAddress": str,
-        "sshPublicKey": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
@@ -216,38 +195,21 @@
 
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
 
-DeleteProjectResultTypeDef = TypedDict(
-    "DeleteProjectResultTypeDef",
-    {
-        "stackId": str,
-        "projectArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteUserProfileRequestRequestTypeDef = TypedDict(
     "DeleteUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 
-DeleteUserProfileResultTypeDef = TypedDict(
-    "DeleteUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -273,39 +235,28 @@
 DescribeUserProfileRequestRequestTypeDef = TypedDict(
     "DescribeUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 
-DescribeUserProfileResultTypeDef = TypedDict(
-    "DescribeUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "displayName": str,
-        "emailAddress": str,
-        "sshPublicKey": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateTeamMemberRequestRequestTypeDef = TypedDict(
     "DisassociateTeamMemberRequestRequestTypeDef",
     {
         "projectId": str,
         "userArn": str,
     },
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
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
 
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
@@ -320,36 +271,14 @@
     {
         "projectId": str,
         "projectArn": str,
     },
     total=False,
 )
 
-_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourcesRequestListResourcesPaginateTypeDef(
-    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
-    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -394,45 +323,14 @@
 class ListTagsForProjectRequestRequestTypeDef(
     _RequiredListTagsForProjectRequestRequestTypeDef,
     _OptionalListTagsForProjectRequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsForProjectResultTypeDef = TypedDict(
-    "ListTagsForProjectResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
-    "_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
-    "_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTeamMembersRequestListTeamMembersPaginateTypeDef(
-    _RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef,
-    _OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTeamMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListTeamMembersRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListTeamMembersRequestRequestTypeDef = TypedDict(
@@ -467,22 +365,14 @@
 )
 
 
 class TeamMemberTypeDef(_RequiredTeamMemberTypeDef, _OptionalTeamMemberTypeDef):
     pass
 
 
-ListUserProfilesRequestListUserProfilesPaginateTypeDef = TypedDict(
-    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListUserProfilesRequestRequestTypeDef = TypedDict(
     "ListUserProfilesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -495,51 +385,22 @@
         "displayName": str,
         "emailAddress": str,
         "sshPublicKey": str,
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
 TagProjectRequestRequestTypeDef = TypedDict(
     "TagProjectRequestRequestTypeDef",
     {
         "id": str,
         "tags": Mapping[str, str],
     },
 )
 
-TagProjectResultTypeDef = TypedDict(
-    "TagProjectResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagProjectRequestRequestTypeDef = TypedDict(
     "UntagProjectRequestRequestTypeDef",
     {
         "id": str,
         "tags": Sequence[str],
     },
 )
@@ -585,24 +446,14 @@
 
 class UpdateTeamMemberRequestRequestTypeDef(
     _RequiredUpdateTeamMemberRequestRequestTypeDef, _OptionalUpdateTeamMemberRequestRequestTypeDef
 ):
     pass
 
 
-UpdateTeamMemberResultTypeDef = TypedDict(
-    "UpdateTeamMemberResultTypeDef",
-    {
-        "userArn": str,
-        "projectRole": str,
-        "remoteAccessAllowed": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 _OptionalUpdateUserProfileRequestRequestTypeDef = TypedDict(
@@ -618,24 +469,113 @@
 
 class UpdateUserProfileRequestRequestTypeDef(
     _RequiredUpdateUserProfileRequestRequestTypeDef, _OptionalUpdateUserProfileRequestRequestTypeDef
 ):
     pass
 
 
+AssociateTeamMemberResultTypeDef = TypedDict(
+    "AssociateTeamMemberResultTypeDef",
+    {
+        "clientRequestToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectResultTypeDef = TypedDict(
+    "CreateProjectResultTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "clientRequestToken": str,
+        "projectTemplateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserProfileResultTypeDef = TypedDict(
+    "CreateUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "displayName": str,
+        "emailAddress": str,
+        "sshPublicKey": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectResultTypeDef = TypedDict(
+    "DeleteProjectResultTypeDef",
+    {
+        "stackId": str,
+        "projectArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteUserProfileResultTypeDef = TypedDict(
+    "DeleteUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUserProfileResultTypeDef = TypedDict(
+    "DescribeUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "displayName": str,
+        "emailAddress": str,
+        "sshPublicKey": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForProjectResultTypeDef = TypedDict(
+    "ListTagsForProjectResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagProjectResultTypeDef = TypedDict(
+    "TagProjectResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTeamMemberResultTypeDef = TypedDict(
+    "UpdateTeamMemberResultTypeDef",
+    {
+        "userArn": str,
+        "projectRole": str,
+        "remoteAccessAllowed": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateUserProfileResultTypeDef = TypedDict(
     "UpdateUserProfileResultTypeDef",
     {
         "userArn": str,
         "displayName": str,
         "emailAddress": str,
         "sshPublicKey": str,
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CodeDestinationTypeDef = TypedDict(
     "CodeDestinationTypeDef",
     {
         "codeCommit": CodeCommitCodeDestinationTypeDef,
@@ -666,51 +606,111 @@
         "arn": str,
         "description": str,
         "clientRequestToken": str,
         "createdTimeStamp": datetime,
         "stackId": str,
         "projectTemplateId": str,
         "status": ProjectStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourcesRequestListResourcesPaginateTypeDef(
+    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
+    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
+    "_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
+    "_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTeamMembersRequestListTeamMembersPaginateTypeDef(
+    _RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef,
+    _OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef,
+):
+    pass
+
+
+ListUserProfilesRequestListUserProfilesPaginateTypeDef = TypedDict(
+    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListProjectsResultTypeDef = TypedDict(
     "ListProjectsResultTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResultTypeDef = TypedDict(
     "ListResourcesResultTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTeamMembersResultTypeDef = TypedDict(
     "ListTeamMembersResultTypeDef",
     {
         "teamMembers": List[TeamMemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserProfilesResultTypeDef = TypedDict(
     "ListUserProfilesResultTypeDef",
     {
         "userProfiles": List[UserProfileSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CodeTypeDef = TypedDict(
     "CodeTypeDef",
     {
         "source": CodeSourceTypeDef,
```

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar/type_defs.pyi` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -18,58 +18,58 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateTeamMemberRequestRequestTypeDef",
-    "AssociateTeamMemberResultTypeDef",
+    "ResponseMetadataTypeDef",
     "CodeCommitCodeDestinationTypeDef",
     "GitHubCodeDestinationTypeDef",
     "S3LocationTypeDef",
-    "CreateProjectResultTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
-    "CreateUserProfileResultTypeDef",
     "DeleteProjectRequestRequestTypeDef",
-    "DeleteProjectResultTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
-    "DeleteUserProfileResultTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "ProjectStatusTypeDef",
     "DescribeUserProfileRequestRequestTypeDef",
-    "DescribeUserProfileResultTypeDef",
     "DisassociateTeamMemberRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
-    "ListResourcesRequestListResourcesPaginateTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListTagsForProjectRequestRequestTypeDef",
-    "ListTagsForProjectResultTypeDef",
-    "ListTeamMembersRequestListTeamMembersPaginateTypeDef",
     "ListTeamMembersRequestRequestTypeDef",
     "TeamMemberTypeDef",
-    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
     "ListUserProfilesRequestRequestTypeDef",
     "UserProfileSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagProjectRequestRequestTypeDef",
-    "TagProjectResultTypeDef",
     "UntagProjectRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "UpdateTeamMemberRequestRequestTypeDef",
-    "UpdateTeamMemberResultTypeDef",
     "UpdateUserProfileRequestRequestTypeDef",
+    "AssociateTeamMemberResultTypeDef",
+    "CreateProjectResultTypeDef",
+    "CreateUserProfileResultTypeDef",
+    "DeleteProjectResultTypeDef",
+    "DeleteUserProfileResultTypeDef",
+    "DescribeUserProfileResultTypeDef",
+    "ListTagsForProjectResultTypeDef",
+    "TagProjectResultTypeDef",
+    "UpdateTeamMemberResultTypeDef",
     "UpdateUserProfileResultTypeDef",
     "CodeDestinationTypeDef",
     "CodeSourceTypeDef",
     "ToolchainSourceTypeDef",
     "DescribeProjectResultTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListResourcesRequestListResourcesPaginateTypeDef",
+    "ListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
     "ListProjectsResultTypeDef",
     "ListResourcesResultTypeDef",
     "ListTeamMembersResultTypeDef",
     "ListUserProfilesResultTypeDef",
     "CodeTypeDef",
     "ToolchainTypeDef",
     "CreateProjectRequestRequestTypeDef",
@@ -94,19 +94,22 @@
 
 class AssociateTeamMemberRequestRequestTypeDef(
     _RequiredAssociateTeamMemberRequestRequestTypeDef,
     _OptionalAssociateTeamMemberRequestRequestTypeDef,
 ):
     pass
 
-AssociateTeamMemberResultTypeDef = TypedDict(
-    "AssociateTeamMemberResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "clientRequestToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CodeCommitCodeDestinationTypeDef = TypedDict(
     "CodeCommitCodeDestinationTypeDef",
     {
         "name": str,
@@ -142,25 +145,14 @@
     {
         "bucketName": str,
         "bucketKey": str,
     },
     total=False,
 )
 
-CreateProjectResultTypeDef = TypedDict(
-    "CreateProjectResultTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "clientRequestToken": str,
-        "projectTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
         "displayName": str,
         "emailAddress": str,
     },
@@ -174,27 +166,14 @@
 )
 
 class CreateUserProfileRequestRequestTypeDef(
     _RequiredCreateUserProfileRequestRequestTypeDef, _OptionalCreateUserProfileRequestRequestTypeDef
 ):
     pass
 
-CreateUserProfileResultTypeDef = TypedDict(
-    "CreateUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "displayName": str,
-        "emailAddress": str,
-        "sshPublicKey": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteProjectRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProjectRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalDeleteProjectRequestRequestTypeDef = TypedDict(
@@ -207,38 +186,21 @@
 )
 
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
-DeleteProjectResultTypeDef = TypedDict(
-    "DeleteProjectResultTypeDef",
-    {
-        "stackId": str,
-        "projectArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteUserProfileRequestRequestTypeDef = TypedDict(
     "DeleteUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 
-DeleteUserProfileResultTypeDef = TypedDict(
-    "DeleteUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -262,39 +224,28 @@
 DescribeUserProfileRequestRequestTypeDef = TypedDict(
     "DescribeUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 
-DescribeUserProfileResultTypeDef = TypedDict(
-    "DescribeUserProfileResultTypeDef",
-    {
-        "userArn": str,
-        "displayName": str,
-        "emailAddress": str,
-        "sshPublicKey": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateTeamMemberRequestRequestTypeDef = TypedDict(
     "DisassociateTeamMemberRequestRequestTypeDef",
     {
         "projectId": str,
         "userArn": str,
     },
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
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
 
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
@@ -309,34 +260,14 @@
     {
         "projectId": str,
         "projectArn": str,
     },
     total=False,
 )
 
-_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourcesRequestListResourcesPaginateTypeDef(
-    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
-    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -377,43 +308,14 @@
 
 class ListTagsForProjectRequestRequestTypeDef(
     _RequiredListTagsForProjectRequestRequestTypeDef,
     _OptionalListTagsForProjectRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForProjectResultTypeDef = TypedDict(
-    "ListTagsForProjectResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
-    "_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    {
-        "projectId": str,
-    },
-)
-_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
-    "_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTeamMembersRequestListTeamMembersPaginateTypeDef(
-    _RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef,
-    _OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef,
-):
-    pass
-
 _RequiredListTeamMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListTeamMembersRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalListTeamMembersRequestRequestTypeDef = TypedDict(
@@ -444,22 +346,14 @@
     },
     total=False,
 )
 
 class TeamMemberTypeDef(_RequiredTeamMemberTypeDef, _OptionalTeamMemberTypeDef):
     pass
 
-ListUserProfilesRequestListUserProfilesPaginateTypeDef = TypedDict(
-    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListUserProfilesRequestRequestTypeDef = TypedDict(
     "ListUserProfilesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -472,51 +366,22 @@
         "displayName": str,
         "emailAddress": str,
         "sshPublicKey": str,
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
 TagProjectRequestRequestTypeDef = TypedDict(
     "TagProjectRequestRequestTypeDef",
     {
         "id": str,
         "tags": Mapping[str, str],
     },
 )
 
-TagProjectResultTypeDef = TypedDict(
-    "TagProjectResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagProjectRequestRequestTypeDef = TypedDict(
     "UntagProjectRequestRequestTypeDef",
     {
         "id": str,
         "tags": Sequence[str],
     },
 )
@@ -558,24 +423,14 @@
 )
 
 class UpdateTeamMemberRequestRequestTypeDef(
     _RequiredUpdateTeamMemberRequestRequestTypeDef, _OptionalUpdateTeamMemberRequestRequestTypeDef
 ):
     pass
 
-UpdateTeamMemberResultTypeDef = TypedDict(
-    "UpdateTeamMemberResultTypeDef",
-    {
-        "userArn": str,
-        "projectRole": str,
-        "remoteAccessAllowed": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateUserProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserProfileRequestRequestTypeDef",
     {
         "userArn": str,
     },
 )
 _OptionalUpdateUserProfileRequestRequestTypeDef = TypedDict(
@@ -589,24 +444,113 @@
 )
 
 class UpdateUserProfileRequestRequestTypeDef(
     _RequiredUpdateUserProfileRequestRequestTypeDef, _OptionalUpdateUserProfileRequestRequestTypeDef
 ):
     pass
 
+AssociateTeamMemberResultTypeDef = TypedDict(
+    "AssociateTeamMemberResultTypeDef",
+    {
+        "clientRequestToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProjectResultTypeDef = TypedDict(
+    "CreateProjectResultTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "clientRequestToken": str,
+        "projectTemplateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserProfileResultTypeDef = TypedDict(
+    "CreateUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "displayName": str,
+        "emailAddress": str,
+        "sshPublicKey": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteProjectResultTypeDef = TypedDict(
+    "DeleteProjectResultTypeDef",
+    {
+        "stackId": str,
+        "projectArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteUserProfileResultTypeDef = TypedDict(
+    "DeleteUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUserProfileResultTypeDef = TypedDict(
+    "DescribeUserProfileResultTypeDef",
+    {
+        "userArn": str,
+        "displayName": str,
+        "emailAddress": str,
+        "sshPublicKey": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForProjectResultTypeDef = TypedDict(
+    "ListTagsForProjectResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagProjectResultTypeDef = TypedDict(
+    "TagProjectResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTeamMemberResultTypeDef = TypedDict(
+    "UpdateTeamMemberResultTypeDef",
+    {
+        "userArn": str,
+        "projectRole": str,
+        "remoteAccessAllowed": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateUserProfileResultTypeDef = TypedDict(
     "UpdateUserProfileResultTypeDef",
     {
         "userArn": str,
         "displayName": str,
         "emailAddress": str,
         "sshPublicKey": str,
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CodeDestinationTypeDef = TypedDict(
     "CodeDestinationTypeDef",
     {
         "codeCommit": CodeCommitCodeDestinationTypeDef,
@@ -637,51 +581,107 @@
         "arn": str,
         "description": str,
         "clientRequestToken": str,
         "createdTimeStamp": datetime,
         "stackId": str,
         "projectTemplateId": str,
         "status": ProjectStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+_RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourcesRequestListResourcesPaginateTypeDef(
+    _RequiredListResourcesRequestListResourcesPaginateTypeDef,
+    _OptionalListResourcesRequestListResourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
+    "_RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    {
+        "projectId": str,
+    },
+)
+_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef = TypedDict(
+    "_OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTeamMembersRequestListTeamMembersPaginateTypeDef(
+    _RequiredListTeamMembersRequestListTeamMembersPaginateTypeDef,
+    _OptionalListTeamMembersRequestListTeamMembersPaginateTypeDef,
+):
+    pass
+
+ListUserProfilesRequestListUserProfilesPaginateTypeDef = TypedDict(
+    "ListUserProfilesRequestListUserProfilesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListProjectsResultTypeDef = TypedDict(
     "ListProjectsResultTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResultTypeDef = TypedDict(
     "ListResourcesResultTypeDef",
     {
         "resources": List[ResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTeamMembersResultTypeDef = TypedDict(
     "ListTeamMembersResultTypeDef",
     {
         "teamMembers": List[TeamMemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserProfilesResultTypeDef = TypedDict(
     "ListUserProfilesResultTypeDef",
     {
         "userProfiles": List[UserProfileSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CodeTypeDef = TypedDict(
     "CodeTypeDef",
     {
         "source": CodeSourceTypeDef,
```

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar.egg-info/PKG-INFO` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar
-Version: 1.28.12
-Summary: Type annotations for boto3.CodeStar 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CodeStar 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar)](https://pepy.tech/project/mypy-boto3-codestar)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStar 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
+[boto3.CodeStar 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
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
 [mypy-boto3-codestar docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,58 +330,58 @@
 
 `mypy_boto3_codestar.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codestar.type_defs import (
     AssociateTeamMemberRequestRequestTypeDef,
-    AssociateTeamMemberResultTypeDef,
+    ResponseMetadataTypeDef,
     CodeCommitCodeDestinationTypeDef,
     GitHubCodeDestinationTypeDef,
     S3LocationTypeDef,
-    CreateProjectResultTypeDef,
     CreateUserProfileRequestRequestTypeDef,
-    CreateUserProfileResultTypeDef,
     DeleteProjectRequestRequestTypeDef,
-    DeleteProjectResultTypeDef,
     DeleteUserProfileRequestRequestTypeDef,
-    DeleteUserProfileResultTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ProjectStatusTypeDef,
     DescribeUserProfileRequestRequestTypeDef,
-    DescribeUserProfileResultTypeDef,
     DisassociateTeamMemberRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForProjectRequestRequestTypeDef,
-    ListTagsForProjectResultTypeDef,
-    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
     ListTeamMembersRequestRequestTypeDef,
     TeamMemberTypeDef,
-    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListUserProfilesRequestRequestTypeDef,
     UserProfileSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagProjectRequestRequestTypeDef,
-    TagProjectResultTypeDef,
     UntagProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     UpdateTeamMemberRequestRequestTypeDef,
-    UpdateTeamMemberResultTypeDef,
     UpdateUserProfileRequestRequestTypeDef,
+    AssociateTeamMemberResultTypeDef,
+    CreateProjectResultTypeDef,
+    CreateUserProfileResultTypeDef,
+    DeleteProjectResultTypeDef,
+    DeleteUserProfileResultTypeDef,
+    DescribeUserProfileResultTypeDef,
+    ListTagsForProjectResultTypeDef,
+    TagProjectResultTypeDef,
+    UpdateTeamMemberResultTypeDef,
     UpdateUserProfileResultTypeDef,
     CodeDestinationTypeDef,
     CodeSourceTypeDef,
     ToolchainSourceTypeDef,
     DescribeProjectResultTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListResourcesRequestListResourcesPaginateTypeDef,
+    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
+    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
     ListProjectsResultTypeDef,
     ListResourcesResultTypeDef,
     ListTeamMembersResultTypeDef,
     ListUserProfilesResultTypeDef,
     CodeTypeDef,
     ToolchainTypeDef,
     CreateProjectRequestRequestTypeDef,
```

### Comparing `mypy-boto3-codestar-1.28.12/mypy_boto3_codestar.egg-info/SOURCES.txt` & `mypy-boto3-codestar-1.28.15/mypy_boto3_codestar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-1.28.12/setup.py` & `mypy-boto3-codestar-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codestar",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_codestar"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeStar 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CodeStar 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

