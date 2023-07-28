# Comparing `tmp/mypy-boto3-rolesanywhere-1.28.12.tar.gz` & `tmp/mypy-boto3-rolesanywhere-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rolesanywhere-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
+gzip compressed data, was "mypy-boto3-rolesanywhere-1.28.15.tar", last modified: Fri Jul 28 20:43:35 2023, max compression
```

## Comparing `mypy-boto3-rolesanywhere-1.28.12.tar` & `mypy-boto3-rolesanywhere-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.689217 mypy-boto3-rolesanywhere-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-07-27 11:49:30.681217 mypy-boto3-rolesanywhere-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13534 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.681217 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20567 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-07-27 11:44:48.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.681217 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15048 2023-07-27 11:49:30.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 11:49:30.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:49:30.000000 mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.689217 mypy-boto3-rolesanywhere-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-27 11:44:47.000000 mypy-boto3-rolesanywhere-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:35.721754 mypy-boto3-rolesanywhere-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:05.000000 mypy-boto3-rolesanywhere-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14972 2023-07-28 20:43:35.717754 mypy-boto3-rolesanywhere-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-07-28 20:37:05.000000 mypy-boto3-rolesanywhere-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:35.709754 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-28 20:37:05.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-28 20:37:05.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-28 20:37:05.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20567 2023-07-28 20:37:06.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-07-28 20:37:05.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-28 20:37:06.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-28 20:37:06.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-28 20:37:06.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-07-28 20:37:06.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:05.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-07-28 20:37:06.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15289 2023-07-28 20:37:06.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:05.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:35.717754 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14972 2023-07-28 20:43:35.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:43:35.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:35.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:35.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:35.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:43:35.000000 mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:35.721754 mypy-boto3-rolesanywhere-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-28 20:37:05.000000 mypy-boto3-rolesanywhere-1.28.15/setup.py
```

### Comparing `mypy-boto3-rolesanywhere-1.28.12/LICENSE` & `mypy-boto3-rolesanywhere-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.12/PKG-INFO` & `mypy-boto3-rolesanywhere-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.28.12
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [mypy-boto3-rolesanywhere docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,47 +345,44 @@
     ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
     PaginatorConfigTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     NotificationSettingDetailTypeDef,
     NotificationSettingKeyTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
-    SourceDataOutputTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
     ListRequestListCrlsPaginateTypeDef,
     ListRequestListProfilesPaginateTypeDef,
     ListRequestListSubjectsPaginateTypeDef,
     ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ResetNotificationSettingsRequestRequestTypeDef,
-    SourceOutputTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
-    TrustAnchorDetailTypeDef,
     CreateTrustAnchorRequestRequestTypeDef,
+    TrustAnchorDetailTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
     ListTrustAnchorsResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
```

### Comparing `mypy-boto3-rolesanywhere-1.28.12/README.md` & `mypy-boto3-rolesanywhere-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [mypy-boto3-rolesanywhere docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,47 +313,44 @@
     ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
     PaginatorConfigTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     NotificationSettingDetailTypeDef,
     NotificationSettingKeyTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
-    SourceDataOutputTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
     ListRequestListCrlsPaginateTypeDef,
     ListRequestListProfilesPaginateTypeDef,
     ListRequestListSubjectsPaginateTypeDef,
     ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ResetNotificationSettingsRequestRequestTypeDef,
-    SourceOutputTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
-    TrustAnchorDetailTypeDef,
     CreateTrustAnchorRequestRequestTypeDef,
+    TrustAnchorDetailTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
     ListTrustAnchorsResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
```

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/__init__.py` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/__init__.pyi` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/__main__.py` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IAMRolesAnywhere 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IAMRolesAnywhere 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere\nOther"
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

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/client.py` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/client.pyi` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/literals.py` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/literals.pyi` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/paginator.py` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/paginator.pyi` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/type_defs.py` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,47 +37,44 @@
     "ResponseMetadataTypeDef",
     "InstancePropertyTypeDef",
     "ProfileDetailTypeDef",
     "PaginatorConfigTypeDef",
     "ListRequestRequestTypeDef",
     "SubjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "NotificationSettingDetailTypeDef",
     "NotificationSettingKeyTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
-    "SourceDataOutputTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCrlRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "SubjectDetailTypeDef",
     "ListProfilesResponseTypeDef",
     "ProfileDetailResponseTypeDef",
     "ListRequestListCrlsPaginateTypeDef",
     "ListRequestListProfilesPaginateTypeDef",
     "ListRequestListSubjectsPaginateTypeDef",
     "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListSubjectsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ResetNotificationSettingsRequestRequestTypeDef",
-    "SourceOutputTypeDef",
     "SourceTypeDef",
     "SubjectDetailResponseTypeDef",
-    "TrustAnchorDetailTypeDef",
     "CreateTrustAnchorRequestRequestTypeDef",
+    "TrustAnchorDetailTypeDef",
     "UpdateTrustAnchorRequestRequestTypeDef",
     "ListTrustAnchorsResponseTypeDef",
     "PutNotificationSettingsResponseTypeDef",
     "ResetNotificationSettingsResponseTypeDef",
     "TrustAnchorDetailResponseTypeDef",
 )
 
@@ -216,22 +213,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 _RequiredNotificationSettingDetailTypeDef = TypedDict(
     "_RequiredNotificationSettingDetailTypeDef",
     {
         "enabled": bool,
         "event": NotificationEventType,
     },
 )
@@ -297,23 +286,14 @@
 ScalarTrustAnchorRequestRequestTypeDef = TypedDict(
     "ScalarTrustAnchorRequestRequestTypeDef",
     {
         "trustAnchorId": str,
     },
 )
 
-SourceDataOutputTypeDef = TypedDict(
-    "SourceDataOutputTypeDef",
-    {
-        "acmPcaArn": str,
-        "x509CertificateData": str,
-    },
-    total=False,
-)
-
 SourceDataTypeDef = TypedDict(
     "SourceDataTypeDef",
     {
         "acmPcaArn": str,
         "x509CertificateData": str,
     },
     total=False,
@@ -454,14 +434,22 @@
     {
         "crls": List[CrlDetailTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SubjectDetailTypeDef = TypedDict(
     "SubjectDetailTypeDef",
     {
         "createdAt": datetime,
         "credentials": List[CredentialSummaryTypeDef],
         "enabled": bool,
         "instanceProperties": List[InstancePropertyTypeDef],
@@ -532,39 +520,22 @@
     {
         "nextToken": str,
         "subjects": List[SubjectSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ResetNotificationSettingsRequestRequestTypeDef = TypedDict(
     "ResetNotificationSettingsRequestRequestTypeDef",
     {
         "notificationSettingKeys": Sequence[NotificationSettingKeyTypeDef],
         "trustAnchorId": str,
     },
 )
 
-SourceOutputTypeDef = TypedDict(
-    "SourceOutputTypeDef",
-    {
-        "sourceData": SourceDataOutputTypeDef,
-        "sourceType": TrustAnchorTypeType,
-    },
-    total=False,
-)
-
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "sourceData": SourceDataTypeDef,
         "sourceType": TrustAnchorTypeType,
     },
     total=False,
@@ -574,29 +545,14 @@
     "SubjectDetailResponseTypeDef",
     {
         "subject": SubjectDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TrustAnchorDetailTypeDef = TypedDict(
-    "TrustAnchorDetailTypeDef",
-    {
-        "createdAt": datetime,
-        "enabled": bool,
-        "name": str,
-        "notificationSettings": List[NotificationSettingDetailTypeDef],
-        "source": SourceOutputTypeDef,
-        "trustAnchorArn": str,
-        "trustAnchorId": str,
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustAnchorRequestRequestTypeDef",
     {
         "name": str,
         "source": SourceTypeDef,
     },
 )
@@ -613,14 +569,29 @@
 
 class CreateTrustAnchorRequestRequestTypeDef(
     _RequiredCreateTrustAnchorRequestRequestTypeDef, _OptionalCreateTrustAnchorRequestRequestTypeDef
 ):
     pass
 
 
+TrustAnchorDetailTypeDef = TypedDict(
+    "TrustAnchorDetailTypeDef",
+    {
+        "createdAt": datetime,
+        "enabled": bool,
+        "name": str,
+        "notificationSettings": List[NotificationSettingDetailTypeDef],
+        "source": SourceTypeDef,
+        "trustAnchorArn": str,
+        "trustAnchorId": str,
+        "updatedAt": datetime,
+    },
+    total=False,
+)
+
 _RequiredUpdateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrustAnchorRequestRequestTypeDef",
     {
         "trustAnchorId": str,
     },
 )
 _OptionalUpdateTrustAnchorRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere/type_defs.pyi` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -36,47 +36,44 @@
     "ResponseMetadataTypeDef",
     "InstancePropertyTypeDef",
     "ProfileDetailTypeDef",
     "PaginatorConfigTypeDef",
     "ListRequestRequestTypeDef",
     "SubjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "NotificationSettingDetailTypeDef",
     "NotificationSettingKeyTypeDef",
     "ScalarCrlRequestRequestTypeDef",
     "ScalarProfileRequestRequestTypeDef",
     "ScalarSubjectRequestRequestTypeDef",
     "ScalarTrustAnchorRequestRequestTypeDef",
-    "SourceDataOutputTypeDef",
     "SourceDataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCrlRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "ImportCrlRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "PutNotificationSettingsRequestRequestTypeDef",
     "CrlDetailResponseTypeDef",
     "ListCrlsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "SubjectDetailTypeDef",
     "ListProfilesResponseTypeDef",
     "ProfileDetailResponseTypeDef",
     "ListRequestListCrlsPaginateTypeDef",
     "ListRequestListProfilesPaginateTypeDef",
     "ListRequestListSubjectsPaginateTypeDef",
     "ListRequestListTrustAnchorsPaginateTypeDef",
     "ListSubjectsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ResetNotificationSettingsRequestRequestTypeDef",
-    "SourceOutputTypeDef",
     "SourceTypeDef",
     "SubjectDetailResponseTypeDef",
-    "TrustAnchorDetailTypeDef",
     "CreateTrustAnchorRequestRequestTypeDef",
+    "TrustAnchorDetailTypeDef",
     "UpdateTrustAnchorRequestRequestTypeDef",
     "ListTrustAnchorsResponseTypeDef",
     "PutNotificationSettingsResponseTypeDef",
     "ResetNotificationSettingsResponseTypeDef",
     "TrustAnchorDetailResponseTypeDef",
 )
 
@@ -213,22 +210,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 _RequiredNotificationSettingDetailTypeDef = TypedDict(
     "_RequiredNotificationSettingDetailTypeDef",
     {
         "enabled": bool,
         "event": NotificationEventType,
     },
 )
@@ -290,23 +279,14 @@
 ScalarTrustAnchorRequestRequestTypeDef = TypedDict(
     "ScalarTrustAnchorRequestRequestTypeDef",
     {
         "trustAnchorId": str,
     },
 )
 
-SourceDataOutputTypeDef = TypedDict(
-    "SourceDataOutputTypeDef",
-    {
-        "acmPcaArn": str,
-        "x509CertificateData": str,
-    },
-    total=False,
-)
-
 SourceDataTypeDef = TypedDict(
     "SourceDataTypeDef",
     {
         "acmPcaArn": str,
         "x509CertificateData": str,
     },
     total=False,
@@ -439,14 +419,22 @@
     {
         "crls": List[CrlDetailTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 SubjectDetailTypeDef = TypedDict(
     "SubjectDetailTypeDef",
     {
         "createdAt": datetime,
         "credentials": List[CredentialSummaryTypeDef],
         "enabled": bool,
         "instanceProperties": List[InstancePropertyTypeDef],
@@ -517,39 +505,22 @@
     {
         "nextToken": str,
         "subjects": List[SubjectSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ResetNotificationSettingsRequestRequestTypeDef = TypedDict(
     "ResetNotificationSettingsRequestRequestTypeDef",
     {
         "notificationSettingKeys": Sequence[NotificationSettingKeyTypeDef],
         "trustAnchorId": str,
     },
 )
 
-SourceOutputTypeDef = TypedDict(
-    "SourceOutputTypeDef",
-    {
-        "sourceData": SourceDataOutputTypeDef,
-        "sourceType": TrustAnchorTypeType,
-    },
-    total=False,
-)
-
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "sourceData": SourceDataTypeDef,
         "sourceType": TrustAnchorTypeType,
     },
     total=False,
@@ -559,29 +530,14 @@
     "SubjectDetailResponseTypeDef",
     {
         "subject": SubjectDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TrustAnchorDetailTypeDef = TypedDict(
-    "TrustAnchorDetailTypeDef",
-    {
-        "createdAt": datetime,
-        "enabled": bool,
-        "name": str,
-        "notificationSettings": List[NotificationSettingDetailTypeDef],
-        "source": SourceOutputTypeDef,
-        "trustAnchorArn": str,
-        "trustAnchorId": str,
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustAnchorRequestRequestTypeDef",
     {
         "name": str,
         "source": SourceTypeDef,
     },
 )
@@ -596,14 +552,29 @@
 )
 
 class CreateTrustAnchorRequestRequestTypeDef(
     _RequiredCreateTrustAnchorRequestRequestTypeDef, _OptionalCreateTrustAnchorRequestRequestTypeDef
 ):
     pass
 
+TrustAnchorDetailTypeDef = TypedDict(
+    "TrustAnchorDetailTypeDef",
+    {
+        "createdAt": datetime,
+        "enabled": bool,
+        "name": str,
+        "notificationSettings": List[NotificationSettingDetailTypeDef],
+        "source": SourceTypeDef,
+        "trustAnchorArn": str,
+        "trustAnchorId": str,
+        "updatedAt": datetime,
+    },
+    total=False,
+)
+
 _RequiredUpdateTrustAnchorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrustAnchorRequestRequestTypeDef",
     {
         "trustAnchorId": str,
     },
 )
 _OptionalUpdateTrustAnchorRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/PKG-INFO` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.28.12
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
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
 [mypy-boto3-rolesanywhere docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,47 +345,44 @@
     ResponseMetadataTypeDef,
     InstancePropertyTypeDef,
     ProfileDetailTypeDef,
     PaginatorConfigTypeDef,
     ListRequestRequestTypeDef,
     SubjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     NotificationSettingDetailTypeDef,
     NotificationSettingKeyTypeDef,
     ScalarCrlRequestRequestTypeDef,
     ScalarProfileRequestRequestTypeDef,
     ScalarSubjectRequestRequestTypeDef,
     ScalarTrustAnchorRequestRequestTypeDef,
-    SourceDataOutputTypeDef,
     SourceDataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCrlRequestRequestTypeDef,
     UpdateProfileRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     ImportCrlRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     PutNotificationSettingsRequestRequestTypeDef,
     CrlDetailResponseTypeDef,
     ListCrlsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SubjectDetailTypeDef,
     ListProfilesResponseTypeDef,
     ProfileDetailResponseTypeDef,
     ListRequestListCrlsPaginateTypeDef,
     ListRequestListProfilesPaginateTypeDef,
     ListRequestListSubjectsPaginateTypeDef,
     ListRequestListTrustAnchorsPaginateTypeDef,
     ListSubjectsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ResetNotificationSettingsRequestRequestTypeDef,
-    SourceOutputTypeDef,
     SourceTypeDef,
     SubjectDetailResponseTypeDef,
-    TrustAnchorDetailTypeDef,
     CreateTrustAnchorRequestRequestTypeDef,
+    TrustAnchorDetailTypeDef,
     UpdateTrustAnchorRequestRequestTypeDef,
     ListTrustAnchorsResponseTypeDef,
     PutNotificationSettingsResponseTypeDef,
     ResetNotificationSettingsResponseTypeDef,
     TrustAnchorDetailResponseTypeDef,
 )
```

### Comparing `mypy-boto3-rolesanywhere-1.28.12/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt` & `mypy-boto3-rolesanywhere-1.28.15/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.28.12/setup.py` & `mypy-boto3-rolesanywhere-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rolesanywhere",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_rolesanywhere"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IAMRolesAnywhere 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.IAMRolesAnywhere 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

