# Comparing `tmp/mypy-boto3-appintegrations-1.28.12.tar.gz` & `tmp/mypy-boto3-appintegrations-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appintegrations-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
+gzip compressed data, was "mypy-boto3-appintegrations-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
```

## Comparing `mypy-boto3-appintegrations-1.28.12.tar` & `mypy-boto3-appintegrations-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.428577 mypy-boto3-appintegrations-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-27 05:34:18.428577 mypy-boto3-appintegrations-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.424577 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-27 05:17:23.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-27 05:17:23.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-27 05:17:23.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-07-27 05:17:23.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.428577 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-27 05:34:18.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-27 05:34:18.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:18.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.428577 mypy-boto3-appintegrations-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.284655 mypy-boto3-appintegrations-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-07-28 20:42:16.280655 mypy-boto3-appintegrations-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.272655 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.276655 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-07-28 20:42:16.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-28 20:42:16.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:16.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:42:16.000000 mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.284655 mypy-boto3-appintegrations-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 20:19:22.000000 mypy-boto3-appintegrations-1.28.15/setup.py
```

### Comparing `mypy-boto3-appintegrations-1.28.12/LICENSE` & `mypy-boto3-appintegrations-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.12/PKG-INFO` & `mypy-boto3-appintegrations-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appintegrations
-Version: 1.28.12
-Summary: Type annotations for boto3.AppIntegrationsService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppIntegrationsService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appintegrations)](https://pepy.tech/project/mypy-boto3-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppIntegrationsService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[boto3.AppIntegrationsService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,44 +300,42 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
     FileConfigurationOutputTypeDef,
-    ScheduleConfigurationOutputTypeDef,
+    ResponseMetadataTypeDef,
     EventFilterTypeDef,
-    CreateEventIntegrationResponseTypeDef,
     DataIntegrationAssociationSummaryTypeDef,
     DataIntegrationSummaryTypeDef,
     DeleteDataIntegrationRequestRequestTypeDef,
     DeleteEventIntegrationRequestRequestTypeDef,
-    EventFilterOutputTypeDef,
     EventIntegrationAssociationTypeDef,
     GetDataIntegrationRequestRequestTypeDef,
     GetEventIntegrationRequestRequestTypeDef,
     ListDataIntegrationAssociationsRequestRequestTypeDef,
     ListDataIntegrationsRequestRequestTypeDef,
     ListEventIntegrationAssociationsRequestRequestTypeDef,
     ListEventIntegrationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
     CreateDataIntegrationResponseTypeDef,
+    CreateEventIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
-    ListDataIntegrationAssociationsResponseTypeDef,
-    ListDataIntegrationsResponseTypeDef,
     EventIntegrationTypeDef,
     GetEventIntegrationResponseTypeDef,
+    ListDataIntegrationAssociationsResponseTypeDef,
+    ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
 )
 
 
 def get_structure() -> FileConfigurationTypeDef:
     return {...}
```

### Comparing `mypy-boto3-appintegrations-1.28.12/README.md` & `mypy-boto3-appintegrations-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appintegrations)](https://pepy.tech/project/mypy-boto3-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppIntegrationsService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[boto3.AppIntegrationsService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -268,44 +268,42 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
     FileConfigurationOutputTypeDef,
-    ScheduleConfigurationOutputTypeDef,
+    ResponseMetadataTypeDef,
     EventFilterTypeDef,
-    CreateEventIntegrationResponseTypeDef,
     DataIntegrationAssociationSummaryTypeDef,
     DataIntegrationSummaryTypeDef,
     DeleteDataIntegrationRequestRequestTypeDef,
     DeleteEventIntegrationRequestRequestTypeDef,
-    EventFilterOutputTypeDef,
     EventIntegrationAssociationTypeDef,
     GetDataIntegrationRequestRequestTypeDef,
     GetEventIntegrationRequestRequestTypeDef,
     ListDataIntegrationAssociationsRequestRequestTypeDef,
     ListDataIntegrationsRequestRequestTypeDef,
     ListEventIntegrationAssociationsRequestRequestTypeDef,
     ListEventIntegrationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
     CreateDataIntegrationResponseTypeDef,
+    CreateEventIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
-    ListDataIntegrationAssociationsResponseTypeDef,
-    ListDataIntegrationsResponseTypeDef,
     EventIntegrationTypeDef,
     GetEventIntegrationResponseTypeDef,
+    ListDataIntegrationAssociationsResponseTypeDef,
+    ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
 )
 
 
 def get_structure() -> FileConfigurationTypeDef:
     return {...}
```

### Comparing `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/__main__.py` & `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppIntegrationsService 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.AppIntegrationsService 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService\nOther"
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

### Comparing `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/client.py` & `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/client.pyi` & `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/literals.py` & `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/literals.pyi` & `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/type_defs.py` & `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,44 +20,42 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FileConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
     "FileConfigurationOutputTypeDef",
-    "ScheduleConfigurationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "EventFilterTypeDef",
-    "CreateEventIntegrationResponseTypeDef",
     "DataIntegrationAssociationSummaryTypeDef",
     "DataIntegrationSummaryTypeDef",
     "DeleteDataIntegrationRequestRequestTypeDef",
     "DeleteEventIntegrationRequestRequestTypeDef",
-    "EventFilterOutputTypeDef",
     "EventIntegrationAssociationTypeDef",
     "GetDataIntegrationRequestRequestTypeDef",
     "GetEventIntegrationRequestRequestTypeDef",
     "ListDataIntegrationAssociationsRequestRequestTypeDef",
     "ListDataIntegrationsRequestRequestTypeDef",
     "ListEventIntegrationAssociationsRequestRequestTypeDef",
     "ListEventIntegrationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataIntegrationRequestRequestTypeDef",
     "UpdateEventIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationResponseTypeDef",
+    "CreateEventIntegrationResponseTypeDef",
     "GetDataIntegrationResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateEventIntegrationRequestRequestTypeDef",
-    "ListDataIntegrationAssociationsResponseTypeDef",
-    "ListDataIntegrationsResponseTypeDef",
     "EventIntegrationTypeDef",
     "GetEventIntegrationResponseTypeDef",
+    "ListDataIntegrationAssociationsResponseTypeDef",
+    "ListDataIntegrationsResponseTypeDef",
     "ListEventIntegrationAssociationsResponseTypeDef",
     "ListEventIntegrationsResponseTypeDef",
 )
 
 _RequiredFileConfigurationTypeDef = TypedDict(
     "_RequiredFileConfigurationTypeDef",
     {
@@ -118,51 +116,32 @@
 
 class FileConfigurationOutputTypeDef(
     _RequiredFileConfigurationOutputTypeDef, _OptionalFileConfigurationOutputTypeDef
 ):
     pass
 
 
-_RequiredScheduleConfigurationOutputTypeDef = TypedDict(
-    "_RequiredScheduleConfigurationOutputTypeDef",
-    {
-        "ScheduleExpression": str,
-    },
-)
-_OptionalScheduleConfigurationOutputTypeDef = TypedDict(
-    "_OptionalScheduleConfigurationOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FirstExecutionFrom": str,
-        "Object": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class ScheduleConfigurationOutputTypeDef(
-    _RequiredScheduleConfigurationOutputTypeDef, _OptionalScheduleConfigurationOutputTypeDef
-):
-    pass
-
-
 EventFilterTypeDef = TypedDict(
     "EventFilterTypeDef",
     {
         "Source": str,
     },
 )
 
-CreateEventIntegrationResponseTypeDef = TypedDict(
-    "CreateEventIntegrationResponseTypeDef",
-    {
-        "EventIntegrationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataIntegrationAssociationSummaryTypeDef = TypedDict(
     "DataIntegrationAssociationSummaryTypeDef",
     {
         "DataIntegrationAssociationArn": str,
         "DataIntegrationArn": str,
         "ClientId": str,
     },
@@ -189,21 +168,14 @@
 DeleteEventIntegrationRequestRequestTypeDef = TypedDict(
     "DeleteEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-EventFilterOutputTypeDef = TypedDict(
-    "EventFilterOutputTypeDef",
-    {
-        "Source": str,
-    },
-)
-
 EventIntegrationAssociationTypeDef = TypedDict(
     "EventIntegrationAssociationTypeDef",
     {
         "EventIntegrationAssociationArn": str,
         "EventIntegrationAssociationId": str,
         "EventIntegrationName": str,
         "ClientId": str,
@@ -294,33 +266,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -412,37 +365,53 @@
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
-        "ScheduleConfiguration": ScheduleConfigurationOutputTypeDef,
+        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
         "ClientToken": str,
         "FileConfiguration": FileConfigurationOutputTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEventIntegrationResponseTypeDef = TypedDict(
+    "CreateEventIntegrationResponseTypeDef",
+    {
+        "EventIntegrationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataIntegrationResponseTypeDef = TypedDict(
     "GetDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
-        "ScheduleConfiguration": ScheduleConfigurationOutputTypeDef,
+        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
         "FileConfiguration": FileConfigurationOutputTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
@@ -464,68 +433,68 @@
 class CreateEventIntegrationRequestRequestTypeDef(
     _RequiredCreateEventIntegrationRequestRequestTypeDef,
     _OptionalCreateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
 
-ListDataIntegrationAssociationsResponseTypeDef = TypedDict(
-    "ListDataIntegrationAssociationsResponseTypeDef",
-    {
-        "DataIntegrationAssociations": List[DataIntegrationAssociationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDataIntegrationsResponseTypeDef = TypedDict(
-    "ListDataIntegrationsResponseTypeDef",
-    {
-        "DataIntegrations": List[DataIntegrationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventIntegrationTypeDef = TypedDict(
     "EventIntegrationTypeDef",
     {
         "EventIntegrationArn": str,
         "Name": str,
         "Description": str,
-        "EventFilter": EventFilterOutputTypeDef,
+        "EventFilter": EventFilterTypeDef,
         "EventBridgeBus": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
 GetEventIntegrationResponseTypeDef = TypedDict(
     "GetEventIntegrationResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "EventIntegrationArn": str,
         "EventBridgeBus": str,
-        "EventFilter": EventFilterOutputTypeDef,
+        "EventFilter": EventFilterTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDataIntegrationAssociationsResponseTypeDef = TypedDict(
+    "ListDataIntegrationAssociationsResponseTypeDef",
+    {
+        "DataIntegrationAssociations": List[DataIntegrationAssociationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDataIntegrationsResponseTypeDef = TypedDict(
+    "ListDataIntegrationsResponseTypeDef",
+    {
+        "DataIntegrations": List[DataIntegrationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListEventIntegrationAssociationsResponseTypeDef",
     {
         "EventIntegrationAssociations": List[EventIntegrationAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventIntegrationsResponseTypeDef = TypedDict(
     "ListEventIntegrationsResponseTypeDef",
     {
         "EventIntegrations": List[EventIntegrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/type_defs.pyi` & `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -19,44 +19,42 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FileConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
     "FileConfigurationOutputTypeDef",
-    "ScheduleConfigurationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "EventFilterTypeDef",
-    "CreateEventIntegrationResponseTypeDef",
     "DataIntegrationAssociationSummaryTypeDef",
     "DataIntegrationSummaryTypeDef",
     "DeleteDataIntegrationRequestRequestTypeDef",
     "DeleteEventIntegrationRequestRequestTypeDef",
-    "EventFilterOutputTypeDef",
     "EventIntegrationAssociationTypeDef",
     "GetDataIntegrationRequestRequestTypeDef",
     "GetEventIntegrationRequestRequestTypeDef",
     "ListDataIntegrationAssociationsRequestRequestTypeDef",
     "ListDataIntegrationsRequestRequestTypeDef",
     "ListEventIntegrationAssociationsRequestRequestTypeDef",
     "ListEventIntegrationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataIntegrationRequestRequestTypeDef",
     "UpdateEventIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationResponseTypeDef",
+    "CreateEventIntegrationResponseTypeDef",
     "GetDataIntegrationResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateEventIntegrationRequestRequestTypeDef",
-    "ListDataIntegrationAssociationsResponseTypeDef",
-    "ListDataIntegrationsResponseTypeDef",
     "EventIntegrationTypeDef",
     "GetEventIntegrationResponseTypeDef",
+    "ListDataIntegrationAssociationsResponseTypeDef",
+    "ListDataIntegrationsResponseTypeDef",
     "ListEventIntegrationAssociationsResponseTypeDef",
     "ListEventIntegrationsResponseTypeDef",
 )
 
 _RequiredFileConfigurationTypeDef = TypedDict(
     "_RequiredFileConfigurationTypeDef",
     {
@@ -111,49 +109,32 @@
 )
 
 class FileConfigurationOutputTypeDef(
     _RequiredFileConfigurationOutputTypeDef, _OptionalFileConfigurationOutputTypeDef
 ):
     pass
 
-_RequiredScheduleConfigurationOutputTypeDef = TypedDict(
-    "_RequiredScheduleConfigurationOutputTypeDef",
-    {
-        "ScheduleExpression": str,
-    },
-)
-_OptionalScheduleConfigurationOutputTypeDef = TypedDict(
-    "_OptionalScheduleConfigurationOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "FirstExecutionFrom": str,
-        "Object": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class ScheduleConfigurationOutputTypeDef(
-    _RequiredScheduleConfigurationOutputTypeDef, _OptionalScheduleConfigurationOutputTypeDef
-):
-    pass
-
 EventFilterTypeDef = TypedDict(
     "EventFilterTypeDef",
     {
         "Source": str,
     },
 )
 
-CreateEventIntegrationResponseTypeDef = TypedDict(
-    "CreateEventIntegrationResponseTypeDef",
-    {
-        "EventIntegrationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataIntegrationAssociationSummaryTypeDef = TypedDict(
     "DataIntegrationAssociationSummaryTypeDef",
     {
         "DataIntegrationAssociationArn": str,
         "DataIntegrationArn": str,
         "ClientId": str,
     },
@@ -180,21 +161,14 @@
 DeleteEventIntegrationRequestRequestTypeDef = TypedDict(
     "DeleteEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-EventFilterOutputTypeDef = TypedDict(
-    "EventFilterOutputTypeDef",
-    {
-        "Source": str,
-    },
-)
-
 EventIntegrationAssociationTypeDef = TypedDict(
     "EventIntegrationAssociationTypeDef",
     {
         "EventIntegrationAssociationArn": str,
         "EventIntegrationAssociationId": str,
         "EventIntegrationName": str,
         "ClientId": str,
@@ -281,33 +255,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -393,37 +348,53 @@
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
-        "ScheduleConfiguration": ScheduleConfigurationOutputTypeDef,
+        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
         "ClientToken": str,
         "FileConfiguration": FileConfigurationOutputTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEventIntegrationResponseTypeDef = TypedDict(
+    "CreateEventIntegrationResponseTypeDef",
+    {
+        "EventIntegrationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataIntegrationResponseTypeDef = TypedDict(
     "GetDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
-        "ScheduleConfiguration": ScheduleConfigurationOutputTypeDef,
+        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
         "FileConfiguration": FileConfigurationOutputTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
@@ -443,68 +414,68 @@
 
 class CreateEventIntegrationRequestRequestTypeDef(
     _RequiredCreateEventIntegrationRequestRequestTypeDef,
     _OptionalCreateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
-ListDataIntegrationAssociationsResponseTypeDef = TypedDict(
-    "ListDataIntegrationAssociationsResponseTypeDef",
-    {
-        "DataIntegrationAssociations": List[DataIntegrationAssociationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDataIntegrationsResponseTypeDef = TypedDict(
-    "ListDataIntegrationsResponseTypeDef",
-    {
-        "DataIntegrations": List[DataIntegrationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventIntegrationTypeDef = TypedDict(
     "EventIntegrationTypeDef",
     {
         "EventIntegrationArn": str,
         "Name": str,
         "Description": str,
-        "EventFilter": EventFilterOutputTypeDef,
+        "EventFilter": EventFilterTypeDef,
         "EventBridgeBus": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
 GetEventIntegrationResponseTypeDef = TypedDict(
     "GetEventIntegrationResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "EventIntegrationArn": str,
         "EventBridgeBus": str,
-        "EventFilter": EventFilterOutputTypeDef,
+        "EventFilter": EventFilterTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDataIntegrationAssociationsResponseTypeDef = TypedDict(
+    "ListDataIntegrationAssociationsResponseTypeDef",
+    {
+        "DataIntegrationAssociations": List[DataIntegrationAssociationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDataIntegrationsResponseTypeDef = TypedDict(
+    "ListDataIntegrationsResponseTypeDef",
+    {
+        "DataIntegrations": List[DataIntegrationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListEventIntegrationAssociationsResponseTypeDef",
     {
         "EventIntegrationAssociations": List[EventIntegrationAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventIntegrationsResponseTypeDef = TypedDict(
     "ListEventIntegrationsResponseTypeDef",
     {
         "EventIntegrations": List[EventIntegrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/PKG-INFO` & `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appintegrations
-Version: 1.28.12
-Summary: Type annotations for boto3.AppIntegrationsService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppIntegrationsService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appintegrations)](https://pepy.tech/project/mypy-boto3-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppIntegrationsService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[boto3.AppIntegrationsService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,44 +300,42 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
     FileConfigurationOutputTypeDef,
-    ScheduleConfigurationOutputTypeDef,
+    ResponseMetadataTypeDef,
     EventFilterTypeDef,
-    CreateEventIntegrationResponseTypeDef,
     DataIntegrationAssociationSummaryTypeDef,
     DataIntegrationSummaryTypeDef,
     DeleteDataIntegrationRequestRequestTypeDef,
     DeleteEventIntegrationRequestRequestTypeDef,
-    EventFilterOutputTypeDef,
     EventIntegrationAssociationTypeDef,
     GetDataIntegrationRequestRequestTypeDef,
     GetEventIntegrationRequestRequestTypeDef,
     ListDataIntegrationAssociationsRequestRequestTypeDef,
     ListDataIntegrationsRequestRequestTypeDef,
     ListEventIntegrationAssociationsRequestRequestTypeDef,
     ListEventIntegrationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
     CreateDataIntegrationResponseTypeDef,
+    CreateEventIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
-    ListDataIntegrationAssociationsResponseTypeDef,
-    ListDataIntegrationsResponseTypeDef,
     EventIntegrationTypeDef,
     GetEventIntegrationResponseTypeDef,
+    ListDataIntegrationAssociationsResponseTypeDef,
+    ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
 )
 
 
 def get_structure() -> FileConfigurationTypeDef:
     return {...}
```

### Comparing `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/SOURCES.txt` & `mypy-boto3-appintegrations-1.28.15/mypy_boto3_appintegrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.12/setup.py` & `mypy-boto3-appintegrations-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appintegrations",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_appintegrations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppIntegrationsService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.AppIntegrationsService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

