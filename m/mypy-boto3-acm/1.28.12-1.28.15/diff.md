# Comparing `tmp/mypy-boto3-acm-1.28.12.tar.gz` & `tmp/mypy-boto3-acm-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-acm-1.28.12.tar", last modified: Thu Jul 27 05:34:13 2023, max compression
+gzip compressed data, was "mypy-boto3-acm-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
```

## Comparing `mypy-boto3-acm-1.28.12.tar` & `mypy-boto3-acm-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.844594 mypy-boto3-acm-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:16:52.000000 mypy-boto3-acm-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-27 05:34:13.844594 mypy-boto3-acm-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-07-27 05:16:52.000000 mypy-boto3-acm-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.840594 mypy-boto3-acm-1.28.12/mypy_boto3_acm/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-27 05:16:52.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-27 05:16:52.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15609 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15592 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:16:52.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-27 05:16:53.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.844594 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-27 05:34:13.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:34:13.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:13.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:13.000000 mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:13.844594 mypy-boto3-acm-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:16:52.000000 mypy-boto3-acm-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.632608 mypy-boto3-acm-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-07-28 20:42:12.628608 mypy-boto3-acm-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.628608 mypy-boto3-acm-1.28.15/mypy_boto3_acm/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-28 20:18:40.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-28 20:18:39.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.628608 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-07-28 20:42:12.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:42:12.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:12.000000 mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.632608 mypy-boto3-acm-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:18:38.000000 mypy-boto3-acm-1.28.15/setup.py
```

### Comparing `mypy-boto3-acm-1.28.12/LICENSE` & `mypy-boto3-acm-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.12/PKG-INFO` & `mypy-boto3-acm-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm
-Version: 1.28.12
-Summary: Type annotations for boto3.ACM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ACM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm)](https://pepy.tech/project/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,53 +357,50 @@
 
 `mypy_boto3_acm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_acm.type_defs import (
     TagTypeDef,
-    CertificateOptionsOutputTypeDef,
+    CertificateOptionsTypeDef,
     ExtendedKeyUsageTypeDef,
     KeyUsageTypeDef,
-    CertificateOptionsTypeDef,
     CertificateSummaryTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DomainValidationOptionTypeDef,
     ResourceRecordTypeDef,
-    ExpiryEventsConfigurationOutputTypeDef,
     ExpiryEventsConfigurationTypeDef,
     ExportCertificateRequestRequestTypeDef,
     FiltersTypeDef,
     GetCertificateRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForCertificateRequestRequestTypeDef,
-    TagOutputTypeDef,
     RenewCertificateRequestRequestTypeDef,
     ResendValidationEmailRequestRequestTypeDef,
     AddTagsToCertificateRequestRequestTypeDef,
     ImportCertificateRequestRequestTypeDef,
     RemoveTagsFromCertificateRequestRequestTypeDef,
     UpdateCertificateOptionsRequestRequestTypeDef,
     DescribeCertificateRequestCertificateValidatedWaitTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportCertificateResponseTypeDef,
     GetCertificateResponseTypeDef,
     ImportCertificateResponseTypeDef,
     ListCertificatesResponseTypeDef,
+    ListTagsForCertificateResponseTypeDef,
     RequestCertificateResponseTypeDef,
     RequestCertificateRequestRequestTypeDef,
     DomainValidationTypeDef,
     GetAccountConfigurationResponseTypeDef,
     PutAccountConfigurationRequestRequestTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
-    ListTagsForCertificateResponseTypeDef,
     RenewalSummaryTypeDef,
     CertificateDetailTypeDef,
     DescribeCertificateResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
```

### Comparing `mypy-boto3-acm-1.28.12/README.md` & `mypy-boto3-acm-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm)](https://pepy.tech/project/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,53 +325,50 @@
 
 `mypy_boto3_acm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_acm.type_defs import (
     TagTypeDef,
-    CertificateOptionsOutputTypeDef,
+    CertificateOptionsTypeDef,
     ExtendedKeyUsageTypeDef,
     KeyUsageTypeDef,
-    CertificateOptionsTypeDef,
     CertificateSummaryTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DomainValidationOptionTypeDef,
     ResourceRecordTypeDef,
-    ExpiryEventsConfigurationOutputTypeDef,
     ExpiryEventsConfigurationTypeDef,
     ExportCertificateRequestRequestTypeDef,
     FiltersTypeDef,
     GetCertificateRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForCertificateRequestRequestTypeDef,
-    TagOutputTypeDef,
     RenewCertificateRequestRequestTypeDef,
     ResendValidationEmailRequestRequestTypeDef,
     AddTagsToCertificateRequestRequestTypeDef,
     ImportCertificateRequestRequestTypeDef,
     RemoveTagsFromCertificateRequestRequestTypeDef,
     UpdateCertificateOptionsRequestRequestTypeDef,
     DescribeCertificateRequestCertificateValidatedWaitTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportCertificateResponseTypeDef,
     GetCertificateResponseTypeDef,
     ImportCertificateResponseTypeDef,
     ListCertificatesResponseTypeDef,
+    ListTagsForCertificateResponseTypeDef,
     RequestCertificateResponseTypeDef,
     RequestCertificateRequestRequestTypeDef,
     DomainValidationTypeDef,
     GetAccountConfigurationResponseTypeDef,
     PutAccountConfigurationRequestRequestTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
-    ListTagsForCertificateResponseTypeDef,
     RenewalSummaryTypeDef,
     CertificateDetailTypeDef,
     DescribeCertificateResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
```

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/__init__.py` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/__init__.pyi` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/__main__.py` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ACM 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.ACM 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM\nOther"
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

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/client.py` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/client.pyi` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/literals.py` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/literals.pyi` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/paginator.py` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/paginator.pyi` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/type_defs.py` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,53 +41,50 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "CertificateOptionsOutputTypeDef",
+    "CertificateOptionsTypeDef",
     "ExtendedKeyUsageTypeDef",
     "KeyUsageTypeDef",
-    "CertificateOptionsTypeDef",
     "CertificateSummaryTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DomainValidationOptionTypeDef",
     "ResourceRecordTypeDef",
-    "ExpiryEventsConfigurationOutputTypeDef",
     "ExpiryEventsConfigurationTypeDef",
     "ExportCertificateRequestRequestTypeDef",
     "FiltersTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListTagsForCertificateRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "RenewCertificateRequestRequestTypeDef",
     "ResendValidationEmailRequestRequestTypeDef",
     "AddTagsToCertificateRequestRequestTypeDef",
     "ImportCertificateRequestRequestTypeDef",
     "RemoveTagsFromCertificateRequestRequestTypeDef",
     "UpdateCertificateOptionsRequestRequestTypeDef",
     "DescribeCertificateRequestCertificateValidatedWaitTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportCertificateResponseTypeDef",
     "GetCertificateResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "ListCertificatesResponseTypeDef",
+    "ListTagsForCertificateResponseTypeDef",
     "RequestCertificateResponseTypeDef",
     "RequestCertificateRequestRequestTypeDef",
     "DomainValidationTypeDef",
     "GetAccountConfigurationResponseTypeDef",
     "PutAccountConfigurationRequestRequestTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListCertificatesRequestListCertificatesPaginateTypeDef",
-    "ListTagsForCertificateResponseTypeDef",
     "RenewalSummaryTypeDef",
     "CertificateDetailTypeDef",
     "DescribeCertificateResponseTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
@@ -104,16 +101,16 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
-CertificateOptionsOutputTypeDef = TypedDict(
-    "CertificateOptionsOutputTypeDef",
+CertificateOptionsTypeDef = TypedDict(
+    "CertificateOptionsTypeDef",
     {
         "CertificateTransparencyLoggingPreference": CertificateTransparencyLoggingPreferenceType,
     },
     total=False,
 )
 
 ExtendedKeyUsageTypeDef = TypedDict(
@@ -129,22 +126,14 @@
     "KeyUsageTypeDef",
     {
         "Name": KeyUsageNameType,
     },
     total=False,
 )
 
-CertificateOptionsTypeDef = TypedDict(
-    "CertificateOptionsTypeDef",
-    {
-        "CertificateTransparencyLoggingPreference": CertificateTransparencyLoggingPreferenceType,
-    },
-    total=False,
-)
-
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "CertificateArn": str,
         "DomainName": str,
         "SubjectAlternativeNameSummaries": List[str],
         "HasAdditionalSubjectAlternativeNames": bool,
@@ -213,22 +202,14 @@
     {
         "Name": str,
         "Type": Literal["CNAME"],
         "Value": str,
     },
 )
 
-ExpiryEventsConfigurationOutputTypeDef = TypedDict(
-    "ExpiryEventsConfigurationOutputTypeDef",
-    {
-        "DaysBeforeExpiry": int,
-    },
-    total=False,
-)
-
 ExpiryEventsConfigurationTypeDef = TypedDict(
     "ExpiryEventsConfigurationTypeDef",
     {
         "DaysBeforeExpiry": int,
     },
     total=False,
 )
@@ -271,33 +252,14 @@
 ListTagsForCertificateRequestRequestTypeDef = TypedDict(
     "ListTagsForCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
-
 RenewCertificateRequestRequestTypeDef = TypedDict(
     "RenewCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
@@ -419,14 +381,22 @@
     {
         "NextToken": str,
         "CertificateSummaryList": List[CertificateSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForCertificateResponseTypeDef = TypedDict(
+    "ListTagsForCertificateResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RequestCertificateResponseTypeDef = TypedDict(
     "RequestCertificateResponseTypeDef",
     {
         "CertificateArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -482,15 +452,15 @@
 class DomainValidationTypeDef(_RequiredDomainValidationTypeDef, _OptionalDomainValidationTypeDef):
     pass
 
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
-        "ExpiryEvents": ExpiryEventsConfigurationOutputTypeDef,
+        "ExpiryEvents": ExpiryEventsConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAccountConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAccountConfigurationRequestRequestTypeDef",
     {
@@ -534,22 +504,14 @@
         "SortBy": Literal["CREATED_AT"],
         "SortOrder": SortOrderType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListTagsForCertificateResponseTypeDef = TypedDict(
-    "ListTagsForCertificateResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredRenewalSummaryTypeDef = TypedDict(
     "_RequiredRenewalSummaryTypeDef",
     {
         "RenewalStatus": RenewalStatusType,
         "DomainValidationOptions": List[DomainValidationTypeDef],
         "UpdatedAt": datetime,
     },
@@ -591,15 +553,15 @@
         "FailureReason": FailureReasonType,
         "Type": CertificateTypeType,
         "RenewalSummary": RenewalSummaryTypeDef,
         "KeyUsages": List[KeyUsageTypeDef],
         "ExtendedKeyUsages": List[ExtendedKeyUsageTypeDef],
         "CertificateAuthorityArn": str,
         "RenewalEligibility": RenewalEligibilityType,
-        "Options": CertificateOptionsOutputTypeDef,
+        "Options": CertificateOptionsTypeDef,
     },
     total=False,
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
```

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/type_defs.pyi` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -40,53 +40,50 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "CertificateOptionsOutputTypeDef",
+    "CertificateOptionsTypeDef",
     "ExtendedKeyUsageTypeDef",
     "KeyUsageTypeDef",
-    "CertificateOptionsTypeDef",
     "CertificateSummaryTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DomainValidationOptionTypeDef",
     "ResourceRecordTypeDef",
-    "ExpiryEventsConfigurationOutputTypeDef",
     "ExpiryEventsConfigurationTypeDef",
     "ExportCertificateRequestRequestTypeDef",
     "FiltersTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListTagsForCertificateRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "RenewCertificateRequestRequestTypeDef",
     "ResendValidationEmailRequestRequestTypeDef",
     "AddTagsToCertificateRequestRequestTypeDef",
     "ImportCertificateRequestRequestTypeDef",
     "RemoveTagsFromCertificateRequestRequestTypeDef",
     "UpdateCertificateOptionsRequestRequestTypeDef",
     "DescribeCertificateRequestCertificateValidatedWaitTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExportCertificateResponseTypeDef",
     "GetCertificateResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "ListCertificatesResponseTypeDef",
+    "ListTagsForCertificateResponseTypeDef",
     "RequestCertificateResponseTypeDef",
     "RequestCertificateRequestRequestTypeDef",
     "DomainValidationTypeDef",
     "GetAccountConfigurationResponseTypeDef",
     "PutAccountConfigurationRequestRequestTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListCertificatesRequestListCertificatesPaginateTypeDef",
-    "ListTagsForCertificateResponseTypeDef",
     "RenewalSummaryTypeDef",
     "CertificateDetailTypeDef",
     "DescribeCertificateResponseTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
@@ -101,16 +98,16 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-CertificateOptionsOutputTypeDef = TypedDict(
-    "CertificateOptionsOutputTypeDef",
+CertificateOptionsTypeDef = TypedDict(
+    "CertificateOptionsTypeDef",
     {
         "CertificateTransparencyLoggingPreference": CertificateTransparencyLoggingPreferenceType,
     },
     total=False,
 )
 
 ExtendedKeyUsageTypeDef = TypedDict(
@@ -126,22 +123,14 @@
     "KeyUsageTypeDef",
     {
         "Name": KeyUsageNameType,
     },
     total=False,
 )
 
-CertificateOptionsTypeDef = TypedDict(
-    "CertificateOptionsTypeDef",
-    {
-        "CertificateTransparencyLoggingPreference": CertificateTransparencyLoggingPreferenceType,
-    },
-    total=False,
-)
-
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "CertificateArn": str,
         "DomainName": str,
         "SubjectAlternativeNameSummaries": List[str],
         "HasAdditionalSubjectAlternativeNames": bool,
@@ -210,22 +199,14 @@
     {
         "Name": str,
         "Type": Literal["CNAME"],
         "Value": str,
     },
 )
 
-ExpiryEventsConfigurationOutputTypeDef = TypedDict(
-    "ExpiryEventsConfigurationOutputTypeDef",
-    {
-        "DaysBeforeExpiry": int,
-    },
-    total=False,
-)
-
 ExpiryEventsConfigurationTypeDef = TypedDict(
     "ExpiryEventsConfigurationTypeDef",
     {
         "DaysBeforeExpiry": int,
     },
     total=False,
 )
@@ -268,31 +249,14 @@
 ListTagsForCertificateRequestRequestTypeDef = TypedDict(
     "ListTagsForCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
 RenewCertificateRequestRequestTypeDef = TypedDict(
     "RenewCertificateRequestRequestTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
@@ -410,14 +374,22 @@
     {
         "NextToken": str,
         "CertificateSummaryList": List[CertificateSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForCertificateResponseTypeDef = TypedDict(
+    "ListTagsForCertificateResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RequestCertificateResponseTypeDef = TypedDict(
     "RequestCertificateResponseTypeDef",
     {
         "CertificateArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -469,15 +441,15 @@
 
 class DomainValidationTypeDef(_RequiredDomainValidationTypeDef, _OptionalDomainValidationTypeDef):
     pass
 
 GetAccountConfigurationResponseTypeDef = TypedDict(
     "GetAccountConfigurationResponseTypeDef",
     {
-        "ExpiryEvents": ExpiryEventsConfigurationOutputTypeDef,
+        "ExpiryEvents": ExpiryEventsConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAccountConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAccountConfigurationRequestRequestTypeDef",
     {
@@ -519,22 +491,14 @@
         "SortBy": Literal["CREATED_AT"],
         "SortOrder": SortOrderType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListTagsForCertificateResponseTypeDef = TypedDict(
-    "ListTagsForCertificateResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredRenewalSummaryTypeDef = TypedDict(
     "_RequiredRenewalSummaryTypeDef",
     {
         "RenewalStatus": RenewalStatusType,
         "DomainValidationOptions": List[DomainValidationTypeDef],
         "UpdatedAt": datetime,
     },
@@ -574,15 +538,15 @@
         "FailureReason": FailureReasonType,
         "Type": CertificateTypeType,
         "RenewalSummary": RenewalSummaryTypeDef,
         "KeyUsages": List[KeyUsageTypeDef],
         "ExtendedKeyUsages": List[ExtendedKeyUsageTypeDef],
         "CertificateAuthorityArn": str,
         "RenewalEligibility": RenewalEligibilityType,
-        "Options": CertificateOptionsOutputTypeDef,
+        "Options": CertificateOptionsTypeDef,
     },
     total=False,
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
```

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/waiter.py` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm/waiter.pyi` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/PKG-INFO` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm
-Version: 1.28.12
-Summary: Type annotations for boto3.ACM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ACM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm)](https://pepy.tech/project/mypy-boto3-acm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
+[boto3.ACM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
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
 [mypy-boto3-acm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,53 +357,50 @@
 
 `mypy_boto3_acm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_acm.type_defs import (
     TagTypeDef,
-    CertificateOptionsOutputTypeDef,
+    CertificateOptionsTypeDef,
     ExtendedKeyUsageTypeDef,
     KeyUsageTypeDef,
-    CertificateOptionsTypeDef,
     CertificateSummaryTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     DomainValidationOptionTypeDef,
     ResourceRecordTypeDef,
-    ExpiryEventsConfigurationOutputTypeDef,
     ExpiryEventsConfigurationTypeDef,
     ExportCertificateRequestRequestTypeDef,
     FiltersTypeDef,
     GetCertificateRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListTagsForCertificateRequestRequestTypeDef,
-    TagOutputTypeDef,
     RenewCertificateRequestRequestTypeDef,
     ResendValidationEmailRequestRequestTypeDef,
     AddTagsToCertificateRequestRequestTypeDef,
     ImportCertificateRequestRequestTypeDef,
     RemoveTagsFromCertificateRequestRequestTypeDef,
     UpdateCertificateOptionsRequestRequestTypeDef,
     DescribeCertificateRequestCertificateValidatedWaitTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportCertificateResponseTypeDef,
     GetCertificateResponseTypeDef,
     ImportCertificateResponseTypeDef,
     ListCertificatesResponseTypeDef,
+    ListTagsForCertificateResponseTypeDef,
     RequestCertificateResponseTypeDef,
     RequestCertificateRequestRequestTypeDef,
     DomainValidationTypeDef,
     GetAccountConfigurationResponseTypeDef,
     PutAccountConfigurationRequestRequestTypeDef,
     ListCertificatesRequestRequestTypeDef,
     ListCertificatesRequestListCertificatesPaginateTypeDef,
-    ListTagsForCertificateResponseTypeDef,
     RenewalSummaryTypeDef,
     CertificateDetailTypeDef,
     DescribeCertificateResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
```

### Comparing `mypy-boto3-acm-1.28.12/mypy_boto3_acm.egg-info/SOURCES.txt` & `mypy-boto3-acm-1.28.15/mypy_boto3_acm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-1.28.12/setup.py` & `mypy-boto3-acm-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-acm",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_acm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ACM 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ACM 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

