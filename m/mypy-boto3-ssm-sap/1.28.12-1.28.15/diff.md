# Comparing `tmp/mypy-boto3-ssm-sap-1.28.12.tar.gz` & `tmp/mypy-boto3-ssm-sap-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-sap-1.28.12.tar", last modified: Thu Jul 27 11:49:43 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-sap-1.28.15.tar", last modified: Fri Jul 28 20:43:49 2023, max compression
```

## Comparing `mypy-boto3-ssm-sap-1.28.12.tar` & `mypy-boto3-ssm-sap-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.725340 mypy-boto3-ssm-sap-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-07-27 11:49:43.725340 mypy-boto3-ssm-sap-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.705340 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-07-27 11:47:33.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17286 2023-07-27 11:47:35.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-07-27 11:47:33.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.725340 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-07-27 11:49:43.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 11:49:43.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:43.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 11:49:43.000000 mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:43.725340 mypy-boto3-ssm-sap-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-27 11:47:32.000000 mypy-boto3-ssm-sap-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.013936 mypy-boto3-ssm-sap-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-07-28 20:43:49.013936 mypy-boto3-ssm-sap-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.005936 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-07-28 20:40:11.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17009 2023-07-28 20:40:11.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.013936 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-07-28 20:43:48.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-28 20:43:48.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:48.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:43:48.000000 mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:49.013936 mypy-boto3-ssm-sap-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-28 20:40:07.000000 mypy-boto3-ssm-sap-1.28.15/setup.py
```

### Comparing `mypy-boto3-ssm-sap-1.28.12/LICENSE` & `mypy-boto3-ssm-sap-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.12/PKG-INFO` & `mypy-boto3-ssm-sap-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-sap
-Version: 1.28.12
-Summary: Type annotations for boto3.SsmSap 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SsmSap 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-sap)](https://pepy.tech/project/mypy-boto3-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SsmSap 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[boto3.SsmSap 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
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
 [mypy-boto3-ssm-sap docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,15 +345,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_ssm_sap.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_sap.type_defs import (
-    ApplicationCredentialOutputTypeDef,
     ApplicationCredentialTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociatedHostTypeDef,
     BackintConfigTypeDef,
     ComponentSummaryTypeDef,
     HostTypeDef,
@@ -401,15 +400,15 @@
     ListDatabasesInputListDatabasesPaginateTypeDef,
     ListOperationsInputListOperationsPaginateTypeDef,
     GetDatabaseOutputTypeDef,
     GetComponentOutputTypeDef,
 )
 
 
-def get_structure() -> ApplicationCredentialOutputTypeDef:
+def get_structure() -> ApplicationCredentialTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-sap-1.28.12/README.md` & `mypy-boto3-ssm-sap-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-sap)](https://pepy.tech/project/mypy-boto3-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SsmSap 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[boto3.SsmSap 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
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
 [mypy-boto3-ssm-sap docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,15 +313,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_ssm_sap.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_sap.type_defs import (
-    ApplicationCredentialOutputTypeDef,
     ApplicationCredentialTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociatedHostTypeDef,
     BackintConfigTypeDef,
     ComponentSummaryTypeDef,
     HostTypeDef,
@@ -369,15 +368,15 @@
     ListDatabasesInputListDatabasesPaginateTypeDef,
     ListOperationsInputListOperationsPaginateTypeDef,
     GetDatabaseOutputTypeDef,
     GetComponentOutputTypeDef,
 )
 
 
-def get_structure() -> ApplicationCredentialOutputTypeDef:
+def get_structure() -> ApplicationCredentialTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/__init__.py` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/__init__.pyi` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/__main__.py` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SsmSap 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.SsmSap 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap\nOther"
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

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/client.py` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/client.pyi` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/literals.py` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/literals.pyi` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/paginator.py` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/paginator.pyi` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/type_defs.py` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ssm-sap service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ssm_sap.type_defs import ApplicationCredentialOutputTypeDef
+    from mypy_boto3_ssm_sap.type_defs import ApplicationCredentialTypeDef
 
-    data: ApplicationCredentialOutputTypeDef = {...}
+    data: ApplicationCredentialTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -37,15 +37,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ApplicationCredentialOutputTypeDef",
     "ApplicationCredentialTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "AssociatedHostTypeDef",
     "BackintConfigTypeDef",
     "ComponentSummaryTypeDef",
     "HostTypeDef",
@@ -92,23 +91,14 @@
     "ListComponentsInputListComponentsPaginateTypeDef",
     "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListOperationsInputListOperationsPaginateTypeDef",
     "GetDatabaseOutputTypeDef",
     "GetComponentOutputTypeDef",
 )
 
-ApplicationCredentialOutputTypeDef = TypedDict(
-    "ApplicationCredentialOutputTypeDef",
-    {
-        "DatabaseName": str,
-        "CredentialType": Literal["ADMIN"],
-        "SecretId": str,
-    },
-)
-
 ApplicationCredentialTypeDef = TypedDict(
     "ApplicationCredentialTypeDef",
     {
         "DatabaseName": str,
         "CredentialType": Literal["ADMIN"],
         "SecretId": str,
     },
@@ -414,15 +404,15 @@
 )
 
 DatabaseTypeDef = TypedDict(
     "DatabaseTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
-        "Credentials": List[ApplicationCredentialOutputTypeDef],
+        "Credentials": List[ApplicationCredentialTypeDef],
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseType": DatabaseTypeType,
         "Arn": str,
         "Status": DatabaseStatusType,
         "PrimaryHost": str,
         "SQLPort": int,
```

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap/type_defs.pyi` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ssm-sap service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ssm_sap.type_defs import ApplicationCredentialOutputTypeDef
+    from mypy_boto3_ssm_sap.type_defs import ApplicationCredentialTypeDef
 
-    data: ApplicationCredentialOutputTypeDef = {...}
+    data: ApplicationCredentialTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -36,15 +36,14 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ApplicationCredentialOutputTypeDef",
     "ApplicationCredentialTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationTypeDef",
     "AssociatedHostTypeDef",
     "BackintConfigTypeDef",
     "ComponentSummaryTypeDef",
     "HostTypeDef",
@@ -91,23 +90,14 @@
     "ListComponentsInputListComponentsPaginateTypeDef",
     "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListOperationsInputListOperationsPaginateTypeDef",
     "GetDatabaseOutputTypeDef",
     "GetComponentOutputTypeDef",
 )
 
-ApplicationCredentialOutputTypeDef = TypedDict(
-    "ApplicationCredentialOutputTypeDef",
-    {
-        "DatabaseName": str,
-        "CredentialType": Literal["ADMIN"],
-        "SecretId": str,
-    },
-)
-
 ApplicationCredentialTypeDef = TypedDict(
     "ApplicationCredentialTypeDef",
     {
         "DatabaseName": str,
         "CredentialType": Literal["ADMIN"],
         "SecretId": str,
     },
@@ -409,15 +399,15 @@
 )
 
 DatabaseTypeDef = TypedDict(
     "DatabaseTypeDef",
     {
         "ApplicationId": str,
         "ComponentId": str,
-        "Credentials": List[ApplicationCredentialOutputTypeDef],
+        "Credentials": List[ApplicationCredentialTypeDef],
         "DatabaseId": str,
         "DatabaseName": str,
         "DatabaseType": DatabaseTypeType,
         "Arn": str,
         "Status": DatabaseStatusType,
         "PrimaryHost": str,
         "SQLPort": int,
```

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/PKG-INFO` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-sap
-Version: 1.28.12
-Summary: Type annotations for boto3.SsmSap 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SsmSap 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-sap.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-sap)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-sap)](https://pepy.tech/project/mypy-boto3-ssm-sap)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SsmSap 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
+[boto3.SsmSap 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#SsmSap)
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
 [mypy-boto3-ssm-sap docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_sap/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,15 +345,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_ssm_sap.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_sap.type_defs import (
-    ApplicationCredentialOutputTypeDef,
     ApplicationCredentialTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationTypeDef,
     AssociatedHostTypeDef,
     BackintConfigTypeDef,
     ComponentSummaryTypeDef,
     HostTypeDef,
@@ -401,15 +400,15 @@
     ListDatabasesInputListDatabasesPaginateTypeDef,
     ListOperationsInputListOperationsPaginateTypeDef,
     GetDatabaseOutputTypeDef,
     GetComponentOutputTypeDef,
 )
 
 
-def get_structure() -> ApplicationCredentialOutputTypeDef:
+def get_structure() -> ApplicationCredentialTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ssm-sap-1.28.12/mypy_boto3_ssm_sap.egg-info/SOURCES.txt` & `mypy-boto3-ssm-sap-1.28.15/mypy_boto3_ssm_sap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-sap-1.28.12/setup.py` & `mypy-boto3-ssm-sap-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-sap",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ssm_sap"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SsmSap 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SsmSap 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

