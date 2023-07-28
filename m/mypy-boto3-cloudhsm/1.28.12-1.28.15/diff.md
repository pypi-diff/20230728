# Comparing `tmp/mypy-boto3-cloudhsm-1.28.12.tar.gz` & `tmp/mypy-boto3-cloudhsm-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudhsm-1.28.12.tar", last modified: Thu Jul 27 05:34:25 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudhsm-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
```

## Comparing `mypy-boto3-cloudhsm-1.28.12.tar` & `mypy-boto3-cloudhsm-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.140562 mypy-boto3-cloudhsm-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-07-27 05:34:25.136562 mypy-boto3-cloudhsm-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.136562 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12773 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.136562 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:25.140562 mypy-boto3-cloudhsm-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:18:42.000000 mypy-boto3-cloudhsm-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.508782 mypy-boto3-cloudhsm-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:57.000000 mypy-boto3-cloudhsm-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-07-28 20:42:25.508782 mypy-boto3-cloudhsm-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-07-28 20:20:57.000000 mypy-boto3-cloudhsm-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.500782 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:20:57.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-28 20:20:57.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:20:57.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15153 2023-07-28 20:20:58.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-28 20:20:57.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-07-28 20:20:58.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-28 20:20:58.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-28 20:20:58.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-28 20:20:58.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:57.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-07-28 20:20:58.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-07-28 20:20:58.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:57.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.508782 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-07-28 20:42:25.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:42:25.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:25.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:42:25.000000 mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.508782 mypy-boto3-cloudhsm-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:20:57.000000 mypy-boto3-cloudhsm-1.28.15/setup.py
```

### Comparing `mypy-boto3-cloudhsm-1.28.12/LICENSE` & `mypy-boto3-cloudhsm-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.12/PKG-INFO` & `mypy-boto3-cloudhsm-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudhsm
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudHSM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudHSM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudhsm)](https://pepy.tech/project/mypy-boto3-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[boto3.CloudHSM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [mypy-boto3-cloudhsm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,59 +331,58 @@
 
 `mypy_boto3_cloudhsm.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudhsm.type_defs import (
     TagTypeDef,
-    AddTagsToResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateHapgRequestRequestTypeDef,
-    CreateHapgResponseTypeDef,
     CreateHsmRequestRequestTypeDef,
-    CreateHsmResponseTypeDef,
     CreateLunaClientRequestRequestTypeDef,
-    CreateLunaClientResponseTypeDef,
     DeleteHapgRequestRequestTypeDef,
-    DeleteHapgResponseTypeDef,
     DeleteHsmRequestRequestTypeDef,
-    DeleteHsmResponseTypeDef,
     DeleteLunaClientRequestRequestTypeDef,
-    DeleteLunaClientResponseTypeDef,
     DescribeHapgRequestRequestTypeDef,
-    DescribeHapgResponseTypeDef,
     DescribeHsmRequestRequestTypeDef,
-    DescribeHsmResponseTypeDef,
     DescribeLunaClientRequestRequestTypeDef,
-    DescribeLunaClientResponseTypeDef,
     GetConfigRequestRequestTypeDef,
-    GetConfigResponseTypeDef,
-    ListAvailableZonesResponseTypeDef,
-    ListHapgsRequestListHapgsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListHapgsRequestRequestTypeDef,
-    ListHapgsResponseTypeDef,
-    ListHsmsRequestListHsmsPaginateTypeDef,
     ListHsmsRequestRequestTypeDef,
-    ListHsmsResponseTypeDef,
-    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
     ListLunaClientsRequestRequestTypeDef,
-    ListLunaClientsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ModifyHapgRequestRequestTypeDef,
-    ModifyHapgResponseTypeDef,
     ModifyHsmRequestRequestTypeDef,
-    ModifyHsmResponseTypeDef,
     ModifyLunaClientRequestRequestTypeDef,
-    ModifyLunaClientResponseTypeDef,
-    PaginatorConfigTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
-    RemoveTagsFromResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
+    AddTagsToResourceResponseTypeDef,
+    CreateHapgResponseTypeDef,
+    CreateHsmResponseTypeDef,
+    CreateLunaClientResponseTypeDef,
+    DeleteHapgResponseTypeDef,
+    DeleteHsmResponseTypeDef,
+    DeleteLunaClientResponseTypeDef,
+    DescribeHapgResponseTypeDef,
+    DescribeHsmResponseTypeDef,
+    DescribeLunaClientResponseTypeDef,
+    GetConfigResponseTypeDef,
+    ListAvailableZonesResponseTypeDef,
+    ListHapgsResponseTypeDef,
+    ListHsmsResponseTypeDef,
+    ListLunaClientsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ModifyHapgResponseTypeDef,
+    ModifyHsmResponseTypeDef,
+    ModifyLunaClientResponseTypeDef,
+    RemoveTagsFromResourceResponseTypeDef,
+    ListHapgsRequestListHapgsPaginateTypeDef,
+    ListHsmsRequestListHsmsPaginateTypeDef,
+    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cloudhsm-1.28.12/README.md` & `mypy-boto3-cloudhsm-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudhsm)](https://pepy.tech/project/mypy-boto3-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[boto3.CloudHSM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [mypy-boto3-cloudhsm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,59 +299,58 @@
 
 `mypy_boto3_cloudhsm.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudhsm.type_defs import (
     TagTypeDef,
-    AddTagsToResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateHapgRequestRequestTypeDef,
-    CreateHapgResponseTypeDef,
     CreateHsmRequestRequestTypeDef,
-    CreateHsmResponseTypeDef,
     CreateLunaClientRequestRequestTypeDef,
-    CreateLunaClientResponseTypeDef,
     DeleteHapgRequestRequestTypeDef,
-    DeleteHapgResponseTypeDef,
     DeleteHsmRequestRequestTypeDef,
-    DeleteHsmResponseTypeDef,
     DeleteLunaClientRequestRequestTypeDef,
-    DeleteLunaClientResponseTypeDef,
     DescribeHapgRequestRequestTypeDef,
-    DescribeHapgResponseTypeDef,
     DescribeHsmRequestRequestTypeDef,
-    DescribeHsmResponseTypeDef,
     DescribeLunaClientRequestRequestTypeDef,
-    DescribeLunaClientResponseTypeDef,
     GetConfigRequestRequestTypeDef,
-    GetConfigResponseTypeDef,
-    ListAvailableZonesResponseTypeDef,
-    ListHapgsRequestListHapgsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListHapgsRequestRequestTypeDef,
-    ListHapgsResponseTypeDef,
-    ListHsmsRequestListHsmsPaginateTypeDef,
     ListHsmsRequestRequestTypeDef,
-    ListHsmsResponseTypeDef,
-    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
     ListLunaClientsRequestRequestTypeDef,
-    ListLunaClientsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ModifyHapgRequestRequestTypeDef,
-    ModifyHapgResponseTypeDef,
     ModifyHsmRequestRequestTypeDef,
-    ModifyHsmResponseTypeDef,
     ModifyLunaClientRequestRequestTypeDef,
-    ModifyLunaClientResponseTypeDef,
-    PaginatorConfigTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
-    RemoveTagsFromResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
+    AddTagsToResourceResponseTypeDef,
+    CreateHapgResponseTypeDef,
+    CreateHsmResponseTypeDef,
+    CreateLunaClientResponseTypeDef,
+    DeleteHapgResponseTypeDef,
+    DeleteHsmResponseTypeDef,
+    DeleteLunaClientResponseTypeDef,
+    DescribeHapgResponseTypeDef,
+    DescribeHsmResponseTypeDef,
+    DescribeLunaClientResponseTypeDef,
+    GetConfigResponseTypeDef,
+    ListAvailableZonesResponseTypeDef,
+    ListHapgsResponseTypeDef,
+    ListHsmsResponseTypeDef,
+    ListLunaClientsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ModifyHapgResponseTypeDef,
+    ModifyHsmResponseTypeDef,
+    ModifyLunaClientResponseTypeDef,
+    RemoveTagsFromResourceResponseTypeDef,
+    ListHapgsRequestListHapgsPaginateTypeDef,
+    ListHsmsRequestListHsmsPaginateTypeDef,
+    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/__init__.py` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/__init__.pyi` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/__main__.py` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudHSM 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudHSM 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM\nOther"
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

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/client.py` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/client.pyi` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/literals.py` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/literals.pyi` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/paginator.py` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/paginator.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,43 +50,43 @@
 class ListHapgsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhapgspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHapgsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhapgspaginator)
         """
 
 
 class ListHsmsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhsmspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHsmsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhsmspaginator)
         """
 
 
 class ListLunaClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listlunaclientspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLunaClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listlunaclientspaginator)
         """
```

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/paginator.pyi` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/paginator.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -47,41 +47,41 @@
 class ListHapgsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhapgspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHapgsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhapgspaginator)
         """
 
 class ListHsmsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhsmspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHsmsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listhsmspaginator)
         """
 
 class ListLunaClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listlunaclientspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLunaClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/paginators/#listlunaclientspaginator)
         """
```

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/type_defs.py` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,92 +24,86 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "AddTagsToResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateHapgRequestRequestTypeDef",
-    "CreateHapgResponseTypeDef",
     "CreateHsmRequestRequestTypeDef",
-    "CreateHsmResponseTypeDef",
     "CreateLunaClientRequestRequestTypeDef",
-    "CreateLunaClientResponseTypeDef",
     "DeleteHapgRequestRequestTypeDef",
-    "DeleteHapgResponseTypeDef",
     "DeleteHsmRequestRequestTypeDef",
-    "DeleteHsmResponseTypeDef",
     "DeleteLunaClientRequestRequestTypeDef",
-    "DeleteLunaClientResponseTypeDef",
     "DescribeHapgRequestRequestTypeDef",
-    "DescribeHapgResponseTypeDef",
     "DescribeHsmRequestRequestTypeDef",
-    "DescribeHsmResponseTypeDef",
     "DescribeLunaClientRequestRequestTypeDef",
-    "DescribeLunaClientResponseTypeDef",
     "GetConfigRequestRequestTypeDef",
-    "GetConfigResponseTypeDef",
-    "ListAvailableZonesResponseTypeDef",
-    "ListHapgsRequestListHapgsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListHapgsRequestRequestTypeDef",
-    "ListHapgsResponseTypeDef",
-    "ListHsmsRequestListHsmsPaginateTypeDef",
     "ListHsmsRequestRequestTypeDef",
-    "ListHsmsResponseTypeDef",
-    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
     "ListLunaClientsRequestRequestTypeDef",
-    "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ModifyHapgRequestRequestTypeDef",
-    "ModifyHapgResponseTypeDef",
     "ModifyHsmRequestRequestTypeDef",
-    "ModifyHsmResponseTypeDef",
     "ModifyLunaClientRequestRequestTypeDef",
-    "ModifyLunaClientResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
-    "RemoveTagsFromResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
+    "AddTagsToResourceResponseTypeDef",
+    "CreateHapgResponseTypeDef",
+    "CreateHsmResponseTypeDef",
+    "CreateLunaClientResponseTypeDef",
+    "DeleteHapgResponseTypeDef",
+    "DeleteHsmResponseTypeDef",
+    "DeleteLunaClientResponseTypeDef",
+    "DescribeHapgResponseTypeDef",
+    "DescribeHsmResponseTypeDef",
+    "DescribeLunaClientResponseTypeDef",
+    "GetConfigResponseTypeDef",
+    "ListAvailableZonesResponseTypeDef",
+    "ListHapgsResponseTypeDef",
+    "ListHsmsResponseTypeDef",
+    "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ModifyHapgResponseTypeDef",
+    "ModifyHsmResponseTypeDef",
+    "ModifyLunaClientResponseTypeDef",
+    "RemoveTagsFromResourceResponseTypeDef",
+    "ListHapgsRequestListHapgsPaginateTypeDef",
+    "ListHsmsRequestListHsmsPaginateTypeDef",
+    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-AddTagsToResourceResponseTypeDef = TypedDict(
-    "AddTagsToResourceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateHapgRequestRequestTypeDef = TypedDict(
     "CreateHapgRequestRequestTypeDef",
     {
         "Label": str,
     },
 )
 
-CreateHapgResponseTypeDef = TypedDict(
-    "CreateHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateHsmRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHsmRequestRequestTypeDef",
     {
         "SubnetId": str,
         "SshKey": str,
         "IamRoleArn": str,
         "SubscriptionType": Literal["PRODUCTION"],
@@ -129,22 +123,14 @@
 
 class CreateHsmRequestRequestTypeDef(
     _RequiredCreateHsmRequestRequestTypeDef, _OptionalCreateHsmRequestRequestTypeDef
 ):
     pass
 
 
-CreateHsmResponseTypeDef = TypedDict(
-    "CreateHsmResponseTypeDef",
-    {
-        "HsmArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLunaClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLunaClientRequestRequestTypeDef",
     {
         "Certificate": str,
     },
 )
 _OptionalCreateLunaClientRequestRequestTypeDef = TypedDict(
@@ -158,265 +144,110 @@
 
 class CreateLunaClientRequestRequestTypeDef(
     _RequiredCreateLunaClientRequestRequestTypeDef, _OptionalCreateLunaClientRequestRequestTypeDef
 ):
     pass
 
 
-CreateLunaClientResponseTypeDef = TypedDict(
-    "CreateLunaClientResponseTypeDef",
-    {
-        "ClientArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteHapgRequestRequestTypeDef = TypedDict(
     "DeleteHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 
-DeleteHapgResponseTypeDef = TypedDict(
-    "DeleteHapgResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteHsmRequestRequestTypeDef = TypedDict(
     "DeleteHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
     },
 )
 
-DeleteHsmResponseTypeDef = TypedDict(
-    "DeleteHsmResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLunaClientRequestRequestTypeDef = TypedDict(
     "DeleteLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
     },
 )
 
-DeleteLunaClientResponseTypeDef = TypedDict(
-    "DeleteLunaClientResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeHapgRequestRequestTypeDef = TypedDict(
     "DescribeHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 
-DescribeHapgResponseTypeDef = TypedDict(
-    "DescribeHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "HapgSerial": str,
-        "HsmsLastActionFailed": List[str],
-        "HsmsPendingDeletion": List[str],
-        "HsmsPendingRegistration": List[str],
-        "Label": str,
-        "LastModifiedTimestamp": str,
-        "PartitionSerialList": List[str],
-        "State": CloudHsmObjectStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeHsmRequestRequestTypeDef = TypedDict(
     "DescribeHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
         "HsmSerialNumber": str,
     },
     total=False,
 )
 
-DescribeHsmResponseTypeDef = TypedDict(
-    "DescribeHsmResponseTypeDef",
-    {
-        "HsmArn": str,
-        "Status": HsmStatusType,
-        "StatusDetails": str,
-        "AvailabilityZone": str,
-        "EniId": str,
-        "EniIp": str,
-        "SubscriptionType": Literal["PRODUCTION"],
-        "SubscriptionStartDate": str,
-        "SubscriptionEndDate": str,
-        "VpcId": str,
-        "SubnetId": str,
-        "IamRoleArn": str,
-        "SerialNumber": str,
-        "VendorName": str,
-        "HsmType": str,
-        "SoftwareVersion": str,
-        "SshPublicKey": str,
-        "SshKeyLastUpdated": str,
-        "ServerCertUri": str,
-        "ServerCertLastUpdated": str,
-        "Partitions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeLunaClientRequestRequestTypeDef = TypedDict(
     "DescribeLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
         "CertificateFingerprint": str,
     },
     total=False,
 )
 
-DescribeLunaClientResponseTypeDef = TypedDict(
-    "DescribeLunaClientResponseTypeDef",
-    {
-        "ClientArn": str,
-        "Certificate": str,
-        "CertificateFingerprint": str,
-        "LastModifiedTimestamp": str,
-        "Label": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetConfigRequestRequestTypeDef = TypedDict(
     "GetConfigRequestRequestTypeDef",
     {
         "ClientArn": str,
         "ClientVersion": ClientVersionType,
         "HapgList": Sequence[str],
     },
 )
 
-GetConfigResponseTypeDef = TypedDict(
-    "GetConfigResponseTypeDef",
-    {
-        "ConfigType": str,
-        "ConfigFile": str,
-        "ConfigCred": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAvailableZonesResponseTypeDef = TypedDict(
-    "ListAvailableZonesResponseTypeDef",
-    {
-        "AZList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListHapgsRequestListHapgsPaginateTypeDef = TypedDict(
-    "ListHapgsRequestListHapgsPaginateTypeDef",
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
 
 ListHapgsRequestRequestTypeDef = TypedDict(
     "ListHapgsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListHapgsResponseTypeDef = TypedDict(
-    "ListHapgsResponseTypeDef",
-    {
-        "HapgList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListHsmsRequestListHsmsPaginateTypeDef = TypedDict(
-    "ListHsmsRequestListHsmsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHsmsRequestRequestTypeDef = TypedDict(
     "ListHsmsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListHsmsResponseTypeDef = TypedDict(
-    "ListHsmsResponseTypeDef",
-    {
-        "HsmList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListLunaClientsRequestListLunaClientsPaginateTypeDef = TypedDict(
-    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLunaClientsRequestRequestTypeDef = TypedDict(
     "ListLunaClientsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListLunaClientsResponseTypeDef = TypedDict(
-    "ListLunaClientsResponseTypeDef",
-    {
-        "ClientList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredModifyHapgRequestRequestTypeDef = TypedDict(
     "_RequiredModifyHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 _OptionalModifyHapgRequestRequestTypeDef = TypedDict(
@@ -431,22 +262,14 @@
 
 class ModifyHapgRequestRequestTypeDef(
     _RequiredModifyHapgRequestRequestTypeDef, _OptionalModifyHapgRequestRequestTypeDef
 ):
     pass
 
 
-ModifyHapgResponseTypeDef = TypedDict(
-    "ModifyHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredModifyHsmRequestRequestTypeDef = TypedDict(
     "_RequiredModifyHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
     },
 )
 _OptionalModifyHsmRequestRequestTypeDef = TypedDict(
@@ -464,83 +287,251 @@
 
 class ModifyHsmRequestRequestTypeDef(
     _RequiredModifyHsmRequestRequestTypeDef, _OptionalModifyHsmRequestRequestTypeDef
 ):
     pass
 
 
-ModifyHsmResponseTypeDef = TypedDict(
-    "ModifyHsmResponseTypeDef",
+ModifyLunaClientRequestRequestTypeDef = TypedDict(
+    "ModifyLunaClientRequestRequestTypeDef",
+    {
+        "ClientArn": str,
+        "Certificate": str,
+    },
+)
+
+RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
+    "RemoveTagsFromResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeyList": Sequence[str],
+    },
+)
+
+AddTagsToResourceRequestRequestTypeDef = TypedDict(
+    "AddTagsToResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagList": Sequence[TagTypeDef],
+    },
+)
+
+AddTagsToResourceResponseTypeDef = TypedDict(
+    "AddTagsToResourceResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateHapgResponseTypeDef = TypedDict(
+    "CreateHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateHsmResponseTypeDef = TypedDict(
+    "CreateHsmResponseTypeDef",
     {
         "HsmArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyLunaClientRequestRequestTypeDef = TypedDict(
-    "ModifyLunaClientRequestRequestTypeDef",
+CreateLunaClientResponseTypeDef = TypedDict(
+    "CreateLunaClientResponseTypeDef",
     {
         "ClientArn": str,
-        "Certificate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyLunaClientResponseTypeDef = TypedDict(
-    "ModifyLunaClientResponseTypeDef",
+DeleteHapgResponseTypeDef = TypedDict(
+    "DeleteHapgResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteHsmResponseTypeDef = TypedDict(
+    "DeleteHsmResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteLunaClientResponseTypeDef = TypedDict(
+    "DeleteLunaClientResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeHapgResponseTypeDef = TypedDict(
+    "DescribeHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "HapgSerial": str,
+        "HsmsLastActionFailed": List[str],
+        "HsmsPendingDeletion": List[str],
+        "HsmsPendingRegistration": List[str],
+        "Label": str,
+        "LastModifiedTimestamp": str,
+        "PartitionSerialList": List[str],
+        "State": CloudHsmObjectStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeHsmResponseTypeDef = TypedDict(
+    "DescribeHsmResponseTypeDef",
+    {
+        "HsmArn": str,
+        "Status": HsmStatusType,
+        "StatusDetails": str,
+        "AvailabilityZone": str,
+        "EniId": str,
+        "EniIp": str,
+        "SubscriptionType": Literal["PRODUCTION"],
+        "SubscriptionStartDate": str,
+        "SubscriptionEndDate": str,
+        "VpcId": str,
+        "SubnetId": str,
+        "IamRoleArn": str,
+        "SerialNumber": str,
+        "VendorName": str,
+        "HsmType": str,
+        "SoftwareVersion": str,
+        "SshPublicKey": str,
+        "SshKeyLastUpdated": str,
+        "ServerCertUri": str,
+        "ServerCertLastUpdated": str,
+        "Partitions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLunaClientResponseTypeDef = TypedDict(
+    "DescribeLunaClientResponseTypeDef",
     {
         "ClientArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Certificate": str,
+        "CertificateFingerprint": str,
+        "LastModifiedTimestamp": str,
+        "Label": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetConfigResponseTypeDef = TypedDict(
+    "GetConfigResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ConfigType": str,
+        "ConfigFile": str,
+        "ConfigCred": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
-    "RemoveTagsFromResourceRequestRequestTypeDef",
+ListAvailableZonesResponseTypeDef = TypedDict(
+    "ListAvailableZonesResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeyList": Sequence[str],
+        "AZList": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListHapgsResponseTypeDef = TypedDict(
+    "ListHapgsResponseTypeDef",
+    {
+        "HapgList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListHsmsResponseTypeDef = TypedDict(
+    "ListHsmsResponseTypeDef",
+    {
+        "HsmList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListLunaClientsResponseTypeDef = TypedDict(
+    "ListLunaClientsResponseTypeDef",
+    {
+        "ClientList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyHapgResponseTypeDef = TypedDict(
+    "ModifyHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyHsmResponseTypeDef = TypedDict(
+    "ModifyHsmResponseTypeDef",
+    {
+        "HsmArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyLunaClientResponseTypeDef = TypedDict(
+    "ModifyLunaClientResponseTypeDef",
+    {
+        "ClientArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveTagsFromResourceResponseTypeDef = TypedDict(
     "RemoveTagsFromResourceResponseTypeDef",
     {
         "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ListHapgsRequestListHapgsPaginateTypeDef = TypedDict(
+    "ListHapgsRequestListHapgsPaginateTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-AddTagsToResourceRequestRequestTypeDef = TypedDict(
-    "AddTagsToResourceRequestRequestTypeDef",
+ListHsmsRequestListHsmsPaginateTypeDef = TypedDict(
+    "ListHsmsRequestListHsmsPaginateTypeDef",
     {
-        "ResourceArn": str,
-        "TagList": Sequence[TagTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListLunaClientsRequestListLunaClientsPaginateTypeDef = TypedDict(
+    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
     {
-        "TagList": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
```

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm/type_defs.pyi` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,92 +23,86 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "AddTagsToResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateHapgRequestRequestTypeDef",
-    "CreateHapgResponseTypeDef",
     "CreateHsmRequestRequestTypeDef",
-    "CreateHsmResponseTypeDef",
     "CreateLunaClientRequestRequestTypeDef",
-    "CreateLunaClientResponseTypeDef",
     "DeleteHapgRequestRequestTypeDef",
-    "DeleteHapgResponseTypeDef",
     "DeleteHsmRequestRequestTypeDef",
-    "DeleteHsmResponseTypeDef",
     "DeleteLunaClientRequestRequestTypeDef",
-    "DeleteLunaClientResponseTypeDef",
     "DescribeHapgRequestRequestTypeDef",
-    "DescribeHapgResponseTypeDef",
     "DescribeHsmRequestRequestTypeDef",
-    "DescribeHsmResponseTypeDef",
     "DescribeLunaClientRequestRequestTypeDef",
-    "DescribeLunaClientResponseTypeDef",
     "GetConfigRequestRequestTypeDef",
-    "GetConfigResponseTypeDef",
-    "ListAvailableZonesResponseTypeDef",
-    "ListHapgsRequestListHapgsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListHapgsRequestRequestTypeDef",
-    "ListHapgsResponseTypeDef",
-    "ListHsmsRequestListHsmsPaginateTypeDef",
     "ListHsmsRequestRequestTypeDef",
-    "ListHsmsResponseTypeDef",
-    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
     "ListLunaClientsRequestRequestTypeDef",
-    "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ModifyHapgRequestRequestTypeDef",
-    "ModifyHapgResponseTypeDef",
     "ModifyHsmRequestRequestTypeDef",
-    "ModifyHsmResponseTypeDef",
     "ModifyLunaClientRequestRequestTypeDef",
-    "ModifyLunaClientResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
-    "RemoveTagsFromResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
+    "AddTagsToResourceResponseTypeDef",
+    "CreateHapgResponseTypeDef",
+    "CreateHsmResponseTypeDef",
+    "CreateLunaClientResponseTypeDef",
+    "DeleteHapgResponseTypeDef",
+    "DeleteHsmResponseTypeDef",
+    "DeleteLunaClientResponseTypeDef",
+    "DescribeHapgResponseTypeDef",
+    "DescribeHsmResponseTypeDef",
+    "DescribeLunaClientResponseTypeDef",
+    "GetConfigResponseTypeDef",
+    "ListAvailableZonesResponseTypeDef",
+    "ListHapgsResponseTypeDef",
+    "ListHsmsResponseTypeDef",
+    "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ModifyHapgResponseTypeDef",
+    "ModifyHsmResponseTypeDef",
+    "ModifyLunaClientResponseTypeDef",
+    "RemoveTagsFromResourceResponseTypeDef",
+    "ListHapgsRequestListHapgsPaginateTypeDef",
+    "ListHsmsRequestListHsmsPaginateTypeDef",
+    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-AddTagsToResourceResponseTypeDef = TypedDict(
-    "AddTagsToResourceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateHapgRequestRequestTypeDef = TypedDict(
     "CreateHapgRequestRequestTypeDef",
     {
         "Label": str,
     },
 )
 
-CreateHapgResponseTypeDef = TypedDict(
-    "CreateHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateHsmRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHsmRequestRequestTypeDef",
     {
         "SubnetId": str,
         "SshKey": str,
         "IamRoleArn": str,
         "SubscriptionType": Literal["PRODUCTION"],
@@ -126,22 +120,14 @@
 )
 
 class CreateHsmRequestRequestTypeDef(
     _RequiredCreateHsmRequestRequestTypeDef, _OptionalCreateHsmRequestRequestTypeDef
 ):
     pass
 
-CreateHsmResponseTypeDef = TypedDict(
-    "CreateHsmResponseTypeDef",
-    {
-        "HsmArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLunaClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLunaClientRequestRequestTypeDef",
     {
         "Certificate": str,
     },
 )
 _OptionalCreateLunaClientRequestRequestTypeDef = TypedDict(
@@ -153,265 +139,110 @@
 )
 
 class CreateLunaClientRequestRequestTypeDef(
     _RequiredCreateLunaClientRequestRequestTypeDef, _OptionalCreateLunaClientRequestRequestTypeDef
 ):
     pass
 
-CreateLunaClientResponseTypeDef = TypedDict(
-    "CreateLunaClientResponseTypeDef",
-    {
-        "ClientArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteHapgRequestRequestTypeDef = TypedDict(
     "DeleteHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 
-DeleteHapgResponseTypeDef = TypedDict(
-    "DeleteHapgResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteHsmRequestRequestTypeDef = TypedDict(
     "DeleteHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
     },
 )
 
-DeleteHsmResponseTypeDef = TypedDict(
-    "DeleteHsmResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLunaClientRequestRequestTypeDef = TypedDict(
     "DeleteLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
     },
 )
 
-DeleteLunaClientResponseTypeDef = TypedDict(
-    "DeleteLunaClientResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeHapgRequestRequestTypeDef = TypedDict(
     "DescribeHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 
-DescribeHapgResponseTypeDef = TypedDict(
-    "DescribeHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "HapgSerial": str,
-        "HsmsLastActionFailed": List[str],
-        "HsmsPendingDeletion": List[str],
-        "HsmsPendingRegistration": List[str],
-        "Label": str,
-        "LastModifiedTimestamp": str,
-        "PartitionSerialList": List[str],
-        "State": CloudHsmObjectStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeHsmRequestRequestTypeDef = TypedDict(
     "DescribeHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
         "HsmSerialNumber": str,
     },
     total=False,
 )
 
-DescribeHsmResponseTypeDef = TypedDict(
-    "DescribeHsmResponseTypeDef",
-    {
-        "HsmArn": str,
-        "Status": HsmStatusType,
-        "StatusDetails": str,
-        "AvailabilityZone": str,
-        "EniId": str,
-        "EniIp": str,
-        "SubscriptionType": Literal["PRODUCTION"],
-        "SubscriptionStartDate": str,
-        "SubscriptionEndDate": str,
-        "VpcId": str,
-        "SubnetId": str,
-        "IamRoleArn": str,
-        "SerialNumber": str,
-        "VendorName": str,
-        "HsmType": str,
-        "SoftwareVersion": str,
-        "SshPublicKey": str,
-        "SshKeyLastUpdated": str,
-        "ServerCertUri": str,
-        "ServerCertLastUpdated": str,
-        "Partitions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeLunaClientRequestRequestTypeDef = TypedDict(
     "DescribeLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
         "CertificateFingerprint": str,
     },
     total=False,
 )
 
-DescribeLunaClientResponseTypeDef = TypedDict(
-    "DescribeLunaClientResponseTypeDef",
-    {
-        "ClientArn": str,
-        "Certificate": str,
-        "CertificateFingerprint": str,
-        "LastModifiedTimestamp": str,
-        "Label": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetConfigRequestRequestTypeDef = TypedDict(
     "GetConfigRequestRequestTypeDef",
     {
         "ClientArn": str,
         "ClientVersion": ClientVersionType,
         "HapgList": Sequence[str],
     },
 )
 
-GetConfigResponseTypeDef = TypedDict(
-    "GetConfigResponseTypeDef",
-    {
-        "ConfigType": str,
-        "ConfigFile": str,
-        "ConfigCred": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAvailableZonesResponseTypeDef = TypedDict(
-    "ListAvailableZonesResponseTypeDef",
-    {
-        "AZList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListHapgsRequestListHapgsPaginateTypeDef = TypedDict(
-    "ListHapgsRequestListHapgsPaginateTypeDef",
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
 
 ListHapgsRequestRequestTypeDef = TypedDict(
     "ListHapgsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListHapgsResponseTypeDef = TypedDict(
-    "ListHapgsResponseTypeDef",
-    {
-        "HapgList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListHsmsRequestListHsmsPaginateTypeDef = TypedDict(
-    "ListHsmsRequestListHsmsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHsmsRequestRequestTypeDef = TypedDict(
     "ListHsmsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListHsmsResponseTypeDef = TypedDict(
-    "ListHsmsResponseTypeDef",
-    {
-        "HsmList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListLunaClientsRequestListLunaClientsPaginateTypeDef = TypedDict(
-    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLunaClientsRequestRequestTypeDef = TypedDict(
     "ListLunaClientsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListLunaClientsResponseTypeDef = TypedDict(
-    "ListLunaClientsResponseTypeDef",
-    {
-        "ClientList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredModifyHapgRequestRequestTypeDef = TypedDict(
     "_RequiredModifyHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 _OptionalModifyHapgRequestRequestTypeDef = TypedDict(
@@ -424,22 +255,14 @@
 )
 
 class ModifyHapgRequestRequestTypeDef(
     _RequiredModifyHapgRequestRequestTypeDef, _OptionalModifyHapgRequestRequestTypeDef
 ):
     pass
 
-ModifyHapgResponseTypeDef = TypedDict(
-    "ModifyHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredModifyHsmRequestRequestTypeDef = TypedDict(
     "_RequiredModifyHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
     },
 )
 _OptionalModifyHsmRequestRequestTypeDef = TypedDict(
@@ -455,83 +278,251 @@
 )
 
 class ModifyHsmRequestRequestTypeDef(
     _RequiredModifyHsmRequestRequestTypeDef, _OptionalModifyHsmRequestRequestTypeDef
 ):
     pass
 
-ModifyHsmResponseTypeDef = TypedDict(
-    "ModifyHsmResponseTypeDef",
+ModifyLunaClientRequestRequestTypeDef = TypedDict(
+    "ModifyLunaClientRequestRequestTypeDef",
+    {
+        "ClientArn": str,
+        "Certificate": str,
+    },
+)
+
+RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
+    "RemoveTagsFromResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeyList": Sequence[str],
+    },
+)
+
+AddTagsToResourceRequestRequestTypeDef = TypedDict(
+    "AddTagsToResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagList": Sequence[TagTypeDef],
+    },
+)
+
+AddTagsToResourceResponseTypeDef = TypedDict(
+    "AddTagsToResourceResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateHapgResponseTypeDef = TypedDict(
+    "CreateHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateHsmResponseTypeDef = TypedDict(
+    "CreateHsmResponseTypeDef",
     {
         "HsmArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyLunaClientRequestRequestTypeDef = TypedDict(
-    "ModifyLunaClientRequestRequestTypeDef",
+CreateLunaClientResponseTypeDef = TypedDict(
+    "CreateLunaClientResponseTypeDef",
     {
         "ClientArn": str,
-        "Certificate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyLunaClientResponseTypeDef = TypedDict(
-    "ModifyLunaClientResponseTypeDef",
+DeleteHapgResponseTypeDef = TypedDict(
+    "DeleteHapgResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteHsmResponseTypeDef = TypedDict(
+    "DeleteHsmResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteLunaClientResponseTypeDef = TypedDict(
+    "DeleteLunaClientResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeHapgResponseTypeDef = TypedDict(
+    "DescribeHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "HapgSerial": str,
+        "HsmsLastActionFailed": List[str],
+        "HsmsPendingDeletion": List[str],
+        "HsmsPendingRegistration": List[str],
+        "Label": str,
+        "LastModifiedTimestamp": str,
+        "PartitionSerialList": List[str],
+        "State": CloudHsmObjectStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeHsmResponseTypeDef = TypedDict(
+    "DescribeHsmResponseTypeDef",
+    {
+        "HsmArn": str,
+        "Status": HsmStatusType,
+        "StatusDetails": str,
+        "AvailabilityZone": str,
+        "EniId": str,
+        "EniIp": str,
+        "SubscriptionType": Literal["PRODUCTION"],
+        "SubscriptionStartDate": str,
+        "SubscriptionEndDate": str,
+        "VpcId": str,
+        "SubnetId": str,
+        "IamRoleArn": str,
+        "SerialNumber": str,
+        "VendorName": str,
+        "HsmType": str,
+        "SoftwareVersion": str,
+        "SshPublicKey": str,
+        "SshKeyLastUpdated": str,
+        "ServerCertUri": str,
+        "ServerCertLastUpdated": str,
+        "Partitions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLunaClientResponseTypeDef = TypedDict(
+    "DescribeLunaClientResponseTypeDef",
     {
         "ClientArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Certificate": str,
+        "CertificateFingerprint": str,
+        "LastModifiedTimestamp": str,
+        "Label": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetConfigResponseTypeDef = TypedDict(
+    "GetConfigResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ConfigType": str,
+        "ConfigFile": str,
+        "ConfigCred": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
-    "RemoveTagsFromResourceRequestRequestTypeDef",
+ListAvailableZonesResponseTypeDef = TypedDict(
+    "ListAvailableZonesResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeyList": Sequence[str],
+        "AZList": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListHapgsResponseTypeDef = TypedDict(
+    "ListHapgsResponseTypeDef",
+    {
+        "HapgList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListHsmsResponseTypeDef = TypedDict(
+    "ListHsmsResponseTypeDef",
+    {
+        "HsmList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListLunaClientsResponseTypeDef = TypedDict(
+    "ListLunaClientsResponseTypeDef",
+    {
+        "ClientList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyHapgResponseTypeDef = TypedDict(
+    "ModifyHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyHsmResponseTypeDef = TypedDict(
+    "ModifyHsmResponseTypeDef",
+    {
+        "HsmArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyLunaClientResponseTypeDef = TypedDict(
+    "ModifyLunaClientResponseTypeDef",
+    {
+        "ClientArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveTagsFromResourceResponseTypeDef = TypedDict(
     "RemoveTagsFromResourceResponseTypeDef",
     {
         "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ListHapgsRequestListHapgsPaginateTypeDef = TypedDict(
+    "ListHapgsRequestListHapgsPaginateTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-AddTagsToResourceRequestRequestTypeDef = TypedDict(
-    "AddTagsToResourceRequestRequestTypeDef",
+ListHsmsRequestListHsmsPaginateTypeDef = TypedDict(
+    "ListHsmsRequestListHsmsPaginateTypeDef",
     {
-        "ResourceArn": str,
-        "TagList": Sequence[TagTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListLunaClientsRequestListLunaClientsPaginateTypeDef = TypedDict(
+    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
     {
-        "TagList": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
```

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/PKG-INFO` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudhsm
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudHSM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudHSM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsm.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudhsm)](https://pepy.tech/project/mypy-boto3-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
+[boto3.CloudHSM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [mypy-boto3-cloudhsm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,59 +331,58 @@
 
 `mypy_boto3_cloudhsm.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudhsm.type_defs import (
     TagTypeDef,
-    AddTagsToResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateHapgRequestRequestTypeDef,
-    CreateHapgResponseTypeDef,
     CreateHsmRequestRequestTypeDef,
-    CreateHsmResponseTypeDef,
     CreateLunaClientRequestRequestTypeDef,
-    CreateLunaClientResponseTypeDef,
     DeleteHapgRequestRequestTypeDef,
-    DeleteHapgResponseTypeDef,
     DeleteHsmRequestRequestTypeDef,
-    DeleteHsmResponseTypeDef,
     DeleteLunaClientRequestRequestTypeDef,
-    DeleteLunaClientResponseTypeDef,
     DescribeHapgRequestRequestTypeDef,
-    DescribeHapgResponseTypeDef,
     DescribeHsmRequestRequestTypeDef,
-    DescribeHsmResponseTypeDef,
     DescribeLunaClientRequestRequestTypeDef,
-    DescribeLunaClientResponseTypeDef,
     GetConfigRequestRequestTypeDef,
-    GetConfigResponseTypeDef,
-    ListAvailableZonesResponseTypeDef,
-    ListHapgsRequestListHapgsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListHapgsRequestRequestTypeDef,
-    ListHapgsResponseTypeDef,
-    ListHsmsRequestListHsmsPaginateTypeDef,
     ListHsmsRequestRequestTypeDef,
-    ListHsmsResponseTypeDef,
-    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
     ListLunaClientsRequestRequestTypeDef,
-    ListLunaClientsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ModifyHapgRequestRequestTypeDef,
-    ModifyHapgResponseTypeDef,
     ModifyHsmRequestRequestTypeDef,
-    ModifyHsmResponseTypeDef,
     ModifyLunaClientRequestRequestTypeDef,
-    ModifyLunaClientResponseTypeDef,
-    PaginatorConfigTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
-    RemoveTagsFromResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
+    AddTagsToResourceResponseTypeDef,
+    CreateHapgResponseTypeDef,
+    CreateHsmResponseTypeDef,
+    CreateLunaClientResponseTypeDef,
+    DeleteHapgResponseTypeDef,
+    DeleteHsmResponseTypeDef,
+    DeleteLunaClientResponseTypeDef,
+    DescribeHapgResponseTypeDef,
+    DescribeHsmResponseTypeDef,
+    DescribeLunaClientResponseTypeDef,
+    GetConfigResponseTypeDef,
+    ListAvailableZonesResponseTypeDef,
+    ListHapgsResponseTypeDef,
+    ListHsmsResponseTypeDef,
+    ListLunaClientsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ModifyHapgResponseTypeDef,
+    ModifyHsmResponseTypeDef,
+    ModifyLunaClientResponseTypeDef,
+    RemoveTagsFromResourceResponseTypeDef,
+    ListHapgsRequestListHapgsPaginateTypeDef,
+    ListHsmsRequestListHsmsPaginateTypeDef,
+    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cloudhsm-1.28.12/mypy_boto3_cloudhsm.egg-info/SOURCES.txt` & `mypy-boto3-cloudhsm-1.28.15/mypy_boto3_cloudhsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsm-1.28.12/setup.py` & `mypy-boto3-cloudhsm-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudhsm",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cloudhsm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudHSM 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CloudHSM 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

