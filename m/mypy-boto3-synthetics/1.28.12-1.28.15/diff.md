# Comparing `tmp/mypy-boto3-synthetics-1.28.12.tar.gz` & `tmp/mypy-boto3-synthetics-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-synthetics-1.28.12.tar", last modified: Thu Jul 27 11:49:46 2023, max compression
+gzip compressed data, was "mypy-boto3-synthetics-1.28.15.tar", last modified: Fri Jul 28 20:43:52 2023, max compression
```

## Comparing `mypy-boto3-synthetics-1.28.12.tar` & `mypy-boto3-synthetics-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.381431 mypy-boto3-synthetics-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-07-27 11:49:46.381431 mypy-boto3-synthetics-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.377431 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19049 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.381431 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-07-27 11:49:46.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 11:49:46.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 11:49:46.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:46.381431 mypy-boto3-synthetics-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.297981 mypy-boto3-synthetics-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:33.000000 mypy-boto3-synthetics-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-07-28 20:43:52.293981 mypy-boto3-synthetics-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-07-28 20:40:33.000000 mypy-boto3-synthetics-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.285981 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-28 20:40:33.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-28 20:40:33.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:40:33.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-07-28 20:40:33.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-07-28 20:40:33.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-28 20:40:33.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-07-28 20:40:33.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:33.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18815 2023-07-28 20:40:34.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18790 2023-07-28 20:40:34.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:33.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.293981 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-07-28 20:43:52.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 20:43:52.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:52.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:52.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:52.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:43:52.000000 mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:52.297981 mypy-boto3-synthetics-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:40:33.000000 mypy-boto3-synthetics-1.28.15/setup.py
```

### Comparing `mypy-boto3-synthetics-1.28.12/LICENSE` & `mypy-boto3-synthetics-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-synthetics-1.28.12/PKG-INFO` & `mypy-boto3-synthetics-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-synthetics
-Version: 1.28.12
-Summary: Type annotations for boto3.Synthetics 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Synthetics 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-synthetics.svg?color=blue)](https://pypi.org/project/mypy-boto3-synthetics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-synthetics)](https://pepy.tech/project/mypy-boto3-synthetics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Synthetics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
+[boto3.Synthetics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
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
 [mypy-boto3-synthetics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,15 +301,14 @@
 
 `mypy_boto3_synthetics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_synthetics.type_defs import (
     S3EncryptionConfigTypeDef,
-    S3EncryptionConfigOutputTypeDef,
     AssociateResourceRequestRequestTypeDef,
     BaseScreenshotOutputTypeDef,
     BaseScreenshotTypeDef,
     CanaryCodeInputTypeDef,
     CanaryCodeOutputTypeDef,
     CanaryRunConfigInputTypeDef,
     CanaryRunConfigOutputTypeDef,
```

### Comparing `mypy-boto3-synthetics-1.28.12/README.md` & `mypy-boto3-synthetics-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-synthetics.svg?color=blue)](https://pypi.org/project/mypy-boto3-synthetics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-synthetics)](https://pepy.tech/project/mypy-boto3-synthetics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Synthetics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
+[boto3.Synthetics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
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
 [mypy-boto3-synthetics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,15 +269,14 @@
 
 `mypy_boto3_synthetics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_synthetics.type_defs import (
     S3EncryptionConfigTypeDef,
-    S3EncryptionConfigOutputTypeDef,
     AssociateResourceRequestRequestTypeDef,
     BaseScreenshotOutputTypeDef,
     BaseScreenshotTypeDef,
     CanaryCodeInputTypeDef,
     CanaryCodeOutputTypeDef,
     CanaryRunConfigInputTypeDef,
     CanaryRunConfigOutputTypeDef,
```

### Comparing `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/__main__.py` & `mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Synthetics 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Synthetics 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics\nOther"
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

### Comparing `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/client.py` & `mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/client.pyi` & `mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/literals.py` & `mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/literals.pyi` & `mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/type_defs.py` & `mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "S3EncryptionConfigTypeDef",
-    "S3EncryptionConfigOutputTypeDef",
     "AssociateResourceRequestRequestTypeDef",
     "BaseScreenshotOutputTypeDef",
     "BaseScreenshotTypeDef",
     "CanaryCodeInputTypeDef",
     "CanaryCodeOutputTypeDef",
     "CanaryRunConfigInputTypeDef",
     "CanaryRunConfigOutputTypeDef",
@@ -99,23 +98,14 @@
     {
         "EncryptionMode": EncryptionModeType,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-S3EncryptionConfigOutputTypeDef = TypedDict(
-    "S3EncryptionConfigOutputTypeDef",
-    {
-        "EncryptionMode": EncryptionModeType,
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
 AssociateResourceRequestRequestTypeDef = TypedDict(
     "AssociateResourceRequestRequestTypeDef",
     {
         "GroupIdentifier": str,
         "ResourceArn": str,
     },
 )
@@ -567,15 +557,15 @@
     },
     total=False,
 )
 
 ArtifactConfigOutputTypeDef = TypedDict(
     "ArtifactConfigOutputTypeDef",
     {
-        "S3Encryption": S3EncryptionConfigOutputTypeDef,
+        "S3Encryption": S3EncryptionConfigTypeDef,
     },
     total=False,
 )
 
 VisualReferenceOutputTypeDef = TypedDict(
     "VisualReferenceOutputTypeDef",
     {
```

### Comparing `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/type_defs.pyi` & `mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "S3EncryptionConfigTypeDef",
-    "S3EncryptionConfigOutputTypeDef",
     "AssociateResourceRequestRequestTypeDef",
     "BaseScreenshotOutputTypeDef",
     "BaseScreenshotTypeDef",
     "CanaryCodeInputTypeDef",
     "CanaryCodeOutputTypeDef",
     "CanaryRunConfigInputTypeDef",
     "CanaryRunConfigOutputTypeDef",
@@ -98,23 +97,14 @@
     {
         "EncryptionMode": EncryptionModeType,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-S3EncryptionConfigOutputTypeDef = TypedDict(
-    "S3EncryptionConfigOutputTypeDef",
-    {
-        "EncryptionMode": EncryptionModeType,
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
 AssociateResourceRequestRequestTypeDef = TypedDict(
     "AssociateResourceRequestRequestTypeDef",
     {
         "GroupIdentifier": str,
         "ResourceArn": str,
     },
 )
@@ -548,15 +538,15 @@
     },
     total=False,
 )
 
 ArtifactConfigOutputTypeDef = TypedDict(
     "ArtifactConfigOutputTypeDef",
     {
-        "S3Encryption": S3EncryptionConfigOutputTypeDef,
+        "S3Encryption": S3EncryptionConfigTypeDef,
     },
     total=False,
 )
 
 VisualReferenceOutputTypeDef = TypedDict(
     "VisualReferenceOutputTypeDef",
     {
```

### Comparing `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/PKG-INFO` & `mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-synthetics
-Version: 1.28.12
-Summary: Type annotations for boto3.Synthetics 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Synthetics 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-synthetics.svg?color=blue)](https://pypi.org/project/mypy-boto3-synthetics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-synthetics)](https://pepy.tech/project/mypy-boto3-synthetics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Synthetics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
+[boto3.Synthetics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
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
 [mypy-boto3-synthetics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,15 +301,14 @@
 
 `mypy_boto3_synthetics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_synthetics.type_defs import (
     S3EncryptionConfigTypeDef,
-    S3EncryptionConfigOutputTypeDef,
     AssociateResourceRequestRequestTypeDef,
     BaseScreenshotOutputTypeDef,
     BaseScreenshotTypeDef,
     CanaryCodeInputTypeDef,
     CanaryCodeOutputTypeDef,
     CanaryRunConfigInputTypeDef,
     CanaryRunConfigOutputTypeDef,
```

### Comparing `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/SOURCES.txt` & `mypy-boto3-synthetics-1.28.15/mypy_boto3_synthetics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-synthetics-1.28.12/setup.py` & `mypy-boto3-synthetics-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-synthetics",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_synthetics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Synthetics 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Synthetics 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

