# Comparing `tmp/mypy-boto3-route53domains-1.28.12.tar.gz` & `tmp/mypy-boto3-route53domains-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53domains-1.28.12.tar", last modified: Thu Jul 27 11:49:33 2023, max compression
+gzip compressed data, was "mypy-boto3-route53domains-1.28.15.tar", last modified: Fri Jul 28 20:43:37 2023, max compression
```

## Comparing `mypy-boto3-route53domains-1.28.12.tar` & `mypy-boto3-route53domains-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.037239 mypy-boto3-route53domains-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-07-27 11:49:33.033239 mypy-boto3-route53domains-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.029239 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28933 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28888 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-27 11:44:55.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-07-27 11:44:55.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28843 2023-07-27 11:44:55.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28820 2023-07-27 11:44:55.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.033239 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-07-27 11:49:32.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 11:49:32.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:32.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:32.000000 mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:33.037239 mypy-boto3-route53domains-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 11:44:54.000000 mypy-boto3-route53domains-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:37.005772 mypy-boto3-route53domains-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17307 2023-07-28 20:43:37.005772 mypy-boto3-route53domains-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:37.005772 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28933 2023-07-28 20:37:19.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28888 2023-07-28 20:37:19.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-28 20:37:19.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-07-28 20:37:19.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-28 20:37:19.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-28 20:37:19.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28505 2023-07-28 20:37:20.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28482 2023-07-28 20:37:20.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:37.005772 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17307 2023-07-28 20:43:36.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:43:36.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:36.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:36.000000 mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:37.005772 mypy-boto3-route53domains-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:37:18.000000 mypy-boto3-route53domains-1.28.15/setup.py
```

### Comparing `mypy-boto3-route53domains-1.28.12/LICENSE` & `mypy-boto3-route53domains-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.12/PKG-INFO` & `mypy-boto3-route53domains-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53domains
-Version: 1.28.12
-Summary: Type annotations for boto3.Route53Domains 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Route53Domains 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53domains)](https://pepy.tech/project/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,15 +353,14 @@
     DnssecSigningAttributesTypeDef,
     BillingRecordTypeDef,
     CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef,
     CheckDomainAvailabilityRequestRequestTypeDef,
     CheckDomainTransferabilityRequestRequestTypeDef,
     DomainTransferabilityTypeDef,
     ConsentTypeDef,
-    ExtraParamOutputTypeDef,
     ExtraParamTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteTagsForDomainRequestRequestTypeDef,
     DisableDomainAutoRenewRequestRequestTypeDef,
     DisableDomainTransferLockRequestRequestTypeDef,
     DisassociateDelegationSignerFromDomainRequestRequestTypeDef,
     DnssecKeyTypeDef,
@@ -378,23 +377,22 @@
     GetOperationDetailRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     SortConditionTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     NameserverTypeDef,
     PushDomainRequestRequestTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
     RenewDomainRequestRequestTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
-    TagTypeDef,
     TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     UpdateDomainContactPrivacyRequestRequestTypeDef,
     ViewBillingRequestRequestTypeDef,
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
@@ -426,16 +424,16 @@
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListPricesRequestListPricesPaginateTypeDef,
     ViewBillingRequestViewBillingPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
-    UpdateDomainNameserversRequestRequestTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
+    UpdateDomainNameserversRequestRequestTypeDef,
     GetDomainDetailResponseTypeDef,
     RegisterDomainRequestRequestTypeDef,
     TransferDomainRequestRequestTypeDef,
     UpdateDomainContactRequestRequestTypeDef,
     ListPricesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-route53domains-1.28.12/README.md` & `mypy-boto3-route53domains-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53domains)](https://pepy.tech/project/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,15 +321,14 @@
     DnssecSigningAttributesTypeDef,
     BillingRecordTypeDef,
     CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef,
     CheckDomainAvailabilityRequestRequestTypeDef,
     CheckDomainTransferabilityRequestRequestTypeDef,
     DomainTransferabilityTypeDef,
     ConsentTypeDef,
-    ExtraParamOutputTypeDef,
     ExtraParamTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteTagsForDomainRequestRequestTypeDef,
     DisableDomainAutoRenewRequestRequestTypeDef,
     DisableDomainTransferLockRequestRequestTypeDef,
     DisassociateDelegationSignerFromDomainRequestRequestTypeDef,
     DnssecKeyTypeDef,
@@ -346,23 +345,22 @@
     GetOperationDetailRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     SortConditionTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     NameserverTypeDef,
     PushDomainRequestRequestTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
     RenewDomainRequestRequestTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
-    TagTypeDef,
     TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     UpdateDomainContactPrivacyRequestRequestTypeDef,
     ViewBillingRequestRequestTypeDef,
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
@@ -394,16 +392,16 @@
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListPricesRequestListPricesPaginateTypeDef,
     ViewBillingRequestViewBillingPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
-    UpdateDomainNameserversRequestRequestTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
+    UpdateDomainNameserversRequestRequestTypeDef,
     GetDomainDetailResponseTypeDef,
     RegisterDomainRequestRequestTypeDef,
     TransferDomainRequestRequestTypeDef,
     UpdateDomainContactRequestRequestTypeDef,
     ListPricesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/__init__.py` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/__init__.pyi` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/__main__.py` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53Domains 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.Route53Domains 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains\nOther"
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

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/client.py` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/client.pyi` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/literals.py` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/literals.pyi` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/paginator.py` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/paginator.pyi` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/type_defs.py` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     "DnssecSigningAttributesTypeDef",
     "BillingRecordTypeDef",
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
     "CheckDomainAvailabilityRequestRequestTypeDef",
     "CheckDomainTransferabilityRequestRequestTypeDef",
     "DomainTransferabilityTypeDef",
     "ConsentTypeDef",
-    "ExtraParamOutputTypeDef",
     "ExtraParamTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteTagsForDomainRequestRequestTypeDef",
     "DisableDomainAutoRenewRequestRequestTypeDef",
     "DisableDomainTransferLockRequestRequestTypeDef",
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
     "DnssecKeyTypeDef",
@@ -71,23 +70,22 @@
     "GetOperationDetailRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "SortConditionTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "OperationSummaryTypeDef",
     "ListPricesRequestRequestTypeDef",
     "ListTagsForDomainRequestRequestTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "NameserverTypeDef",
     "PushDomainRequestRequestTypeDef",
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     "RenewDomainRequestRequestTypeDef",
     "ResendContactReachabilityEmailRequestRequestTypeDef",
     "ResendOperationAuthorizationRequestRequestTypeDef",
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
-    "TagTypeDef",
     "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     "UpdateDomainContactPrivacyRequestRequestTypeDef",
     "ViewBillingRequestRequestTypeDef",
     "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     "AssociateDelegationSignerToDomainResponseTypeDef",
     "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     "CheckDomainAvailabilityResponseTypeDef",
@@ -119,16 +117,16 @@
     "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListPricesRequestListPricesPaginateTypeDef",
     "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListTagsForDomainResponseTypeDef",
-    "UpdateDomainNameserversRequestRequestTypeDef",
     "UpdateTagsForDomainRequestRequestTypeDef",
+    "UpdateDomainNameserversRequestRequestTypeDef",
     "GetDomainDetailResponseTypeDef",
     "RegisterDomainRequestRequestTypeDef",
     "TransferDomainRequestRequestTypeDef",
     "UpdateDomainContactRequestRequestTypeDef",
     "ListPricesResponseTypeDef",
 )
 
@@ -236,22 +234,14 @@
     "ConsentTypeDef",
     {
         "MaxPrice": float,
         "Currency": str,
     },
 )
 
-ExtraParamOutputTypeDef = TypedDict(
-    "ExtraParamOutputTypeDef",
-    {
-        "Name": ExtraParamNameType,
-        "Value": str,
-    },
-)
-
 ExtraParamTypeDef = TypedDict(
     "ExtraParamTypeDef",
     {
         "Name": ExtraParamNameType,
         "Value": str,
     },
 )
@@ -468,16 +458,16 @@
 ListTagsForDomainRequestRequestTypeDef = TypedDict(
     "ListTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -555,23 +545,14 @@
 RetrieveDomainAuthCodeRequestRequestTypeDef = TypedDict(
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 TransferDomainToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "AccountId": str,
     },
 )
@@ -826,15 +807,15 @@
         "City": str,
         "State": str,
         "CountryCode": CountryCodeType,
         "ZipCode": str,
         "PhoneNumber": str,
         "Email": str,
         "Fax": str,
-        "ExtraParams": List[ExtraParamOutputTypeDef],
+        "ExtraParams": List[ExtraParamTypeDef],
     },
     total=False,
 )
 
 ContactDetailTypeDef = TypedDict(
     "ContactDetailTypeDef",
     {
@@ -947,60 +928,60 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForDomainResponseTypeDef = TypedDict(
     "ListTagsForDomainResponseTypeDef",
     {
-        "TagList": List[TagOutputTypeDef],
+        "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
+_RequiredUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
-        "Nameservers": Sequence[NameserverTypeDef],
     },
 )
-_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
+_OptionalUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTagsForDomainRequestRequestTypeDef",
     {
-        "FIAuthKey": str,
+        "TagsToUpdate": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class UpdateDomainNameserversRequestRequestTypeDef(
-    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
-    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
+class UpdateTagsForDomainRequestRequestTypeDef(
+    _RequiredUpdateTagsForDomainRequestRequestTypeDef,
+    _OptionalUpdateTagsForDomainRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateTagsForDomainRequestRequestTypeDef",
+_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
     {
         "DomainName": str,
+        "Nameservers": Sequence[NameserverTypeDef],
     },
 )
-_OptionalUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateTagsForDomainRequestRequestTypeDef",
+_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
     {
-        "TagsToUpdate": Sequence[TagTypeDef],
+        "FIAuthKey": str,
     },
     total=False,
 )
 
 
-class UpdateTagsForDomainRequestRequestTypeDef(
-    _RequiredUpdateTagsForDomainRequestRequestTypeDef,
-    _OptionalUpdateTagsForDomainRequestRequestTypeDef,
+class UpdateDomainNameserversRequestRequestTypeDef(
+    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
+    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
 ):
     pass
 
 
 GetDomainDetailResponseTypeDef = TypedDict(
     "GetDomainDetailResponseTypeDef",
     {
```

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains/type_defs.pyi` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     "DnssecSigningAttributesTypeDef",
     "BillingRecordTypeDef",
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
     "CheckDomainAvailabilityRequestRequestTypeDef",
     "CheckDomainTransferabilityRequestRequestTypeDef",
     "DomainTransferabilityTypeDef",
     "ConsentTypeDef",
-    "ExtraParamOutputTypeDef",
     "ExtraParamTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteTagsForDomainRequestRequestTypeDef",
     "DisableDomainAutoRenewRequestRequestTypeDef",
     "DisableDomainTransferLockRequestRequestTypeDef",
     "DisassociateDelegationSignerFromDomainRequestRequestTypeDef",
     "DnssecKeyTypeDef",
@@ -70,23 +69,22 @@
     "GetOperationDetailRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "SortConditionTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "OperationSummaryTypeDef",
     "ListPricesRequestRequestTypeDef",
     "ListTagsForDomainRequestRequestTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "NameserverTypeDef",
     "PushDomainRequestRequestTypeDef",
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     "RenewDomainRequestRequestTypeDef",
     "ResendContactReachabilityEmailRequestRequestTypeDef",
     "ResendOperationAuthorizationRequestRequestTypeDef",
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
-    "TagTypeDef",
     "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     "UpdateDomainContactPrivacyRequestRequestTypeDef",
     "ViewBillingRequestRequestTypeDef",
     "AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef",
     "AssociateDelegationSignerToDomainResponseTypeDef",
     "CancelDomainTransferToAnotherAwsAccountResponseTypeDef",
     "CheckDomainAvailabilityResponseTypeDef",
@@ -118,16 +116,16 @@
     "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListPricesRequestListPricesPaginateTypeDef",
     "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListTagsForDomainResponseTypeDef",
-    "UpdateDomainNameserversRequestRequestTypeDef",
     "UpdateTagsForDomainRequestRequestTypeDef",
+    "UpdateDomainNameserversRequestRequestTypeDef",
     "GetDomainDetailResponseTypeDef",
     "RegisterDomainRequestRequestTypeDef",
     "TransferDomainRequestRequestTypeDef",
     "UpdateDomainContactRequestRequestTypeDef",
     "ListPricesResponseTypeDef",
 )
 
@@ -231,22 +229,14 @@
     "ConsentTypeDef",
     {
         "MaxPrice": float,
         "Currency": str,
     },
 )
 
-ExtraParamOutputTypeDef = TypedDict(
-    "ExtraParamOutputTypeDef",
-    {
-        "Name": ExtraParamNameType,
-        "Value": str,
-    },
-)
-
 ExtraParamTypeDef = TypedDict(
     "ExtraParamTypeDef",
     {
         "Name": ExtraParamNameType,
         "Value": str,
     },
 )
@@ -461,16 +451,16 @@
 ListTagsForDomainRequestRequestTypeDef = TypedDict(
     "ListTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -544,23 +534,14 @@
 RetrieveDomainAuthCodeRequestRequestTypeDef = TypedDict(
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 TransferDomainToAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "AccountId": str,
     },
 )
@@ -813,15 +794,15 @@
         "City": str,
         "State": str,
         "CountryCode": CountryCodeType,
         "ZipCode": str,
         "PhoneNumber": str,
         "Email": str,
         "Fax": str,
-        "ExtraParams": List[ExtraParamOutputTypeDef],
+        "ExtraParams": List[ExtraParamTypeDef],
     },
     total=False,
 )
 
 ContactDetailTypeDef = TypedDict(
     "ContactDetailTypeDef",
     {
@@ -934,57 +915,57 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForDomainResponseTypeDef = TypedDict(
     "ListTagsForDomainResponseTypeDef",
     {
-        "TagList": List[TagOutputTypeDef],
+        "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
+_RequiredUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTagsForDomainRequestRequestTypeDef",
     {
         "DomainName": str,
-        "Nameservers": Sequence[NameserverTypeDef],
     },
 )
-_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
+_OptionalUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTagsForDomainRequestRequestTypeDef",
     {
-        "FIAuthKey": str,
+        "TagsToUpdate": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class UpdateDomainNameserversRequestRequestTypeDef(
-    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
-    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
+class UpdateTagsForDomainRequestRequestTypeDef(
+    _RequiredUpdateTagsForDomainRequestRequestTypeDef,
+    _OptionalUpdateTagsForDomainRequestRequestTypeDef,
 ):
     pass
 
-_RequiredUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateTagsForDomainRequestRequestTypeDef",
+_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
     {
         "DomainName": str,
+        "Nameservers": Sequence[NameserverTypeDef],
     },
 )
-_OptionalUpdateTagsForDomainRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateTagsForDomainRequestRequestTypeDef",
+_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
     {
-        "TagsToUpdate": Sequence[TagTypeDef],
+        "FIAuthKey": str,
     },
     total=False,
 )
 
-class UpdateTagsForDomainRequestRequestTypeDef(
-    _RequiredUpdateTagsForDomainRequestRequestTypeDef,
-    _OptionalUpdateTagsForDomainRequestRequestTypeDef,
+class UpdateDomainNameserversRequestRequestTypeDef(
+    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
+    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
 ):
     pass
 
 GetDomainDetailResponseTypeDef = TypedDict(
     "GetDomainDetailResponseTypeDef",
     {
         "DomainName": str,
```

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/PKG-INFO` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53domains
-Version: 1.28.12
-Summary: Type annotations for boto3.Route53Domains 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Route53Domains 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53domains.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53domains)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53domains)](https://pepy.tech/project/mypy-boto3-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Domains 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[boto3.Route53Domains 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [mypy-boto3-route53domains docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53domains/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,15 +353,14 @@
     DnssecSigningAttributesTypeDef,
     BillingRecordTypeDef,
     CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef,
     CheckDomainAvailabilityRequestRequestTypeDef,
     CheckDomainTransferabilityRequestRequestTypeDef,
     DomainTransferabilityTypeDef,
     ConsentTypeDef,
-    ExtraParamOutputTypeDef,
     ExtraParamTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteTagsForDomainRequestRequestTypeDef,
     DisableDomainAutoRenewRequestRequestTypeDef,
     DisableDomainTransferLockRequestRequestTypeDef,
     DisassociateDelegationSignerFromDomainRequestRequestTypeDef,
     DnssecKeyTypeDef,
@@ -378,23 +377,22 @@
     GetOperationDetailRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     SortConditionTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
     ListPricesRequestRequestTypeDef,
     ListTagsForDomainRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     NameserverTypeDef,
     PushDomainRequestRequestTypeDef,
     RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef,
     RenewDomainRequestRequestTypeDef,
     ResendContactReachabilityEmailRequestRequestTypeDef,
     ResendOperationAuthorizationRequestRequestTypeDef,
     RetrieveDomainAuthCodeRequestRequestTypeDef,
-    TagTypeDef,
     TransferDomainToAnotherAwsAccountRequestRequestTypeDef,
     UpdateDomainContactPrivacyRequestRequestTypeDef,
     ViewBillingRequestRequestTypeDef,
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
@@ -426,16 +424,16 @@
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListPricesRequestListPricesPaginateTypeDef,
     ViewBillingRequestViewBillingPaginateTypeDef,
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
-    UpdateDomainNameserversRequestRequestTypeDef,
     UpdateTagsForDomainRequestRequestTypeDef,
+    UpdateDomainNameserversRequestRequestTypeDef,
     GetDomainDetailResponseTypeDef,
     RegisterDomainRequestRequestTypeDef,
     TransferDomainRequestRequestTypeDef,
     UpdateDomainContactRequestRequestTypeDef,
     ListPricesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-route53domains-1.28.12/mypy_boto3_route53domains.egg-info/SOURCES.txt` & `mypy-boto3-route53domains-1.28.15/mypy_boto3_route53domains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53domains-1.28.12/setup.py` & `mypy-boto3-route53domains-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53domains",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_route53domains"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53Domains 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Route53Domains 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

