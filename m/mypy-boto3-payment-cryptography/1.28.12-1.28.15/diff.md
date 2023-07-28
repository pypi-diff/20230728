# Comparing `tmp/mypy-boto3-payment-cryptography-1.28.12.tar.gz` & `tmp/mypy-boto3-payment-cryptography-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-payment-cryptography-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
+gzip compressed data, was "mypy-boto3-payment-cryptography-1.28.15.tar", last modified: Fri Jul 28 20:43:27 2023, max compression
```

## Comparing `mypy-boto3-payment-cryptography-1.28.12.tar` & `mypy-boto3-payment-cryptography-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.781132 mypy-boto3-payment-cryptography-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15793 2023-07-27 11:49:21.781132 mypy-boto3-payment-cryptography-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.781132 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18642 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.781132 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15793 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 11:49:21.000000 mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.781132 mypy-boto3-payment-cryptography-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-27 11:41:13.000000 mypy-boto3-payment-cryptography-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:27.233638 mypy-boto3-payment-cryptography-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15707 2023-07-28 20:43:27.229638 mypy-boto3-payment-cryptography-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:27.225638 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-28 20:33:12.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-07-28 20:33:15.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-07-28 20:33:14.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:27.229638 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15707 2023-07-28 20:43:26.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:43:27.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:26.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:26.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:26.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 20:43:26.000000 mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:27.233638 mypy-boto3-payment-cryptography-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-28 20:33:11.000000 mypy-boto3-payment-cryptography-1.28.15/setup.py
```

### Comparing `mypy-boto3-payment-cryptography-1.28.12/LICENSE` & `mypy-boto3-payment-cryptography-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.12/PKG-INFO` & `mypy-boto3-payment-cryptography-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography
-Version: 1.28.12
-Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-payment-cryptography)](https://pepy.tech/project/mypy-boto3-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyControlPlane 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[boto3.PaymentCryptographyControlPlane 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
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
 [mypy-boto3-payment-cryptography docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,46 +354,43 @@
     GetAliasInputRequestTypeDef,
     GetKeyInputRequestTypeDef,
     GetParametersForExportInputRequestTypeDef,
     GetParametersForImportInputRequestTypeDef,
     GetPublicKeyCertificateInputRequestTypeDef,
     ImportTr31KeyBlockTypeDef,
     ImportTr34KeyBlockTypeDef,
-    KeyModesOfUseOutputTypeDef,
     KeyModesOfUseTypeDef,
     PaginatorConfigTypeDef,
     ListAliasesInputRequestTypeDef,
     ListKeysInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
     RestoreKeyInputRequestTypeDef,
     StartKeyUsageInputRequestTypeDef,
     StopKeyUsageInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateAliasInputRequestTypeDef,
     CreateAliasOutputTypeDef,
     GetAliasOutputTypeDef,
     GetParametersForExportOutputTypeDef,
     GetParametersForImportOutputTypeDef,
     GetPublicKeyCertificateOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ExportKeyMaterialTypeDef,
     ExportKeyOutputTypeDef,
-    KeyAttributesOutputTypeDef,
     KeyAttributesTypeDef,
     ListAliasesInputListAliasesPaginateTypeDef,
     ListKeysInputListKeysPaginateTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ExportKeyInputRequestTypeDef,
+    CreateKeyInputRequestTypeDef,
     KeySummaryTypeDef,
     KeyTypeDef,
-    CreateKeyInputRequestTypeDef,
     RootCertificatePublicKeyTypeDef,
     TrustedCertificatePublicKeyTypeDef,
     ListKeysOutputTypeDef,
     CreateKeyOutputTypeDef,
     DeleteKeyOutputTypeDef,
     GetKeyOutputTypeDef,
     ImportKeyOutputTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.28.12/README.md` & `mypy-boto3-payment-cryptography-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-payment-cryptography)](https://pepy.tech/project/mypy-boto3-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyControlPlane 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[boto3.PaymentCryptographyControlPlane 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
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
 [mypy-boto3-payment-cryptography docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,46 +322,43 @@
     GetAliasInputRequestTypeDef,
     GetKeyInputRequestTypeDef,
     GetParametersForExportInputRequestTypeDef,
     GetParametersForImportInputRequestTypeDef,
     GetPublicKeyCertificateInputRequestTypeDef,
     ImportTr31KeyBlockTypeDef,
     ImportTr34KeyBlockTypeDef,
-    KeyModesOfUseOutputTypeDef,
     KeyModesOfUseTypeDef,
     PaginatorConfigTypeDef,
     ListAliasesInputRequestTypeDef,
     ListKeysInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
     RestoreKeyInputRequestTypeDef,
     StartKeyUsageInputRequestTypeDef,
     StopKeyUsageInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateAliasInputRequestTypeDef,
     CreateAliasOutputTypeDef,
     GetAliasOutputTypeDef,
     GetParametersForExportOutputTypeDef,
     GetParametersForImportOutputTypeDef,
     GetPublicKeyCertificateOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ExportKeyMaterialTypeDef,
     ExportKeyOutputTypeDef,
-    KeyAttributesOutputTypeDef,
     KeyAttributesTypeDef,
     ListAliasesInputListAliasesPaginateTypeDef,
     ListKeysInputListKeysPaginateTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ExportKeyInputRequestTypeDef,
+    CreateKeyInputRequestTypeDef,
     KeySummaryTypeDef,
     KeyTypeDef,
-    CreateKeyInputRequestTypeDef,
     RootCertificatePublicKeyTypeDef,
     TrustedCertificatePublicKeyTypeDef,
     ListKeysOutputTypeDef,
     CreateKeyOutputTypeDef,
     DeleteKeyOutputTypeDef,
     GetKeyOutputTypeDef,
     ImportKeyOutputTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/__init__.py` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/__init__.pyi` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/__main__.py` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PaymentCryptographyControlPlane 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.PaymentCryptographyControlPlane 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane\nOther"
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

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/client.py` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/client.pyi` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/literals.py` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/literals.pyi` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/paginator.py` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/paginator.pyi` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/type_defs.py` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasTypeDef",
     "CreateAliasInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DeleteAliasInputRequestTypeDef",
     "DeleteKeyInputRequestTypeDef",
@@ -49,46 +48,43 @@
     "GetAliasInputRequestTypeDef",
     "GetKeyInputRequestTypeDef",
     "GetParametersForExportInputRequestTypeDef",
     "GetParametersForImportInputRequestTypeDef",
     "GetPublicKeyCertificateInputRequestTypeDef",
     "ImportTr31KeyBlockTypeDef",
     "ImportTr34KeyBlockTypeDef",
-    "KeyModesOfUseOutputTypeDef",
     "KeyModesOfUseTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesInputRequestTypeDef",
     "ListKeysInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagOutputTypeDef",
     "RestoreKeyInputRequestTypeDef",
     "StartKeyUsageInputRequestTypeDef",
     "StopKeyUsageInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateAliasInputRequestTypeDef",
     "CreateAliasOutputTypeDef",
     "GetAliasOutputTypeDef",
     "GetParametersForExportOutputTypeDef",
     "GetParametersForImportOutputTypeDef",
     "GetPublicKeyCertificateOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ExportKeyMaterialTypeDef",
     "ExportKeyOutputTypeDef",
-    "KeyAttributesOutputTypeDef",
     "KeyAttributesTypeDef",
     "ListAliasesInputListAliasesPaginateTypeDef",
     "ListKeysInputListKeysPaginateTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ExportKeyInputRequestTypeDef",
+    "CreateKeyInputRequestTypeDef",
     "KeySummaryTypeDef",
     "KeyTypeDef",
-    "CreateKeyInputRequestTypeDef",
     "RootCertificatePublicKeyTypeDef",
     "TrustedCertificatePublicKeyTypeDef",
     "ListKeysOutputTypeDef",
     "CreateKeyOutputTypeDef",
     "DeleteKeyOutputTypeDef",
     "GetKeyOutputTypeDef",
     "ImportKeyOutputTypeDef",
@@ -109,40 +105,36 @@
     "_OptionalAliasTypeDef",
     {
         "KeyArn": str,
     },
     total=False,
 )
 
-
 class AliasTypeDef(_RequiredAliasTypeDef, _OptionalAliasTypeDef):
     pass
 
-
 _RequiredCreateAliasInputRequestTypeDef = TypedDict(
     "_RequiredCreateAliasInputRequestTypeDef",
     {
         "AliasName": str,
     },
 )
 _OptionalCreateAliasInputRequestTypeDef = TypedDict(
     "_OptionalCreateAliasInputRequestTypeDef",
     {
         "KeyArn": str,
     },
     total=False,
 )
 
-
 class CreateAliasInputRequestTypeDef(
     _RequiredCreateAliasInputRequestTypeDef, _OptionalCreateAliasInputRequestTypeDef
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -160,19 +152,17 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-
 DeleteAliasInputRequestTypeDef = TypedDict(
     "DeleteAliasInputRequestTypeDef",
     {
         "AliasName": str,
     },
 )
 
@@ -186,21 +176,19 @@
     "_OptionalDeleteKeyInputRequestTypeDef",
     {
         "DeleteKeyInDays": int,
     },
     total=False,
 )
 
-
 class DeleteKeyInputRequestTypeDef(
     _RequiredDeleteKeyInputRequestTypeDef, _OptionalDeleteKeyInputRequestTypeDef
 ):
     pass
 
-
 ExportTr31KeyBlockTypeDef = TypedDict(
     "ExportTr31KeyBlockTypeDef",
     {
         "WrappingKeyIdentifier": str,
     },
 )
 
@@ -217,21 +205,19 @@
     "_OptionalExportTr34KeyBlockTypeDef",
     {
         "RandomNonce": str,
     },
     total=False,
 )
 
-
 class ExportTr34KeyBlockTypeDef(
     _RequiredExportTr34KeyBlockTypeDef, _OptionalExportTr34KeyBlockTypeDef
 ):
     pass
 
-
 WrappedKeyTypeDef = TypedDict(
     "WrappedKeyTypeDef",
     {
         "KeyMaterial": str,
         "WrappedKeyMaterialFormat": WrappedKeyMaterialFormatType,
         "WrappingKeyArn": str,
     },
@@ -296,37 +282,19 @@
     "_OptionalImportTr34KeyBlockTypeDef",
     {
         "RandomNonce": str,
     },
     total=False,
 )
 
-
 class ImportTr34KeyBlockTypeDef(
     _RequiredImportTr34KeyBlockTypeDef, _OptionalImportTr34KeyBlockTypeDef
 ):
     pass
 
-
-KeyModesOfUseOutputTypeDef = TypedDict(
-    "KeyModesOfUseOutputTypeDef",
-    {
-        "Decrypt": bool,
-        "DeriveKey": bool,
-        "Encrypt": bool,
-        "Generate": bool,
-        "NoRestrictions": bool,
-        "Sign": bool,
-        "Unwrap": bool,
-        "Verify": bool,
-        "Wrap": bool,
-    },
-    total=False,
-)
-
 KeyModesOfUseTypeDef = TypedDict(
     "KeyModesOfUseTypeDef",
     {
         "Decrypt": bool,
         "DeriveKey": bool,
         "Encrypt": bool,
         "Generate": bool,
@@ -379,40 +347,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-
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
 RestoreKeyInputRequestTypeDef = TypedDict(
     "RestoreKeyInputRequestTypeDef",
     {
         "KeyIdentifier": str,
     },
 )
 
@@ -448,21 +395,19 @@
     "_OptionalUpdateAliasInputRequestTypeDef",
     {
         "KeyArn": str,
     },
     total=False,
 )
 
-
 class UpdateAliasInputRequestTypeDef(
     _RequiredUpdateAliasInputRequestTypeDef, _OptionalUpdateAliasInputRequestTypeDef
 ):
     pass
 
-
 CreateAliasOutputTypeDef = TypedDict(
     "CreateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -521,14 +466,23 @@
     "UpdateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -546,24 +500,14 @@
     "ExportKeyOutputTypeDef",
     {
         "WrappedKey": WrappedKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-KeyAttributesOutputTypeDef = TypedDict(
-    "KeyAttributesOutputTypeDef",
-    {
-        "KeyAlgorithm": KeyAlgorithmType,
-        "KeyClass": KeyClassType,
-        "KeyModesOfUse": KeyModesOfUseOutputTypeDef,
-        "KeyUsage": KeyUsageType,
-    },
-)
-
 KeyAttributesTypeDef = TypedDict(
     "KeyAttributesTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "KeyClass": KeyClassType,
         "KeyModesOfUse": KeyModesOfUseTypeDef,
         "KeyUsage": KeyUsageType,
@@ -597,59 +541,70 @@
     "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ExportKeyInputRequestTypeDef = TypedDict(
     "ExportKeyInputRequestTypeDef",
     {
         "ExportKeyIdentifier": str,
         "KeyMaterial": ExportKeyMaterialTypeDef,
     },
 )
 
+_RequiredCreateKeyInputRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyInputRequestTypeDef",
+    {
+        "Exportable": bool,
+        "KeyAttributes": KeyAttributesTypeDef,
+    },
+)
+_OptionalCreateKeyInputRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyInputRequestTypeDef",
+    {
+        "Enabled": bool,
+        "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateKeyInputRequestTypeDef(
+    _RequiredCreateKeyInputRequestTypeDef, _OptionalCreateKeyInputRequestTypeDef
+):
+    pass
+
 KeySummaryTypeDef = TypedDict(
     "KeySummaryTypeDef",
     {
         "Enabled": bool,
         "Exportable": bool,
         "KeyArn": str,
-        "KeyAttributes": KeyAttributesOutputTypeDef,
+        "KeyAttributes": KeyAttributesTypeDef,
         "KeyCheckValue": str,
         "KeyState": KeyStateType,
     },
 )
 
 _RequiredKeyTypeDef = TypedDict(
     "_RequiredKeyTypeDef",
     {
         "CreateTimestamp": datetime,
         "Enabled": bool,
         "Exportable": bool,
         "KeyArn": str,
-        "KeyAttributes": KeyAttributesOutputTypeDef,
+        "KeyAttributes": KeyAttributesTypeDef,
         "KeyCheckValue": str,
         "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
         "KeyOrigin": KeyOriginType,
         "KeyState": KeyStateType,
     },
 )
 _OptionalKeyTypeDef = TypedDict(
@@ -659,43 +614,17 @@
         "DeleteTimestamp": datetime,
         "UsageStartTimestamp": datetime,
         "UsageStopTimestamp": datetime,
     },
     total=False,
 )
 
-
 class KeyTypeDef(_RequiredKeyTypeDef, _OptionalKeyTypeDef):
     pass
 
-
-_RequiredCreateKeyInputRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyInputRequestTypeDef",
-    {
-        "Exportable": bool,
-        "KeyAttributes": KeyAttributesTypeDef,
-    },
-)
-_OptionalCreateKeyInputRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyInputRequestTypeDef",
-    {
-        "Enabled": bool,
-        "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateKeyInputRequestTypeDef(
-    _RequiredCreateKeyInputRequestTypeDef, _OptionalCreateKeyInputRequestTypeDef
-):
-    pass
-
-
 RootCertificatePublicKeyTypeDef = TypedDict(
     "RootCertificatePublicKeyTypeDef",
     {
         "KeyAttributes": KeyAttributesTypeDef,
         "PublicKeyCertificate": str,
     },
 )
@@ -797,12 +726,11 @@
         "Enabled": bool,
         "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ImportKeyInputRequestTypeDef(
     _RequiredImportKeyInputRequestTypeDef, _OptionalImportKeyInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography/type_defs.pyi` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AliasTypeDef",
     "CreateAliasInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DeleteAliasInputRequestTypeDef",
     "DeleteKeyInputRequestTypeDef",
@@ -48,46 +49,43 @@
     "GetAliasInputRequestTypeDef",
     "GetKeyInputRequestTypeDef",
     "GetParametersForExportInputRequestTypeDef",
     "GetParametersForImportInputRequestTypeDef",
     "GetPublicKeyCertificateInputRequestTypeDef",
     "ImportTr31KeyBlockTypeDef",
     "ImportTr34KeyBlockTypeDef",
-    "KeyModesOfUseOutputTypeDef",
     "KeyModesOfUseTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesInputRequestTypeDef",
     "ListKeysInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagOutputTypeDef",
     "RestoreKeyInputRequestTypeDef",
     "StartKeyUsageInputRequestTypeDef",
     "StopKeyUsageInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateAliasInputRequestTypeDef",
     "CreateAliasOutputTypeDef",
     "GetAliasOutputTypeDef",
     "GetParametersForExportOutputTypeDef",
     "GetParametersForImportOutputTypeDef",
     "GetPublicKeyCertificateOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ExportKeyMaterialTypeDef",
     "ExportKeyOutputTypeDef",
-    "KeyAttributesOutputTypeDef",
     "KeyAttributesTypeDef",
     "ListAliasesInputListAliasesPaginateTypeDef",
     "ListKeysInputListKeysPaginateTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ExportKeyInputRequestTypeDef",
+    "CreateKeyInputRequestTypeDef",
     "KeySummaryTypeDef",
     "KeyTypeDef",
-    "CreateKeyInputRequestTypeDef",
     "RootCertificatePublicKeyTypeDef",
     "TrustedCertificatePublicKeyTypeDef",
     "ListKeysOutputTypeDef",
     "CreateKeyOutputTypeDef",
     "DeleteKeyOutputTypeDef",
     "GetKeyOutputTypeDef",
     "ImportKeyOutputTypeDef",
@@ -108,36 +106,40 @@
     "_OptionalAliasTypeDef",
     {
         "KeyArn": str,
     },
     total=False,
 )
 
+
 class AliasTypeDef(_RequiredAliasTypeDef, _OptionalAliasTypeDef):
     pass
 
+
 _RequiredCreateAliasInputRequestTypeDef = TypedDict(
     "_RequiredCreateAliasInputRequestTypeDef",
     {
         "AliasName": str,
     },
 )
 _OptionalCreateAliasInputRequestTypeDef = TypedDict(
     "_OptionalCreateAliasInputRequestTypeDef",
     {
         "KeyArn": str,
     },
     total=False,
 )
 
+
 class CreateAliasInputRequestTypeDef(
     _RequiredCreateAliasInputRequestTypeDef, _OptionalCreateAliasInputRequestTypeDef
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -155,17 +157,19 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+
 DeleteAliasInputRequestTypeDef = TypedDict(
     "DeleteAliasInputRequestTypeDef",
     {
         "AliasName": str,
     },
 )
 
@@ -179,19 +183,21 @@
     "_OptionalDeleteKeyInputRequestTypeDef",
     {
         "DeleteKeyInDays": int,
     },
     total=False,
 )
 
+
 class DeleteKeyInputRequestTypeDef(
     _RequiredDeleteKeyInputRequestTypeDef, _OptionalDeleteKeyInputRequestTypeDef
 ):
     pass
 
+
 ExportTr31KeyBlockTypeDef = TypedDict(
     "ExportTr31KeyBlockTypeDef",
     {
         "WrappingKeyIdentifier": str,
     },
 )
 
@@ -208,19 +214,21 @@
     "_OptionalExportTr34KeyBlockTypeDef",
     {
         "RandomNonce": str,
     },
     total=False,
 )
 
+
 class ExportTr34KeyBlockTypeDef(
     _RequiredExportTr34KeyBlockTypeDef, _OptionalExportTr34KeyBlockTypeDef
 ):
     pass
 
+
 WrappedKeyTypeDef = TypedDict(
     "WrappedKeyTypeDef",
     {
         "KeyMaterial": str,
         "WrappedKeyMaterialFormat": WrappedKeyMaterialFormatType,
         "WrappingKeyArn": str,
     },
@@ -285,34 +293,20 @@
     "_OptionalImportTr34KeyBlockTypeDef",
     {
         "RandomNonce": str,
     },
     total=False,
 )
 
+
 class ImportTr34KeyBlockTypeDef(
     _RequiredImportTr34KeyBlockTypeDef, _OptionalImportTr34KeyBlockTypeDef
 ):
     pass
 
-KeyModesOfUseOutputTypeDef = TypedDict(
-    "KeyModesOfUseOutputTypeDef",
-    {
-        "Decrypt": bool,
-        "DeriveKey": bool,
-        "Encrypt": bool,
-        "Generate": bool,
-        "NoRestrictions": bool,
-        "Sign": bool,
-        "Unwrap": bool,
-        "Verify": bool,
-        "Wrap": bool,
-    },
-    total=False,
-)
 
 KeyModesOfUseTypeDef = TypedDict(
     "KeyModesOfUseTypeDef",
     {
         "Decrypt": bool,
         "DeriveKey": bool,
         "Encrypt": bool,
@@ -366,35 +360,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
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
 
 RestoreKeyInputRequestTypeDef = TypedDict(
     "RestoreKeyInputRequestTypeDef",
     {
         "KeyIdentifier": str,
     },
 )
@@ -431,19 +410,21 @@
     "_OptionalUpdateAliasInputRequestTypeDef",
     {
         "KeyArn": str,
     },
     total=False,
 )
 
+
 class UpdateAliasInputRequestTypeDef(
     _RequiredUpdateAliasInputRequestTypeDef, _OptionalUpdateAliasInputRequestTypeDef
 ):
     pass
 
+
 CreateAliasOutputTypeDef = TypedDict(
     "CreateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -502,14 +483,23 @@
     "UpdateAliasOutputTypeDef",
     {
         "Alias": AliasTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -527,24 +517,14 @@
     "ExportKeyOutputTypeDef",
     {
         "WrappedKey": WrappedKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-KeyAttributesOutputTypeDef = TypedDict(
-    "KeyAttributesOutputTypeDef",
-    {
-        "KeyAlgorithm": KeyAlgorithmType,
-        "KeyClass": KeyClassType,
-        "KeyModesOfUse": KeyModesOfUseOutputTypeDef,
-        "KeyUsage": KeyUsageType,
-    },
-)
-
 KeyAttributesTypeDef = TypedDict(
     "KeyAttributesTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "KeyClass": KeyClassType,
         "KeyModesOfUse": KeyModesOfUseTypeDef,
         "KeyUsage": KeyUsageType,
@@ -578,57 +558,74 @@
     "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 ExportKeyInputRequestTypeDef = TypedDict(
     "ExportKeyInputRequestTypeDef",
     {
         "ExportKeyIdentifier": str,
         "KeyMaterial": ExportKeyMaterialTypeDef,
     },
 )
 
+_RequiredCreateKeyInputRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyInputRequestTypeDef",
+    {
+        "Exportable": bool,
+        "KeyAttributes": KeyAttributesTypeDef,
+    },
+)
+_OptionalCreateKeyInputRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyInputRequestTypeDef",
+    {
+        "Enabled": bool,
+        "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateKeyInputRequestTypeDef(
+    _RequiredCreateKeyInputRequestTypeDef, _OptionalCreateKeyInputRequestTypeDef
+):
+    pass
+
+
 KeySummaryTypeDef = TypedDict(
     "KeySummaryTypeDef",
     {
         "Enabled": bool,
         "Exportable": bool,
         "KeyArn": str,
-        "KeyAttributes": KeyAttributesOutputTypeDef,
+        "KeyAttributes": KeyAttributesTypeDef,
         "KeyCheckValue": str,
         "KeyState": KeyStateType,
     },
 )
 
 _RequiredKeyTypeDef = TypedDict(
     "_RequiredKeyTypeDef",
     {
         "CreateTimestamp": datetime,
         "Enabled": bool,
         "Exportable": bool,
         "KeyArn": str,
-        "KeyAttributes": KeyAttributesOutputTypeDef,
+        "KeyAttributes": KeyAttributesTypeDef,
         "KeyCheckValue": str,
         "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
         "KeyOrigin": KeyOriginType,
         "KeyState": KeyStateType,
     },
 )
 _OptionalKeyTypeDef = TypedDict(
@@ -638,38 +635,18 @@
         "DeleteTimestamp": datetime,
         "UsageStartTimestamp": datetime,
         "UsageStopTimestamp": datetime,
     },
     total=False,
 )
 
+
 class KeyTypeDef(_RequiredKeyTypeDef, _OptionalKeyTypeDef):
     pass
 
-_RequiredCreateKeyInputRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyInputRequestTypeDef",
-    {
-        "Exportable": bool,
-        "KeyAttributes": KeyAttributesTypeDef,
-    },
-)
-_OptionalCreateKeyInputRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyInputRequestTypeDef",
-    {
-        "Enabled": bool,
-        "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateKeyInputRequestTypeDef(
-    _RequiredCreateKeyInputRequestTypeDef, _OptionalCreateKeyInputRequestTypeDef
-):
-    pass
 
 RootCertificatePublicKeyTypeDef = TypedDict(
     "RootCertificatePublicKeyTypeDef",
     {
         "KeyAttributes": KeyAttributesTypeDef,
         "PublicKeyCertificate": str,
     },
@@ -772,11 +749,12 @@
         "Enabled": bool,
         "KeyCheckValueAlgorithm": KeyCheckValueAlgorithmType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ImportKeyInputRequestTypeDef(
     _RequiredImportKeyInputRequestTypeDef, _OptionalImportKeyInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/PKG-INFO` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-payment-cryptography
-Version: 1.28.12
-Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.PaymentCryptographyControlPlane 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-payment-cryptography.svg?color=blue)](https://pypi.org/project/mypy-boto3-payment-cryptography)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-payment-cryptography)](https://pepy.tech/project/mypy-boto3-payment-cryptography)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PaymentCryptographyControlPlane 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
+[boto3.PaymentCryptographyControlPlane 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#PaymentCryptographyControlPlane)
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
 [mypy-boto3-payment-cryptography docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_payment_cryptography/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,46 +354,43 @@
     GetAliasInputRequestTypeDef,
     GetKeyInputRequestTypeDef,
     GetParametersForExportInputRequestTypeDef,
     GetParametersForImportInputRequestTypeDef,
     GetPublicKeyCertificateInputRequestTypeDef,
     ImportTr31KeyBlockTypeDef,
     ImportTr34KeyBlockTypeDef,
-    KeyModesOfUseOutputTypeDef,
     KeyModesOfUseTypeDef,
     PaginatorConfigTypeDef,
     ListAliasesInputRequestTypeDef,
     ListKeysInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
     RestoreKeyInputRequestTypeDef,
     StartKeyUsageInputRequestTypeDef,
     StopKeyUsageInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateAliasInputRequestTypeDef,
     CreateAliasOutputTypeDef,
     GetAliasOutputTypeDef,
     GetParametersForExportOutputTypeDef,
     GetParametersForImportOutputTypeDef,
     GetPublicKeyCertificateOutputTypeDef,
     ListAliasesOutputTypeDef,
     UpdateAliasOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ExportKeyMaterialTypeDef,
     ExportKeyOutputTypeDef,
-    KeyAttributesOutputTypeDef,
     KeyAttributesTypeDef,
     ListAliasesInputListAliasesPaginateTypeDef,
     ListKeysInputListKeysPaginateTypeDef,
     ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ExportKeyInputRequestTypeDef,
+    CreateKeyInputRequestTypeDef,
     KeySummaryTypeDef,
     KeyTypeDef,
-    CreateKeyInputRequestTypeDef,
     RootCertificatePublicKeyTypeDef,
     TrustedCertificatePublicKeyTypeDef,
     ListKeysOutputTypeDef,
     CreateKeyOutputTypeDef,
     DeleteKeyOutputTypeDef,
     GetKeyOutputTypeDef,
     ImportKeyOutputTypeDef,
```

### Comparing `mypy-boto3-payment-cryptography-1.28.12/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt` & `mypy-boto3-payment-cryptography-1.28.15/mypy_boto3_payment_cryptography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-payment-cryptography-1.28.12/setup.py` & `mypy-boto3-payment-cryptography-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-payment-cryptography",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_payment_cryptography"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PaymentCryptographyControlPlane 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.PaymentCryptographyControlPlane 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

