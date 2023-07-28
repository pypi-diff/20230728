# Comparing `tmp/mypy-boto3-healthlake-1.28.12.tar.gz` & `tmp/mypy-boto3-healthlake-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-healthlake-1.28.12.tar", last modified: Thu Jul 27 05:34:45 2023, max compression
+gzip compressed data, was "mypy-boto3-healthlake-1.28.15.tar", last modified: Fri Jul 28 20:42:53 2023, max compression
```

## Comparing `mypy-boto3-healthlake-1.28.12.tar` & `mypy-boto3-healthlake-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.736496 mypy-boto3-healthlake-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-07-27 05:34:45.736496 mypy-boto3-healthlake-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.736496 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-27 05:23:18.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-07-27 05:23:18.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16502 2023-07-27 05:23:18.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-07-27 05:23:18.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.736496 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-07-27 05:34:45.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 05:34:45.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:45.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:45.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:45.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:45.000000 mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:45.736496 mypy-boto3-healthlake-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:23:17.000000 mypy-boto3-healthlake-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.337173 mypy-boto3-healthlake-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-07-28 20:42:53.333173 mypy-boto3-healthlake-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.321172 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-07-28 20:27:21.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.333173 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-07-28 20:42:53.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 20:42:53.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:53.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:53.000000 mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:53.337173 mypy-boto3-healthlake-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:27:20.000000 mypy-boto3-healthlake-1.28.15/setup.py
```

### Comparing `mypy-boto3-healthlake-1.28.12/LICENSE` & `mypy-boto3-healthlake-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.28.12/PKG-INFO` & `mypy-boto3-healthlake-1.28.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-healthlake
-Version: 1.28.12
-Summary: Type annotations for boto3.HealthLake 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.HealthLake 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-healthlake)](https://pepy.tech/project/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,46 +304,38 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
-    CreateFHIRDatastoreResponseTypeDef,
+    ResponseMetadataTypeDef,
     DatastoreFilterTypeDef,
-    IdentityProviderConfigurationOutputTypeDef,
-    PreloadDataConfigOutputTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
-    DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
-    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
-    KmsEncryptionConfigOutputTypeDef,
     KmsEncryptionConfigTypeDef,
     ListFHIRExportJobsRequestRequestTypeDef,
     ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    StartFHIRExportJobResponseTypeDef,
-    StartFHIRImportJobResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateFHIRDatastoreResponseTypeDef,
+    DeleteFHIRDatastoreResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartFHIRExportJobResponseTypeDef,
+    StartFHIRImportJobResponseTypeDef,
     ListFHIRDatastoresRequestRequestTypeDef,
-    SseConfigurationOutputTypeDef,
     SseConfigurationTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    OutputDataConfigOutputTypeDef,
     OutputDataConfigTypeDef,
-    DatastorePropertiesTypeDef,
     CreateFHIRDatastoreRequestRequestTypeDef,
+    DatastorePropertiesTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
     StartFHIRExportJobRequestRequestTypeDef,
     StartFHIRImportJobRequestRequestTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
     ListFHIRDatastoresResponseTypeDef,
     DescribeFHIRExportJobResponseTypeDef,
```

### Comparing `mypy-boto3-healthlake-1.28.12/README.md` & `mypy-boto3-healthlake-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-healthlake)](https://pepy.tech/project/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,46 +272,38 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
-    CreateFHIRDatastoreResponseTypeDef,
+    ResponseMetadataTypeDef,
     DatastoreFilterTypeDef,
-    IdentityProviderConfigurationOutputTypeDef,
-    PreloadDataConfigOutputTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
-    DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
-    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
-    KmsEncryptionConfigOutputTypeDef,
     KmsEncryptionConfigTypeDef,
     ListFHIRExportJobsRequestRequestTypeDef,
     ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    StartFHIRExportJobResponseTypeDef,
-    StartFHIRImportJobResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateFHIRDatastoreResponseTypeDef,
+    DeleteFHIRDatastoreResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartFHIRExportJobResponseTypeDef,
+    StartFHIRImportJobResponseTypeDef,
     ListFHIRDatastoresRequestRequestTypeDef,
-    SseConfigurationOutputTypeDef,
     SseConfigurationTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    OutputDataConfigOutputTypeDef,
     OutputDataConfigTypeDef,
-    DatastorePropertiesTypeDef,
     CreateFHIRDatastoreRequestRequestTypeDef,
+    DatastorePropertiesTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
     StartFHIRExportJobRequestRequestTypeDef,
     StartFHIRImportJobRequestRequestTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
     ListFHIRDatastoresResponseTypeDef,
     DescribeFHIRExportJobResponseTypeDef,
```

### Comparing `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/__main__.py` & `mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.HealthLake 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.HealthLake 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake\nOther"
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

### Comparing `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/client.py` & `mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/client.pyi` & `mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/literals.py` & `mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/literals.pyi` & `mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/type_defs.py` & `mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/type_defs.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,46 +27,38 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
-    "CreateFHIRDatastoreResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DatastoreFilterTypeDef",
-    "IdentityProviderConfigurationOutputTypeDef",
-    "PreloadDataConfigOutputTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
-    "DeleteFHIRDatastoreResponseTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
     "DescribeFHIRImportJobRequestRequestTypeDef",
-    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
-    "KmsEncryptionConfigOutputTypeDef",
     "KmsEncryptionConfigTypeDef",
     "ListFHIRExportJobsRequestRequestTypeDef",
     "ListFHIRImportJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "S3ConfigurationOutputTypeDef",
     "S3ConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartFHIRExportJobResponseTypeDef",
-    "StartFHIRImportJobResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateFHIRDatastoreResponseTypeDef",
+    "DeleteFHIRDatastoreResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartFHIRExportJobResponseTypeDef",
+    "StartFHIRImportJobResponseTypeDef",
     "ListFHIRDatastoresRequestRequestTypeDef",
-    "SseConfigurationOutputTypeDef",
     "SseConfigurationTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "OutputDataConfigOutputTypeDef",
     "OutputDataConfigTypeDef",
-    "DatastorePropertiesTypeDef",
     "CreateFHIRDatastoreRequestRequestTypeDef",
+    "DatastorePropertiesTypeDef",
     "ExportJobPropertiesTypeDef",
     "ImportJobPropertiesTypeDef",
     "StartFHIRExportJobRequestRequestTypeDef",
     "StartFHIRImportJobRequestRequestTypeDef",
     "DescribeFHIRDatastoreResponseTypeDef",
     "ListFHIRDatastoresResponseTypeDef",
     "DescribeFHIRExportJobResponseTypeDef",
@@ -109,85 +101,43 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateFHIRDatastoreResponseTypeDef = TypedDict(
-    "CreateFHIRDatastoreResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "DatastoreEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DatastoreFilterTypeDef = TypedDict(
     "DatastoreFilterTypeDef",
     {
         "DatastoreName": str,
         "DatastoreStatus": DatastoreStatusType,
         "CreatedBefore": Union[datetime, str],
         "CreatedAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredIdentityProviderConfigurationOutputTypeDef = TypedDict(
-    "_RequiredIdentityProviderConfigurationOutputTypeDef",
-    {
-        "AuthorizationStrategy": AuthorizationStrategyType,
-    },
-)
-_OptionalIdentityProviderConfigurationOutputTypeDef = TypedDict(
-    "_OptionalIdentityProviderConfigurationOutputTypeDef",
-    {
-        "FineGrainedAuthorizationEnabled": bool,
-        "Metadata": str,
-        "IdpLambdaArn": str,
-    },
-    total=False,
-)
-
-
-class IdentityProviderConfigurationOutputTypeDef(
-    _RequiredIdentityProviderConfigurationOutputTypeDef,
-    _OptionalIdentityProviderConfigurationOutputTypeDef,
-):
-    pass
-
-
-PreloadDataConfigOutputTypeDef = TypedDict(
-    "PreloadDataConfigOutputTypeDef",
-    {
-        "PreloadDataType": Literal["SYNTHEA"],
-    },
-)
-
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
-DeleteFHIRDatastoreResponseTypeDef = TypedDict(
-    "DeleteFHIRDatastoreResponseTypeDef",
-    {
-        "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "DatastoreEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
@@ -203,51 +153,22 @@
     "DescribeFHIRImportJobRequestRequestTypeDef",
     {
         "DatastoreId": str,
         "JobId": str,
     },
 )
 
-InputDataConfigOutputTypeDef = TypedDict(
-    "InputDataConfigOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-    total=False,
-)
-
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
     total=False,
 )
 
-_RequiredKmsEncryptionConfigOutputTypeDef = TypedDict(
-    "_RequiredKmsEncryptionConfigOutputTypeDef",
-    {
-        "CmkType": CmkTypeType,
-    },
-)
-_OptionalKmsEncryptionConfigOutputTypeDef = TypedDict(
-    "_OptionalKmsEncryptionConfigOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class KmsEncryptionConfigOutputTypeDef(
-    _RequiredKmsEncryptionConfigOutputTypeDef, _OptionalKmsEncryptionConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredKmsEncryptionConfigTypeDef = TypedDict(
     "_RequiredKmsEncryptionConfigTypeDef",
     {
         "CmkType": CmkTypeType,
     },
 )
 _OptionalKmsEncryptionConfigTypeDef = TypedDict(
@@ -322,197 +243,177 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+S3ConfigurationTypeDef = TypedDict(
+    "S3ConfigurationTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "S3Uri": str,
+        "KmsKeyId": str,
     },
 )
 
-S3ConfigurationOutputTypeDef = TypedDict(
-    "S3ConfigurationOutputTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "S3Uri": str,
-        "KmsKeyId": str,
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-S3ConfigurationTypeDef = TypedDict(
-    "S3ConfigurationTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "S3Uri": str,
-        "KmsKeyId": str,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateFHIRDatastoreResponseTypeDef = TypedDict(
+    "CreateFHIRDatastoreResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "DatastoreEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFHIRDatastoreResponseTypeDef = TypedDict(
+    "DeleteFHIRDatastoreResponseTypeDef",
+    {
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "DatastoreEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFHIRExportJobResponseTypeDef = TypedDict(
     "StartFHIRExportJobResponseTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "DatastoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFHIRImportJobResponseTypeDef = TypedDict(
     "StartFHIRImportJobResponseTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "DatastoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRDatastoresRequestRequestTypeDef = TypedDict(
     "ListFHIRDatastoresRequestRequestTypeDef",
     {
         "Filter": DatastoreFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-SseConfigurationOutputTypeDef = TypedDict(
-    "SseConfigurationOutputTypeDef",
-    {
-        "KmsEncryptionConfig": KmsEncryptionConfigOutputTypeDef,
-    },
-)
-
 SseConfigurationTypeDef = TypedDict(
     "SseConfigurationTypeDef",
     {
         "KmsEncryptionConfig": KmsEncryptionConfigTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-OutputDataConfigOutputTypeDef = TypedDict(
-    "OutputDataConfigOutputTypeDef",
-    {
-        "S3Configuration": S3ConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 OutputDataConfigTypeDef = TypedDict(
     "OutputDataConfigTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredDatastorePropertiesTypeDef = TypedDict(
-    "_RequiredDatastorePropertiesTypeDef",
+_RequiredCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFHIRDatastoreRequestRequestTypeDef",
     {
-        "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
         "DatastoreTypeVersion": Literal["R4"],
-        "DatastoreEndpoint": str,
     },
 )
-_OptionalDatastorePropertiesTypeDef = TypedDict(
-    "_OptionalDatastorePropertiesTypeDef",
+_OptionalCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreName": str,
-        "CreatedAt": datetime,
-        "SseConfiguration": SseConfigurationOutputTypeDef,
-        "PreloadDataConfig": PreloadDataConfigOutputTypeDef,
-        "IdentityProviderConfiguration": IdentityProviderConfigurationOutputTypeDef,
+        "SseConfiguration": SseConfigurationTypeDef,
+        "PreloadDataConfig": PreloadDataConfigTypeDef,
+        "ClientToken": str,
+        "Tags": Sequence[TagTypeDef],
+        "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class DatastorePropertiesTypeDef(
-    _RequiredDatastorePropertiesTypeDef, _OptionalDatastorePropertiesTypeDef
+class CreateFHIRDatastoreRequestRequestTypeDef(
+    _RequiredCreateFHIRDatastoreRequestRequestTypeDef,
+    _OptionalCreateFHIRDatastoreRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFHIRDatastoreRequestRequestTypeDef",
+_RequiredDatastorePropertiesTypeDef = TypedDict(
+    "_RequiredDatastorePropertiesTypeDef",
     {
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
         "DatastoreTypeVersion": Literal["R4"],
+        "DatastoreEndpoint": str,
     },
 )
-_OptionalCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFHIRDatastoreRequestRequestTypeDef",
+_OptionalDatastorePropertiesTypeDef = TypedDict(
+    "_OptionalDatastorePropertiesTypeDef",
     {
         "DatastoreName": str,
+        "CreatedAt": datetime,
         "SseConfiguration": SseConfigurationTypeDef,
         "PreloadDataConfig": PreloadDataConfigTypeDef,
-        "ClientToken": str,
-        "Tags": Sequence[TagTypeDef],
         "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class CreateFHIRDatastoreRequestRequestTypeDef(
-    _RequiredCreateFHIRDatastoreRequestRequestTypeDef,
-    _OptionalCreateFHIRDatastoreRequestRequestTypeDef,
+class DatastorePropertiesTypeDef(
+    _RequiredDatastorePropertiesTypeDef, _OptionalDatastorePropertiesTypeDef
 ):
     pass
 
 
 _RequiredExportJobPropertiesTypeDef = TypedDict(
     "_RequiredExportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "SubmitTime": datetime,
         "DatastoreId": str,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
     },
 )
 _OptionalExportJobPropertiesTypeDef = TypedDict(
     "_OptionalExportJobPropertiesTypeDef",
     {
         "JobName": str,
         "EndTime": datetime,
@@ -532,23 +433,23 @@
 _RequiredImportJobPropertiesTypeDef = TypedDict(
     "_RequiredImportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "SubmitTime": datetime,
         "DatastoreId": str,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "InputDataConfig": InputDataConfigTypeDef,
     },
 )
 _OptionalImportJobPropertiesTypeDef = TypedDict(
     "_OptionalImportJobPropertiesTypeDef",
     {
         "JobName": str,
         "EndTime": datetime,
-        "JobOutputDataConfig": OutputDataConfigOutputTypeDef,
+        "JobOutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "Message": str,
     },
     total=False,
 )
 
 
@@ -609,53 +510,53 @@
     pass
 
 
 DescribeFHIRDatastoreResponseTypeDef = TypedDict(
     "DescribeFHIRDatastoreResponseTypeDef",
     {
         "DatastoreProperties": DatastorePropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRDatastoresResponseTypeDef = TypedDict(
     "ListFHIRDatastoresResponseTypeDef",
     {
         "DatastorePropertiesList": List[DatastorePropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFHIRExportJobResponseTypeDef = TypedDict(
     "DescribeFHIRExportJobResponseTypeDef",
     {
         "ExportJobProperties": ExportJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRExportJobsResponseTypeDef = TypedDict(
     "ListFHIRExportJobsResponseTypeDef",
     {
         "ExportJobPropertiesList": List[ExportJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFHIRImportJobResponseTypeDef = TypedDict(
     "DescribeFHIRImportJobResponseTypeDef",
     {
         "ImportJobProperties": ImportJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRImportJobsResponseTypeDef = TypedDict(
     "ListFHIRImportJobsResponseTypeDef",
     {
         "ImportJobPropertiesList": List[ImportJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake/type_defs.pyi` & `mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake/type_defs.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -26,46 +26,38 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "IdentityProviderConfigurationTypeDef",
     "PreloadDataConfigTypeDef",
     "TagTypeDef",
-    "CreateFHIRDatastoreResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DatastoreFilterTypeDef",
-    "IdentityProviderConfigurationOutputTypeDef",
-    "PreloadDataConfigOutputTypeDef",
     "DeleteFHIRDatastoreRequestRequestTypeDef",
-    "DeleteFHIRDatastoreResponseTypeDef",
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     "DescribeFHIRExportJobRequestRequestTypeDef",
     "DescribeFHIRImportJobRequestRequestTypeDef",
-    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
-    "KmsEncryptionConfigOutputTypeDef",
     "KmsEncryptionConfigTypeDef",
     "ListFHIRExportJobsRequestRequestTypeDef",
     "ListFHIRImportJobsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "S3ConfigurationOutputTypeDef",
     "S3ConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartFHIRExportJobResponseTypeDef",
-    "StartFHIRImportJobResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateFHIRDatastoreResponseTypeDef",
+    "DeleteFHIRDatastoreResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartFHIRExportJobResponseTypeDef",
+    "StartFHIRImportJobResponseTypeDef",
     "ListFHIRDatastoresRequestRequestTypeDef",
-    "SseConfigurationOutputTypeDef",
     "SseConfigurationTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "OutputDataConfigOutputTypeDef",
     "OutputDataConfigTypeDef",
-    "DatastorePropertiesTypeDef",
     "CreateFHIRDatastoreRequestRequestTypeDef",
+    "DatastorePropertiesTypeDef",
     "ExportJobPropertiesTypeDef",
     "ImportJobPropertiesTypeDef",
     "StartFHIRExportJobRequestRequestTypeDef",
     "StartFHIRImportJobRequestRequestTypeDef",
     "DescribeFHIRDatastoreResponseTypeDef",
     "ListFHIRDatastoresResponseTypeDef",
     "DescribeFHIRExportJobResponseTypeDef",
@@ -106,83 +98,43 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateFHIRDatastoreResponseTypeDef = TypedDict(
-    "CreateFHIRDatastoreResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "DatastoreEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DatastoreFilterTypeDef = TypedDict(
     "DatastoreFilterTypeDef",
     {
         "DatastoreName": str,
         "DatastoreStatus": DatastoreStatusType,
         "CreatedBefore": Union[datetime, str],
         "CreatedAfter": Union[datetime, str],
     },
     total=False,
 )
 
-_RequiredIdentityProviderConfigurationOutputTypeDef = TypedDict(
-    "_RequiredIdentityProviderConfigurationOutputTypeDef",
-    {
-        "AuthorizationStrategy": AuthorizationStrategyType,
-    },
-)
-_OptionalIdentityProviderConfigurationOutputTypeDef = TypedDict(
-    "_OptionalIdentityProviderConfigurationOutputTypeDef",
-    {
-        "FineGrainedAuthorizationEnabled": bool,
-        "Metadata": str,
-        "IdpLambdaArn": str,
-    },
-    total=False,
-)
-
-class IdentityProviderConfigurationOutputTypeDef(
-    _RequiredIdentityProviderConfigurationOutputTypeDef,
-    _OptionalIdentityProviderConfigurationOutputTypeDef,
-):
-    pass
-
-PreloadDataConfigOutputTypeDef = TypedDict(
-    "PreloadDataConfigOutputTypeDef",
-    {
-        "PreloadDataType": Literal["SYNTHEA"],
-    },
-)
-
 DeleteFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
-DeleteFHIRDatastoreResponseTypeDef = TypedDict(
-    "DeleteFHIRDatastoreResponseTypeDef",
-    {
-        "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
-        "DatastoreEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFHIRDatastoreRequestRequestTypeDef = TypedDict(
     "DescribeFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreId": str,
     },
 )
 
@@ -198,49 +150,22 @@
     "DescribeFHIRImportJobRequestRequestTypeDef",
     {
         "DatastoreId": str,
         "JobId": str,
     },
 )
 
-InputDataConfigOutputTypeDef = TypedDict(
-    "InputDataConfigOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-    total=False,
-)
-
 InputDataConfigTypeDef = TypedDict(
     "InputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
     total=False,
 )
 
-_RequiredKmsEncryptionConfigOutputTypeDef = TypedDict(
-    "_RequiredKmsEncryptionConfigOutputTypeDef",
-    {
-        "CmkType": CmkTypeType,
-    },
-)
-_OptionalKmsEncryptionConfigOutputTypeDef = TypedDict(
-    "_OptionalKmsEncryptionConfigOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class KmsEncryptionConfigOutputTypeDef(
-    _RequiredKmsEncryptionConfigOutputTypeDef, _OptionalKmsEncryptionConfigOutputTypeDef
-):
-    pass
-
 _RequiredKmsEncryptionConfigTypeDef = TypedDict(
     "_RequiredKmsEncryptionConfigTypeDef",
     {
         "CmkType": CmkTypeType,
     },
 )
 _OptionalKmsEncryptionConfigTypeDef = TypedDict(
@@ -309,193 +234,173 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+S3ConfigurationTypeDef = TypedDict(
+    "S3ConfigurationTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "S3Uri": str,
+        "KmsKeyId": str,
     },
 )
 
-S3ConfigurationOutputTypeDef = TypedDict(
-    "S3ConfigurationOutputTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "S3Uri": str,
-        "KmsKeyId": str,
+        "ResourceARN": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-S3ConfigurationTypeDef = TypedDict(
-    "S3ConfigurationTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "S3Uri": str,
-        "KmsKeyId": str,
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateFHIRDatastoreResponseTypeDef = TypedDict(
+    "CreateFHIRDatastoreResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "DatastoreEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFHIRDatastoreResponseTypeDef = TypedDict(
+    "DeleteFHIRDatastoreResponseTypeDef",
+    {
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
+        "DatastoreEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFHIRExportJobResponseTypeDef = TypedDict(
     "StartFHIRExportJobResponseTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "DatastoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFHIRImportJobResponseTypeDef = TypedDict(
     "StartFHIRImportJobResponseTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "DatastoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "TagKeys": Sequence[str],
-    },
-)
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRDatastoresRequestRequestTypeDef = TypedDict(
     "ListFHIRDatastoresRequestRequestTypeDef",
     {
         "Filter": DatastoreFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-SseConfigurationOutputTypeDef = TypedDict(
-    "SseConfigurationOutputTypeDef",
-    {
-        "KmsEncryptionConfig": KmsEncryptionConfigOutputTypeDef,
-    },
-)
-
 SseConfigurationTypeDef = TypedDict(
     "SseConfigurationTypeDef",
     {
         "KmsEncryptionConfig": KmsEncryptionConfigTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-OutputDataConfigOutputTypeDef = TypedDict(
-    "OutputDataConfigOutputTypeDef",
-    {
-        "S3Configuration": S3ConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 OutputDataConfigTypeDef = TypedDict(
     "OutputDataConfigTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredDatastorePropertiesTypeDef = TypedDict(
-    "_RequiredDatastorePropertiesTypeDef",
+_RequiredCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFHIRDatastoreRequestRequestTypeDef",
     {
-        "DatastoreId": str,
-        "DatastoreArn": str,
-        "DatastoreStatus": DatastoreStatusType,
         "DatastoreTypeVersion": Literal["R4"],
-        "DatastoreEndpoint": str,
     },
 )
-_OptionalDatastorePropertiesTypeDef = TypedDict(
-    "_OptionalDatastorePropertiesTypeDef",
+_OptionalCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFHIRDatastoreRequestRequestTypeDef",
     {
         "DatastoreName": str,
-        "CreatedAt": datetime,
-        "SseConfiguration": SseConfigurationOutputTypeDef,
-        "PreloadDataConfig": PreloadDataConfigOutputTypeDef,
-        "IdentityProviderConfiguration": IdentityProviderConfigurationOutputTypeDef,
+        "SseConfiguration": SseConfigurationTypeDef,
+        "PreloadDataConfig": PreloadDataConfigTypeDef,
+        "ClientToken": str,
+        "Tags": Sequence[TagTypeDef],
+        "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
-class DatastorePropertiesTypeDef(
-    _RequiredDatastorePropertiesTypeDef, _OptionalDatastorePropertiesTypeDef
+class CreateFHIRDatastoreRequestRequestTypeDef(
+    _RequiredCreateFHIRDatastoreRequestRequestTypeDef,
+    _OptionalCreateFHIRDatastoreRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFHIRDatastoreRequestRequestTypeDef",
+_RequiredDatastorePropertiesTypeDef = TypedDict(
+    "_RequiredDatastorePropertiesTypeDef",
     {
+        "DatastoreId": str,
+        "DatastoreArn": str,
+        "DatastoreStatus": DatastoreStatusType,
         "DatastoreTypeVersion": Literal["R4"],
+        "DatastoreEndpoint": str,
     },
 )
-_OptionalCreateFHIRDatastoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFHIRDatastoreRequestRequestTypeDef",
+_OptionalDatastorePropertiesTypeDef = TypedDict(
+    "_OptionalDatastorePropertiesTypeDef",
     {
         "DatastoreName": str,
+        "CreatedAt": datetime,
         "SseConfiguration": SseConfigurationTypeDef,
         "PreloadDataConfig": PreloadDataConfigTypeDef,
-        "ClientToken": str,
-        "Tags": Sequence[TagTypeDef],
         "IdentityProviderConfiguration": IdentityProviderConfigurationTypeDef,
     },
     total=False,
 )
 
-class CreateFHIRDatastoreRequestRequestTypeDef(
-    _RequiredCreateFHIRDatastoreRequestRequestTypeDef,
-    _OptionalCreateFHIRDatastoreRequestRequestTypeDef,
+class DatastorePropertiesTypeDef(
+    _RequiredDatastorePropertiesTypeDef, _OptionalDatastorePropertiesTypeDef
 ):
     pass
 
 _RequiredExportJobPropertiesTypeDef = TypedDict(
     "_RequiredExportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "SubmitTime": datetime,
         "DatastoreId": str,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
     },
 )
 _OptionalExportJobPropertiesTypeDef = TypedDict(
     "_OptionalExportJobPropertiesTypeDef",
     {
         "JobName": str,
         "EndTime": datetime,
@@ -513,23 +418,23 @@
 _RequiredImportJobPropertiesTypeDef = TypedDict(
     "_RequiredImportJobPropertiesTypeDef",
     {
         "JobId": str,
         "JobStatus": JobStatusType,
         "SubmitTime": datetime,
         "DatastoreId": str,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "InputDataConfig": InputDataConfigTypeDef,
     },
 )
 _OptionalImportJobPropertiesTypeDef = TypedDict(
     "_OptionalImportJobPropertiesTypeDef",
     {
         "JobName": str,
         "EndTime": datetime,
-        "JobOutputDataConfig": OutputDataConfigOutputTypeDef,
+        "JobOutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
         "Message": str,
     },
     total=False,
 )
 
 class ImportJobPropertiesTypeDef(
@@ -584,53 +489,53 @@
 ):
     pass
 
 DescribeFHIRDatastoreResponseTypeDef = TypedDict(
     "DescribeFHIRDatastoreResponseTypeDef",
     {
         "DatastoreProperties": DatastorePropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRDatastoresResponseTypeDef = TypedDict(
     "ListFHIRDatastoresResponseTypeDef",
     {
         "DatastorePropertiesList": List[DatastorePropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFHIRExportJobResponseTypeDef = TypedDict(
     "DescribeFHIRExportJobResponseTypeDef",
     {
         "ExportJobProperties": ExportJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRExportJobsResponseTypeDef = TypedDict(
     "ListFHIRExportJobsResponseTypeDef",
     {
         "ExportJobPropertiesList": List[ExportJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFHIRImportJobResponseTypeDef = TypedDict(
     "DescribeFHIRImportJobResponseTypeDef",
     {
         "ImportJobProperties": ImportJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFHIRImportJobsResponseTypeDef = TypedDict(
     "ListFHIRImportJobsResponseTypeDef",
     {
         "ImportJobPropertiesList": List[ImportJobPropertiesTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/PKG-INFO` & `mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-healthlake
-Version: 1.28.12
-Summary: Type annotations for boto3.HealthLake 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.HealthLake 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-healthlake.svg?color=blue)](https://pypi.org/project/mypy-boto3-healthlake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-healthlake)](https://pepy.tech/project/mypy-boto3-healthlake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthLake 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
+[boto3.HealthLake 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
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
 [mypy-boto3-healthlake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_healthlake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,46 +304,38 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_healthlake.type_defs import (
     IdentityProviderConfigurationTypeDef,
     PreloadDataConfigTypeDef,
     TagTypeDef,
-    CreateFHIRDatastoreResponseTypeDef,
+    ResponseMetadataTypeDef,
     DatastoreFilterTypeDef,
-    IdentityProviderConfigurationOutputTypeDef,
-    PreloadDataConfigOutputTypeDef,
     DeleteFHIRDatastoreRequestRequestTypeDef,
-    DeleteFHIRDatastoreResponseTypeDef,
     DescribeFHIRDatastoreRequestRequestTypeDef,
     DescribeFHIRExportJobRequestRequestTypeDef,
     DescribeFHIRImportJobRequestRequestTypeDef,
-    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
-    KmsEncryptionConfigOutputTypeDef,
     KmsEncryptionConfigTypeDef,
     ListFHIRExportJobsRequestRequestTypeDef,
     ListFHIRImportJobsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
-    ResponseMetadataTypeDef,
-    StartFHIRExportJobResponseTypeDef,
-    StartFHIRImportJobResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateFHIRDatastoreResponseTypeDef,
+    DeleteFHIRDatastoreResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartFHIRExportJobResponseTypeDef,
+    StartFHIRImportJobResponseTypeDef,
     ListFHIRDatastoresRequestRequestTypeDef,
-    SseConfigurationOutputTypeDef,
     SseConfigurationTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    OutputDataConfigOutputTypeDef,
     OutputDataConfigTypeDef,
-    DatastorePropertiesTypeDef,
     CreateFHIRDatastoreRequestRequestTypeDef,
+    DatastorePropertiesTypeDef,
     ExportJobPropertiesTypeDef,
     ImportJobPropertiesTypeDef,
     StartFHIRExportJobRequestRequestTypeDef,
     StartFHIRImportJobRequestRequestTypeDef,
     DescribeFHIRDatastoreResponseTypeDef,
     ListFHIRDatastoresResponseTypeDef,
     DescribeFHIRExportJobResponseTypeDef,
```

### Comparing `mypy-boto3-healthlake-1.28.12/mypy_boto3_healthlake.egg-info/SOURCES.txt` & `mypy-boto3-healthlake-1.28.15/mypy_boto3_healthlake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-healthlake-1.28.12/setup.py` & `mypy-boto3-healthlake-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-healthlake",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_healthlake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.HealthLake 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.HealthLake 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

