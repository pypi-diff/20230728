# Comparing `tmp/mypy-boto3-rbin-1.28.12.tar.gz` & `tmp/mypy-boto3-rbin-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rbin-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
+gzip compressed data, was "mypy-boto3-rbin-1.28.15.tar", last modified: Fri Jul 28 20:43:31 2023, max compression
```

## Comparing `mypy-boto3-rbin-1.28.12.tar` & `mypy-boto3-rbin-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.637188 mypy-boto3-rbin-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-07-27 11:49:27.633188 mypy-boto3-rbin-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.621188 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.633188 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-07-27 11:49:27.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-27 11:49:27.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 11:49:27.000000 mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.637188 mypy-boto3-rbin-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-27 11:43:57.000000 mypy-boto3-rbin-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:31.257693 mypy-boto3-rbin-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-28 20:43:31.257693 mypy-boto3-rbin-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:31.253693 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:31.257693 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-07-28 20:43:31.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-28 20:43:31.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:31.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:31.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:31.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 20:43:31.000000 mypy-boto3-rbin-1.28.15/mypy_boto3_rbin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:31.257693 mypy-boto3-rbin-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-28 20:36:12.000000 mypy-boto3-rbin-1.28.15/setup.py
```

### Comparing `mypy-boto3-rbin-1.28.12/LICENSE` & `mypy-boto3-rbin-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.12/PKG-INFO` & `mypy-boto3-rbin-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rbin
-Version: 1.28.12
-Summary: Type annotations for boto3.RecycleBin 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.RecycleBin 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rbin)](https://pepy.tech/project/mypy-boto3-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RecycleBin 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[boto3.RecycleBin 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [mypy-boto3-rbin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,42 +326,37 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rbin.type_defs import (
     ResourceTagTypeDef,
     RetentionPeriodTypeDef,
     TagTypeDef,
-    ResourceTagOutputTypeDef,
     ResponseMetadataTypeDef,
-    RetentionPeriodOutputTypeDef,
-    TagOutputTypeDef,
     DeleteRuleRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    UnlockDelayOutputTypeDef,
     UnlockDelayTypeDef,
     UnlockRuleRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ListRulesRequestRequestTypeDef,
+    RuleSummaryTypeDef,
     UpdateRuleRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    RuleSummaryTypeDef,
-    UpdateRuleResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    UpdateRuleResponseTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
-    LockConfigurationOutputTypeDef,
     LockConfigurationTypeDef,
     ListRulesResponseTypeDef,
+    CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
+    LockRuleRequestRequestTypeDef,
     LockRuleResponseTypeDef,
     UnlockRuleResponseTypeDef,
-    CreateRuleRequestRequestTypeDef,
-    LockRuleRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ResourceTagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-rbin-1.28.12/README.md` & `mypy-boto3-rbin-1.28.15/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rbin)](https://pepy.tech/project/mypy-boto3-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RecycleBin 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[boto3.RecycleBin 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [mypy-boto3-rbin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -294,42 +294,37 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rbin.type_defs import (
     ResourceTagTypeDef,
     RetentionPeriodTypeDef,
     TagTypeDef,
-    ResourceTagOutputTypeDef,
     ResponseMetadataTypeDef,
-    RetentionPeriodOutputTypeDef,
-    TagOutputTypeDef,
     DeleteRuleRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    UnlockDelayOutputTypeDef,
     UnlockDelayTypeDef,
     UnlockRuleRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ListRulesRequestRequestTypeDef,
+    RuleSummaryTypeDef,
     UpdateRuleRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    RuleSummaryTypeDef,
-    UpdateRuleResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    UpdateRuleResponseTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
-    LockConfigurationOutputTypeDef,
     LockConfigurationTypeDef,
     ListRulesResponseTypeDef,
+    CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
+    LockRuleRequestRequestTypeDef,
     LockRuleResponseTypeDef,
     UnlockRuleResponseTypeDef,
-    CreateRuleRequestRequestTypeDef,
-    LockRuleRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ResourceTagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/__init__.py` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/__init__.pyi` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/__main__.py` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RecycleBin 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.RecycleBin 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin\nOther"
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

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/client.py` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/client.pyi` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/literals.py` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/literals.pyi` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/paginator.py` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/paginator.pyi` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/type_defs.py` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -22,47 +22,41 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResourceTagTypeDef",
     "RetentionPeriodTypeDef",
     "TagTypeDef",
-    "ResourceTagOutputTypeDef",
     "ResponseMetadataTypeDef",
-    "RetentionPeriodOutputTypeDef",
-    "TagOutputTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "UnlockDelayOutputTypeDef",
     "UnlockDelayTypeDef",
     "UnlockRuleRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ListRulesRequestRequestTypeDef",
+    "RuleSummaryTypeDef",
     "UpdateRuleRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "RuleSummaryTypeDef",
-    "UpdateRuleResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "UpdateRuleResponseTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
-    "LockConfigurationOutputTypeDef",
     "LockConfigurationTypeDef",
     "ListRulesResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
+    "LockRuleRequestRequestTypeDef",
     "LockRuleResponseTypeDef",
     "UnlockRuleResponseTypeDef",
-    "CreateRuleRequestRequestTypeDef",
-    "LockRuleRequestRequestTypeDef",
 )
 
 _RequiredResourceTagTypeDef = TypedDict(
     "_RequiredResourceTagTypeDef",
     {
         "ResourceTagKey": str,
     },
@@ -71,19 +65,17 @@
     "_OptionalResourceTagTypeDef",
     {
         "ResourceTagValue": str,
     },
     total=False,
 )
 
-
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
-
 RetentionPeriodTypeDef = TypedDict(
     "RetentionPeriodTypeDef",
     {
         "RetentionPeriodValue": int,
         "RetentionPeriodUnit": Literal["DAYS"],
     },
 )
@@ -92,62 +84,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-_RequiredResourceTagOutputTypeDef = TypedDict(
-    "_RequiredResourceTagOutputTypeDef",
-    {
-        "ResourceTagKey": str,
-    },
-)
-_OptionalResourceTagOutputTypeDef = TypedDict(
-    "_OptionalResourceTagOutputTypeDef",
-    {
-        "ResourceTagValue": str,
-    },
-    total=False,
-)
-
-
-class ResourceTagOutputTypeDef(
-    _RequiredResourceTagOutputTypeDef, _OptionalResourceTagOutputTypeDef
-):
-    pass
-
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RetentionPeriodOutputTypeDef = TypedDict(
-    "RetentionPeriodOutputTypeDef",
-    {
-        "RetentionPeriodValue": int,
-        "RetentionPeriodUnit": Literal["DAYS"],
-    },
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -171,22 +126,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-UnlockDelayOutputTypeDef = TypedDict(
-    "UnlockDelayOutputTypeDef",
-    {
-        "UnlockDelayValue": int,
-        "UnlockDelayUnit": Literal["DAYS"],
-    },
-)
-
 UnlockDelayTypeDef = TypedDict(
     "UnlockDelayTypeDef",
     {
         "UnlockDelayValue": int,
         "UnlockDelayUnit": Literal["DAYS"],
     },
 )
@@ -219,20 +166,29 @@
         "NextToken": str,
         "ResourceTags": Sequence[ResourceTagTypeDef],
         "LockState": LockStateType,
     },
     total=False,
 )
 
-
 class ListRulesRequestRequestTypeDef(
     _RequiredListRulesRequestRequestTypeDef, _OptionalListRulesRequestRequestTypeDef
 ):
     pass
 
+RuleSummaryTypeDef = TypedDict(
+    "RuleSummaryTypeDef",
+    {
+        "Identifier": str,
+        "Description": str,
+        "RetentionPeriod": RetentionPeriodTypeDef,
+        "LockState": LockStateType,
+    },
+    total=False,
+)
 
 _RequiredUpdateRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
@@ -243,63 +199,50 @@
         "Description": str,
         "ResourceType": ResourceTypeType,
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
-
 class UpdateRuleRequestRequestTypeDef(
     _RequiredUpdateRuleRequestRequestTypeDef, _OptionalUpdateRuleRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-RuleSummaryTypeDef = TypedDict(
-    "RuleSummaryTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "Identifier": str,
-        "Description": str,
-        "RetentionPeriod": RetentionPeriodOutputTypeDef,
-        "LockState": LockStateType,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 UpdateRuleResponseTypeDef = TypedDict(
     "UpdateRuleResponseTypeDef",
     {
         "Identifier": str,
-        "RetentionPeriod": RetentionPeriodOutputTypeDef,
+        "RetentionPeriod": RetentionPeriodTypeDef,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
         "LockState": LockStateType,
         "LockEndTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
     "_RequiredListRulesRequestListRulesPaginateTypeDef",
     {
         "ResourceType": ResourceTypeType,
     },
 )
 _OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
@@ -308,29 +251,20 @@
         "ResourceTags": Sequence[ResourceTagTypeDef],
         "LockState": LockStateType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListRulesRequestListRulesPaginateTypeDef(
     _RequiredListRulesRequestListRulesPaginateTypeDef,
     _OptionalListRulesRequestListRulesPaginateTypeDef,
 ):
     pass
 
-
-LockConfigurationOutputTypeDef = TypedDict(
-    "LockConfigurationOutputTypeDef",
-    {
-        "UnlockDelay": UnlockDelayOutputTypeDef,
-    },
-)
-
 LockConfigurationTypeDef = TypedDict(
     "LockConfigurationTypeDef",
     {
         "UnlockDelay": UnlockDelayTypeDef,
     },
 )
 
@@ -339,102 +273,100 @@
     {
         "Rules": List[RuleSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleRequestRequestTypeDef",
+    {
+        "RetentionPeriod": RetentionPeriodTypeDef,
+        "ResourceType": ResourceTypeType,
+    },
+)
+_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "LockConfiguration": LockConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class CreateRuleRequestRequestTypeDef(
+    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+):
+    pass
+
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
         "Identifier": str,
-        "RetentionPeriod": RetentionPeriodOutputTypeDef,
+        "RetentionPeriod": RetentionPeriodTypeDef,
         "Description": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResourceType": ResourceTypeType,
-        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationOutputTypeDef,
+        "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "Identifier": str,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "RetentionPeriod": RetentionPeriodOutputTypeDef,
-        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "RetentionPeriod": RetentionPeriodTypeDef,
+        "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationOutputTypeDef,
+        "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
         "LockEndTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LockRuleRequestRequestTypeDef = TypedDict(
+    "LockRuleRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "LockConfiguration": LockConfigurationTypeDef,
+    },
+)
+
 LockRuleResponseTypeDef = TypedDict(
     "LockRuleResponseTypeDef",
     {
         "Identifier": str,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "RetentionPeriod": RetentionPeriodOutputTypeDef,
-        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "RetentionPeriod": RetentionPeriodTypeDef,
+        "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationOutputTypeDef,
+        "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UnlockRuleResponseTypeDef = TypedDict(
     "UnlockRuleResponseTypeDef",
     {
         "Identifier": str,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "RetentionPeriod": RetentionPeriodOutputTypeDef,
-        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "RetentionPeriod": RetentionPeriodTypeDef,
+        "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationOutputTypeDef,
+        "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
         "LockEndTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleRequestRequestTypeDef",
-    {
-        "RetentionPeriod": RetentionPeriodTypeDef,
-        "ResourceType": ResourceTypeType,
-    },
-)
-_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-        "LockConfiguration": LockConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateRuleRequestRequestTypeDef(
-    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
-):
-    pass
-
-
-LockRuleRequestRequestTypeDef = TypedDict(
-    "LockRuleRequestRequestTypeDef",
-    {
-        "Identifier": str,
-        "LockConfiguration": LockConfigurationTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin/type_defs.pyi` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin/type_defs.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,46 +22,42 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ResourceTagTypeDef",
     "RetentionPeriodTypeDef",
     "TagTypeDef",
-    "ResourceTagOutputTypeDef",
     "ResponseMetadataTypeDef",
-    "RetentionPeriodOutputTypeDef",
-    "TagOutputTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "UnlockDelayOutputTypeDef",
     "UnlockDelayTypeDef",
     "UnlockRuleRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ListRulesRequestRequestTypeDef",
+    "RuleSummaryTypeDef",
     "UpdateRuleRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "RuleSummaryTypeDef",
-    "UpdateRuleResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "UpdateRuleResponseTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
-    "LockConfigurationOutputTypeDef",
     "LockConfigurationTypeDef",
     "ListRulesResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
+    "LockRuleRequestRequestTypeDef",
     "LockRuleResponseTypeDef",
     "UnlockRuleResponseTypeDef",
-    "CreateRuleRequestRequestTypeDef",
-    "LockRuleRequestRequestTypeDef",
 )
 
 _RequiredResourceTagTypeDef = TypedDict(
     "_RequiredResourceTagTypeDef",
     {
         "ResourceTagKey": str,
     },
@@ -70,17 +66,19 @@
     "_OptionalResourceTagTypeDef",
     {
         "ResourceTagValue": str,
     },
     total=False,
 )
 
+
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
+
 RetentionPeriodTypeDef = TypedDict(
     "RetentionPeriodTypeDef",
     {
         "RetentionPeriodValue": int,
         "RetentionPeriodUnit": Literal["DAYS"],
     },
 )
@@ -89,60 +87,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-_RequiredResourceTagOutputTypeDef = TypedDict(
-    "_RequiredResourceTagOutputTypeDef",
-    {
-        "ResourceTagKey": str,
-    },
-)
-_OptionalResourceTagOutputTypeDef = TypedDict(
-    "_OptionalResourceTagOutputTypeDef",
-    {
-        "ResourceTagValue": str,
-    },
-    total=False,
-)
-
-class ResourceTagOutputTypeDef(
-    _RequiredResourceTagOutputTypeDef, _OptionalResourceTagOutputTypeDef
-):
-    pass
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RetentionPeriodOutputTypeDef = TypedDict(
-    "RetentionPeriodOutputTypeDef",
-    {
-        "RetentionPeriodValue": int,
-        "RetentionPeriodUnit": Literal["DAYS"],
-    },
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 DeleteRuleRequestRequestTypeDef = TypedDict(
     "DeleteRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -166,22 +129,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-UnlockDelayOutputTypeDef = TypedDict(
-    "UnlockDelayOutputTypeDef",
-    {
-        "UnlockDelayValue": int,
-        "UnlockDelayUnit": Literal["DAYS"],
-    },
-)
-
 UnlockDelayTypeDef = TypedDict(
     "UnlockDelayTypeDef",
     {
         "UnlockDelayValue": int,
         "UnlockDelayUnit": Literal["DAYS"],
     },
 )
@@ -214,19 +169,32 @@
         "NextToken": str,
         "ResourceTags": Sequence[ResourceTagTypeDef],
         "LockState": LockStateType,
     },
     total=False,
 )
 
+
 class ListRulesRequestRequestTypeDef(
     _RequiredListRulesRequestRequestTypeDef, _OptionalListRulesRequestRequestTypeDef
 ):
     pass
 
+
+RuleSummaryTypeDef = TypedDict(
+    "RuleSummaryTypeDef",
+    {
+        "Identifier": str,
+        "Description": str,
+        "RetentionPeriod": RetentionPeriodTypeDef,
+        "LockState": LockStateType,
+    },
+    total=False,
+)
+
 _RequiredUpdateRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRuleRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 _OptionalUpdateRuleRequestRequestTypeDef = TypedDict(
@@ -236,61 +204,52 @@
         "Description": str,
         "ResourceType": ResourceTypeType,
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
+
 class UpdateRuleRequestRequestTypeDef(
     _RequiredUpdateRuleRequestRequestTypeDef, _OptionalUpdateRuleRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-RuleSummaryTypeDef = TypedDict(
-    "RuleSummaryTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "Identifier": str,
-        "Description": str,
-        "RetentionPeriod": RetentionPeriodOutputTypeDef,
-        "LockState": LockStateType,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 UpdateRuleResponseTypeDef = TypedDict(
     "UpdateRuleResponseTypeDef",
     {
         "Identifier": str,
-        "RetentionPeriod": RetentionPeriodOutputTypeDef,
+        "RetentionPeriod": RetentionPeriodTypeDef,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
         "LockState": LockStateType,
         "LockEndTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
     "_RequiredListRulesRequestListRulesPaginateTypeDef",
     {
         "ResourceType": ResourceTypeType,
     },
 )
 _OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
@@ -299,26 +258,21 @@
         "ResourceTags": Sequence[ResourceTagTypeDef],
         "LockState": LockStateType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListRulesRequestListRulesPaginateTypeDef(
     _RequiredListRulesRequestListRulesPaginateTypeDef,
     _OptionalListRulesRequestListRulesPaginateTypeDef,
 ):
     pass
 
-LockConfigurationOutputTypeDef = TypedDict(
-    "LockConfigurationOutputTypeDef",
-    {
-        "UnlockDelay": UnlockDelayOutputTypeDef,
-    },
-)
 
 LockConfigurationTypeDef = TypedDict(
     "LockConfigurationTypeDef",
     {
         "UnlockDelay": UnlockDelayTypeDef,
     },
 )
@@ -328,100 +282,102 @@
     {
         "Rules": List[RuleSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleRequestRequestTypeDef",
+    {
+        "RetentionPeriod": RetentionPeriodTypeDef,
+        "ResourceType": ResourceTypeType,
+    },
+)
+_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "LockConfiguration": LockConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateRuleRequestRequestTypeDef(
+    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+):
+    pass
+
+
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
         "Identifier": str,
-        "RetentionPeriod": RetentionPeriodOutputTypeDef,
+        "RetentionPeriod": RetentionPeriodTypeDef,
         "Description": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResourceType": ResourceTypeType,
-        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationOutputTypeDef,
+        "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
         "Identifier": str,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "RetentionPeriod": RetentionPeriodOutputTypeDef,
-        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "RetentionPeriod": RetentionPeriodTypeDef,
+        "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationOutputTypeDef,
+        "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
         "LockEndTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LockRuleRequestRequestTypeDef = TypedDict(
+    "LockRuleRequestRequestTypeDef",
+    {
+        "Identifier": str,
+        "LockConfiguration": LockConfigurationTypeDef,
+    },
+)
+
 LockRuleResponseTypeDef = TypedDict(
     "LockRuleResponseTypeDef",
     {
         "Identifier": str,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "RetentionPeriod": RetentionPeriodOutputTypeDef,
-        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "RetentionPeriod": RetentionPeriodTypeDef,
+        "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationOutputTypeDef,
+        "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UnlockRuleResponseTypeDef = TypedDict(
     "UnlockRuleResponseTypeDef",
     {
         "Identifier": str,
         "Description": str,
         "ResourceType": ResourceTypeType,
-        "RetentionPeriod": RetentionPeriodOutputTypeDef,
-        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "RetentionPeriod": RetentionPeriodTypeDef,
+        "ResourceTags": List[ResourceTagTypeDef],
         "Status": RuleStatusType,
-        "LockConfiguration": LockConfigurationOutputTypeDef,
+        "LockConfiguration": LockConfigurationTypeDef,
         "LockState": LockStateType,
         "LockEndTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleRequestRequestTypeDef",
-    {
-        "RetentionPeriod": RetentionPeriodTypeDef,
-        "ResourceType": ResourceTypeType,
-    },
-)
-_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-        "LockConfiguration": LockConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class CreateRuleRequestRequestTypeDef(
-    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
-):
-    pass
-
-LockRuleRequestRequestTypeDef = TypedDict(
-    "LockRuleRequestRequestTypeDef",
-    {
-        "Identifier": str,
-        "LockConfiguration": LockConfigurationTypeDef,
-    },
-)
```

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/PKG-INFO` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rbin
-Version: 1.28.12
-Summary: Type annotations for boto3.RecycleBin 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.RecycleBin 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rbin.svg?color=blue)](https://pypi.org/project/mypy-boto3-rbin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rbin)](https://pepy.tech/project/mypy-boto3-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RecycleBin 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[boto3.RecycleBin 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [mypy-boto3-rbin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rbin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,42 +326,37 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_rbin.type_defs import (
     ResourceTagTypeDef,
     RetentionPeriodTypeDef,
     TagTypeDef,
-    ResourceTagOutputTypeDef,
     ResponseMetadataTypeDef,
-    RetentionPeriodOutputTypeDef,
-    TagOutputTypeDef,
     DeleteRuleRequestRequestTypeDef,
     GetRuleRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    UnlockDelayOutputTypeDef,
     UnlockDelayTypeDef,
     UnlockRuleRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ListRulesRequestRequestTypeDef,
+    RuleSummaryTypeDef,
     UpdateRuleRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    RuleSummaryTypeDef,
-    UpdateRuleResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    UpdateRuleResponseTypeDef,
     ListRulesRequestListRulesPaginateTypeDef,
-    LockConfigurationOutputTypeDef,
     LockConfigurationTypeDef,
     ListRulesResponseTypeDef,
+    CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
+    LockRuleRequestRequestTypeDef,
     LockRuleResponseTypeDef,
     UnlockRuleResponseTypeDef,
-    CreateRuleRequestRequestTypeDef,
-    LockRuleRequestRequestTypeDef,
 )
 
 
 def get_structure() -> ResourceTagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-rbin-1.28.12/mypy_boto3_rbin.egg-info/SOURCES.txt` & `mypy-boto3-rbin-1.28.15/mypy_boto3_rbin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rbin-1.28.12/setup.py` & `mypy-boto3-rbin-1.28.15/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rbin",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_rbin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RecycleBin 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.RecycleBin 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

