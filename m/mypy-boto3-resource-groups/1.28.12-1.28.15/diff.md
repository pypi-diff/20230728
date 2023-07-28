# Comparing `tmp/mypy-boto3-resource-groups-1.28.12.tar.gz` & `tmp/mypy-boto3-resource-groups-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resource-groups-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
+gzip compressed data, was "mypy-boto3-resource-groups-1.28.15.tar", last modified: Fri Jul 28 20:43:34 2023, max compression
```

## Comparing `mypy-boto3-resource-groups-1.28.12.tar` & `mypy-boto3-resource-groups-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.365214 mypy-boto3-resource-groups-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15451 2023-07-27 11:49:30.357214 mypy-boto3-resource-groups-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.357214 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-27 11:44:40.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-07-27 11:44:40.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.357214 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15451 2023-07-27 11:49:30.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 11:49:30.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 11:49:30.000000 mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.365214 mypy-boto3-resource-groups-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-27 11:44:39.000000 mypy-boto3-resource-groups-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:34.181733 mypy-boto3-resource-groups-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-28 20:43:34.181733 mypy-boto3-resource-groups-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:34.181733 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16986 2023-07-28 20:37:00.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-07-28 20:37:00.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:34.181733 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15419 2023-07-28 20:43:33.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 20:43:33.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:33.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:43:33.000000 mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:34.181733 mypy-boto3-resource-groups-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-28 20:36:59.000000 mypy-boto3-resource-groups-1.28.15/setup.py
```

### Comparing `mypy-boto3-resource-groups-1.28.12/LICENSE` & `mypy-boto3-resource-groups-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.12/PKG-INFO` & `mypy-boto3-resource-groups-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-groups
-Version: 1.28.12
-Summary: Type annotations for boto3.ResourceGroups 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ResourceGroups 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-groups)](https://pepy.tech/project/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,15 +341,14 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
-    ResourceQueryOutputTypeDef,
     ResponseMetadataTypeDef,
     DeleteGroupInputRequestTypeDef,
     FailedResourceTypeDef,
     GetGroupConfigurationInputRequestTypeDef,
     GetGroupInputRequestTypeDef,
     GetGroupQueryInputRequestTypeDef,
     GetTagsInputRequestTypeDef,
@@ -365,17 +364,17 @@
     ResourceStatusTypeDef,
     QueryErrorTypeDef,
     TagInputRequestTypeDef,
     UngroupResourcesInputRequestTypeDef,
     UntagInputRequestTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateGroupInputRequestTypeDef,
+    GroupQueryTypeDef,
     SearchResourcesInputRequestTypeDef,
     UpdateGroupQueryInputRequestTypeDef,
-    GroupQueryTypeDef,
     DeleteGroupOutputTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetGroupOutputTypeDef,
     GetTagsOutputTypeDef,
     TagOutputTypeDef,
     UntagOutputTypeDef,
     UpdateAccountSettingsOutputTypeDef,
```

### Comparing `mypy-boto3-resource-groups-1.28.12/README.md` & `mypy-boto3-resource-groups-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-groups)](https://pepy.tech/project/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,15 +309,14 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
-    ResourceQueryOutputTypeDef,
     ResponseMetadataTypeDef,
     DeleteGroupInputRequestTypeDef,
     FailedResourceTypeDef,
     GetGroupConfigurationInputRequestTypeDef,
     GetGroupInputRequestTypeDef,
     GetGroupQueryInputRequestTypeDef,
     GetTagsInputRequestTypeDef,
@@ -333,17 +332,17 @@
     ResourceStatusTypeDef,
     QueryErrorTypeDef,
     TagInputRequestTypeDef,
     UngroupResourcesInputRequestTypeDef,
     UntagInputRequestTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateGroupInputRequestTypeDef,
+    GroupQueryTypeDef,
     SearchResourcesInputRequestTypeDef,
     UpdateGroupQueryInputRequestTypeDef,
-    GroupQueryTypeDef,
     DeleteGroupOutputTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetGroupOutputTypeDef,
     GetTagsOutputTypeDef,
     TagOutputTypeDef,
     UntagOutputTypeDef,
     UpdateAccountSettingsOutputTypeDef,
```

### Comparing `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/__init__.py` & `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/__init__.pyi` & `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/client.py` & `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/client.pyi` & `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/literals.py` & `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/literals.pyi` & `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/paginator.py` & `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/paginator.pyi` & `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/type_defs.py` & `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountSettingsTypeDef",
     "ResourceQueryTypeDef",
     "GroupTypeDef",
-    "ResourceQueryOutputTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
     "GetGroupConfigurationInputRequestTypeDef",
     "GetGroupInputRequestTypeDef",
     "GetGroupQueryInputRequestTypeDef",
     "GetTagsInputRequestTypeDef",
@@ -57,17 +56,17 @@
     "ResourceStatusTypeDef",
     "QueryErrorTypeDef",
     "TagInputRequestTypeDef",
     "UngroupResourcesInputRequestTypeDef",
     "UntagInputRequestTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateGroupInputRequestTypeDef",
+    "GroupQueryTypeDef",
     "SearchResourcesInputRequestTypeDef",
     "UpdateGroupQueryInputRequestTypeDef",
-    "GroupQueryTypeDef",
     "DeleteGroupOutputTypeDef",
     "GetAccountSettingsOutputTypeDef",
     "GetGroupOutputTypeDef",
     "GetTagsOutputTypeDef",
     "TagOutputTypeDef",
     "UntagOutputTypeDef",
     "UpdateAccountSettingsOutputTypeDef",
@@ -128,22 +127,14 @@
 )
 
 
 class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
     pass
 
 
-ResourceQueryOutputTypeDef = TypedDict(
-    "ResourceQueryOutputTypeDef",
-    {
-        "Type": QueryTypeType,
-        "Query": str,
-    },
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -361,14 +352,22 @@
         "GroupName": str,
         "Group": str,
         "Description": str,
     },
     total=False,
 )
 
+GroupQueryTypeDef = TypedDict(
+    "GroupQueryTypeDef",
+    {
+        "GroupName": str,
+        "ResourceQuery": ResourceQueryTypeDef,
+    },
+)
+
 _RequiredSearchResourcesInputRequestTypeDef = TypedDict(
     "_RequiredSearchResourcesInputRequestTypeDef",
     {
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
 _OptionalSearchResourcesInputRequestTypeDef = TypedDict(
@@ -405,22 +404,14 @@
 
 class UpdateGroupQueryInputRequestTypeDef(
     _RequiredUpdateGroupQueryInputRequestTypeDef, _OptionalUpdateGroupQueryInputRequestTypeDef
 ):
     pass
 
 
-GroupQueryTypeDef = TypedDict(
-    "GroupQueryTypeDef",
-    {
-        "GroupName": str,
-        "ResourceQuery": ResourceQueryOutputTypeDef,
-    },
-)
-
 DeleteGroupOutputTypeDef = TypedDict(
     "DeleteGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -710,15 +701,15 @@
     },
 )
 
 CreateGroupOutputTypeDef = TypedDict(
     "CreateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResourceQuery": ResourceQueryOutputTypeDef,
+        "ResourceQuery": ResourceQueryTypeDef,
         "Tags": Dict[str, str],
         "GroupConfiguration": GroupConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupConfigurationOutputTypeDef = TypedDict(
```

### Comparing `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups/type_defs.pyi` & `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountSettingsTypeDef",
     "ResourceQueryTypeDef",
     "GroupTypeDef",
-    "ResourceQueryOutputTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
     "GetGroupConfigurationInputRequestTypeDef",
     "GetGroupInputRequestTypeDef",
     "GetGroupQueryInputRequestTypeDef",
     "GetTagsInputRequestTypeDef",
@@ -56,17 +55,17 @@
     "ResourceStatusTypeDef",
     "QueryErrorTypeDef",
     "TagInputRequestTypeDef",
     "UngroupResourcesInputRequestTypeDef",
     "UntagInputRequestTypeDef",
     "UpdateAccountSettingsInputRequestTypeDef",
     "UpdateGroupInputRequestTypeDef",
+    "GroupQueryTypeDef",
     "SearchResourcesInputRequestTypeDef",
     "UpdateGroupQueryInputRequestTypeDef",
-    "GroupQueryTypeDef",
     "DeleteGroupOutputTypeDef",
     "GetAccountSettingsOutputTypeDef",
     "GetGroupOutputTypeDef",
     "GetTagsOutputTypeDef",
     "TagOutputTypeDef",
     "UntagOutputTypeDef",
     "UpdateAccountSettingsOutputTypeDef",
@@ -125,22 +124,14 @@
     },
     total=False,
 )
 
 class GroupTypeDef(_RequiredGroupTypeDef, _OptionalGroupTypeDef):
     pass
 
-ResourceQueryOutputTypeDef = TypedDict(
-    "ResourceQueryOutputTypeDef",
-    {
-        "Type": QueryTypeType,
-        "Query": str,
-    },
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -354,14 +345,22 @@
         "GroupName": str,
         "Group": str,
         "Description": str,
     },
     total=False,
 )
 
+GroupQueryTypeDef = TypedDict(
+    "GroupQueryTypeDef",
+    {
+        "GroupName": str,
+        "ResourceQuery": ResourceQueryTypeDef,
+    },
+)
+
 _RequiredSearchResourcesInputRequestTypeDef = TypedDict(
     "_RequiredSearchResourcesInputRequestTypeDef",
     {
         "ResourceQuery": ResourceQueryTypeDef,
     },
 )
 _OptionalSearchResourcesInputRequestTypeDef = TypedDict(
@@ -394,22 +393,14 @@
 )
 
 class UpdateGroupQueryInputRequestTypeDef(
     _RequiredUpdateGroupQueryInputRequestTypeDef, _OptionalUpdateGroupQueryInputRequestTypeDef
 ):
     pass
 
-GroupQueryTypeDef = TypedDict(
-    "GroupQueryTypeDef",
-    {
-        "GroupName": str,
-        "ResourceQuery": ResourceQueryOutputTypeDef,
-    },
-)
-
 DeleteGroupOutputTypeDef = TypedDict(
     "DeleteGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -691,15 +682,15 @@
     },
 )
 
 CreateGroupOutputTypeDef = TypedDict(
     "CreateGroupOutputTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResourceQuery": ResourceQueryOutputTypeDef,
+        "ResourceQuery": ResourceQueryTypeDef,
         "Tags": Dict[str, str],
         "GroupConfiguration": GroupConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupConfigurationOutputTypeDef = TypedDict(
```

### Comparing `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/PKG-INFO` & `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-groups
-Version: 1.28.12
-Summary: Type annotations for boto3.ResourceGroups 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ResourceGroups 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-groups.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-groups)](https://pepy.tech/project/mypy-boto3-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceGroups 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[boto3.ResourceGroups 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
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
 [mypy-boto3-resource-groups docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_groups/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,15 +341,14 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resource_groups.type_defs import (
     AccountSettingsTypeDef,
     ResourceQueryTypeDef,
     GroupTypeDef,
-    ResourceQueryOutputTypeDef,
     ResponseMetadataTypeDef,
     DeleteGroupInputRequestTypeDef,
     FailedResourceTypeDef,
     GetGroupConfigurationInputRequestTypeDef,
     GetGroupInputRequestTypeDef,
     GetGroupQueryInputRequestTypeDef,
     GetTagsInputRequestTypeDef,
@@ -365,17 +364,17 @@
     ResourceStatusTypeDef,
     QueryErrorTypeDef,
     TagInputRequestTypeDef,
     UngroupResourcesInputRequestTypeDef,
     UntagInputRequestTypeDef,
     UpdateAccountSettingsInputRequestTypeDef,
     UpdateGroupInputRequestTypeDef,
+    GroupQueryTypeDef,
     SearchResourcesInputRequestTypeDef,
     UpdateGroupQueryInputRequestTypeDef,
-    GroupQueryTypeDef,
     DeleteGroupOutputTypeDef,
     GetAccountSettingsOutputTypeDef,
     GetGroupOutputTypeDef,
     GetTagsOutputTypeDef,
     TagOutputTypeDef,
     UntagOutputTypeDef,
     UpdateAccountSettingsOutputTypeDef,
```

### Comparing `mypy-boto3-resource-groups-1.28.12/mypy_boto3_resource_groups.egg-info/SOURCES.txt` & `mypy-boto3-resource-groups-1.28.15/mypy_boto3_resource_groups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-groups-1.28.12/setup.py` & `mypy-boto3-resource-groups-1.28.15/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resource-groups",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_resource_groups"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResourceGroups 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ResourceGroups 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

