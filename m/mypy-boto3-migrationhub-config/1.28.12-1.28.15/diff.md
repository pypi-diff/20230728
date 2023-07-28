# Comparing `tmp/mypy-boto3-migrationhub-config-1.28.12.tar.gz` & `tmp/mypy-boto3-migrationhub-config-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhub-config-1.28.12.tar", last modified: Thu Jul 27 05:35:03 2023, max compression
+gzip compressed data, was "mypy-boto3-migrationhub-config-1.28.15.tar", last modified: Fri Jul 28 20:43:19 2023, max compression
```

## Comparing `mypy-boto3-migrationhub-config-1.28.12.tar` & `mypy-boto3-migrationhub-config-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.852431 mypy-boto3-migrationhub-config-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-27 05:35:03.852431 mypy-boto3-migrationhub-config-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.848431 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-27 05:26:41.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.852431 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-27 05:35:03.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-27 05:35:03.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:03.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 05:35:03.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:03.852431 mypy-boto3-migrationhub-config-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:19.881537 mypy-boto3-migrationhub-config-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-07-28 20:43:19.877537 mypy-boto3-migrationhub-config-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:19.869537 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-28 20:32:03.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:19.877537 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-07-28 20:43:19.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 20:43:19.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:19.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:19.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:19.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 20:43:19.000000 mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:19.881537 mypy-boto3-migrationhub-config-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-28 20:32:02.000000 mypy-boto3-migrationhub-config-1.28.15/setup.py
```

### Comparing `mypy-boto3-migrationhub-config-1.28.12/LICENSE` & `mypy-boto3-migrationhub-config-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.12/PKG-INFO` & `mypy-boto3-migrationhub-config-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhub-config
-Version: 1.28.12
-Summary: Type annotations for boto3.MigrationHubConfig 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MigrationHubConfig 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhub-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhub-config)](https://pepy.tech/project/mypy-boto3-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[boto3.MigrationHubConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
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
 [mypy-boto3-migrationhub-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,20 +298,19 @@
 
 `mypy_boto3_migrationhub_config.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhub_config.type_defs import (
     TargetTypeDef,
-    GetHomeRegionResultTypeDef,
-    TargetOutputTypeDef,
     ResponseMetadataTypeDef,
     CreateHomeRegionControlRequestRequestTypeDef,
     DescribeHomeRegionControlsRequestRequestTypeDef,
     HomeRegionControlTypeDef,
+    GetHomeRegionResultTypeDef,
     CreateHomeRegionControlResultTypeDef,
     DescribeHomeRegionControlsResultTypeDef,
 )
 
 
 def get_structure() -> TargetTypeDef:
     return {...}
```

### Comparing `mypy-boto3-migrationhub-config-1.28.12/README.md` & `mypy-boto3-migrationhub-config-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhub-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhub-config)](https://pepy.tech/project/mypy-boto3-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[boto3.MigrationHubConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
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
 [mypy-boto3-migrationhub-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,20 +266,19 @@
 
 `mypy_boto3_migrationhub_config.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhub_config.type_defs import (
     TargetTypeDef,
-    GetHomeRegionResultTypeDef,
-    TargetOutputTypeDef,
     ResponseMetadataTypeDef,
     CreateHomeRegionControlRequestRequestTypeDef,
     DescribeHomeRegionControlsRequestRequestTypeDef,
     HomeRegionControlTypeDef,
+    GetHomeRegionResultTypeDef,
     CreateHomeRegionControlResultTypeDef,
     DescribeHomeRegionControlsResultTypeDef,
 )
 
 
 def get_structure() -> TargetTypeDef:
     return {...}
```

### Comparing `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/__main__.py` & `mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubConfig 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MigrationHubConfig 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig\nOther"
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

### Comparing `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/client.py` & `mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/client.pyi` & `mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/literals.py` & `mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/literals.pyi` & `mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/type_defs.py` & `mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,20 +23,19 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TargetTypeDef",
-    "GetHomeRegionResultTypeDef",
-    "TargetOutputTypeDef",
     "ResponseMetadataTypeDef",
     "CreateHomeRegionControlRequestRequestTypeDef",
     "DescribeHomeRegionControlsRequestRequestTypeDef",
     "HomeRegionControlTypeDef",
+    "GetHomeRegionResultTypeDef",
     "CreateHomeRegionControlResultTypeDef",
     "DescribeHomeRegionControlsResultTypeDef",
 )
 
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
@@ -52,41 +51,14 @@
 )
 
 
 class TargetTypeDef(_RequiredTargetTypeDef, _OptionalTargetTypeDef):
     pass
 
 
-GetHomeRegionResultTypeDef = TypedDict(
-    "GetHomeRegionResultTypeDef",
-    {
-        "HomeRegion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredTargetOutputTypeDef = TypedDict(
-    "_RequiredTargetOutputTypeDef",
-    {
-        "Type": Literal["ACCOUNT"],
-    },
-)
-_OptionalTargetOutputTypeDef = TypedDict(
-    "_OptionalTargetOutputTypeDef",
-    {
-        "Id": str,
-    },
-    total=False,
-)
-
-
-class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
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
@@ -130,29 +102,37 @@
 )
 
 HomeRegionControlTypeDef = TypedDict(
     "HomeRegionControlTypeDef",
     {
         "ControlId": str,
         "HomeRegion": str,
-        "Target": TargetOutputTypeDef,
+        "Target": TargetTypeDef,
         "RequestedTime": datetime,
     },
     total=False,
 )
 
+GetHomeRegionResultTypeDef = TypedDict(
+    "GetHomeRegionResultTypeDef",
+    {
+        "HomeRegion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateHomeRegionControlResultTypeDef = TypedDict(
     "CreateHomeRegionControlResultTypeDef",
     {
         "HomeRegionControl": HomeRegionControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeHomeRegionControlsResultTypeDef = TypedDict(
     "DescribeHomeRegionControlsResultTypeDef",
     {
         "HomeRegionControls": List[HomeRegionControlTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/type_defs.pyi` & `mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -22,20 +22,19 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TargetTypeDef",
-    "GetHomeRegionResultTypeDef",
-    "TargetOutputTypeDef",
     "ResponseMetadataTypeDef",
     "CreateHomeRegionControlRequestRequestTypeDef",
     "DescribeHomeRegionControlsRequestRequestTypeDef",
     "HomeRegionControlTypeDef",
+    "GetHomeRegionResultTypeDef",
     "CreateHomeRegionControlResultTypeDef",
     "DescribeHomeRegionControlsResultTypeDef",
 )
 
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
@@ -49,39 +48,14 @@
     },
     total=False,
 )
 
 class TargetTypeDef(_RequiredTargetTypeDef, _OptionalTargetTypeDef):
     pass
 
-GetHomeRegionResultTypeDef = TypedDict(
-    "GetHomeRegionResultTypeDef",
-    {
-        "HomeRegion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredTargetOutputTypeDef = TypedDict(
-    "_RequiredTargetOutputTypeDef",
-    {
-        "Type": Literal["ACCOUNT"],
-    },
-)
-_OptionalTargetOutputTypeDef = TypedDict(
-    "_OptionalTargetOutputTypeDef",
-    {
-        "Id": str,
-    },
-    total=False,
-)
-
-class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
-    pass
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -123,29 +97,37 @@
 )
 
 HomeRegionControlTypeDef = TypedDict(
     "HomeRegionControlTypeDef",
     {
         "ControlId": str,
         "HomeRegion": str,
-        "Target": TargetOutputTypeDef,
+        "Target": TargetTypeDef,
         "RequestedTime": datetime,
     },
     total=False,
 )
 
+GetHomeRegionResultTypeDef = TypedDict(
+    "GetHomeRegionResultTypeDef",
+    {
+        "HomeRegion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateHomeRegionControlResultTypeDef = TypedDict(
     "CreateHomeRegionControlResultTypeDef",
     {
         "HomeRegionControl": HomeRegionControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeHomeRegionControlsResultTypeDef = TypedDict(
     "DescribeHomeRegionControlsResultTypeDef",
     {
         "HomeRegionControls": List[HomeRegionControlTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/PKG-INFO` & `mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhub-config
-Version: 1.28.12
-Summary: Type annotations for boto3.MigrationHubConfig 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MigrationHubConfig 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhub-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhub-config)](https://pepy.tech/project/mypy-boto3-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[boto3.MigrationHubConfig 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
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
 [mypy-boto3-migrationhub-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,20 +298,19 @@
 
 `mypy_boto3_migrationhub_config.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhub_config.type_defs import (
     TargetTypeDef,
-    GetHomeRegionResultTypeDef,
-    TargetOutputTypeDef,
     ResponseMetadataTypeDef,
     CreateHomeRegionControlRequestRequestTypeDef,
     DescribeHomeRegionControlsRequestRequestTypeDef,
     HomeRegionControlTypeDef,
+    GetHomeRegionResultTypeDef,
     CreateHomeRegionControlResultTypeDef,
     DescribeHomeRegionControlsResultTypeDef,
 )
 
 
 def get_structure() -> TargetTypeDef:
     return {...}
```

### Comparing `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/SOURCES.txt` & `mypy-boto3-migrationhub-config-1.28.15/mypy_boto3_migrationhub_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.12/setup.py` & `mypy-boto3-migrationhub-config-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhub-config",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_migrationhub_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubConfig 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MigrationHubConfig 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

