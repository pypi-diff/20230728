# Comparing `tmp/mypy-boto3-service-quotas-1.28.12.tar.gz` & `tmp/mypy-boto3-service-quotas-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-service-quotas-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
+gzip compressed data, was "mypy-boto3-service-quotas-1.28.15.tar", last modified: Fri Jul 28 20:43:43 2023, max compression
```

## Comparing `mypy-boto3-service-quotas-1.28.12.tar` & `mypy-boto3-service-quotas-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.481290 mypy-boto3-service-quotas-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-07-27 11:49:38.481290 mypy-boto3-service-quotas-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.477290 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17651 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:39.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.481290 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-07-27 11:49:38.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 11:49:38.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:38.000000 mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.481290 mypy-boto3-service-quotas-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 11:46:38.000000 mypy-boto3-service-quotas-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:43.293858 mypy-boto3-service-quotas-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:06.000000 mypy-boto3-service-quotas-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-07-28 20:43:43.289858 mypy-boto3-service-quotas-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-07-28 20:39:06.000000 mypy-boto3-service-quotas-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:43.285858 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-28 20:39:06.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-28 20:39:06.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:39:06.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-07-28 20:39:07.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-07-28 20:39:06.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-28 20:39:07.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-28 20:39:07.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-28 20:39:07.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-07-28 20:39:07.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:06.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17522 2023-07-28 20:39:07.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17509 2023-07-28 20:39:07.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:06.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:43.289858 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-07-28 20:43:43.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:43:43.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:43.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:43.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:43.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:43.000000 mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:43.293858 mypy-boto3-service-quotas-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:39:06.000000 mypy-boto3-service-quotas-1.28.15/setup.py
```

### Comparing `mypy-boto3-service-quotas-1.28.12/LICENSE` & `mypy-boto3-service-quotas-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.12/PKG-INFO` & `mypy-boto3-service-quotas-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-service-quotas
-Version: 1.28.12
-Summary: Type annotations for boto3.ServiceQuotas 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ServiceQuotas 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-service-quotas)](https://pepy.tech/project/mypy-boto3-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceQuotas 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[boto3.ServiceQuotas 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [mypy-boto3-service-quotas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,20 +369,19 @@
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
     ListServiceQuotasRequestRequestTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     MetricInfoTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
     QuotaPeriodTypeDef,
     RequestServiceQuotaIncreaseRequestRequestTypeDef,
-    TagTypeDef,
     UntagResourceRequestRequestTypeDef,
     GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
     RequestServiceQuotaIncreaseResponseTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
@@ -392,16 +391,16 @@
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
     ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ServiceQuotaTypeDef,
     TagResourceRequestRequestTypeDef,
+    ServiceQuotaTypeDef,
     GetAWSDefaultServiceQuotaResponseTypeDef,
     GetServiceQuotaResponseTypeDef,
     ListAWSDefaultServiceQuotasResponseTypeDef,
     ListServiceQuotasResponseTypeDef,
 )
```

### Comparing `mypy-boto3-service-quotas-1.28.12/README.md` & `mypy-boto3-service-quotas-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-service-quotas)](https://pepy.tech/project/mypy-boto3-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceQuotas 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[boto3.ServiceQuotas 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [mypy-boto3-service-quotas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -337,20 +337,19 @@
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
     ListServiceQuotasRequestRequestTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     MetricInfoTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
     QuotaPeriodTypeDef,
     RequestServiceQuotaIncreaseRequestRequestTypeDef,
-    TagTypeDef,
     UntagResourceRequestRequestTypeDef,
     GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
     RequestServiceQuotaIncreaseResponseTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
@@ -360,16 +359,16 @@
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
     ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ServiceQuotaTypeDef,
     TagResourceRequestRequestTypeDef,
+    ServiceQuotaTypeDef,
     GetAWSDefaultServiceQuotaResponseTypeDef,
     GetServiceQuotaResponseTypeDef,
     ListAWSDefaultServiceQuotasResponseTypeDef,
     ListServiceQuotasResponseTypeDef,
 )
```

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/__init__.py` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/__init__.pyi` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/__main__.py` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServiceQuotas 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ServiceQuotas 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas\nOther"
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

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/client.py` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/client.pyi` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/literals.py` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/literals.pyi` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/paginator.py` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/paginator.pyi` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/type_defs.py` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,19 @@
     "ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
     "ListServiceQuotasRequestRequestTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ServiceInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "MetricInfoTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     "QuotaPeriodTypeDef",
     "RequestServiceQuotaIncreaseRequestRequestTypeDef",
-    "TagTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "GetAssociationForServiceQuotaTemplateResponseTypeDef",
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     "RequestServiceQuotaIncreaseResponseTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
@@ -66,16 +65,16 @@
     "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
     "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ServiceQuotaTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "ServiceQuotaTypeDef",
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     "GetServiceQuotaResponseTypeDef",
     "ListAWSDefaultServiceQuotasResponseTypeDef",
     "ListServiceQuotasResponseTypeDef",
 )
 
 DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef = TypedDict(
@@ -298,16 +297,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 )
 
 MetricInfoTypeDef = TypedDict(
@@ -345,22 +344,14 @@
     {
         "ServiceCode": str,
         "QuotaCode": str,
         "DesiredValue": float,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -538,19 +529,27 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 ServiceQuotaTypeDef = TypedDict(
     "ServiceQuotaTypeDef",
     {
         "ServiceCode": str,
         "ServiceName": str,
         "QuotaArn": str,
         "QuotaCode": str,
@@ -562,22 +561,14 @@
         "UsageMetric": MetricInfoTypeDef,
         "Period": QuotaPeriodTypeDef,
         "ErrorReason": ErrorReasonTypeDef,
     },
     total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 GetAWSDefaultServiceQuotaResponseTypeDef = TypedDict(
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas/type_defs.pyi` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,19 @@
     "ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef",
     "ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef",
     "ListServiceQuotasRequestRequestTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ServiceInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "MetricInfoTypeDef",
     "PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef",
     "QuotaPeriodTypeDef",
     "RequestServiceQuotaIncreaseRequestRequestTypeDef",
-    "TagTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "GetAssociationForServiceQuotaTemplateResponseTypeDef",
     "GetRequestedServiceQuotaChangeResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef",
     "ListRequestedServiceQuotaChangeHistoryResponseTypeDef",
     "RequestServiceQuotaIncreaseResponseTypeDef",
     "GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef",
@@ -65,16 +64,16 @@
     "ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef",
     "ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef",
     "ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef",
     "ListServiceQuotasRequestListServiceQuotasPaginateTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ServiceQuotaTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "ServiceQuotaTypeDef",
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     "GetServiceQuotaResponseTypeDef",
     "ListAWSDefaultServiceQuotasResponseTypeDef",
     "ListServiceQuotasResponseTypeDef",
 )
 
 DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef = TypedDict(
@@ -291,16 +290,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 )
 
 MetricInfoTypeDef = TypedDict(
@@ -338,22 +337,14 @@
     {
         "ServiceCode": str,
         "QuotaCode": str,
         "DesiredValue": float,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -525,19 +516,27 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 ServiceQuotaTypeDef = TypedDict(
     "ServiceQuotaTypeDef",
     {
         "ServiceCode": str,
         "ServiceName": str,
         "QuotaArn": str,
         "QuotaCode": str,
@@ -549,22 +548,14 @@
         "UsageMetric": MetricInfoTypeDef,
         "Period": QuotaPeriodTypeDef,
         "ErrorReason": ErrorReasonTypeDef,
     },
     total=False,
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 GetAWSDefaultServiceQuotaResponseTypeDef = TypedDict(
     "GetAWSDefaultServiceQuotaResponseTypeDef",
     {
         "Quota": ServiceQuotaTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/PKG-INFO` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-service-quotas
-Version: 1.28.12
-Summary: Type annotations for boto3.ServiceQuotas 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ServiceQuotas 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-service-quotas.svg?color=blue)](https://pypi.org/project/mypy-boto3-service-quotas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-service-quotas)](https://pepy.tech/project/mypy-boto3-service-quotas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceQuotas 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
+[boto3.ServiceQuotas 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#ServiceQuotas)
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
 [mypy-boto3-service-quotas docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_service_quotas/).
 
 See how it helps to find and fix potential bugs:
 
@@ -369,20 +369,19 @@
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef,
     ListServiceQuotasRequestRequestTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     MetricInfoTypeDef,
     PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef,
     QuotaPeriodTypeDef,
     RequestServiceQuotaIncreaseRequestRequestTypeDef,
-    TagTypeDef,
     UntagResourceRequestRequestTypeDef,
     GetAssociationForServiceQuotaTemplateResponseTypeDef,
     GetRequestedServiceQuotaChangeResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef,
     ListRequestedServiceQuotaChangeHistoryResponseTypeDef,
     RequestServiceQuotaIncreaseResponseTypeDef,
     GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef,
@@ -392,16 +391,16 @@
     ListRequestedServiceQuotaChangeHistoryByQuotaRequestListRequestedServiceQuotaChangeHistoryByQuotaPaginateTypeDef,
     ListRequestedServiceQuotaChangeHistoryRequestListRequestedServiceQuotaChangeHistoryPaginateTypeDef,
     ListServiceQuotaIncreaseRequestsInTemplateRequestListServiceQuotaIncreaseRequestsInTemplatePaginateTypeDef,
     ListServiceQuotasRequestListServiceQuotasPaginateTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ServiceQuotaTypeDef,
     TagResourceRequestRequestTypeDef,
+    ServiceQuotaTypeDef,
     GetAWSDefaultServiceQuotaResponseTypeDef,
     GetServiceQuotaResponseTypeDef,
     ListAWSDefaultServiceQuotasResponseTypeDef,
     ListServiceQuotasResponseTypeDef,
 )
```

### Comparing `mypy-boto3-service-quotas-1.28.12/mypy_boto3_service_quotas.egg-info/SOURCES.txt` & `mypy-boto3-service-quotas-1.28.15/mypy_boto3_service_quotas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-service-quotas-1.28.12/setup.py` & `mypy-boto3-service-quotas-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-service-quotas",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_service_quotas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServiceQuotas 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ServiceQuotas 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

