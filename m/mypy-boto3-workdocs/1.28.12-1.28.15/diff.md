# Comparing `tmp/mypy-boto3-workdocs-1.28.12.tar.gz` & `tmp/mypy-boto3-workdocs-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workdocs-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
+gzip compressed data, was "mypy-boto3-workdocs-1.28.15.tar", last modified: Fri Jul 28 20:43:57 2023, max compression
```

## Comparing `mypy-boto3-workdocs-1.28.12.tar` & `mypy-boto3-workdocs-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.849495 mypy-boto3-workdocs-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-07-27 11:49:49.849495 mypy-boto3-workdocs-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.849495 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38652 2023-07-27 11:48:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38591 2023-07-27 11:48:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-07-27 11:48:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-07-27 11:48:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13859 2023-07-27 11:48:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-07-27 11:48:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50773 2023-07-27 11:48:50.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50682 2023-07-27 11:48:50.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.849495 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-07-27 11:49:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 11:49:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:49.000000 mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.849495 mypy-boto3-workdocs-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:48:48.000000 mypy-boto3-workdocs-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:57.078047 mypy-boto3-workdocs-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:32.000000 mypy-boto3-workdocs-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-07-28 20:43:57.070047 mypy-boto3-workdocs-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-07-28 20:41:32.000000 mypy-boto3-workdocs-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:57.066047 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-28 20:41:32.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-28 20:41:32.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:41:32.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38652 2023-07-28 20:41:32.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38591 2023-07-28 20:41:32.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13880 2023-07-28 20:41:33.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-07-28 20:41:32.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13859 2023-07-28 20:41:32.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-07-28 20:41:32.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:32.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50540 2023-07-28 20:41:34.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50449 2023-07-28 20:41:33.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:32.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:57.070047 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-07-28 20:43:56.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:43:56.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:56.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:56.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:56.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:56.000000 mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:57.078047 mypy-boto3-workdocs-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:41:31.000000 mypy-boto3-workdocs-1.28.15/setup.py
```

### Comparing `mypy-boto3-workdocs-1.28.12/LICENSE` & `mypy-boto3-workdocs-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.12/PKG-INFO` & `mypy-boto3-workdocs-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workdocs
-Version: 1.28.12
-Summary: Type annotations for boto3.WorkDocs 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.WorkDocs 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workdocs)](https://pepy.tech/project/mypy-boto3-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkDocs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[boto3.WorkDocs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [mypy-boto3-workdocs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -450,29 +450,29 @@
     UploadMetadataTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
-    StorageRuleTypeOutputTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     UpdateDocumentVersionRequestRequestTypeDef,
     UpdateFolderRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     ResourceMetadataTypeDef,
     AddResourcePermissionsRequestRequestTypeDef,
     AddResourcePermissionsResponseTypeDef,
     CreateFolderResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
+    UserStorageMetadataTypeDef,
     DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
     DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
     DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
@@ -482,25 +482,24 @@
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
     FiltersTypeDef,
     PrincipalTypeDef,
     ResourcePathTypeDef,
-    UserStorageMetadataTypeDef,
+    UserTypeDef,
     DescribeFolderContentsResponseTypeDef,
     GetDocumentResponseTypeDef,
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
     SearchResourcesRequestRequestTypeDef,
     SearchResourcesRequestSearchResourcesPaginateTypeDef,
     DescribeResourcePermissionsResponseTypeDef,
     GetDocumentPathResponseTypeDef,
     GetFolderPathResponseTypeDef,
-    UserTypeDef,
     ActivateUserResponseTypeDef,
     CommentMetadataTypeDef,
     CommentTypeDef,
     CreateUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     GetCurrentUserResponseTypeDef,
     UpdateUserResponseTypeDef,
```

### Comparing `mypy-boto3-workdocs-1.28.12/README.md` & `mypy-boto3-workdocs-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workdocs)](https://pepy.tech/project/mypy-boto3-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkDocs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[boto3.WorkDocs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [mypy-boto3-workdocs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -418,29 +418,29 @@
     UploadMetadataTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
-    StorageRuleTypeOutputTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     UpdateDocumentVersionRequestRequestTypeDef,
     UpdateFolderRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     ResourceMetadataTypeDef,
     AddResourcePermissionsRequestRequestTypeDef,
     AddResourcePermissionsResponseTypeDef,
     CreateFolderResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
+    UserStorageMetadataTypeDef,
     DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
     DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
     DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
@@ -450,25 +450,24 @@
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
     FiltersTypeDef,
     PrincipalTypeDef,
     ResourcePathTypeDef,
-    UserStorageMetadataTypeDef,
+    UserTypeDef,
     DescribeFolderContentsResponseTypeDef,
     GetDocumentResponseTypeDef,
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
     SearchResourcesRequestRequestTypeDef,
     SearchResourcesRequestSearchResourcesPaginateTypeDef,
     DescribeResourcePermissionsResponseTypeDef,
     GetDocumentPathResponseTypeDef,
     GetFolderPathResponseTypeDef,
-    UserTypeDef,
     ActivateUserResponseTypeDef,
     CommentMetadataTypeDef,
     CommentTypeDef,
     CreateUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     GetCurrentUserResponseTypeDef,
     UpdateUserResponseTypeDef,
```

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/__init__.py` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/__init__.pyi` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/__main__.py` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkDocs 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.WorkDocs 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs\nOther"
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

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/client.py` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/client.pyi` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/literals.py` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/literals.pyi` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/paginator.py` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/paginator.pyi` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/type_defs.py` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,29 +112,29 @@
     "UploadMetadataTypeDef",
     "PermissionInfoTypeDef",
     "RemoveAllResourcePermissionsRequestRequestTypeDef",
     "RemoveResourcePermissionRequestRequestTypeDef",
     "ResourcePathComponentTypeDef",
     "RestoreDocumentVersionsRequestRequestTypeDef",
     "SearchSortResultTypeDef",
-    "StorageRuleTypeOutputTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
     "UpdateDocumentVersionRequestRequestTypeDef",
     "UpdateFolderRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ResourceMetadataTypeDef",
     "AddResourcePermissionsRequestRequestTypeDef",
     "AddResourcePermissionsResponseTypeDef",
     "CreateFolderResponseTypeDef",
     "DescribeRootFoldersResponseTypeDef",
     "GetFolderResponseTypeDef",
     "CreateNotificationSubscriptionResponseTypeDef",
     "DescribeNotificationSubscriptionsResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
+    "UserStorageMetadataTypeDef",
     "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
     "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
     "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
     "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
     "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
     "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
@@ -144,25 +144,24 @@
     "DocumentMetadataTypeDef",
     "GetDocumentVersionResponseTypeDef",
     "DescribeGroupsResponseTypeDef",
     "ParticipantsTypeDef",
     "FiltersTypeDef",
     "PrincipalTypeDef",
     "ResourcePathTypeDef",
-    "UserStorageMetadataTypeDef",
+    "UserTypeDef",
     "DescribeFolderContentsResponseTypeDef",
     "GetDocumentResponseTypeDef",
     "GetResourcesResponseTypeDef",
     "InitiateDocumentVersionUploadResponseTypeDef",
     "SearchResourcesRequestRequestTypeDef",
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "DescribeResourcePermissionsResponseTypeDef",
     "GetDocumentPathResponseTypeDef",
     "GetFolderPathResponseTypeDef",
-    "UserTypeDef",
     "ActivateUserResponseTypeDef",
     "CommentMetadataTypeDef",
     "CommentTypeDef",
     "CreateUserResponseTypeDef",
     "DescribeUsersResponseTypeDef",
     "GetCurrentUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
@@ -1159,23 +1158,14 @@
     {
         "Field": OrderByFieldTypeType,
         "Order": SortOrderType,
     },
     total=False,
 )
 
-StorageRuleTypeOutputTypeDef = TypedDict(
-    "StorageRuleTypeOutputTypeDef",
-    {
-        "StorageAllocatedInBytes": int,
-        "StorageType": StorageTypeType,
-    },
-    total=False,
-)
-
 _RequiredUpdateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalUpdateDocumentRequestRequestTypeDef = TypedDict(
@@ -1392,14 +1382,23 @@
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
 
+UserStorageMetadataTypeDef = TypedDict(
+    "UserStorageMetadataTypeDef",
+    {
+        "StorageUtilizedInBytes": int,
+        "StorageRule": StorageRuleTypeTypeDef,
+    },
+    total=False,
+)
+
 DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
     "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     {
         "AuthenticationToken": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "OrganizationId": str,
@@ -1678,19 +1677,32 @@
     "ResourcePathTypeDef",
     {
         "Components": List[ResourcePathComponentTypeDef],
     },
     total=False,
 )
 
-UserStorageMetadataTypeDef = TypedDict(
-    "UserStorageMetadataTypeDef",
+UserTypeDef = TypedDict(
+    "UserTypeDef",
     {
-        "StorageUtilizedInBytes": int,
-        "StorageRule": StorageRuleTypeOutputTypeDef,
+        "Id": str,
+        "Username": str,
+        "EmailAddress": str,
+        "GivenName": str,
+        "Surname": str,
+        "OrganizationId": str,
+        "RootFolderId": str,
+        "RecycleBinFolderId": str,
+        "Status": UserStatusTypeType,
+        "Type": UserTypeType,
+        "CreatedTimestamp": datetime,
+        "ModifiedTimestamp": datetime,
+        "TimeZoneId": str,
+        "Locale": LocaleTypeType,
+        "Storage": UserStorageMetadataTypeDef,
     },
     total=False,
 )
 
 DescribeFolderContentsResponseTypeDef = TypedDict(
     "DescribeFolderContentsResponseTypeDef",
     {
@@ -1781,36 +1793,14 @@
     "GetFolderPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserTypeDef = TypedDict(
-    "UserTypeDef",
-    {
-        "Id": str,
-        "Username": str,
-        "EmailAddress": str,
-        "GivenName": str,
-        "Surname": str,
-        "OrganizationId": str,
-        "RootFolderId": str,
-        "RecycleBinFolderId": str,
-        "Status": UserStatusTypeType,
-        "Type": UserTypeType,
-        "CreatedTimestamp": datetime,
-        "ModifiedTimestamp": datetime,
-        "TimeZoneId": str,
-        "Locale": LocaleTypeType,
-        "Storage": UserStorageMetadataTypeDef,
-    },
-    total=False,
-)
-
 ActivateUserResponseTypeDef = TypedDict(
     "ActivateUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs/type_defs.pyi` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -111,29 +111,29 @@
     "UploadMetadataTypeDef",
     "PermissionInfoTypeDef",
     "RemoveAllResourcePermissionsRequestRequestTypeDef",
     "RemoveResourcePermissionRequestRequestTypeDef",
     "ResourcePathComponentTypeDef",
     "RestoreDocumentVersionsRequestRequestTypeDef",
     "SearchSortResultTypeDef",
-    "StorageRuleTypeOutputTypeDef",
     "UpdateDocumentRequestRequestTypeDef",
     "UpdateDocumentVersionRequestRequestTypeDef",
     "UpdateFolderRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ResourceMetadataTypeDef",
     "AddResourcePermissionsRequestRequestTypeDef",
     "AddResourcePermissionsResponseTypeDef",
     "CreateFolderResponseTypeDef",
     "DescribeRootFoldersResponseTypeDef",
     "GetFolderResponseTypeDef",
     "CreateNotificationSubscriptionResponseTypeDef",
     "DescribeNotificationSubscriptionsResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
+    "UserStorageMetadataTypeDef",
     "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     "DescribeCommentsRequestDescribeCommentsPaginateTypeDef",
     "DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef",
     "DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef",
     "DescribeGroupsRequestDescribeGroupsPaginateTypeDef",
     "DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef",
     "DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef",
@@ -143,25 +143,24 @@
     "DocumentMetadataTypeDef",
     "GetDocumentVersionResponseTypeDef",
     "DescribeGroupsResponseTypeDef",
     "ParticipantsTypeDef",
     "FiltersTypeDef",
     "PrincipalTypeDef",
     "ResourcePathTypeDef",
-    "UserStorageMetadataTypeDef",
+    "UserTypeDef",
     "DescribeFolderContentsResponseTypeDef",
     "GetDocumentResponseTypeDef",
     "GetResourcesResponseTypeDef",
     "InitiateDocumentVersionUploadResponseTypeDef",
     "SearchResourcesRequestRequestTypeDef",
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "DescribeResourcePermissionsResponseTypeDef",
     "GetDocumentPathResponseTypeDef",
     "GetFolderPathResponseTypeDef",
-    "UserTypeDef",
     "ActivateUserResponseTypeDef",
     "CommentMetadataTypeDef",
     "CommentTypeDef",
     "CreateUserResponseTypeDef",
     "DescribeUsersResponseTypeDef",
     "GetCurrentUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
@@ -1096,23 +1095,14 @@
     {
         "Field": OrderByFieldTypeType,
         "Order": SortOrderType,
     },
     total=False,
 )
 
-StorageRuleTypeOutputTypeDef = TypedDict(
-    "StorageRuleTypeOutputTypeDef",
-    {
-        "StorageAllocatedInBytes": int,
-        "StorageType": StorageTypeType,
-    },
-    total=False,
-)
-
 _RequiredUpdateDocumentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDocumentRequestRequestTypeDef",
     {
         "DocumentId": str,
     },
 )
 _OptionalUpdateDocumentRequestRequestTypeDef = TypedDict(
@@ -1317,14 +1307,23 @@
 )
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
+UserStorageMetadataTypeDef = TypedDict(
+    "UserStorageMetadataTypeDef",
+    {
+        "StorageUtilizedInBytes": int,
+        "StorageRule": StorageRuleTypeTypeDef,
+    },
+    total=False,
+)
+
 DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef = TypedDict(
     "DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef",
     {
         "AuthenticationToken": str,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
         "OrganizationId": str,
@@ -1589,19 +1588,32 @@
     "ResourcePathTypeDef",
     {
         "Components": List[ResourcePathComponentTypeDef],
     },
     total=False,
 )
 
-UserStorageMetadataTypeDef = TypedDict(
-    "UserStorageMetadataTypeDef",
+UserTypeDef = TypedDict(
+    "UserTypeDef",
     {
-        "StorageUtilizedInBytes": int,
-        "StorageRule": StorageRuleTypeOutputTypeDef,
+        "Id": str,
+        "Username": str,
+        "EmailAddress": str,
+        "GivenName": str,
+        "Surname": str,
+        "OrganizationId": str,
+        "RootFolderId": str,
+        "RecycleBinFolderId": str,
+        "Status": UserStatusTypeType,
+        "Type": UserTypeType,
+        "CreatedTimestamp": datetime,
+        "ModifiedTimestamp": datetime,
+        "TimeZoneId": str,
+        "Locale": LocaleTypeType,
+        "Storage": UserStorageMetadataTypeDef,
     },
     total=False,
 )
 
 DescribeFolderContentsResponseTypeDef = TypedDict(
     "DescribeFolderContentsResponseTypeDef",
     {
@@ -1692,36 +1704,14 @@
     "GetFolderPathResponseTypeDef",
     {
         "Path": ResourcePathTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserTypeDef = TypedDict(
-    "UserTypeDef",
-    {
-        "Id": str,
-        "Username": str,
-        "EmailAddress": str,
-        "GivenName": str,
-        "Surname": str,
-        "OrganizationId": str,
-        "RootFolderId": str,
-        "RecycleBinFolderId": str,
-        "Status": UserStatusTypeType,
-        "Type": UserTypeType,
-        "CreatedTimestamp": datetime,
-        "ModifiedTimestamp": datetime,
-        "TimeZoneId": str,
-        "Locale": LocaleTypeType,
-        "Storage": UserStorageMetadataTypeDef,
-    },
-    total=False,
-)
-
 ActivateUserResponseTypeDef = TypedDict(
     "ActivateUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/PKG-INFO` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workdocs
-Version: 1.28.12
-Summary: Type annotations for boto3.WorkDocs 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.WorkDocs 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workdocs.svg?color=blue)](https://pypi.org/project/mypy-boto3-workdocs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workdocs)](https://pepy.tech/project/mypy-boto3-workdocs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkDocs 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
+[boto3.WorkDocs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs)
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
 [mypy-boto3-workdocs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workdocs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -450,29 +450,29 @@
     UploadMetadataTypeDef,
     PermissionInfoTypeDef,
     RemoveAllResourcePermissionsRequestRequestTypeDef,
     RemoveResourcePermissionRequestRequestTypeDef,
     ResourcePathComponentTypeDef,
     RestoreDocumentVersionsRequestRequestTypeDef,
     SearchSortResultTypeDef,
-    StorageRuleTypeOutputTypeDef,
     UpdateDocumentRequestRequestTypeDef,
     UpdateDocumentVersionRequestRequestTypeDef,
     UpdateFolderRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     ResourceMetadataTypeDef,
     AddResourcePermissionsRequestRequestTypeDef,
     AddResourcePermissionsResponseTypeDef,
     CreateFolderResponseTypeDef,
     DescribeRootFoldersResponseTypeDef,
     GetFolderResponseTypeDef,
     CreateNotificationSubscriptionResponseTypeDef,
     DescribeNotificationSubscriptionsResponseTypeDef,
     CreateUserRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
+    UserStorageMetadataTypeDef,
     DescribeActivitiesRequestDescribeActivitiesPaginateTypeDef,
     DescribeCommentsRequestDescribeCommentsPaginateTypeDef,
     DescribeDocumentVersionsRequestDescribeDocumentVersionsPaginateTypeDef,
     DescribeFolderContentsRequestDescribeFolderContentsPaginateTypeDef,
     DescribeGroupsRequestDescribeGroupsPaginateTypeDef,
     DescribeNotificationSubscriptionsRequestDescribeNotificationSubscriptionsPaginateTypeDef,
     DescribeResourcePermissionsRequestDescribeResourcePermissionsPaginateTypeDef,
@@ -482,25 +482,24 @@
     DocumentMetadataTypeDef,
     GetDocumentVersionResponseTypeDef,
     DescribeGroupsResponseTypeDef,
     ParticipantsTypeDef,
     FiltersTypeDef,
     PrincipalTypeDef,
     ResourcePathTypeDef,
-    UserStorageMetadataTypeDef,
+    UserTypeDef,
     DescribeFolderContentsResponseTypeDef,
     GetDocumentResponseTypeDef,
     GetResourcesResponseTypeDef,
     InitiateDocumentVersionUploadResponseTypeDef,
     SearchResourcesRequestRequestTypeDef,
     SearchResourcesRequestSearchResourcesPaginateTypeDef,
     DescribeResourcePermissionsResponseTypeDef,
     GetDocumentPathResponseTypeDef,
     GetFolderPathResponseTypeDef,
-    UserTypeDef,
     ActivateUserResponseTypeDef,
     CommentMetadataTypeDef,
     CommentTypeDef,
     CreateUserResponseTypeDef,
     DescribeUsersResponseTypeDef,
     GetCurrentUserResponseTypeDef,
     UpdateUserResponseTypeDef,
```

### Comparing `mypy-boto3-workdocs-1.28.12/mypy_boto3_workdocs.egg-info/SOURCES.txt` & `mypy-boto3-workdocs-1.28.15/mypy_boto3_workdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workdocs-1.28.12/setup.py` & `mypy-boto3-workdocs-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workdocs",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_workdocs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkDocs 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.WorkDocs 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

