# Comparing `tmp/mypy-boto3-identitystore-1.28.12.tar.gz` & `tmp/mypy-boto3-identitystore-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-identitystore-1.28.12.tar", last modified: Thu Jul 27 05:34:46 2023, max compression
+gzip compressed data, was "mypy-boto3-identitystore-1.28.15.tar", last modified: Fri Jul 28 20:42:56 2023, max compression
```

## Comparing `mypy-boto3-identitystore-1.28.12.tar` & `mypy-boto3-identitystore-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.736492 mypy-boto3-identitystore-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15467 2023-07-27 05:34:46.736492 mypy-boto3-identitystore-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.736492 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-27 05:23:28.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-27 05:23:28.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-27 05:23:28.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20678 2023-07-27 05:23:28.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-07-27 05:23:28.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.736492 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15467 2023-07-27 05:34:46.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 05:34:46.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:46.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:46.000000 mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:46.736492 mypy-boto3-identitystore-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 05:23:27.000000 mypy-boto3-identitystore-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.133211 mypy-boto3-identitystore-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-07-28 20:42:56.133211 mypy-boto3-identitystore-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.109211 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19238 2023-07-28 20:27:35.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19209 2023-07-28 20:27:35.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.113211 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-07-28 20:42:55.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:42:55.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:55.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:55.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:55.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:55.000000 mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:56.133211 mypy-boto3-identitystore-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 20:27:34.000000 mypy-boto3-identitystore-1.28.15/setup.py
```

### Comparing `mypy-boto3-identitystore-1.28.12/LICENSE` & `mypy-boto3-identitystore-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.12/PKG-INFO` & `mypy-boto3-identitystore-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-identitystore
-Version: 1.28.12
-Summary: Type annotations for boto3.IdentityStore 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IdentityStore 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-identitystore)](https://pepy.tech/project/mypy-boto3-identitystore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IdentityStore 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
+[boto3.IdentityStore 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
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
 [mypy-boto3-identitystore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,77 +334,71 @@
 ### Typed dictionaries
 
 `mypy_boto3_identitystore.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_identitystore.type_defs import (
-    AddressOutputTypeDef,
     AddressTypeDef,
     ExternalIdTypeDef,
     UniqueAttributeTypeDef,
     AttributeOperationTypeDef,
     MemberIdTypeDef,
-    CreateGroupMembershipResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateGroupRequestRequestTypeDef,
-    CreateGroupResponseTypeDef,
     EmailTypeDef,
     NameTypeDef,
     PhoneNumberTypeDef,
-    CreateUserResponseTypeDef,
     DeleteGroupMembershipRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeGroupMembershipRequestRequestTypeDef,
-    MemberIdOutputTypeDef,
     DescribeGroupRequestRequestTypeDef,
-    ExternalIdOutputTypeDef,
     DescribeUserRequestRequestTypeDef,
-    EmailOutputTypeDef,
-    NameOutputTypeDef,
-    PhoneNumberOutputTypeDef,
     FilterTypeDef,
-    GetGroupIdResponseTypeDef,
-    GetGroupMembershipIdResponseTypeDef,
-    GetUserIdResponseTypeDef,
-    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-    ListGroupMembershipsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListGroupMembershipsRequestRequestTypeDef,
+    GroupTypeDef,
     AlternateIdentifierTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
     GetGroupMembershipIdRequestRequestTypeDef,
+    GroupMembershipExistenceResultTypeDef,
+    GroupMembershipTypeDef,
     IsMemberInGroupsRequestRequestTypeDef,
-    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     ListGroupMembershipsForMemberRequestRequestTypeDef,
-    CreateUserRequestRequestTypeDef,
+    CreateGroupMembershipResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateUserResponseTypeDef,
     DescribeGroupMembershipResponseTypeDef,
-    GroupMembershipExistenceResultTypeDef,
-    GroupMembershipTypeDef,
     DescribeGroupResponseTypeDef,
-    GroupTypeDef,
+    GetGroupIdResponseTypeDef,
+    GetGroupMembershipIdResponseTypeDef,
+    GetUserIdResponseTypeDef,
+    CreateUserRequestRequestTypeDef,
     DescribeUserResponseTypeDef,
     UserTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
+    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListGroupsResponseTypeDef,
     GetGroupIdRequestRequestTypeDef,
     GetUserIdRequestRequestTypeDef,
     IsMemberInGroupsResponseTypeDef,
     ListGroupMembershipsForMemberResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
-    ListGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
 )
 
 
-def get_structure() -> AddressOutputTypeDef:
+def get_structure() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-identitystore-1.28.12/README.md` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-identitystore
+Version: 1.28.15
+Summary: Type annotations for boto3.IdentityStore 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 identitystore type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-identitystore"></a>
 
 # mypy-boto3-identitystore
 
 [![PyPI - mypy-boto3-identitystore](https://img.shields.io/pypi/v/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-identitystore)](https://pepy.tech/project/mypy-boto3-identitystore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IdentityStore 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
+[boto3.IdentityStore 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
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
 [mypy-boto3-identitystore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,77 +334,71 @@
 ### Typed dictionaries
 
 `mypy_boto3_identitystore.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_identitystore.type_defs import (
-    AddressOutputTypeDef,
     AddressTypeDef,
     ExternalIdTypeDef,
     UniqueAttributeTypeDef,
     AttributeOperationTypeDef,
     MemberIdTypeDef,
-    CreateGroupMembershipResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateGroupRequestRequestTypeDef,
-    CreateGroupResponseTypeDef,
     EmailTypeDef,
     NameTypeDef,
     PhoneNumberTypeDef,
-    CreateUserResponseTypeDef,
     DeleteGroupMembershipRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeGroupMembershipRequestRequestTypeDef,
-    MemberIdOutputTypeDef,
     DescribeGroupRequestRequestTypeDef,
-    ExternalIdOutputTypeDef,
     DescribeUserRequestRequestTypeDef,
-    EmailOutputTypeDef,
-    NameOutputTypeDef,
-    PhoneNumberOutputTypeDef,
     FilterTypeDef,
-    GetGroupIdResponseTypeDef,
-    GetGroupMembershipIdResponseTypeDef,
-    GetUserIdResponseTypeDef,
-    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-    ListGroupMembershipsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListGroupMembershipsRequestRequestTypeDef,
+    GroupTypeDef,
     AlternateIdentifierTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
     GetGroupMembershipIdRequestRequestTypeDef,
+    GroupMembershipExistenceResultTypeDef,
+    GroupMembershipTypeDef,
     IsMemberInGroupsRequestRequestTypeDef,
-    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     ListGroupMembershipsForMemberRequestRequestTypeDef,
-    CreateUserRequestRequestTypeDef,
+    CreateGroupMembershipResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateUserResponseTypeDef,
     DescribeGroupMembershipResponseTypeDef,
-    GroupMembershipExistenceResultTypeDef,
-    GroupMembershipTypeDef,
     DescribeGroupResponseTypeDef,
-    GroupTypeDef,
+    GetGroupIdResponseTypeDef,
+    GetGroupMembershipIdResponseTypeDef,
+    GetUserIdResponseTypeDef,
+    CreateUserRequestRequestTypeDef,
     DescribeUserResponseTypeDef,
     UserTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
+    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListGroupsResponseTypeDef,
     GetGroupIdRequestRequestTypeDef,
     GetUserIdRequestRequestTypeDef,
     IsMemberInGroupsResponseTypeDef,
     ListGroupMembershipsForMemberResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
-    ListGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
 )
 
 
-def get_structure() -> AddressOutputTypeDef:
+def get_structure() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/__init__.py` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/__init__.pyi` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/__main__.py` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IdentityStore 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IdentityStore 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore\nOther"
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

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/client.py` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/client.pyi` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/literals.py` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/literals.pyi` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/paginator.py` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,92 +42,82 @@
 __all__ = (
     "ListGroupMembershipsPaginator",
     "ListGroupMembershipsForMemberPaginator",
     "ListGroupsPaginator",
     "ListUsersPaginator",
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
 class ListGroupMembershipsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMemberships)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        IdentityStoreId: str,
-        GroupId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, IdentityStoreId: str, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupMembershipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMemberships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipspaginator)
         """
 
-
 class ListGroupMembershipsForMemberPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMembershipsForMember)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipsformemberpaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         MemberId: MemberIdTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupMembershipsForMemberResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMembershipsForMember.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipsformemberpaginator)
         """
 
-
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupspaginator)
         """
 
-
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listuserspaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/paginator.pyi` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,86 +42,88 @@
 __all__ = (
     "ListGroupMembershipsPaginator",
     "ListGroupMembershipsForMemberPaginator",
     "ListGroupsPaginator",
     "ListUsersPaginator",
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
 class ListGroupMembershipsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMemberships)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        IdentityStoreId: str,
-        GroupId: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, IdentityStoreId: str, GroupId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupMembershipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMemberships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipspaginator)
         """
 
+
 class ListGroupMembershipsForMemberPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMembershipsForMember)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipsformemberpaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         MemberId: MemberIdTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupMembershipsForMemberResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroupMembershipsForMember.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupmembershipsformemberpaginator)
         """
 
+
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listgroupspaginator)
         """
 
+
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listuserspaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityStoreId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/type_defs.py` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,105 +2,84 @@
 Type annotations for identitystore service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_identitystore.type_defs import AddressOutputTypeDef
+    from mypy_boto3_identitystore.type_defs import AddressTypeDef
 
-    data: AddressOutputTypeDef = {...}
+    data: AddressTypeDef = {...}
     ```
 """
 import sys
 from typing import Any, Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AddressOutputTypeDef",
     "AddressTypeDef",
     "ExternalIdTypeDef",
     "UniqueAttributeTypeDef",
     "AttributeOperationTypeDef",
     "MemberIdTypeDef",
-    "CreateGroupMembershipResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateGroupRequestRequestTypeDef",
-    "CreateGroupResponseTypeDef",
     "EmailTypeDef",
     "NameTypeDef",
     "PhoneNumberTypeDef",
-    "CreateUserResponseTypeDef",
     "DeleteGroupMembershipRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeGroupMembershipRequestRequestTypeDef",
-    "MemberIdOutputTypeDef",
     "DescribeGroupRequestRequestTypeDef",
-    "ExternalIdOutputTypeDef",
     "DescribeUserRequestRequestTypeDef",
-    "EmailOutputTypeDef",
-    "NameOutputTypeDef",
-    "PhoneNumberOutputTypeDef",
     "FilterTypeDef",
-    "GetGroupIdResponseTypeDef",
-    "GetGroupMembershipIdResponseTypeDef",
-    "GetUserIdResponseTypeDef",
-    "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
-    "ListGroupMembershipsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListGroupMembershipsRequestRequestTypeDef",
+    "GroupTypeDef",
     "AlternateIdentifierTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
     "GetGroupMembershipIdRequestRequestTypeDef",
+    "GroupMembershipExistenceResultTypeDef",
+    "GroupMembershipTypeDef",
     "IsMemberInGroupsRequestRequestTypeDef",
-    "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
     "ListGroupMembershipsForMemberRequestRequestTypeDef",
-    "CreateUserRequestRequestTypeDef",
+    "CreateGroupMembershipResponseTypeDef",
+    "CreateGroupResponseTypeDef",
+    "CreateUserResponseTypeDef",
     "DescribeGroupMembershipResponseTypeDef",
-    "GroupMembershipExistenceResultTypeDef",
-    "GroupMembershipTypeDef",
     "DescribeGroupResponseTypeDef",
-    "GroupTypeDef",
+    "GetGroupIdResponseTypeDef",
+    "GetGroupMembershipIdResponseTypeDef",
+    "GetUserIdResponseTypeDef",
+    "CreateUserRequestRequestTypeDef",
     "DescribeUserResponseTypeDef",
     "UserTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
+    "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+    "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
+    "ListGroupsResponseTypeDef",
     "GetGroupIdRequestRequestTypeDef",
     "GetUserIdRequestRequestTypeDef",
     "IsMemberInGroupsResponseTypeDef",
     "ListGroupMembershipsForMemberResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
-    "ListGroupsResponseTypeDef",
     "ListUsersResponseTypeDef",
 )
 
-AddressOutputTypeDef = TypedDict(
-    "AddressOutputTypeDef",
-    {
-        "StreetAddress": str,
-        "Locality": str,
-        "Region": str,
-        "PostalCode": str,
-        "Country": str,
-        "Formatted": str,
-        "Type": str,
-        "Primary": bool,
-    },
-    total=False,
-)
-
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "StreetAddress": str,
         "Locality": str,
         "Region": str,
         "PostalCode": str,
@@ -153,20 +132,22 @@
     "MemberIdTypeDef",
     {
         "UserId": str,
     },
     total=False,
 )
 
-CreateGroupMembershipResponseTypeDef = TypedDict(
-    "CreateGroupMembershipResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "MembershipId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
@@ -184,23 +165,14 @@
 
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
 
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EmailTypeDef = TypedDict(
     "EmailTypeDef",
     {
         "Value": str,
         "Type": str,
         "Primary": bool,
     },
@@ -226,23 +198,14 @@
         "Value": str,
         "Type": str,
         "Primary": bool,
     },
     total=False,
 )
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "UserId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGroupMembershipRequestRequestTypeDef = TypedDict(
     "DeleteGroupMembershipRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MembershipId": str,
     },
 )
@@ -267,137 +230,48 @@
     "DescribeGroupMembershipRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MembershipId": str,
     },
 )
 
-MemberIdOutputTypeDef = TypedDict(
-    "MemberIdOutputTypeDef",
-    {
-        "UserId": str,
-    },
-    total=False,
-)
-
 DescribeGroupRequestRequestTypeDef = TypedDict(
     "DescribeGroupRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
     },
 )
 
-ExternalIdOutputTypeDef = TypedDict(
-    "ExternalIdOutputTypeDef",
-    {
-        "Issuer": str,
-        "Id": str,
-    },
-)
-
 DescribeUserRequestRequestTypeDef = TypedDict(
     "DescribeUserRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "UserId": str,
     },
 )
 
-EmailOutputTypeDef = TypedDict(
-    "EmailOutputTypeDef",
-    {
-        "Value": str,
-        "Type": str,
-        "Primary": bool,
-    },
-    total=False,
-)
-
-NameOutputTypeDef = TypedDict(
-    "NameOutputTypeDef",
-    {
-        "Formatted": str,
-        "FamilyName": str,
-        "GivenName": str,
-        "MiddleName": str,
-        "HonorificPrefix": str,
-        "HonorificSuffix": str,
-    },
-    total=False,
-)
-
-PhoneNumberOutputTypeDef = TypedDict(
-    "PhoneNumberOutputTypeDef",
-    {
-        "Value": str,
-        "Type": str,
-        "Primary": bool,
-    },
-    total=False,
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "AttributePath": str,
         "AttributeValue": str,
     },
 )
 
-GetGroupIdResponseTypeDef = TypedDict(
-    "GetGroupIdResponseTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetGroupMembershipIdResponseTypeDef = TypedDict(
-    "GetGroupMembershipIdResponseTypeDef",
-    {
-        "MembershipId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetUserIdResponseTypeDef = TypedDict(
-    "GetUserIdResponseTypeDef",
-    {
-        "UserId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
-    {
-        "IdentityStoreId": str,
-        "GroupId": str,
-    },
-)
-_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
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
 
-
-class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
-    _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-    _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGroupMembershipsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
     },
 )
@@ -414,35 +288,36 @@
 class ListGroupMembershipsRequestRequestTypeDef(
     _RequiredListGroupMembershipsRequestRequestTypeDef,
     _OptionalListGroupMembershipsRequestRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGroupTypeDef = TypedDict(
+    "_RequiredGroupTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "GroupId": str,
+        "IdentityStoreId": str,
     },
-    total=False,
 )
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_OptionalGroupTypeDef = TypedDict(
+    "_OptionalGroupTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DisplayName": str,
+        "ExternalIds": List[ExternalIdTypeDef],
+        "Description": str,
     },
+    total=False,
 )
 
+
+class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
+    pass
+
+
 AlternateIdentifierTypeDef = TypedDict(
     "AlternateIdentifierTypeDef",
     {
         "ExternalId": ExternalIdTypeDef,
         "UniqueAttribute": UniqueAttributeTypeDef,
     },
     total=False,
@@ -480,50 +355,54 @@
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
 
-IsMemberInGroupsRequestRequestTypeDef = TypedDict(
-    "IsMemberInGroupsRequestRequestTypeDef",
+GroupMembershipExistenceResultTypeDef = TypedDict(
+    "GroupMembershipExistenceResultTypeDef",
     {
-        "IdentityStoreId": str,
+        "GroupId": str,
         "MemberId": MemberIdTypeDef,
-        "GroupIds": Sequence[str],
+        "MembershipExists": bool,
     },
+    total=False,
 )
 
-_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-        {
-            "IdentityStoreId": str,
-            "MemberId": MemberIdTypeDef,
-        },
-    )
+_RequiredGroupMembershipTypeDef = TypedDict(
+    "_RequiredGroupMembershipTypeDef",
+    {
+        "IdentityStoreId": str,
+    },
 )
-_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
+_OptionalGroupMembershipTypeDef = TypedDict(
+    "_OptionalGroupMembershipTypeDef",
+    {
+        "MembershipId": str,
+        "GroupId": str,
+        "MemberId": MemberIdTypeDef,
+    },
+    total=False,
 )
 
 
-class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
-    _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-    _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-):
+class GroupMembershipTypeDef(_RequiredGroupMembershipTypeDef, _OptionalGroupMembershipTypeDef):
     pass
 
 
+IsMemberInGroupsRequestRequestTypeDef = TypedDict(
+    "IsMemberInGroupsRequestRequestTypeDef",
+    {
+        "IdentityStoreId": str,
+        "MemberId": MemberIdTypeDef,
+        "GroupIds": Sequence[str],
+    },
+)
+
 _RequiredListGroupMembershipsForMemberRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsForMemberRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
@@ -540,271 +419,331 @@
 class ListGroupMembershipsForMemberRequestRequestTypeDef(
     _RequiredListGroupMembershipsForMemberRequestRequestTypeDef,
     _OptionalListGroupMembershipsForMemberRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateUserRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateUserRequestRequestTypeDef",
+CreateGroupMembershipResponseTypeDef = TypedDict(
+    "CreateGroupMembershipResponseTypeDef",
     {
+        "MembershipId": str,
         "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateUserRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateUserRequestRequestTypeDef",
+
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
     {
-        "UserName": str,
-        "Name": NameTypeDef,
-        "DisplayName": str,
-        "NickName": str,
-        "ProfileUrl": str,
-        "Emails": Sequence[EmailTypeDef],
-        "Addresses": Sequence[AddressTypeDef],
-        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
-        "UserType": str,
-        "Title": str,
-        "PreferredLanguage": str,
-        "Locale": str,
-        "Timezone": str,
+        "GroupId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateUserRequestRequestTypeDef(
-    _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
-):
-    pass
-
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "UserId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 DescribeGroupMembershipResponseTypeDef = TypedDict(
     "DescribeGroupMembershipResponseTypeDef",
     {
         "IdentityStoreId": str,
         "MembershipId": str,
         "GroupId": str,
-        "MemberId": MemberIdOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MemberId": MemberIdTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GroupMembershipExistenceResultTypeDef = TypedDict(
-    "GroupMembershipExistenceResultTypeDef",
+DescribeGroupResponseTypeDef = TypedDict(
+    "DescribeGroupResponseTypeDef",
     {
         "GroupId": str,
-        "MemberId": MemberIdOutputTypeDef,
-        "MembershipExists": bool,
+        "DisplayName": str,
+        "ExternalIds": List[ExternalIdTypeDef],
+        "Description": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredGroupMembershipTypeDef = TypedDict(
-    "_RequiredGroupMembershipTypeDef",
+GetGroupIdResponseTypeDef = TypedDict(
+    "GetGroupIdResponseTypeDef",
     {
+        "GroupId": str,
         "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGroupMembershipTypeDef = TypedDict(
-    "_OptionalGroupMembershipTypeDef",
+
+GetGroupMembershipIdResponseTypeDef = TypedDict(
+    "GetGroupMembershipIdResponseTypeDef",
     {
         "MembershipId": str,
-        "GroupId": str,
-        "MemberId": MemberIdOutputTypeDef,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class GroupMembershipTypeDef(_RequiredGroupMembershipTypeDef, _OptionalGroupMembershipTypeDef):
-    pass
-
-
-DescribeGroupResponseTypeDef = TypedDict(
-    "DescribeGroupResponseTypeDef",
+GetUserIdResponseTypeDef = TypedDict(
+    "GetUserIdResponseTypeDef",
     {
-        "GroupId": str,
-        "DisplayName": str,
-        "ExternalIds": List[ExternalIdOutputTypeDef],
-        "Description": str,
+        "UserId": str,
         "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGroupTypeDef = TypedDict(
-    "_RequiredGroupTypeDef",
+_RequiredCreateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateUserRequestRequestTypeDef",
     {
-        "GroupId": str,
         "IdentityStoreId": str,
     },
 )
-_OptionalGroupTypeDef = TypedDict(
-    "_OptionalGroupTypeDef",
+_OptionalCreateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateUserRequestRequestTypeDef",
     {
+        "UserName": str,
+        "Name": NameTypeDef,
         "DisplayName": str,
-        "ExternalIds": List[ExternalIdOutputTypeDef],
-        "Description": str,
+        "NickName": str,
+        "ProfileUrl": str,
+        "Emails": Sequence[EmailTypeDef],
+        "Addresses": Sequence[AddressTypeDef],
+        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
+        "UserType": str,
+        "Title": str,
+        "PreferredLanguage": str,
+        "Locale": str,
+        "Timezone": str,
     },
     total=False,
 )
 
 
-class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
+class CreateUserRequestRequestTypeDef(
+    _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
+):
     pass
 
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "UserName": str,
         "UserId": str,
-        "ExternalIds": List[ExternalIdOutputTypeDef],
-        "Name": NameOutputTypeDef,
+        "ExternalIds": List[ExternalIdTypeDef],
+        "Name": NameTypeDef,
         "DisplayName": str,
         "NickName": str,
         "ProfileUrl": str,
-        "Emails": List[EmailOutputTypeDef],
-        "Addresses": List[AddressOutputTypeDef],
-        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
+        "Emails": List[EmailTypeDef],
+        "Addresses": List[AddressTypeDef],
+        "PhoneNumbers": List[PhoneNumberTypeDef],
         "UserType": str,
         "Title": str,
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
         "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "UserId": str,
         "IdentityStoreId": str,
     },
 )
 _OptionalUserTypeDef = TypedDict(
     "_OptionalUserTypeDef",
     {
         "UserName": str,
-        "ExternalIds": List[ExternalIdOutputTypeDef],
-        "Name": NameOutputTypeDef,
+        "ExternalIds": List[ExternalIdTypeDef],
+        "Name": NameTypeDef,
         "DisplayName": str,
         "NickName": str,
         "ProfileUrl": str,
-        "Emails": List[EmailOutputTypeDef],
-        "Addresses": List[AddressOutputTypeDef],
-        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
+        "Emails": List[EmailTypeDef],
+        "Addresses": List[AddressTypeDef],
+        "PhoneNumbers": List[PhoneNumberTypeDef],
         "UserType": str,
         "Title": str,
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
     },
     total=False,
 )
 
 
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
 
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+_RequiredListGroupsRequestRequestTypeDef = TypedDict(
+    "_RequiredListGroupsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+_OptionalListGroupsRequestRequestTypeDef = TypedDict(
+    "_OptionalListGroupsRequestRequestTypeDef",
     {
+        "MaxResults": int,
+        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+class ListGroupsRequestRequestTypeDef(
+    _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListGroupsRequestRequestTypeDef = TypedDict(
-    "_RequiredListGroupsRequestRequestTypeDef",
+_RequiredListUsersRequestRequestTypeDef = TypedDict(
+    "_RequiredListUsersRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListGroupsRequestRequestTypeDef = TypedDict(
-    "_OptionalListGroupsRequestRequestTypeDef",
+_OptionalListUsersRequestRequestTypeDef = TypedDict(
+    "_OptionalListUsersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
 
-class ListGroupsRequestRequestTypeDef(
-    _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
+class ListUsersRequestRequestTypeDef(
+    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+        {
+            "IdentityStoreId": str,
+            "MemberId": MemberIdTypeDef,
+        },
+    )
+)
+_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
+    _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+    _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
     {
         "IdentityStoreId": str,
+        "GroupId": str,
     },
 )
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
+    _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+    _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "IdentityStoreId": str,
+    },
+)
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListUsersRequestRequestTypeDef = TypedDict(
-    "_RequiredListUsersRequestRequestTypeDef",
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListUsersRequestRequestTypeDef = TypedDict(
-    "_OptionalListUsersRequestRequestTypeDef",
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListUsersRequestRequestTypeDef(
-    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
 
+ListGroupsResponseTypeDef = TypedDict(
+    "ListGroupsResponseTypeDef",
+    {
+        "Groups": List[GroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetGroupIdRequestRequestTypeDef = TypedDict(
     "GetGroupIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "AlternateIdentifier": AlternateIdentifierTypeDef,
     },
 )
@@ -817,46 +756,37 @@
     },
 )
 
 IsMemberInGroupsResponseTypeDef = TypedDict(
     "IsMemberInGroupsResponseTypeDef",
     {
         "Results": List[GroupMembershipExistenceResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupMembershipsForMemberResponseTypeDef = TypedDict(
     "ListGroupMembershipsForMemberResponseTypeDef",
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupMembershipsResponseTypeDef = TypedDict(
     "ListGroupMembershipsResponseTypeDef",
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListGroupsResponseTypeDef = TypedDict(
-    "ListGroupsResponseTypeDef",
-    {
-        "Groups": List[GroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore/type_defs.pyi` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,104 +2,83 @@
 Type annotations for identitystore service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_identitystore.type_defs import AddressOutputTypeDef
+    from mypy_boto3_identitystore.type_defs import AddressTypeDef
 
-    data: AddressOutputTypeDef = {...}
+    data: AddressTypeDef = {...}
     ```
 """
 import sys
 from typing import Any, Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AddressOutputTypeDef",
     "AddressTypeDef",
     "ExternalIdTypeDef",
     "UniqueAttributeTypeDef",
     "AttributeOperationTypeDef",
     "MemberIdTypeDef",
-    "CreateGroupMembershipResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateGroupRequestRequestTypeDef",
-    "CreateGroupResponseTypeDef",
     "EmailTypeDef",
     "NameTypeDef",
     "PhoneNumberTypeDef",
-    "CreateUserResponseTypeDef",
     "DeleteGroupMembershipRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeGroupMembershipRequestRequestTypeDef",
-    "MemberIdOutputTypeDef",
     "DescribeGroupRequestRequestTypeDef",
-    "ExternalIdOutputTypeDef",
     "DescribeUserRequestRequestTypeDef",
-    "EmailOutputTypeDef",
-    "NameOutputTypeDef",
-    "PhoneNumberOutputTypeDef",
     "FilterTypeDef",
-    "GetGroupIdResponseTypeDef",
-    "GetGroupMembershipIdResponseTypeDef",
-    "GetUserIdResponseTypeDef",
-    "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
-    "ListGroupMembershipsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListGroupMembershipsRequestRequestTypeDef",
+    "GroupTypeDef",
     "AlternateIdentifierTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
     "GetGroupMembershipIdRequestRequestTypeDef",
+    "GroupMembershipExistenceResultTypeDef",
+    "GroupMembershipTypeDef",
     "IsMemberInGroupsRequestRequestTypeDef",
-    "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
     "ListGroupMembershipsForMemberRequestRequestTypeDef",
-    "CreateUserRequestRequestTypeDef",
+    "CreateGroupMembershipResponseTypeDef",
+    "CreateGroupResponseTypeDef",
+    "CreateUserResponseTypeDef",
     "DescribeGroupMembershipResponseTypeDef",
-    "GroupMembershipExistenceResultTypeDef",
-    "GroupMembershipTypeDef",
     "DescribeGroupResponseTypeDef",
-    "GroupTypeDef",
+    "GetGroupIdResponseTypeDef",
+    "GetGroupMembershipIdResponseTypeDef",
+    "GetUserIdResponseTypeDef",
+    "CreateUserRequestRequestTypeDef",
     "DescribeUserResponseTypeDef",
     "UserTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
+    "ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+    "ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
+    "ListGroupsResponseTypeDef",
     "GetGroupIdRequestRequestTypeDef",
     "GetUserIdRequestRequestTypeDef",
     "IsMemberInGroupsResponseTypeDef",
     "ListGroupMembershipsForMemberResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
-    "ListGroupsResponseTypeDef",
     "ListUsersResponseTypeDef",
 )
 
-AddressOutputTypeDef = TypedDict(
-    "AddressOutputTypeDef",
-    {
-        "StreetAddress": str,
-        "Locality": str,
-        "Region": str,
-        "PostalCode": str,
-        "Country": str,
-        "Formatted": str,
-        "Type": str,
-        "Primary": bool,
-    },
-    total=False,
-)
-
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "StreetAddress": str,
         "Locality": str,
         "Region": str,
         "PostalCode": str,
@@ -150,20 +129,22 @@
     "MemberIdTypeDef",
     {
         "UserId": str,
     },
     total=False,
 )
 
-CreateGroupMembershipResponseTypeDef = TypedDict(
-    "CreateGroupMembershipResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "MembershipId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
@@ -179,23 +160,14 @@
 )
 
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
-CreateGroupResponseTypeDef = TypedDict(
-    "CreateGroupResponseTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EmailTypeDef = TypedDict(
     "EmailTypeDef",
     {
         "Value": str,
         "Type": str,
         "Primary": bool,
     },
@@ -221,23 +193,14 @@
         "Value": str,
         "Type": str,
         "Primary": bool,
     },
     total=False,
 )
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "UserId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGroupMembershipRequestRequestTypeDef = TypedDict(
     "DeleteGroupMembershipRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MembershipId": str,
     },
 )
@@ -262,135 +225,48 @@
     "DescribeGroupMembershipRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MembershipId": str,
     },
 )
 
-MemberIdOutputTypeDef = TypedDict(
-    "MemberIdOutputTypeDef",
-    {
-        "UserId": str,
-    },
-    total=False,
-)
-
 DescribeGroupRequestRequestTypeDef = TypedDict(
     "DescribeGroupRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
     },
 )
 
-ExternalIdOutputTypeDef = TypedDict(
-    "ExternalIdOutputTypeDef",
-    {
-        "Issuer": str,
-        "Id": str,
-    },
-)
-
 DescribeUserRequestRequestTypeDef = TypedDict(
     "DescribeUserRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "UserId": str,
     },
 )
 
-EmailOutputTypeDef = TypedDict(
-    "EmailOutputTypeDef",
-    {
-        "Value": str,
-        "Type": str,
-        "Primary": bool,
-    },
-    total=False,
-)
-
-NameOutputTypeDef = TypedDict(
-    "NameOutputTypeDef",
-    {
-        "Formatted": str,
-        "FamilyName": str,
-        "GivenName": str,
-        "MiddleName": str,
-        "HonorificPrefix": str,
-        "HonorificSuffix": str,
-    },
-    total=False,
-)
-
-PhoneNumberOutputTypeDef = TypedDict(
-    "PhoneNumberOutputTypeDef",
-    {
-        "Value": str,
-        "Type": str,
-        "Primary": bool,
-    },
-    total=False,
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "AttributePath": str,
         "AttributeValue": str,
     },
 )
 
-GetGroupIdResponseTypeDef = TypedDict(
-    "GetGroupIdResponseTypeDef",
-    {
-        "GroupId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetGroupMembershipIdResponseTypeDef = TypedDict(
-    "GetGroupMembershipIdResponseTypeDef",
-    {
-        "MembershipId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetUserIdResponseTypeDef = TypedDict(
-    "GetUserIdResponseTypeDef",
-    {
-        "UserId": str,
-        "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
-    {
-        "IdentityStoreId": str,
-        "GroupId": str,
-    },
-)
-_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
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
 
-class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
-    _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-    _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-):
-    pass
-
 _RequiredListGroupMembershipsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "GroupId": str,
     },
 )
@@ -405,35 +281,34 @@
 
 class ListGroupMembershipsRequestRequestTypeDef(
     _RequiredListGroupMembershipsRequestRequestTypeDef,
     _OptionalListGroupMembershipsRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGroupTypeDef = TypedDict(
+    "_RequiredGroupTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "GroupId": str,
+        "IdentityStoreId": str,
     },
-    total=False,
 )
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_OptionalGroupTypeDef = TypedDict(
+    "_OptionalGroupTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DisplayName": str,
+        "ExternalIds": List[ExternalIdTypeDef],
+        "Description": str,
     },
+    total=False,
 )
 
+class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
+    pass
+
 AlternateIdentifierTypeDef = TypedDict(
     "AlternateIdentifierTypeDef",
     {
         "ExternalId": ExternalIdTypeDef,
         "UniqueAttribute": UniqueAttributeTypeDef,
     },
     total=False,
@@ -471,48 +346,52 @@
     {
         "IdentityStoreId": str,
         "GroupId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
 
-IsMemberInGroupsRequestRequestTypeDef = TypedDict(
-    "IsMemberInGroupsRequestRequestTypeDef",
+GroupMembershipExistenceResultTypeDef = TypedDict(
+    "GroupMembershipExistenceResultTypeDef",
     {
-        "IdentityStoreId": str,
+        "GroupId": str,
         "MemberId": MemberIdTypeDef,
-        "GroupIds": Sequence[str],
+        "MembershipExists": bool,
     },
+    total=False,
 )
 
-_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-        {
-            "IdentityStoreId": str,
-            "MemberId": MemberIdTypeDef,
-        },
-    )
+_RequiredGroupMembershipTypeDef = TypedDict(
+    "_RequiredGroupMembershipTypeDef",
+    {
+        "IdentityStoreId": str,
+    },
 )
-_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
+_OptionalGroupMembershipTypeDef = TypedDict(
+    "_OptionalGroupMembershipTypeDef",
+    {
+        "MembershipId": str,
+        "GroupId": str,
+        "MemberId": MemberIdTypeDef,
+    },
+    total=False,
 )
 
-class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
-    _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-    _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
-):
+class GroupMembershipTypeDef(_RequiredGroupMembershipTypeDef, _OptionalGroupMembershipTypeDef):
     pass
 
+IsMemberInGroupsRequestRequestTypeDef = TypedDict(
+    "IsMemberInGroupsRequestRequestTypeDef",
+    {
+        "IdentityStoreId": str,
+        "MemberId": MemberIdTypeDef,
+        "GroupIds": Sequence[str],
+    },
+)
+
 _RequiredListGroupMembershipsForMemberRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembershipsForMemberRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "MemberId": MemberIdTypeDef,
     },
 )
@@ -527,255 +406,315 @@
 
 class ListGroupMembershipsForMemberRequestRequestTypeDef(
     _RequiredListGroupMembershipsForMemberRequestRequestTypeDef,
     _OptionalListGroupMembershipsForMemberRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateUserRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateUserRequestRequestTypeDef",
+CreateGroupMembershipResponseTypeDef = TypedDict(
+    "CreateGroupMembershipResponseTypeDef",
     {
+        "MembershipId": str,
         "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateUserRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateUserRequestRequestTypeDef",
+
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
     {
-        "UserName": str,
-        "Name": NameTypeDef,
-        "DisplayName": str,
-        "NickName": str,
-        "ProfileUrl": str,
-        "Emails": Sequence[EmailTypeDef],
-        "Addresses": Sequence[AddressTypeDef],
-        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
-        "UserType": str,
-        "Title": str,
-        "PreferredLanguage": str,
-        "Locale": str,
-        "Timezone": str,
+        "GroupId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateUserRequestRequestTypeDef(
-    _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
-):
-    pass
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "UserId": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 DescribeGroupMembershipResponseTypeDef = TypedDict(
     "DescribeGroupMembershipResponseTypeDef",
     {
         "IdentityStoreId": str,
         "MembershipId": str,
         "GroupId": str,
-        "MemberId": MemberIdOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MemberId": MemberIdTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GroupMembershipExistenceResultTypeDef = TypedDict(
-    "GroupMembershipExistenceResultTypeDef",
+DescribeGroupResponseTypeDef = TypedDict(
+    "DescribeGroupResponseTypeDef",
     {
         "GroupId": str,
-        "MemberId": MemberIdOutputTypeDef,
-        "MembershipExists": bool,
+        "DisplayName": str,
+        "ExternalIds": List[ExternalIdTypeDef],
+        "Description": str,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredGroupMembershipTypeDef = TypedDict(
-    "_RequiredGroupMembershipTypeDef",
+GetGroupIdResponseTypeDef = TypedDict(
+    "GetGroupIdResponseTypeDef",
     {
+        "GroupId": str,
         "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGroupMembershipTypeDef = TypedDict(
-    "_OptionalGroupMembershipTypeDef",
+
+GetGroupMembershipIdResponseTypeDef = TypedDict(
+    "GetGroupMembershipIdResponseTypeDef",
     {
         "MembershipId": str,
-        "GroupId": str,
-        "MemberId": MemberIdOutputTypeDef,
+        "IdentityStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class GroupMembershipTypeDef(_RequiredGroupMembershipTypeDef, _OptionalGroupMembershipTypeDef):
-    pass
-
-DescribeGroupResponseTypeDef = TypedDict(
-    "DescribeGroupResponseTypeDef",
+GetUserIdResponseTypeDef = TypedDict(
+    "GetUserIdResponseTypeDef",
     {
-        "GroupId": str,
-        "DisplayName": str,
-        "ExternalIds": List[ExternalIdOutputTypeDef],
-        "Description": str,
+        "UserId": str,
         "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGroupTypeDef = TypedDict(
-    "_RequiredGroupTypeDef",
+_RequiredCreateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateUserRequestRequestTypeDef",
     {
-        "GroupId": str,
         "IdentityStoreId": str,
     },
 )
-_OptionalGroupTypeDef = TypedDict(
-    "_OptionalGroupTypeDef",
+_OptionalCreateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateUserRequestRequestTypeDef",
     {
+        "UserName": str,
+        "Name": NameTypeDef,
         "DisplayName": str,
-        "ExternalIds": List[ExternalIdOutputTypeDef],
-        "Description": str,
+        "NickName": str,
+        "ProfileUrl": str,
+        "Emails": Sequence[EmailTypeDef],
+        "Addresses": Sequence[AddressTypeDef],
+        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
+        "UserType": str,
+        "Title": str,
+        "PreferredLanguage": str,
+        "Locale": str,
+        "Timezone": str,
     },
     total=False,
 )
 
-class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
+class CreateUserRequestRequestTypeDef(
+    _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
+):
     pass
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "UserName": str,
         "UserId": str,
-        "ExternalIds": List[ExternalIdOutputTypeDef],
-        "Name": NameOutputTypeDef,
+        "ExternalIds": List[ExternalIdTypeDef],
+        "Name": NameTypeDef,
         "DisplayName": str,
         "NickName": str,
         "ProfileUrl": str,
-        "Emails": List[EmailOutputTypeDef],
-        "Addresses": List[AddressOutputTypeDef],
-        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
+        "Emails": List[EmailTypeDef],
+        "Addresses": List[AddressTypeDef],
+        "PhoneNumbers": List[PhoneNumberTypeDef],
         "UserType": str,
         "Title": str,
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
         "IdentityStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "UserId": str,
         "IdentityStoreId": str,
     },
 )
 _OptionalUserTypeDef = TypedDict(
     "_OptionalUserTypeDef",
     {
         "UserName": str,
-        "ExternalIds": List[ExternalIdOutputTypeDef],
-        "Name": NameOutputTypeDef,
+        "ExternalIds": List[ExternalIdTypeDef],
+        "Name": NameTypeDef,
         "DisplayName": str,
         "NickName": str,
         "ProfileUrl": str,
-        "Emails": List[EmailOutputTypeDef],
-        "Addresses": List[AddressOutputTypeDef],
-        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
+        "Emails": List[EmailTypeDef],
+        "Addresses": List[AddressTypeDef],
+        "PhoneNumbers": List[PhoneNumberTypeDef],
         "UserType": str,
         "Title": str,
         "PreferredLanguage": str,
         "Locale": str,
         "Timezone": str,
     },
     total=False,
 )
 
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+_RequiredListGroupsRequestRequestTypeDef = TypedDict(
+    "_RequiredListGroupsRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+_OptionalListGroupsRequestRequestTypeDef = TypedDict(
+    "_OptionalListGroupsRequestRequestTypeDef",
     {
+        "MaxResults": int,
+        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+class ListGroupsRequestRequestTypeDef(
+    _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListGroupsRequestRequestTypeDef = TypedDict(
-    "_RequiredListGroupsRequestRequestTypeDef",
+_RequiredListUsersRequestRequestTypeDef = TypedDict(
+    "_RequiredListUsersRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListGroupsRequestRequestTypeDef = TypedDict(
-    "_OptionalListGroupsRequestRequestTypeDef",
+_OptionalListUsersRequestRequestTypeDef = TypedDict(
+    "_OptionalListUsersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-class ListGroupsRequestRequestTypeDef(
-    _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
+class ListUsersRequestRequestTypeDef(
+    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+        {
+            "IdentityStoreId": str,
+            "MemberId": MemberIdTypeDef,
+        },
+    )
+)
+_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(
+    _RequiredListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+    _OptionalListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+):
+    pass
+
+_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
     {
         "IdentityStoreId": str,
+        "GroupId": str,
     },
 )
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(
+    _RequiredListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+    _OptionalListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+):
+    pass
+
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "IdentityStoreId": str,
+    },
+)
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
 ):
     pass
 
-_RequiredListUsersRequestRequestTypeDef = TypedDict(
-    "_RequiredListUsersRequestRequestTypeDef",
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "IdentityStoreId": str,
     },
 )
-_OptionalListUsersRequestRequestTypeDef = TypedDict(
-    "_OptionalListUsersRequestRequestTypeDef",
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListUsersRequestRequestTypeDef(
-    _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
+ListGroupsResponseTypeDef = TypedDict(
+    "ListGroupsResponseTypeDef",
+    {
+        "Groups": List[GroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetGroupIdRequestRequestTypeDef = TypedDict(
     "GetGroupIdRequestRequestTypeDef",
     {
         "IdentityStoreId": str,
         "AlternateIdentifier": AlternateIdentifierTypeDef,
     },
 )
@@ -788,46 +727,37 @@
     },
 )
 
 IsMemberInGroupsResponseTypeDef = TypedDict(
     "IsMemberInGroupsResponseTypeDef",
     {
         "Results": List[GroupMembershipExistenceResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupMembershipsForMemberResponseTypeDef = TypedDict(
     "ListGroupMembershipsForMemberResponseTypeDef",
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupMembershipsResponseTypeDef = TypedDict(
     "ListGroupMembershipsResponseTypeDef",
     {
         "GroupMemberships": List[GroupMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListGroupsResponseTypeDef = TypedDict(
-    "ListGroupsResponseTypeDef",
-    {
-        "Groups": List[GroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/PKG-INFO` & `mypy-boto3-identitystore-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-identitystore
-Version: 1.28.12
-Summary: Type annotations for boto3.IdentityStore 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 identitystore type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-identitystore"></a>
 
 # mypy-boto3-identitystore
 
 [![PyPI - mypy-boto3-identitystore](https://img.shields.io/pypi/v/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-identitystore.svg?color=blue)](https://pypi.org/project/mypy-boto3-identitystore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-identitystore)](https://pepy.tech/project/mypy-boto3-identitystore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IdentityStore 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
+[boto3.IdentityStore 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
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
 [mypy-boto3-identitystore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_identitystore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,77 +302,71 @@
 ### Typed dictionaries
 
 `mypy_boto3_identitystore.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_identitystore.type_defs import (
-    AddressOutputTypeDef,
     AddressTypeDef,
     ExternalIdTypeDef,
     UniqueAttributeTypeDef,
     AttributeOperationTypeDef,
     MemberIdTypeDef,
-    CreateGroupMembershipResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateGroupRequestRequestTypeDef,
-    CreateGroupResponseTypeDef,
     EmailTypeDef,
     NameTypeDef,
     PhoneNumberTypeDef,
-    CreateUserResponseTypeDef,
     DeleteGroupMembershipRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeGroupMembershipRequestRequestTypeDef,
-    MemberIdOutputTypeDef,
     DescribeGroupRequestRequestTypeDef,
-    ExternalIdOutputTypeDef,
     DescribeUserRequestRequestTypeDef,
-    EmailOutputTypeDef,
-    NameOutputTypeDef,
-    PhoneNumberOutputTypeDef,
     FilterTypeDef,
-    GetGroupIdResponseTypeDef,
-    GetGroupMembershipIdResponseTypeDef,
-    GetUserIdResponseTypeDef,
-    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
-    ListGroupMembershipsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListGroupMembershipsRequestRequestTypeDef,
+    GroupTypeDef,
     AlternateIdentifierTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     CreateGroupMembershipRequestRequestTypeDef,
     GetGroupMembershipIdRequestRequestTypeDef,
+    GroupMembershipExistenceResultTypeDef,
+    GroupMembershipTypeDef,
     IsMemberInGroupsRequestRequestTypeDef,
-    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
     ListGroupMembershipsForMemberRequestRequestTypeDef,
-    CreateUserRequestRequestTypeDef,
+    CreateGroupMembershipResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateUserResponseTypeDef,
     DescribeGroupMembershipResponseTypeDef,
-    GroupMembershipExistenceResultTypeDef,
-    GroupMembershipTypeDef,
     DescribeGroupResponseTypeDef,
-    GroupTypeDef,
+    GetGroupIdResponseTypeDef,
+    GetGroupMembershipIdResponseTypeDef,
+    GetUserIdResponseTypeDef,
+    CreateUserRequestRequestTypeDef,
     DescribeUserResponseTypeDef,
     UserTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
+    ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef,
+    ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListGroupsResponseTypeDef,
     GetGroupIdRequestRequestTypeDef,
     GetUserIdRequestRequestTypeDef,
     IsMemberInGroupsResponseTypeDef,
     ListGroupMembershipsForMemberResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
-    ListGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
 )
 
 
-def get_structure() -> AddressOutputTypeDef:
+def get_structure() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-identitystore-1.28.12/mypy_boto3_identitystore.egg-info/SOURCES.txt` & `mypy-boto3-identitystore-1.28.15/mypy_boto3_identitystore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-identitystore-1.28.12/setup.py` & `mypy-boto3-identitystore-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-identitystore",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_identitystore"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IdentityStore 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.IdentityStore 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

