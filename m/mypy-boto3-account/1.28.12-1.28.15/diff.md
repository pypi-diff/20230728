# Comparing `tmp/mypy-boto3-account-1.28.12.tar.gz` & `tmp/mypy-boto3-account-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-account-1.28.12.tar", last modified: Thu Jul 27 05:34:13 2023, max compression
+gzip compressed data, was "mypy-boto3-account-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
```

## Comparing `mypy-boto3-account-1.28.12.tar` & `mypy-boto3-account-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.840594 mypy-boto3-account-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-07-27 05:34:13.840594 mypy-boto3-account-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.820594 mypy-boto3-account-1.28.12/mypy_boto3_account/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/mypy_boto3_account/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.820594 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-07-27 05:34:13.000000 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 05:34:13.000000 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:13.000000 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:13.000000 mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:13.840594 mypy-boto3-account-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:16:52.000000 mypy-boto3-account-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.604608 mypy-boto3-account-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:37.000000 mypy-boto3-account-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-07-28 20:42:12.600608 mypy-boto3-account-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-28 20:18:37.000000 mypy-boto3-account-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.592608 mypy-boto3-account-1.28.15/mypy_boto3_account/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-28 20:18:37.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-28 20:18:37.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:18:37.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-28 20:18:38.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-28 20:18:38.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-07-28 20:18:38.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-07-28 20:18:38.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-28 20:18:38.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-28 20:18:38.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:37.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-28 20:18:38.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-07-28 20:18:38.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:37.000000 mypy-boto3-account-1.28.15/mypy_boto3_account/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.600608 mypy-boto3-account-1.28.15/mypy_boto3_account.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-07-28 20:42:12.000000 mypy-boto3-account-1.28.15/mypy_boto3_account.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-28 20:42:12.000000 mypy-boto3-account-1.28.15/mypy_boto3_account.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-account-1.28.15/mypy_boto3_account.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-account-1.28.15/mypy_boto3_account.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-account-1.28.15/mypy_boto3_account.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:12.000000 mypy-boto3-account-1.28.15/mypy_boto3_account.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.604608 mypy-boto3-account-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:18:37.000000 mypy-boto3-account-1.28.15/setup.py
```

### Comparing `mypy-boto3-account-1.28.12/LICENSE` & `mypy-boto3-account-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.12/PKG-INFO` & `mypy-boto3-account-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-account
-Version: 1.28.12
-Summary: Type annotations for boto3.Account 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Account 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-account)](https://pepy.tech/project/mypy-boto3-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Account 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[boto3.Account 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
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
 [mypy-boto3-account docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,15 +320,14 @@
 
 `mypy_boto3_account.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_account.type_defs import (
     AlternateContactTypeDef,
-    ContactInformationOutputTypeDef,
     ContactInformationTypeDef,
     DeleteAlternateContactRequestRequestTypeDef,
     DisableRegionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EnableRegionRequestRequestTypeDef,
     GetAlternateContactRequestRequestTypeDef,
     GetContactInformationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-account-1.28.12/README.md` & `mypy-boto3-account-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-account)](https://pepy.tech/project/mypy-boto3-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Account 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[boto3.Account 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
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
 [mypy-boto3-account docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,15 +288,14 @@
 
 `mypy_boto3_account.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_account.type_defs import (
     AlternateContactTypeDef,
-    ContactInformationOutputTypeDef,
     ContactInformationTypeDef,
     DeleteAlternateContactRequestRequestTypeDef,
     DisableRegionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EnableRegionRequestRequestTypeDef,
     GetAlternateContactRequestRequestTypeDef,
     GetContactInformationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account/__init__.py` & `mypy-boto3-account-1.28.15/mypy_boto3_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account/__init__.pyi` & `mypy-boto3-account-1.28.15/mypy_boto3_account/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account/__main__.py` & `mypy-boto3-account-1.28.15/mypy_boto3_account/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Account 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Account 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account\nOther"
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

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account/client.py` & `mypy-boto3-account-1.28.15/mypy_boto3_account/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account/client.pyi` & `mypy-boto3-account-1.28.15/mypy_boto3_account/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account/literals.py` & `mypy-boto3-account-1.28.15/mypy_boto3_account/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account/literals.pyi` & `mypy-boto3-account-1.28.15/mypy_boto3_account/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account/paginator.py` & `mypy-boto3-account-1.28.15/mypy_boto3_account/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account/paginator.pyi` & `mypy-boto3-account-1.28.15/mypy_boto3_account/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account/type_defs.py` & `mypy-boto3-account-1.28.15/mypy_boto3_account/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AlternateContactTypeDef",
-    "ContactInformationOutputTypeDef",
     "ContactInformationTypeDef",
     "DeleteAlternateContactRequestRequestTypeDef",
     "DisableRegionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EnableRegionRequestRequestTypeDef",
     "GetAlternateContactRequestRequestTypeDef",
     "GetContactInformationRequestRequestTypeDef",
@@ -54,45 +53,14 @@
         "Name": str,
         "PhoneNumber": str,
         "Title": str,
     },
     total=False,
 )
 
-_RequiredContactInformationOutputTypeDef = TypedDict(
-    "_RequiredContactInformationOutputTypeDef",
-    {
-        "AddressLine1": str,
-        "City": str,
-        "CountryCode": str,
-        "FullName": str,
-        "PhoneNumber": str,
-        "PostalCode": str,
-    },
-)
-_OptionalContactInformationOutputTypeDef = TypedDict(
-    "_OptionalContactInformationOutputTypeDef",
-    {
-        "AddressLine2": str,
-        "AddressLine3": str,
-        "CompanyName": str,
-        "DistrictOrCounty": str,
-        "StateOrRegion": str,
-        "WebsiteUrl": str,
-    },
-    total=False,
-)
-
-
-class ContactInformationOutputTypeDef(
-    _RequiredContactInformationOutputTypeDef, _OptionalContactInformationOutputTypeDef
-):
-    pass
-
-
 _RequiredContactInformationTypeDef = TypedDict(
     "_RequiredContactInformationTypeDef",
     {
         "AddressLine1": str,
         "City": str,
         "CountryCode": str,
         "FullName": str,
@@ -339,15 +307,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContactInformationResponseTypeDef = TypedDict(
     "GetContactInformationResponseTypeDef",
     {
-        "ContactInformation": ContactInformationOutputTypeDef,
+        "ContactInformation": ContactInformationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegionOptStatusResponseTypeDef = TypedDict(
     "GetRegionOptStatusResponseTypeDef",
     {
```

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account/type_defs.pyi` & `mypy-boto3-account-1.28.15/mypy_boto3_account/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlternateContactTypeDef",
-    "ContactInformationOutputTypeDef",
     "ContactInformationTypeDef",
     "DeleteAlternateContactRequestRequestTypeDef",
     "DisableRegionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EnableRegionRequestRequestTypeDef",
     "GetAlternateContactRequestRequestTypeDef",
     "GetContactInformationRequestRequestTypeDef",
@@ -53,43 +52,14 @@
         "Name": str,
         "PhoneNumber": str,
         "Title": str,
     },
     total=False,
 )
 
-_RequiredContactInformationOutputTypeDef = TypedDict(
-    "_RequiredContactInformationOutputTypeDef",
-    {
-        "AddressLine1": str,
-        "City": str,
-        "CountryCode": str,
-        "FullName": str,
-        "PhoneNumber": str,
-        "PostalCode": str,
-    },
-)
-_OptionalContactInformationOutputTypeDef = TypedDict(
-    "_OptionalContactInformationOutputTypeDef",
-    {
-        "AddressLine2": str,
-        "AddressLine3": str,
-        "CompanyName": str,
-        "DistrictOrCounty": str,
-        "StateOrRegion": str,
-        "WebsiteUrl": str,
-    },
-    total=False,
-)
-
-class ContactInformationOutputTypeDef(
-    _RequiredContactInformationOutputTypeDef, _OptionalContactInformationOutputTypeDef
-):
-    pass
-
 _RequiredContactInformationTypeDef = TypedDict(
     "_RequiredContactInformationTypeDef",
     {
         "AddressLine1": str,
         "City": str,
         "CountryCode": str,
         "FullName": str,
@@ -320,15 +290,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContactInformationResponseTypeDef = TypedDict(
     "GetContactInformationResponseTypeDef",
     {
-        "ContactInformation": ContactInformationOutputTypeDef,
+        "ContactInformation": ContactInformationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegionOptStatusResponseTypeDef = TypedDict(
     "GetRegionOptStatusResponseTypeDef",
     {
```

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/PKG-INFO` & `mypy-boto3-account-1.28.15/mypy_boto3_account.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-account
-Version: 1.28.12
-Summary: Type annotations for boto3.Account 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Account 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-account.svg?color=blue)](https://pypi.org/project/mypy-boto3-account)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-account)](https://pepy.tech/project/mypy-boto3-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Account 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[boto3.Account 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
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
 [mypy-boto3-account docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_account/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,15 +320,14 @@
 
 `mypy_boto3_account.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_account.type_defs import (
     AlternateContactTypeDef,
-    ContactInformationOutputTypeDef,
     ContactInformationTypeDef,
     DeleteAlternateContactRequestRequestTypeDef,
     DisableRegionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     EnableRegionRequestRequestTypeDef,
     GetAlternateContactRequestRequestTypeDef,
     GetContactInformationRequestRequestTypeDef,
```

### Comparing `mypy-boto3-account-1.28.12/mypy_boto3_account.egg-info/SOURCES.txt` & `mypy-boto3-account-1.28.15/mypy_boto3_account.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-account-1.28.12/setup.py` & `mypy-boto3-account-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-account",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_account"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Account 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Account 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

