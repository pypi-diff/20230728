# Comparing `tmp/mypy-boto3-acm-pca-1.28.12.tar.gz` & `tmp/mypy-boto3-acm-pca-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-acm-pca-1.28.12.tar", last modified: Thu Jul 27 05:34:13 2023, max compression
+gzip compressed data, was "mypy-boto3-acm-pca-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
```

## Comparing `mypy-boto3-acm-pca-1.28.12.tar` & `mypy-boto3-acm-pca-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.844594 mypy-boto3-acm-pca-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-07-27 05:34:13.844594 mypy-boto3-acm-pca-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.824594 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22381 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22345 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32740 2023-07-27 05:16:55.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32687 2023-07-27 05:16:55.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-27 05:16:54.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.824594 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17619 2023-07-27 05:34:13.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 05:34:13.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:13.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:13.000000 mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:13.844594 mypy-boto3-acm-pca-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-27 05:16:53.000000 mypy-boto3-acm-pca-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.724609 mypy-boto3-acm-pca-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-07-28 20:42:12.716609 mypy-boto3-acm-pca-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15841 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.712609 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22381 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22345 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-07-28 20:18:41.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-28 20:18:41.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29584 2023-07-28 20:18:42.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29539 2023-07-28 20:18:41.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.712609 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-07-28 20:42:12.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-28 20:42:12.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:12.000000 mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.724609 mypy-boto3-acm-pca-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-28 20:18:40.000000 mypy-boto3-acm-pca-1.28.15/setup.py
```

### Comparing `mypy-boto3-acm-pca-1.28.12/LICENSE` & `mypy-boto3-acm-pca-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.12/PKG-INFO` & `mypy-boto3-acm-pca-1.28.15/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm-pca
-Version: 1.28.12
-Summary: Type annotations for boto3.ACMPCA 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ACMPCA 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm-pca)](https://pepy.tech/project/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,51 +377,43 @@
 ### Typed dictionaries
 
 `mypy_boto3_acm_pca.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_acm_pca.type_defs import (
-    CustomAttributeOutputTypeDef,
     CustomAttributeTypeDef,
-    AccessMethodOutputTypeDef,
     AccessMethodTypeDef,
     CreateCertificateAuthorityAuditReportRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreatePermissionRequestRequestTypeDef,
-    CrlConfigurationOutputTypeDef,
     CrlConfigurationTypeDef,
-    KeyUsageOutputTypeDef,
     KeyUsageTypeDef,
     CustomExtensionTypeDef,
     DeleteCertificateAuthorityRequestRequestTypeDef,
     DeletePermissionRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateAuthorityAuditReportRequestRequestTypeDef,
     DescribeCertificateAuthorityRequestRequestTypeDef,
-    EdiPartyNameOutputTypeDef,
     EdiPartyNameTypeDef,
     ExtendedKeyUsageTypeDef,
-    OtherNameOutputTypeDef,
     OtherNameTypeDef,
     GetCertificateAuthorityCertificateRequestRequestTypeDef,
     GetCertificateAuthorityCsrRequestRequestTypeDef,
     GetCertificateRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     ValidityTypeDef,
     PaginatorConfigTypeDef,
     ListCertificateAuthoritiesRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
-    OcspConfigurationOutputTypeDef,
     OcspConfigurationTypeDef,
     QualifierTypeDef,
     PutPolicyRequestRequestTypeDef,
     RestoreCertificateAuthorityRequestRequestTypeDef,
     RevokeCertificateRequestRequestTypeDef,
     ASN1SubjectOutputTypeDef,
     ASN1SubjectTypeDef,
@@ -430,25 +422,24 @@
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
     GetCertificateResponseTypeDef,
     GetPolicyResponseTypeDef,
     IssueCertificateResponseTypeDef,
+    ListTagsResponseTypeDef,
     TagCertificateAuthorityRequestRequestTypeDef,
     UntagCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
     GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
     GetCertificateRequestCertificateIssuedWaitTypeDef,
     ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListPermissionsResponseTypeDef,
-    ListTagsResponseTypeDef,
-    RevocationConfigurationOutputTypeDef,
     RevocationConfigurationTypeDef,
     PolicyQualifierInfoTypeDef,
     GeneralNameOutputTypeDef,
     GeneralNameTypeDef,
     UpdateCertificateAuthorityRequestRequestTypeDef,
     PolicyInformationTypeDef,
     AccessDescriptionOutputTypeDef,
@@ -463,15 +454,15 @@
     CertificateAuthorityTypeDef,
     CreateCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     ListCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> CustomAttributeOutputTypeDef:
+def get_structure() -> CustomAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-acm-pca-1.28.12/README.md` & `mypy-boto3-acm-pca-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm-pca)](https://pepy.tech/project/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,51 +345,43 @@
 ### Typed dictionaries
 
 `mypy_boto3_acm_pca.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_acm_pca.type_defs import (
-    CustomAttributeOutputTypeDef,
     CustomAttributeTypeDef,
-    AccessMethodOutputTypeDef,
     AccessMethodTypeDef,
     CreateCertificateAuthorityAuditReportRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreatePermissionRequestRequestTypeDef,
-    CrlConfigurationOutputTypeDef,
     CrlConfigurationTypeDef,
-    KeyUsageOutputTypeDef,
     KeyUsageTypeDef,
     CustomExtensionTypeDef,
     DeleteCertificateAuthorityRequestRequestTypeDef,
     DeletePermissionRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateAuthorityAuditReportRequestRequestTypeDef,
     DescribeCertificateAuthorityRequestRequestTypeDef,
-    EdiPartyNameOutputTypeDef,
     EdiPartyNameTypeDef,
     ExtendedKeyUsageTypeDef,
-    OtherNameOutputTypeDef,
     OtherNameTypeDef,
     GetCertificateAuthorityCertificateRequestRequestTypeDef,
     GetCertificateAuthorityCsrRequestRequestTypeDef,
     GetCertificateRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     ValidityTypeDef,
     PaginatorConfigTypeDef,
     ListCertificateAuthoritiesRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
-    OcspConfigurationOutputTypeDef,
     OcspConfigurationTypeDef,
     QualifierTypeDef,
     PutPolicyRequestRequestTypeDef,
     RestoreCertificateAuthorityRequestRequestTypeDef,
     RevokeCertificateRequestRequestTypeDef,
     ASN1SubjectOutputTypeDef,
     ASN1SubjectTypeDef,
@@ -398,25 +390,24 @@
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
     GetCertificateResponseTypeDef,
     GetPolicyResponseTypeDef,
     IssueCertificateResponseTypeDef,
+    ListTagsResponseTypeDef,
     TagCertificateAuthorityRequestRequestTypeDef,
     UntagCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
     GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
     GetCertificateRequestCertificateIssuedWaitTypeDef,
     ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListPermissionsResponseTypeDef,
-    ListTagsResponseTypeDef,
-    RevocationConfigurationOutputTypeDef,
     RevocationConfigurationTypeDef,
     PolicyQualifierInfoTypeDef,
     GeneralNameOutputTypeDef,
     GeneralNameTypeDef,
     UpdateCertificateAuthorityRequestRequestTypeDef,
     PolicyInformationTypeDef,
     AccessDescriptionOutputTypeDef,
@@ -431,15 +422,15 @@
     CertificateAuthorityTypeDef,
     CreateCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     ListCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> CustomAttributeOutputTypeDef:
+def get_structure() -> CustomAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/__init__.py` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/__init__.pyi` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/__main__.py` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ACMPCA 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.ACMPCA 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA\nOther"
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

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/client.py` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/client.pyi` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/literals.py` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/literals.pyi` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/paginator.py` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/paginator.pyi` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/type_defs.py` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for acm-pca service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_acm_pca.type_defs import CustomAttributeOutputTypeDef
+    from mypy_boto3_acm_pca.type_defs import CustomAttributeTypeDef
 
-    data: CustomAttributeOutputTypeDef = {...}
+    data: CustomAttributeTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -43,51 +43,43 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "CustomAttributeOutputTypeDef",
     "CustomAttributeTypeDef",
-    "AccessMethodOutputTypeDef",
     "AccessMethodTypeDef",
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreatePermissionRequestRequestTypeDef",
-    "CrlConfigurationOutputTypeDef",
     "CrlConfigurationTypeDef",
-    "KeyUsageOutputTypeDef",
     "KeyUsageTypeDef",
     "CustomExtensionTypeDef",
     "DeleteCertificateAuthorityRequestRequestTypeDef",
     "DeletePermissionRequestRequestTypeDef",
     "DeletePolicyRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCertificateAuthorityAuditReportRequestRequestTypeDef",
     "DescribeCertificateAuthorityRequestRequestTypeDef",
-    "EdiPartyNameOutputTypeDef",
     "EdiPartyNameTypeDef",
     "ExtendedKeyUsageTypeDef",
-    "OtherNameOutputTypeDef",
     "OtherNameTypeDef",
     "GetCertificateAuthorityCertificateRequestRequestTypeDef",
     "GetCertificateAuthorityCsrRequestRequestTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "ValidityTypeDef",
     "PaginatorConfigTypeDef",
     "ListCertificateAuthoritiesRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "OcspConfigurationOutputTypeDef",
     "OcspConfigurationTypeDef",
     "QualifierTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "RestoreCertificateAuthorityRequestRequestTypeDef",
     "RevokeCertificateRequestRequestTypeDef",
     "ASN1SubjectOutputTypeDef",
     "ASN1SubjectTypeDef",
@@ -96,25 +88,24 @@
     "DescribeCertificateAuthorityAuditReportResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCertificateAuthorityCertificateResponseTypeDef",
     "GetCertificateAuthorityCsrResponseTypeDef",
     "GetCertificateResponseTypeDef",
     "GetPolicyResponseTypeDef",
     "IssueCertificateResponseTypeDef",
+    "ListTagsResponseTypeDef",
     "TagCertificateAuthorityRequestRequestTypeDef",
     "UntagCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef",
     "GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     "GetCertificateRequestCertificateIssuedWaitTypeDef",
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListPermissionsResponseTypeDef",
-    "ListTagsResponseTypeDef",
-    "RevocationConfigurationOutputTypeDef",
     "RevocationConfigurationTypeDef",
     "PolicyQualifierInfoTypeDef",
     "GeneralNameOutputTypeDef",
     "GeneralNameTypeDef",
     "UpdateCertificateAuthorityRequestRequestTypeDef",
     "PolicyInformationTypeDef",
     "AccessDescriptionOutputTypeDef",
@@ -128,39 +119,22 @@
     "IssueCertificateRequestRequestTypeDef",
     "CertificateAuthorityTypeDef",
     "CreateCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityResponseTypeDef",
     "ListCertificateAuthoritiesResponseTypeDef",
 )
 
-CustomAttributeOutputTypeDef = TypedDict(
-    "CustomAttributeOutputTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "Value": str,
-    },
-)
-
 CustomAttributeTypeDef = TypedDict(
     "CustomAttributeTypeDef",
     {
         "ObjectIdentifier": str,
         "Value": str,
     },
 )
 
-AccessMethodOutputTypeDef = TypedDict(
-    "AccessMethodOutputTypeDef",
-    {
-        "CustomObjectIdentifier": str,
-        "AccessMethodType": AccessMethodTypeType,
-    },
-    total=False,
-)
-
 AccessMethodTypeDef = TypedDict(
     "AccessMethodTypeDef",
     {
         "CustomObjectIdentifier": str,
         "AccessMethodType": AccessMethodTypeType,
     },
     total=False,
@@ -224,38 +198,14 @@
 
 class CreatePermissionRequestRequestTypeDef(
     _RequiredCreatePermissionRequestRequestTypeDef, _OptionalCreatePermissionRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredCrlConfigurationOutputTypeDef = TypedDict(
-    "_RequiredCrlConfigurationOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalCrlConfigurationOutputTypeDef = TypedDict(
-    "_OptionalCrlConfigurationOutputTypeDef",
-    {
-        "ExpirationInDays": int,
-        "CustomCname": str,
-        "S3BucketName": str,
-        "S3ObjectAcl": S3ObjectAclType,
-    },
-    total=False,
-)
-
-
-class CrlConfigurationOutputTypeDef(
-    _RequiredCrlConfigurationOutputTypeDef, _OptionalCrlConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredCrlConfigurationTypeDef = TypedDict(
     "_RequiredCrlConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCrlConfigurationTypeDef = TypedDict(
@@ -270,30 +220,14 @@
 )
 
 
 class CrlConfigurationTypeDef(_RequiredCrlConfigurationTypeDef, _OptionalCrlConfigurationTypeDef):
     pass
 
 
-KeyUsageOutputTypeDef = TypedDict(
-    "KeyUsageOutputTypeDef",
-    {
-        "DigitalSignature": bool,
-        "NonRepudiation": bool,
-        "KeyEncipherment": bool,
-        "DataEncipherment": bool,
-        "KeyAgreement": bool,
-        "KeyCertSign": bool,
-        "CRLSign": bool,
-        "EncipherOnly": bool,
-        "DecipherOnly": bool,
-    },
-    total=False,
-)
-
 KeyUsageTypeDef = TypedDict(
     "KeyUsageTypeDef",
     {
         "DigitalSignature": bool,
         "NonRepudiation": bool,
         "KeyEncipherment": bool,
         "DataEncipherment": bool,
@@ -397,35 +331,14 @@
 DescribeCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "DescribeCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 
-_RequiredEdiPartyNameOutputTypeDef = TypedDict(
-    "_RequiredEdiPartyNameOutputTypeDef",
-    {
-        "PartyName": str,
-    },
-)
-_OptionalEdiPartyNameOutputTypeDef = TypedDict(
-    "_OptionalEdiPartyNameOutputTypeDef",
-    {
-        "NameAssigner": str,
-    },
-    total=False,
-)
-
-
-class EdiPartyNameOutputTypeDef(
-    _RequiredEdiPartyNameOutputTypeDef, _OptionalEdiPartyNameOutputTypeDef
-):
-    pass
-
-
 _RequiredEdiPartyNameTypeDef = TypedDict(
     "_RequiredEdiPartyNameTypeDef",
     {
         "PartyName": str,
     },
 )
 _OptionalEdiPartyNameTypeDef = TypedDict(
@@ -446,22 +359,14 @@
     {
         "ExtendedKeyUsageType": ExtendedKeyUsageTypeType,
         "ExtendedKeyUsageObjectIdentifier": str,
     },
     total=False,
 )
 
-OtherNameOutputTypeDef = TypedDict(
-    "OtherNameOutputTypeDef",
-    {
-        "TypeId": str,
-        "Value": str,
-    },
-)
-
 OtherNameTypeDef = TypedDict(
     "OtherNameTypeDef",
     {
         "TypeId": str,
         "Value": str,
     },
 )
@@ -599,54 +504,14 @@
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
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
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
-
-_RequiredOcspConfigurationOutputTypeDef = TypedDict(
-    "_RequiredOcspConfigurationOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalOcspConfigurationOutputTypeDef = TypedDict(
-    "_OptionalOcspConfigurationOutputTypeDef",
-    {
-        "OcspCustomCname": str,
-    },
-    total=False,
-)
-
-
-class OcspConfigurationOutputTypeDef(
-    _RequiredOcspConfigurationOutputTypeDef, _OptionalOcspConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredOcspConfigurationTypeDef = TypedDict(
     "_RequiredOcspConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalOcspConfigurationTypeDef = TypedDict(
@@ -708,15 +573,15 @@
         "Locality": str,
         "Title": str,
         "Surname": str,
         "GivenName": str,
         "Initials": str,
         "Pseudonym": str,
         "GenerationQualifier": str,
-        "CustomAttributes": List[CustomAttributeOutputTypeDef],
+        "CustomAttributes": List[CustomAttributeTypeDef],
     },
     total=False,
 )
 
 ASN1SubjectTypeDef = TypedDict(
     "ASN1SubjectTypeDef",
     {
@@ -812,14 +677,23 @@
     "IssueCertificateResponseTypeDef",
     {
         "CertificateArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "TagCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -957,32 +831,14 @@
     {
         "Permissions": List[PermissionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RevocationConfigurationOutputTypeDef = TypedDict(
-    "RevocationConfigurationOutputTypeDef",
-    {
-        "CrlConfiguration": CrlConfigurationOutputTypeDef,
-        "OcspConfiguration": OcspConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 RevocationConfigurationTypeDef = TypedDict(
     "RevocationConfigurationTypeDef",
     {
         "CrlConfiguration": CrlConfigurationTypeDef,
         "OcspConfiguration": OcspConfigurationTypeDef,
     },
     total=False,
@@ -995,19 +851,19 @@
         "Qualifier": QualifierTypeDef,
     },
 )
 
 GeneralNameOutputTypeDef = TypedDict(
     "GeneralNameOutputTypeDef",
     {
-        "OtherName": OtherNameOutputTypeDef,
+        "OtherName": OtherNameTypeDef,
         "Rfc822Name": str,
         "DnsName": str,
         "DirectoryName": ASN1SubjectOutputTypeDef,
-        "EdiPartyName": EdiPartyNameOutputTypeDef,
+        "EdiPartyName": EdiPartyNameTypeDef,
         "UniformResourceIdentifier": str,
         "IpAddress": str,
         "RegisteredId": str,
     },
     total=False,
 )
 
@@ -1069,15 +925,15 @@
 ):
     pass
 
 
 AccessDescriptionOutputTypeDef = TypedDict(
     "AccessDescriptionOutputTypeDef",
     {
-        "AccessMethod": AccessMethodOutputTypeDef,
+        "AccessMethod": AccessMethodTypeDef,
         "AccessLocation": GeneralNameOutputTypeDef,
     },
 )
 
 AccessDescriptionTypeDef = TypedDict(
     "AccessDescriptionTypeDef",
     {
@@ -1097,15 +953,15 @@
     },
     total=False,
 )
 
 CsrExtensionsOutputTypeDef = TypedDict(
     "CsrExtensionsOutputTypeDef",
     {
-        "KeyUsage": KeyUsageOutputTypeDef,
+        "KeyUsage": KeyUsageTypeDef,
         "SubjectInformationAccess": List[AccessDescriptionOutputTypeDef],
     },
     total=False,
 )
 
 CsrExtensionsTypeDef = TypedDict(
     "CsrExtensionsTypeDef",
@@ -1210,15 +1066,15 @@
         "Type": CertificateAuthorityTypeType,
         "Serial": str,
         "Status": CertificateAuthorityStatusType,
         "NotBefore": datetime,
         "NotAfter": datetime,
         "FailureReason": FailureReasonType,
         "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationOutputTypeDef,
-        "RevocationConfiguration": RevocationConfigurationOutputTypeDef,
+        "RevocationConfiguration": RevocationConfigurationTypeDef,
         "RestorableUntil": datetime,
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/type_defs.pyi` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for acm-pca service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_acm_pca.type_defs import CustomAttributeOutputTypeDef
+    from mypy_boto3_acm_pca.type_defs import CustomAttributeTypeDef
 
-    data: CustomAttributeOutputTypeDef = {...}
+    data: CustomAttributeTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -42,51 +42,43 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "CustomAttributeOutputTypeDef",
     "CustomAttributeTypeDef",
-    "AccessMethodOutputTypeDef",
     "AccessMethodTypeDef",
     "CreateCertificateAuthorityAuditReportRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreatePermissionRequestRequestTypeDef",
-    "CrlConfigurationOutputTypeDef",
     "CrlConfigurationTypeDef",
-    "KeyUsageOutputTypeDef",
     "KeyUsageTypeDef",
     "CustomExtensionTypeDef",
     "DeleteCertificateAuthorityRequestRequestTypeDef",
     "DeletePermissionRequestRequestTypeDef",
     "DeletePolicyRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCertificateAuthorityAuditReportRequestRequestTypeDef",
     "DescribeCertificateAuthorityRequestRequestTypeDef",
-    "EdiPartyNameOutputTypeDef",
     "EdiPartyNameTypeDef",
     "ExtendedKeyUsageTypeDef",
-    "OtherNameOutputTypeDef",
     "OtherNameTypeDef",
     "GetCertificateAuthorityCertificateRequestRequestTypeDef",
     "GetCertificateAuthorityCsrRequestRequestTypeDef",
     "GetCertificateRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "ValidityTypeDef",
     "PaginatorConfigTypeDef",
     "ListCertificateAuthoritiesRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "OcspConfigurationOutputTypeDef",
     "OcspConfigurationTypeDef",
     "QualifierTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "RestoreCertificateAuthorityRequestRequestTypeDef",
     "RevokeCertificateRequestRequestTypeDef",
     "ASN1SubjectOutputTypeDef",
     "ASN1SubjectTypeDef",
@@ -95,25 +87,24 @@
     "DescribeCertificateAuthorityAuditReportResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCertificateAuthorityCertificateResponseTypeDef",
     "GetCertificateAuthorityCsrResponseTypeDef",
     "GetCertificateResponseTypeDef",
     "GetPolicyResponseTypeDef",
     "IssueCertificateResponseTypeDef",
+    "ListTagsResponseTypeDef",
     "TagCertificateAuthorityRequestRequestTypeDef",
     "UntagCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef",
     "GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     "GetCertificateRequestCertificateIssuedWaitTypeDef",
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListPermissionsResponseTypeDef",
-    "ListTagsResponseTypeDef",
-    "RevocationConfigurationOutputTypeDef",
     "RevocationConfigurationTypeDef",
     "PolicyQualifierInfoTypeDef",
     "GeneralNameOutputTypeDef",
     "GeneralNameTypeDef",
     "UpdateCertificateAuthorityRequestRequestTypeDef",
     "PolicyInformationTypeDef",
     "AccessDescriptionOutputTypeDef",
@@ -127,39 +118,22 @@
     "IssueCertificateRequestRequestTypeDef",
     "CertificateAuthorityTypeDef",
     "CreateCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityResponseTypeDef",
     "ListCertificateAuthoritiesResponseTypeDef",
 )
 
-CustomAttributeOutputTypeDef = TypedDict(
-    "CustomAttributeOutputTypeDef",
-    {
-        "ObjectIdentifier": str,
-        "Value": str,
-    },
-)
-
 CustomAttributeTypeDef = TypedDict(
     "CustomAttributeTypeDef",
     {
         "ObjectIdentifier": str,
         "Value": str,
     },
 )
 
-AccessMethodOutputTypeDef = TypedDict(
-    "AccessMethodOutputTypeDef",
-    {
-        "CustomObjectIdentifier": str,
-        "AccessMethodType": AccessMethodTypeType,
-    },
-    total=False,
-)
-
 AccessMethodTypeDef = TypedDict(
     "AccessMethodTypeDef",
     {
         "CustomObjectIdentifier": str,
         "AccessMethodType": AccessMethodTypeType,
     },
     total=False,
@@ -219,36 +193,14 @@
 )
 
 class CreatePermissionRequestRequestTypeDef(
     _RequiredCreatePermissionRequestRequestTypeDef, _OptionalCreatePermissionRequestRequestTypeDef
 ):
     pass
 
-_RequiredCrlConfigurationOutputTypeDef = TypedDict(
-    "_RequiredCrlConfigurationOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalCrlConfigurationOutputTypeDef = TypedDict(
-    "_OptionalCrlConfigurationOutputTypeDef",
-    {
-        "ExpirationInDays": int,
-        "CustomCname": str,
-        "S3BucketName": str,
-        "S3ObjectAcl": S3ObjectAclType,
-    },
-    total=False,
-)
-
-class CrlConfigurationOutputTypeDef(
-    _RequiredCrlConfigurationOutputTypeDef, _OptionalCrlConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredCrlConfigurationTypeDef = TypedDict(
     "_RequiredCrlConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalCrlConfigurationTypeDef = TypedDict(
@@ -261,30 +213,14 @@
     },
     total=False,
 )
 
 class CrlConfigurationTypeDef(_RequiredCrlConfigurationTypeDef, _OptionalCrlConfigurationTypeDef):
     pass
 
-KeyUsageOutputTypeDef = TypedDict(
-    "KeyUsageOutputTypeDef",
-    {
-        "DigitalSignature": bool,
-        "NonRepudiation": bool,
-        "KeyEncipherment": bool,
-        "DataEncipherment": bool,
-        "KeyAgreement": bool,
-        "KeyCertSign": bool,
-        "CRLSign": bool,
-        "EncipherOnly": bool,
-        "DecipherOnly": bool,
-    },
-    total=False,
-)
-
 KeyUsageTypeDef = TypedDict(
     "KeyUsageTypeDef",
     {
         "DigitalSignature": bool,
         "NonRepudiation": bool,
         "KeyEncipherment": bool,
         "DataEncipherment": bool,
@@ -382,33 +318,14 @@
 DescribeCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "DescribeCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
     },
 )
 
-_RequiredEdiPartyNameOutputTypeDef = TypedDict(
-    "_RequiredEdiPartyNameOutputTypeDef",
-    {
-        "PartyName": str,
-    },
-)
-_OptionalEdiPartyNameOutputTypeDef = TypedDict(
-    "_OptionalEdiPartyNameOutputTypeDef",
-    {
-        "NameAssigner": str,
-    },
-    total=False,
-)
-
-class EdiPartyNameOutputTypeDef(
-    _RequiredEdiPartyNameOutputTypeDef, _OptionalEdiPartyNameOutputTypeDef
-):
-    pass
-
 _RequiredEdiPartyNameTypeDef = TypedDict(
     "_RequiredEdiPartyNameTypeDef",
     {
         "PartyName": str,
     },
 )
 _OptionalEdiPartyNameTypeDef = TypedDict(
@@ -427,22 +344,14 @@
     {
         "ExtendedKeyUsageType": ExtendedKeyUsageTypeType,
         "ExtendedKeyUsageObjectIdentifier": str,
     },
     total=False,
 )
 
-OtherNameOutputTypeDef = TypedDict(
-    "OtherNameOutputTypeDef",
-    {
-        "TypeId": str,
-        "Value": str,
-    },
-)
-
 OtherNameTypeDef = TypedDict(
     "OtherNameTypeDef",
     {
         "TypeId": str,
         "Value": str,
     },
 )
@@ -574,50 +483,14 @@
 )
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
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
-
-_RequiredOcspConfigurationOutputTypeDef = TypedDict(
-    "_RequiredOcspConfigurationOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalOcspConfigurationOutputTypeDef = TypedDict(
-    "_OptionalOcspConfigurationOutputTypeDef",
-    {
-        "OcspCustomCname": str,
-    },
-    total=False,
-)
-
-class OcspConfigurationOutputTypeDef(
-    _RequiredOcspConfigurationOutputTypeDef, _OptionalOcspConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredOcspConfigurationTypeDef = TypedDict(
     "_RequiredOcspConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalOcspConfigurationTypeDef = TypedDict(
@@ -677,15 +550,15 @@
         "Locality": str,
         "Title": str,
         "Surname": str,
         "GivenName": str,
         "Initials": str,
         "Pseudonym": str,
         "GenerationQualifier": str,
-        "CustomAttributes": List[CustomAttributeOutputTypeDef],
+        "CustomAttributes": List[CustomAttributeTypeDef],
     },
     total=False,
 )
 
 ASN1SubjectTypeDef = TypedDict(
     "ASN1SubjectTypeDef",
     {
@@ -781,14 +654,23 @@
     "IssueCertificateResponseTypeDef",
     {
         "CertificateArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "TagCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -916,32 +798,14 @@
     {
         "Permissions": List[PermissionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RevocationConfigurationOutputTypeDef = TypedDict(
-    "RevocationConfigurationOutputTypeDef",
-    {
-        "CrlConfiguration": CrlConfigurationOutputTypeDef,
-        "OcspConfiguration": OcspConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 RevocationConfigurationTypeDef = TypedDict(
     "RevocationConfigurationTypeDef",
     {
         "CrlConfiguration": CrlConfigurationTypeDef,
         "OcspConfiguration": OcspConfigurationTypeDef,
     },
     total=False,
@@ -954,19 +818,19 @@
         "Qualifier": QualifierTypeDef,
     },
 )
 
 GeneralNameOutputTypeDef = TypedDict(
     "GeneralNameOutputTypeDef",
     {
-        "OtherName": OtherNameOutputTypeDef,
+        "OtherName": OtherNameTypeDef,
         "Rfc822Name": str,
         "DnsName": str,
         "DirectoryName": ASN1SubjectOutputTypeDef,
-        "EdiPartyName": EdiPartyNameOutputTypeDef,
+        "EdiPartyName": EdiPartyNameTypeDef,
         "UniformResourceIdentifier": str,
         "IpAddress": str,
         "RegisteredId": str,
     },
     total=False,
 )
 
@@ -1024,15 +888,15 @@
     _RequiredPolicyInformationTypeDef, _OptionalPolicyInformationTypeDef
 ):
     pass
 
 AccessDescriptionOutputTypeDef = TypedDict(
     "AccessDescriptionOutputTypeDef",
     {
-        "AccessMethod": AccessMethodOutputTypeDef,
+        "AccessMethod": AccessMethodTypeDef,
         "AccessLocation": GeneralNameOutputTypeDef,
     },
 )
 
 AccessDescriptionTypeDef = TypedDict(
     "AccessDescriptionTypeDef",
     {
@@ -1052,15 +916,15 @@
     },
     total=False,
 )
 
 CsrExtensionsOutputTypeDef = TypedDict(
     "CsrExtensionsOutputTypeDef",
     {
-        "KeyUsage": KeyUsageOutputTypeDef,
+        "KeyUsage": KeyUsageTypeDef,
         "SubjectInformationAccess": List[AccessDescriptionOutputTypeDef],
     },
     total=False,
 )
 
 CsrExtensionsTypeDef = TypedDict(
     "CsrExtensionsTypeDef",
@@ -1159,15 +1023,15 @@
         "Type": CertificateAuthorityTypeType,
         "Serial": str,
         "Status": CertificateAuthorityStatusType,
         "NotBefore": datetime,
         "NotAfter": datetime,
         "FailureReason": FailureReasonType,
         "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationOutputTypeDef,
-        "RevocationConfiguration": RevocationConfigurationOutputTypeDef,
+        "RevocationConfiguration": RevocationConfigurationTypeDef,
         "RestorableUntil": datetime,
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/waiter.py` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca/waiter.pyi` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/PKG-INFO` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm-pca
-Version: 1.28.12
-Summary: Type annotations for boto3.ACMPCA 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ACMPCA 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm-pca)](https://pepy.tech/project/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
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
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
 
@@ -377,51 +377,43 @@
 ### Typed dictionaries
 
 `mypy_boto3_acm_pca.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_acm_pca.type_defs import (
-    CustomAttributeOutputTypeDef,
     CustomAttributeTypeDef,
-    AccessMethodOutputTypeDef,
     AccessMethodTypeDef,
     CreateCertificateAuthorityAuditReportRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreatePermissionRequestRequestTypeDef,
-    CrlConfigurationOutputTypeDef,
     CrlConfigurationTypeDef,
-    KeyUsageOutputTypeDef,
     KeyUsageTypeDef,
     CustomExtensionTypeDef,
     DeleteCertificateAuthorityRequestRequestTypeDef,
     DeletePermissionRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCertificateAuthorityAuditReportRequestRequestTypeDef,
     DescribeCertificateAuthorityRequestRequestTypeDef,
-    EdiPartyNameOutputTypeDef,
     EdiPartyNameTypeDef,
     ExtendedKeyUsageTypeDef,
-    OtherNameOutputTypeDef,
     OtherNameTypeDef,
     GetCertificateAuthorityCertificateRequestRequestTypeDef,
     GetCertificateAuthorityCsrRequestRequestTypeDef,
     GetCertificateRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     ImportCertificateAuthorityCertificateRequestRequestTypeDef,
     ValidityTypeDef,
     PaginatorConfigTypeDef,
     ListCertificateAuthoritiesRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     ListTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
-    OcspConfigurationOutputTypeDef,
     OcspConfigurationTypeDef,
     QualifierTypeDef,
     PutPolicyRequestRequestTypeDef,
     RestoreCertificateAuthorityRequestRequestTypeDef,
     RevokeCertificateRequestRequestTypeDef,
     ASN1SubjectOutputTypeDef,
     ASN1SubjectTypeDef,
@@ -430,25 +422,24 @@
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
     GetCertificateResponseTypeDef,
     GetPolicyResponseTypeDef,
     IssueCertificateResponseTypeDef,
+    ListTagsResponseTypeDef,
     TagCertificateAuthorityRequestRequestTypeDef,
     UntagCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityAuditReportRequestAuditReportCreatedWaitTypeDef,
     GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef,
     GetCertificateRequestCertificateIssuedWaitTypeDef,
     ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef,
     ListPermissionsRequestListPermissionsPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListPermissionsResponseTypeDef,
-    ListTagsResponseTypeDef,
-    RevocationConfigurationOutputTypeDef,
     RevocationConfigurationTypeDef,
     PolicyQualifierInfoTypeDef,
     GeneralNameOutputTypeDef,
     GeneralNameTypeDef,
     UpdateCertificateAuthorityRequestRequestTypeDef,
     PolicyInformationTypeDef,
     AccessDescriptionOutputTypeDef,
@@ -463,15 +454,15 @@
     CertificateAuthorityTypeDef,
     CreateCertificateAuthorityRequestRequestTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     ListCertificateAuthoritiesResponseTypeDef,
 )
 
 
-def get_structure() -> CustomAttributeOutputTypeDef:
+def get_structure() -> CustomAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-acm-pca-1.28.12/mypy_boto3_acm_pca.egg-info/SOURCES.txt` & `mypy-boto3-acm-pca-1.28.15/mypy_boto3_acm_pca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-acm-pca-1.28.12/setup.py` & `mypy-boto3-acm-pca-1.28.15/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-acm-pca",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_acm_pca"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ACMPCA 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ACMPCA 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

