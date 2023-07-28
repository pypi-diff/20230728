# Comparing `tmp/mypy-boto3-servicecatalog-appregistry-1.28.12.tar.gz` & `tmp/mypy-boto3-servicecatalog-appregistry-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicecatalog-appregistry-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
+gzip compressed data, was "mypy-boto3-servicecatalog-appregistry-1.28.15.tar", last modified: Fri Jul 28 20:43:44 2023, max compression
```

## Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12.tar` & `mypy-boto3-servicecatalog-appregistry-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.617291 mypy-boto3-servicecatalog-appregistry-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-27 11:49:38.617291 mypy-boto3-servicecatalog-appregistry-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.617291 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21071 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22117 2023-07-27 11:46:47.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22096 2023-07-27 11:46:47.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.617291 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.617291 mypy-boto3-servicecatalog-appregistry-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-appregistry-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.281872 mypy-boto3-servicecatalog-appregistry-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-07-28 20:43:44.281872 mypy-boto3-servicecatalog-appregistry-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.273872 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21071 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21668 2023-07-28 20:39:18.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21647 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:17.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.281872 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17142 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:44.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:44.281872 mypy-boto3-servicecatalog-appregistry-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-28 20:39:16.000000 mypy-boto3-servicecatalog-appregistry-1.28.15/setup.py
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/LICENSE` & `mypy-boto3-servicecatalog-appregistry-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/PKG-INFO` & `mypy-boto3-servicecatalog-appregistry-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog-appregistry
-Version: 1.28.12
-Summary: Type annotations for boto3.AppRegistry 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppRegistry 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog-appregistry)](https://pepy.tech/project/mypy-boto3-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRegistry 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
+[boto3.AppRegistry 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [mypy-boto3-servicecatalog-appregistry docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,15 +345,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_servicecatalog_appregistry.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_servicecatalog_appregistry.type_defs import (
-    TagQueryConfigurationOutputTypeDef,
     TagQueryConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociateAttributeGroupRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateResourceRequestRequestTypeDef,
     AttributeGroupDetailsTypeDef,
@@ -378,15 +377,14 @@
     ListTagsForResourceRequestRequestTypeDef,
     ResourceDetailsTypeDef,
     SyncResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateAttributeGroupRequestRequestTypeDef,
-    AppRegistryConfigurationOutputTypeDef,
     AppRegistryConfigurationTypeDef,
     AssociateAttributeGroupResponseTypeDef,
     AssociateResourceResponseTypeDef,
     CreateApplicationResponseTypeDef,
     DeleteApplicationResponseTypeDef,
     DisassociateAttributeGroupResponseTypeDef,
     DisassociateResourceResponseTypeDef,
@@ -415,15 +413,15 @@
     GetApplicationResponseTypeDef,
     ResourceTypeDef,
     ListAssociatedResourcesResponseTypeDef,
     GetAssociatedResourceResponseTypeDef,
 )
 
 
-def get_structure() -> TagQueryConfigurationOutputTypeDef:
+def get_structure() -> TagQueryConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/README.md` & `mypy-boto3-servicecatalog-appregistry-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog-appregistry)](https://pepy.tech/project/mypy-boto3-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRegistry 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
+[boto3.AppRegistry 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [mypy-boto3-servicecatalog-appregistry docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,15 +313,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_servicecatalog_appregistry.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_servicecatalog_appregistry.type_defs import (
-    TagQueryConfigurationOutputTypeDef,
     TagQueryConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociateAttributeGroupRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateResourceRequestRequestTypeDef,
     AttributeGroupDetailsTypeDef,
@@ -346,15 +345,14 @@
     ListTagsForResourceRequestRequestTypeDef,
     ResourceDetailsTypeDef,
     SyncResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateAttributeGroupRequestRequestTypeDef,
-    AppRegistryConfigurationOutputTypeDef,
     AppRegistryConfigurationTypeDef,
     AssociateAttributeGroupResponseTypeDef,
     AssociateResourceResponseTypeDef,
     CreateApplicationResponseTypeDef,
     DeleteApplicationResponseTypeDef,
     DisassociateAttributeGroupResponseTypeDef,
     DisassociateResourceResponseTypeDef,
@@ -383,15 +381,15 @@
     GetApplicationResponseTypeDef,
     ResourceTypeDef,
     ListAssociatedResourcesResponseTypeDef,
     GetAssociatedResourceResponseTypeDef,
 )
 
 
-def get_structure() -> TagQueryConfigurationOutputTypeDef:
+def get_structure() -> TagQueryConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/__init__.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/__init__.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/__main__.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppRegistry 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.AppRegistry 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry\nOther"
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

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/client.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/client.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/literals.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/literals.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/paginator.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/paginator.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/type_defs.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for servicecatalog-appregistry service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_servicecatalog_appregistry.type_defs import TagQueryConfigurationOutputTypeDef
+    from mypy_boto3_servicecatalog_appregistry.type_defs import TagQueryConfigurationTypeDef
 
-    data: TagQueryConfigurationOutputTypeDef = {...}
+    data: TagQueryConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ResourceGroupStateType, ResourceTypeType, SyncActionType
@@ -20,15 +20,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "TagQueryConfigurationOutputTypeDef",
     "TagQueryConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "AssociateAttributeGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateResourceRequestRequestTypeDef",
     "AttributeGroupDetailsTypeDef",
@@ -53,15 +52,14 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceDetailsTypeDef",
     "SyncResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateAttributeGroupRequestRequestTypeDef",
-    "AppRegistryConfigurationOutputTypeDef",
     "AppRegistryConfigurationTypeDef",
     "AssociateAttributeGroupResponseTypeDef",
     "AssociateResourceResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "DeleteApplicationResponseTypeDef",
     "DisassociateAttributeGroupResponseTypeDef",
     "DisassociateResourceResponseTypeDef",
@@ -89,22 +87,14 @@
     "PutConfigurationRequestRequestTypeDef",
     "GetApplicationResponseTypeDef",
     "ResourceTypeDef",
     "ListAssociatedResourcesResponseTypeDef",
     "GetAssociatedResourceResponseTypeDef",
 )
 
-TagQueryConfigurationOutputTypeDef = TypedDict(
-    "TagQueryConfigurationOutputTypeDef",
-    {
-        "tagKey": str,
-    },
-    total=False,
-)
-
 TagQueryConfigurationTypeDef = TypedDict(
     "TagQueryConfigurationTypeDef",
     {
         "tagKey": str,
     },
     total=False,
 )
@@ -493,22 +483,14 @@
 class UpdateAttributeGroupRequestRequestTypeDef(
     _RequiredUpdateAttributeGroupRequestRequestTypeDef,
     _OptionalUpdateAttributeGroupRequestRequestTypeDef,
 ):
     pass
 
 
-AppRegistryConfigurationOutputTypeDef = TypedDict(
-    "AppRegistryConfigurationOutputTypeDef",
-    {
-        "tagQueryConfiguration": TagQueryConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 AppRegistryConfigurationTypeDef = TypedDict(
     "AppRegistryConfigurationTypeDef",
     {
         "tagQueryConfiguration": TagQueryConfigurationTypeDef,
     },
     total=False,
 )
@@ -786,15 +768,15 @@
     },
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
-        "configuration": AppRegistryConfigurationOutputTypeDef,
+        "configuration": AppRegistryConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutConfigurationRequestRequestTypeDef = TypedDict(
     "PutConfigurationRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry/type_defs.pyi` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,31 @@
 Type annotations for servicecatalog-appregistry service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_servicecatalog_appregistry.type_defs import TagQueryConfigurationOutputTypeDef
+    from mypy_boto3_servicecatalog_appregistry.type_defs import TagQueryConfigurationTypeDef
 
-    data: TagQueryConfigurationOutputTypeDef = {...}
+    data: TagQueryConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ResourceGroupStateType, ResourceTypeType, SyncActionType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "TagQueryConfigurationOutputTypeDef",
     "TagQueryConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "AssociateAttributeGroupRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateResourceRequestRequestTypeDef",
     "AttributeGroupDetailsTypeDef",
@@ -52,15 +51,14 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceDetailsTypeDef",
     "SyncResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateAttributeGroupRequestRequestTypeDef",
-    "AppRegistryConfigurationOutputTypeDef",
     "AppRegistryConfigurationTypeDef",
     "AssociateAttributeGroupResponseTypeDef",
     "AssociateResourceResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "DeleteApplicationResponseTypeDef",
     "DisassociateAttributeGroupResponseTypeDef",
     "DisassociateResourceResponseTypeDef",
@@ -88,22 +86,14 @@
     "PutConfigurationRequestRequestTypeDef",
     "GetApplicationResponseTypeDef",
     "ResourceTypeDef",
     "ListAssociatedResourcesResponseTypeDef",
     "GetAssociatedResourceResponseTypeDef",
 )
 
-TagQueryConfigurationOutputTypeDef = TypedDict(
-    "TagQueryConfigurationOutputTypeDef",
-    {
-        "tagKey": str,
-    },
-    total=False,
-)
-
 TagQueryConfigurationTypeDef = TypedDict(
     "TagQueryConfigurationTypeDef",
     {
         "tagKey": str,
     },
     total=False,
 )
@@ -478,22 +468,14 @@
 
 class UpdateAttributeGroupRequestRequestTypeDef(
     _RequiredUpdateAttributeGroupRequestRequestTypeDef,
     _OptionalUpdateAttributeGroupRequestRequestTypeDef,
 ):
     pass
 
-AppRegistryConfigurationOutputTypeDef = TypedDict(
-    "AppRegistryConfigurationOutputTypeDef",
-    {
-        "tagQueryConfiguration": TagQueryConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 AppRegistryConfigurationTypeDef = TypedDict(
     "AppRegistryConfigurationTypeDef",
     {
         "tagQueryConfiguration": TagQueryConfigurationTypeDef,
     },
     total=False,
 )
@@ -765,15 +747,15 @@
     },
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
-        "configuration": AppRegistryConfigurationOutputTypeDef,
+        "configuration": AppRegistryConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutConfigurationRequestRequestTypeDef = TypedDict(
     "PutConfigurationRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog-appregistry
-Version: 1.28.12
-Summary: Type annotations for boto3.AppRegistry 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppRegistry 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog-appregistry.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog-appregistry)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog-appregistry)](https://pepy.tech/project/mypy-boto3-servicecatalog-appregistry)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRegistry 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
+[boto3.AppRegistry 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#AppRegistry)
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
 [mypy-boto3-servicecatalog-appregistry docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog_appregistry/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,15 +345,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_servicecatalog_appregistry.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_servicecatalog_appregistry.type_defs import (
-    TagQueryConfigurationOutputTypeDef,
     TagQueryConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociateAttributeGroupRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociateResourceRequestRequestTypeDef,
     AttributeGroupDetailsTypeDef,
@@ -378,15 +377,14 @@
     ListTagsForResourceRequestRequestTypeDef,
     ResourceDetailsTypeDef,
     SyncResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateAttributeGroupRequestRequestTypeDef,
-    AppRegistryConfigurationOutputTypeDef,
     AppRegistryConfigurationTypeDef,
     AssociateAttributeGroupResponseTypeDef,
     AssociateResourceResponseTypeDef,
     CreateApplicationResponseTypeDef,
     DeleteApplicationResponseTypeDef,
     DisassociateAttributeGroupResponseTypeDef,
     DisassociateResourceResponseTypeDef,
@@ -415,15 +413,15 @@
     GetApplicationResponseTypeDef,
     ResourceTypeDef,
     ListAssociatedResourcesResponseTypeDef,
     GetAssociatedResourceResponseTypeDef,
 )
 
 
-def get_structure() -> TagQueryConfigurationOutputTypeDef:
+def get_structure() -> TagQueryConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt` & `mypy-boto3-servicecatalog-appregistry-1.28.15/mypy_boto3_servicecatalog_appregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-appregistry-1.28.12/setup.py` & `mypy-boto3-servicecatalog-appregistry-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-servicecatalog-appregistry",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_servicecatalog_appregistry"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppRegistry 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.AppRegistry 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

