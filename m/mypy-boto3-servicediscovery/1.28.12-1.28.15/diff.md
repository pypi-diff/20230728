# Comparing `tmp/mypy-boto3-servicediscovery-1.28.12.tar.gz` & `tmp/mypy-boto3-servicediscovery-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicediscovery-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
+gzip compressed data, was "mypy-boto3-servicediscovery-1.28.15.tar", last modified: Fri Jul 28 20:43:44 2023, max compression
```

## Comparing `mypy-boto3-servicediscovery-1.28.12.tar` & `mypy-boto3-servicediscovery-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.765293 mypy-boto3-servicediscovery-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-07-27 11:49:38.757293 mypy-boto3-servicediscovery-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15821 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.757293 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22776 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30085 2023-07-27 11:46:49.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-07-27 11:46:48.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.757293 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-07-27 11:49:38.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 11:49:38.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 11:49:38.000000 mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.765293 mypy-boto3-servicediscovery-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 11:46:47.000000 mypy-boto3-servicediscovery-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.369873 mypy-boto3-servicediscovery-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:18.000000 mypy-boto3-servicediscovery-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-07-28 20:43:44.357873 mypy-boto3-servicediscovery-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15671 2023-07-28 20:39:18.000000 mypy-boto3-servicediscovery-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.349872 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-28 20:39:18.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-28 20:39:18.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 20:39:18.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-28 20:39:19.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22776 2023-07-28 20:39:19.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-07-28 20:39:19.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-07-28 20:39:19.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-28 20:39:19.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-28 20:39:19.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:18.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28902 2023-07-28 20:39:20.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28864 2023-07-28 20:39:19.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:18.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.357873 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-07-28 20:43:44.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:43:44.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:44.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:44.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:44.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:43:44.000000 mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:44.369873 mypy-boto3-servicediscovery-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 20:39:18.000000 mypy-boto3-servicediscovery-1.28.15/setup.py
```

### Comparing `mypy-boto3-servicediscovery-1.28.12/LICENSE` & `mypy-boto3-servicediscovery-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.12/PKG-INFO` & `mypy-boto3-servicediscovery-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicediscovery
-Version: 1.28.12
-Summary: Type annotations for boto3.ServiceDiscovery 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ServiceDiscovery 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicediscovery)](https://pepy.tech/project/mypy-boto3-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceDiscovery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[boto3.ServiceDiscovery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [mypy-boto3-servicediscovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,96 +357,91 @@
     HealthCheckCustomConfigTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
     DiscoverInstancesRequestRequestTypeDef,
     HttpInstanceSummaryTypeDef,
     DnsRecordTypeDef,
-    DnsRecordOutputTypeDef,
-    SOAOutputTypeDef,
+    SOATypeDef,
     GetInstanceRequestRequestTypeDef,
     InstanceTypeDef,
     GetInstancesHealthStatusRequestRequestTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     OperationTypeDef,
     GetServiceRequestRequestTypeDef,
-    HealthCheckConfigOutputTypeDef,
-    HealthCheckCustomConfigOutputTypeDef,
     HttpNamespaceChangeTypeDef,
     HttpPropertiesTypeDef,
     InstanceSummaryTypeDef,
     PaginatorConfigTypeDef,
     ListInstancesRequestRequestTypeDef,
     NamespaceFilterTypeDef,
     OperationFilterTypeDef,
     OperationSummaryTypeDef,
     ServiceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     SOAChangeTypeDef,
-    SOATypeDef,
     RegisterInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
     CreateHttpNamespaceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateHttpNamespaceResponseTypeDef,
     CreatePrivateDnsNamespaceResponseTypeDef,
     CreatePublicDnsNamespaceResponseTypeDef,
     DeleteNamespaceResponseTypeDef,
     DeregisterInstanceResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetInstancesHealthStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RegisterInstanceResponseTypeDef,
     UpdateHttpNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceResponseTypeDef,
     UpdatePublicDnsNamespaceResponseTypeDef,
     UpdateServiceResponseTypeDef,
     DiscoverInstancesResponseTypeDef,
     DnsConfigChangeTypeDef,
-    DnsConfigTypeDef,
     DnsConfigOutputTypeDef,
+    DnsConfigTypeDef,
     DnsPropertiesTypeDef,
+    PrivateDnsPropertiesMutableTypeDef,
+    PublicDnsPropertiesMutableTypeDef,
     GetInstanceResponseTypeDef,
     GetOperationResponseTypeDef,
     UpdateHttpNamespaceRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PrivateDnsPropertiesMutableChangeTypeDef,
     PublicDnsPropertiesMutableChangeTypeDef,
-    PrivateDnsPropertiesMutableTypeDef,
-    PublicDnsPropertiesMutableTypeDef,
     ServiceChangeTypeDef,
-    CreateServiceRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ServiceTypeDef,
+    CreateServiceRequestRequestTypeDef,
     NamespacePropertiesTypeDef,
-    PrivateDnsNamespacePropertiesChangeTypeDef,
-    PublicDnsNamespacePropertiesChangeTypeDef,
     PrivateDnsNamespacePropertiesTypeDef,
     PublicDnsNamespacePropertiesTypeDef,
+    PrivateDnsNamespacePropertiesChangeTypeDef,
+    PublicDnsNamespacePropertiesChangeTypeDef,
     UpdateServiceRequestRequestTypeDef,
     ListServicesResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceResponseTypeDef,
     NamespaceSummaryTypeDef,
     NamespaceTypeDef,
-    PrivateDnsNamespaceChangeTypeDef,
-    PublicDnsNamespaceChangeTypeDef,
     CreatePrivateDnsNamespaceRequestRequestTypeDef,
     CreatePublicDnsNamespaceRequestRequestTypeDef,
+    PrivateDnsNamespaceChangeTypeDef,
+    PublicDnsNamespaceChangeTypeDef,
     ListNamespacesResponseTypeDef,
     GetNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceRequestRequestTypeDef,
     UpdatePublicDnsNamespaceRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-servicediscovery-1.28.12/README.md` & `mypy-boto3-servicediscovery-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicediscovery)](https://pepy.tech/project/mypy-boto3-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceDiscovery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[boto3.ServiceDiscovery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [mypy-boto3-servicediscovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,96 +325,91 @@
     HealthCheckCustomConfigTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
     DiscoverInstancesRequestRequestTypeDef,
     HttpInstanceSummaryTypeDef,
     DnsRecordTypeDef,
-    DnsRecordOutputTypeDef,
-    SOAOutputTypeDef,
+    SOATypeDef,
     GetInstanceRequestRequestTypeDef,
     InstanceTypeDef,
     GetInstancesHealthStatusRequestRequestTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     OperationTypeDef,
     GetServiceRequestRequestTypeDef,
-    HealthCheckConfigOutputTypeDef,
-    HealthCheckCustomConfigOutputTypeDef,
     HttpNamespaceChangeTypeDef,
     HttpPropertiesTypeDef,
     InstanceSummaryTypeDef,
     PaginatorConfigTypeDef,
     ListInstancesRequestRequestTypeDef,
     NamespaceFilterTypeDef,
     OperationFilterTypeDef,
     OperationSummaryTypeDef,
     ServiceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     SOAChangeTypeDef,
-    SOATypeDef,
     RegisterInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
     CreateHttpNamespaceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateHttpNamespaceResponseTypeDef,
     CreatePrivateDnsNamespaceResponseTypeDef,
     CreatePublicDnsNamespaceResponseTypeDef,
     DeleteNamespaceResponseTypeDef,
     DeregisterInstanceResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetInstancesHealthStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RegisterInstanceResponseTypeDef,
     UpdateHttpNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceResponseTypeDef,
     UpdatePublicDnsNamespaceResponseTypeDef,
     UpdateServiceResponseTypeDef,
     DiscoverInstancesResponseTypeDef,
     DnsConfigChangeTypeDef,
-    DnsConfigTypeDef,
     DnsConfigOutputTypeDef,
+    DnsConfigTypeDef,
     DnsPropertiesTypeDef,
+    PrivateDnsPropertiesMutableTypeDef,
+    PublicDnsPropertiesMutableTypeDef,
     GetInstanceResponseTypeDef,
     GetOperationResponseTypeDef,
     UpdateHttpNamespaceRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PrivateDnsPropertiesMutableChangeTypeDef,
     PublicDnsPropertiesMutableChangeTypeDef,
-    PrivateDnsPropertiesMutableTypeDef,
-    PublicDnsPropertiesMutableTypeDef,
     ServiceChangeTypeDef,
-    CreateServiceRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ServiceTypeDef,
+    CreateServiceRequestRequestTypeDef,
     NamespacePropertiesTypeDef,
-    PrivateDnsNamespacePropertiesChangeTypeDef,
-    PublicDnsNamespacePropertiesChangeTypeDef,
     PrivateDnsNamespacePropertiesTypeDef,
     PublicDnsNamespacePropertiesTypeDef,
+    PrivateDnsNamespacePropertiesChangeTypeDef,
+    PublicDnsNamespacePropertiesChangeTypeDef,
     UpdateServiceRequestRequestTypeDef,
     ListServicesResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceResponseTypeDef,
     NamespaceSummaryTypeDef,
     NamespaceTypeDef,
-    PrivateDnsNamespaceChangeTypeDef,
-    PublicDnsNamespaceChangeTypeDef,
     CreatePrivateDnsNamespaceRequestRequestTypeDef,
     CreatePublicDnsNamespaceRequestRequestTypeDef,
+    PrivateDnsNamespaceChangeTypeDef,
+    PublicDnsNamespaceChangeTypeDef,
     ListNamespacesResponseTypeDef,
     GetNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceRequestRequestTypeDef,
     UpdatePublicDnsNamespaceRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/__init__.py` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/__init__.pyi` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/__main__.py` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServiceDiscovery 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ServiceDiscovery 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery\nOther"
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

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/client.py` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/client.pyi` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/literals.py` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/literals.pyi` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/paginator.py` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/paginator.pyi` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/type_defs.py` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,96 +49,91 @@
     "HealthCheckCustomConfigTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
     "DiscoverInstancesRequestRequestTypeDef",
     "HttpInstanceSummaryTypeDef",
     "DnsRecordTypeDef",
-    "DnsRecordOutputTypeDef",
-    "SOAOutputTypeDef",
+    "SOATypeDef",
     "GetInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
     "GetInstancesHealthStatusRequestRequestTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "OperationTypeDef",
     "GetServiceRequestRequestTypeDef",
-    "HealthCheckConfigOutputTypeDef",
-    "HealthCheckCustomConfigOutputTypeDef",
     "HttpNamespaceChangeTypeDef",
     "HttpPropertiesTypeDef",
     "InstanceSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "NamespaceFilterTypeDef",
     "OperationFilterTypeDef",
     "OperationSummaryTypeDef",
     "ServiceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "SOAChangeTypeDef",
-    "SOATypeDef",
     "RegisterInstanceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
     "CreateHttpNamespaceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateHttpNamespaceResponseTypeDef",
     "CreatePrivateDnsNamespaceResponseTypeDef",
     "CreatePublicDnsNamespaceResponseTypeDef",
     "DeleteNamespaceResponseTypeDef",
     "DeregisterInstanceResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetInstancesHealthStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RegisterInstanceResponseTypeDef",
     "UpdateHttpNamespaceResponseTypeDef",
     "UpdatePrivateDnsNamespaceResponseTypeDef",
     "UpdatePublicDnsNamespaceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
     "DiscoverInstancesResponseTypeDef",
     "DnsConfigChangeTypeDef",
-    "DnsConfigTypeDef",
     "DnsConfigOutputTypeDef",
+    "DnsConfigTypeDef",
     "DnsPropertiesTypeDef",
+    "PrivateDnsPropertiesMutableTypeDef",
+    "PublicDnsPropertiesMutableTypeDef",
     "GetInstanceResponseTypeDef",
     "GetOperationResponseTypeDef",
     "UpdateHttpNamespaceRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
     "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PrivateDnsPropertiesMutableChangeTypeDef",
     "PublicDnsPropertiesMutableChangeTypeDef",
-    "PrivateDnsPropertiesMutableTypeDef",
-    "PublicDnsPropertiesMutableTypeDef",
     "ServiceChangeTypeDef",
-    "CreateServiceRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ServiceTypeDef",
+    "CreateServiceRequestRequestTypeDef",
     "NamespacePropertiesTypeDef",
-    "PrivateDnsNamespacePropertiesChangeTypeDef",
-    "PublicDnsNamespacePropertiesChangeTypeDef",
     "PrivateDnsNamespacePropertiesTypeDef",
     "PublicDnsNamespacePropertiesTypeDef",
+    "PrivateDnsNamespacePropertiesChangeTypeDef",
+    "PublicDnsNamespacePropertiesChangeTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "ListServicesResponseTypeDef",
     "CreateServiceResponseTypeDef",
     "GetServiceResponseTypeDef",
     "NamespaceSummaryTypeDef",
     "NamespaceTypeDef",
-    "PrivateDnsNamespaceChangeTypeDef",
-    "PublicDnsNamespaceChangeTypeDef",
     "CreatePrivateDnsNamespaceRequestRequestTypeDef",
     "CreatePublicDnsNamespaceRequestRequestTypeDef",
+    "PrivateDnsNamespaceChangeTypeDef",
+    "PublicDnsNamespaceChangeTypeDef",
     "ListNamespacesResponseTypeDef",
     "GetNamespaceResponseTypeDef",
     "UpdatePrivateDnsNamespaceRequestRequestTypeDef",
     "UpdatePublicDnsNamespaceRequestRequestTypeDef",
 )
 
 TagTypeDef = TypedDict(
@@ -253,24 +248,16 @@
     "DnsRecordTypeDef",
     {
         "Type": RecordTypeType,
         "TTL": int,
     },
 )
 
-DnsRecordOutputTypeDef = TypedDict(
-    "DnsRecordOutputTypeDef",
-    {
-        "Type": RecordTypeType,
-        "TTL": int,
-    },
-)
-
-SOAOutputTypeDef = TypedDict(
-    "SOAOutputTypeDef",
+SOATypeDef = TypedDict(
+    "SOATypeDef",
     {
         "TTL": int,
     },
 )
 
 GetInstanceRequestRequestTypeDef = TypedDict(
     "GetInstanceRequestRequestTypeDef",
@@ -356,44 +343,14 @@
 GetServiceRequestRequestTypeDef = TypedDict(
     "GetServiceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-_RequiredHealthCheckConfigOutputTypeDef = TypedDict(
-    "_RequiredHealthCheckConfigOutputTypeDef",
-    {
-        "Type": HealthCheckTypeType,
-    },
-)
-_OptionalHealthCheckConfigOutputTypeDef = TypedDict(
-    "_OptionalHealthCheckConfigOutputTypeDef",
-    {
-        "ResourcePath": str,
-        "FailureThreshold": int,
-    },
-    total=False,
-)
-
-
-class HealthCheckConfigOutputTypeDef(
-    _RequiredHealthCheckConfigOutputTypeDef, _OptionalHealthCheckConfigOutputTypeDef
-):
-    pass
-
-
-HealthCheckCustomConfigOutputTypeDef = TypedDict(
-    "HealthCheckCustomConfigOutputTypeDef",
-    {
-        "FailureThreshold": int,
-    },
-    total=False,
-)
-
 HttpNamespaceChangeTypeDef = TypedDict(
     "HttpNamespaceChangeTypeDef",
     {
         "Description": str,
     },
 )
 
@@ -518,36 +475,21 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 SOAChangeTypeDef = TypedDict(
     "SOAChangeTypeDef",
     {
         "TTL": int,
     },
 )
 
-SOATypeDef = TypedDict(
-    "SOATypeDef",
-    {
-        "TTL": int,
-    },
-)
-
 _RequiredRegisterInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
         "Attributes": Mapping[str, str],
     },
@@ -668,14 +610,22 @@
     {
         "Status": Dict[str, HealthStatusType],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RegisterInstanceResponseTypeDef = TypedDict(
     "RegisterInstanceResponseTypeDef",
     {
         "OperationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -723,63 +673,77 @@
 DnsConfigChangeTypeDef = TypedDict(
     "DnsConfigChangeTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
     },
 )
 
-_RequiredDnsConfigTypeDef = TypedDict(
-    "_RequiredDnsConfigTypeDef",
+_RequiredDnsConfigOutputTypeDef = TypedDict(
+    "_RequiredDnsConfigOutputTypeDef",
     {
-        "DnsRecords": Sequence[DnsRecordTypeDef],
+        "DnsRecords": List[DnsRecordTypeDef],
     },
 )
-_OptionalDnsConfigTypeDef = TypedDict(
-    "_OptionalDnsConfigTypeDef",
+_OptionalDnsConfigOutputTypeDef = TypedDict(
+    "_OptionalDnsConfigOutputTypeDef",
     {
         "NamespaceId": str,
         "RoutingPolicy": RoutingPolicyType,
     },
     total=False,
 )
 
 
-class DnsConfigTypeDef(_RequiredDnsConfigTypeDef, _OptionalDnsConfigTypeDef):
+class DnsConfigOutputTypeDef(_RequiredDnsConfigOutputTypeDef, _OptionalDnsConfigOutputTypeDef):
     pass
 
 
-_RequiredDnsConfigOutputTypeDef = TypedDict(
-    "_RequiredDnsConfigOutputTypeDef",
+_RequiredDnsConfigTypeDef = TypedDict(
+    "_RequiredDnsConfigTypeDef",
     {
-        "DnsRecords": List[DnsRecordOutputTypeDef],
+        "DnsRecords": Sequence[DnsRecordTypeDef],
     },
 )
-_OptionalDnsConfigOutputTypeDef = TypedDict(
-    "_OptionalDnsConfigOutputTypeDef",
+_OptionalDnsConfigTypeDef = TypedDict(
+    "_OptionalDnsConfigTypeDef",
     {
         "NamespaceId": str,
         "RoutingPolicy": RoutingPolicyType,
     },
     total=False,
 )
 
 
-class DnsConfigOutputTypeDef(_RequiredDnsConfigOutputTypeDef, _OptionalDnsConfigOutputTypeDef):
+class DnsConfigTypeDef(_RequiredDnsConfigTypeDef, _OptionalDnsConfigTypeDef):
     pass
 
 
 DnsPropertiesTypeDef = TypedDict(
     "DnsPropertiesTypeDef",
     {
         "HostedZoneId": str,
-        "SOA": SOAOutputTypeDef,
+        "SOA": SOATypeDef,
     },
     total=False,
 )
 
+PrivateDnsPropertiesMutableTypeDef = TypedDict(
+    "PrivateDnsPropertiesMutableTypeDef",
+    {
+        "SOA": SOATypeDef,
+    },
+)
+
+PublicDnsPropertiesMutableTypeDef = TypedDict(
+    "PublicDnsPropertiesMutableTypeDef",
+    {
+        "SOA": SOATypeDef,
+    },
+)
+
 GetInstanceResponseTypeDef = TypedDict(
     "GetInstanceResponseTypeDef",
     {
         "Instance": InstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -908,56 +872,70 @@
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[ServiceFilterTypeDef],
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PrivateDnsPropertiesMutableChangeTypeDef = TypedDict(
     "PrivateDnsPropertiesMutableChangeTypeDef",
     {
         "SOA": SOAChangeTypeDef,
     },
 )
 
 PublicDnsPropertiesMutableChangeTypeDef = TypedDict(
     "PublicDnsPropertiesMutableChangeTypeDef",
     {
         "SOA": SOAChangeTypeDef,
     },
 )
 
-PrivateDnsPropertiesMutableTypeDef = TypedDict(
-    "PrivateDnsPropertiesMutableTypeDef",
+ServiceChangeTypeDef = TypedDict(
+    "ServiceChangeTypeDef",
     {
-        "SOA": SOATypeDef,
+        "Description": str,
+        "DnsConfig": DnsConfigChangeTypeDef,
+        "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
+    total=False,
 )
 
-PublicDnsPropertiesMutableTypeDef = TypedDict(
-    "PublicDnsPropertiesMutableTypeDef",
+ServiceSummaryTypeDef = TypedDict(
+    "ServiceSummaryTypeDef",
     {
-        "SOA": SOATypeDef,
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Type": ServiceTypeType,
+        "Description": str,
+        "InstanceCount": int,
+        "DnsConfig": DnsConfigOutputTypeDef,
+        "HealthCheckConfig": HealthCheckConfigTypeDef,
+        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
+        "CreateDate": datetime,
     },
+    total=False,
 )
 
-ServiceChangeTypeDef = TypedDict(
-    "ServiceChangeTypeDef",
+ServiceTypeDef = TypedDict(
+    "ServiceTypeDef",
     {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "NamespaceId": str,
         "Description": str,
-        "DnsConfig": DnsConfigChangeTypeDef,
+        "InstanceCount": int,
+        "DnsConfig": DnsConfigOutputTypeDef,
+        "Type": ServiceTypeType,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
+        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
+        "CreateDate": datetime,
+        "CreatorRequestId": str,
     },
     total=False,
 )
 
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
@@ -982,57 +960,35 @@
 
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
 
-ServiceSummaryTypeDef = TypedDict(
-    "ServiceSummaryTypeDef",
+NamespacePropertiesTypeDef = TypedDict(
+    "NamespacePropertiesTypeDef",
     {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Type": ServiceTypeType,
-        "Description": str,
-        "InstanceCount": int,
-        "DnsConfig": DnsConfigOutputTypeDef,
-        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
-        "HealthCheckCustomConfig": HealthCheckCustomConfigOutputTypeDef,
-        "CreateDate": datetime,
+        "DnsProperties": DnsPropertiesTypeDef,
+        "HttpProperties": HttpPropertiesTypeDef,
     },
     total=False,
 )
 
-ServiceTypeDef = TypedDict(
-    "ServiceTypeDef",
+PrivateDnsNamespacePropertiesTypeDef = TypedDict(
+    "PrivateDnsNamespacePropertiesTypeDef",
     {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "NamespaceId": str,
-        "Description": str,
-        "InstanceCount": int,
-        "DnsConfig": DnsConfigOutputTypeDef,
-        "Type": ServiceTypeType,
-        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
-        "HealthCheckCustomConfig": HealthCheckCustomConfigOutputTypeDef,
-        "CreateDate": datetime,
-        "CreatorRequestId": str,
+        "DnsProperties": PrivateDnsPropertiesMutableTypeDef,
     },
-    total=False,
 )
 
-NamespacePropertiesTypeDef = TypedDict(
-    "NamespacePropertiesTypeDef",
+PublicDnsNamespacePropertiesTypeDef = TypedDict(
+    "PublicDnsNamespacePropertiesTypeDef",
     {
-        "DnsProperties": DnsPropertiesTypeDef,
-        "HttpProperties": HttpPropertiesTypeDef,
+        "DnsProperties": PublicDnsPropertiesMutableTypeDef,
     },
-    total=False,
 )
 
 PrivateDnsNamespacePropertiesChangeTypeDef = TypedDict(
     "PrivateDnsNamespacePropertiesChangeTypeDef",
     {
         "DnsProperties": PrivateDnsPropertiesMutableChangeTypeDef,
     },
@@ -1041,28 +997,14 @@
 PublicDnsNamespacePropertiesChangeTypeDef = TypedDict(
     "PublicDnsNamespacePropertiesChangeTypeDef",
     {
         "DnsProperties": PublicDnsPropertiesMutableChangeTypeDef,
     },
 )
 
-PrivateDnsNamespacePropertiesTypeDef = TypedDict(
-    "PrivateDnsNamespacePropertiesTypeDef",
-    {
-        "DnsProperties": PrivateDnsPropertiesMutableTypeDef,
-    },
-)
-
-PublicDnsNamespacePropertiesTypeDef = TypedDict(
-    "PublicDnsNamespacePropertiesTypeDef",
-    {
-        "DnsProperties": PublicDnsPropertiesMutableTypeDef,
-    },
-)
-
 UpdateServiceRequestRequestTypeDef = TypedDict(
     "UpdateServiceRequestRequestTypeDef",
     {
         "Id": str,
         "Service": ServiceChangeTypeDef,
     },
 )
@@ -1119,32 +1061,14 @@
         "Properties": NamespacePropertiesTypeDef,
         "CreateDate": datetime,
         "CreatorRequestId": str,
     },
     total=False,
 )
 
-PrivateDnsNamespaceChangeTypeDef = TypedDict(
-    "PrivateDnsNamespaceChangeTypeDef",
-    {
-        "Description": str,
-        "Properties": PrivateDnsNamespacePropertiesChangeTypeDef,
-    },
-    total=False,
-)
-
-PublicDnsNamespaceChangeTypeDef = TypedDict(
-    "PublicDnsNamespaceChangeTypeDef",
-    {
-        "Description": str,
-        "Properties": PublicDnsNamespacePropertiesChangeTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreatePrivateDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "Name": str,
         "Vpc": str,
     },
 )
@@ -1188,14 +1112,32 @@
 class CreatePublicDnsNamespaceRequestRequestTypeDef(
     _RequiredCreatePublicDnsNamespaceRequestRequestTypeDef,
     _OptionalCreatePublicDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
 
+PrivateDnsNamespaceChangeTypeDef = TypedDict(
+    "PrivateDnsNamespaceChangeTypeDef",
+    {
+        "Description": str,
+        "Properties": PrivateDnsNamespacePropertiesChangeTypeDef,
+    },
+    total=False,
+)
+
+PublicDnsNamespaceChangeTypeDef = TypedDict(
+    "PublicDnsNamespaceChangeTypeDef",
+    {
+        "Description": str,
+        "Properties": PublicDnsNamespacePropertiesChangeTypeDef,
+    },
+    total=False,
+)
+
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "Namespaces": List[NamespaceSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery/type_defs.pyi` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -48,96 +48,91 @@
     "HealthCheckCustomConfigTypeDef",
     "DeleteNamespaceRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
     "DiscoverInstancesRequestRequestTypeDef",
     "HttpInstanceSummaryTypeDef",
     "DnsRecordTypeDef",
-    "DnsRecordOutputTypeDef",
-    "SOAOutputTypeDef",
+    "SOATypeDef",
     "GetInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
     "GetInstancesHealthStatusRequestRequestTypeDef",
     "GetNamespaceRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "OperationTypeDef",
     "GetServiceRequestRequestTypeDef",
-    "HealthCheckConfigOutputTypeDef",
-    "HealthCheckCustomConfigOutputTypeDef",
     "HttpNamespaceChangeTypeDef",
     "HttpPropertiesTypeDef",
     "InstanceSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "NamespaceFilterTypeDef",
     "OperationFilterTypeDef",
     "OperationSummaryTypeDef",
     "ServiceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "SOAChangeTypeDef",
-    "SOATypeDef",
     "RegisterInstanceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateInstanceCustomHealthStatusRequestRequestTypeDef",
     "CreateHttpNamespaceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateHttpNamespaceResponseTypeDef",
     "CreatePrivateDnsNamespaceResponseTypeDef",
     "CreatePublicDnsNamespaceResponseTypeDef",
     "DeleteNamespaceResponseTypeDef",
     "DeregisterInstanceResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetInstancesHealthStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RegisterInstanceResponseTypeDef",
     "UpdateHttpNamespaceResponseTypeDef",
     "UpdatePrivateDnsNamespaceResponseTypeDef",
     "UpdatePublicDnsNamespaceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
     "DiscoverInstancesResponseTypeDef",
     "DnsConfigChangeTypeDef",
-    "DnsConfigTypeDef",
     "DnsConfigOutputTypeDef",
+    "DnsConfigTypeDef",
     "DnsPropertiesTypeDef",
+    "PrivateDnsPropertiesMutableTypeDef",
+    "PublicDnsPropertiesMutableTypeDef",
     "GetInstanceResponseTypeDef",
     "GetOperationResponseTypeDef",
     "UpdateHttpNamespaceRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
     "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PrivateDnsPropertiesMutableChangeTypeDef",
     "PublicDnsPropertiesMutableChangeTypeDef",
-    "PrivateDnsPropertiesMutableTypeDef",
-    "PublicDnsPropertiesMutableTypeDef",
     "ServiceChangeTypeDef",
-    "CreateServiceRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ServiceTypeDef",
+    "CreateServiceRequestRequestTypeDef",
     "NamespacePropertiesTypeDef",
-    "PrivateDnsNamespacePropertiesChangeTypeDef",
-    "PublicDnsNamespacePropertiesChangeTypeDef",
     "PrivateDnsNamespacePropertiesTypeDef",
     "PublicDnsNamespacePropertiesTypeDef",
+    "PrivateDnsNamespacePropertiesChangeTypeDef",
+    "PublicDnsNamespacePropertiesChangeTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "ListServicesResponseTypeDef",
     "CreateServiceResponseTypeDef",
     "GetServiceResponseTypeDef",
     "NamespaceSummaryTypeDef",
     "NamespaceTypeDef",
-    "PrivateDnsNamespaceChangeTypeDef",
-    "PublicDnsNamespaceChangeTypeDef",
     "CreatePrivateDnsNamespaceRequestRequestTypeDef",
     "CreatePublicDnsNamespaceRequestRequestTypeDef",
+    "PrivateDnsNamespaceChangeTypeDef",
+    "PublicDnsNamespaceChangeTypeDef",
     "ListNamespacesResponseTypeDef",
     "GetNamespaceResponseTypeDef",
     "UpdatePrivateDnsNamespaceRequestRequestTypeDef",
     "UpdatePublicDnsNamespaceRequestRequestTypeDef",
 )
 
 TagTypeDef = TypedDict(
@@ -248,24 +243,16 @@
     "DnsRecordTypeDef",
     {
         "Type": RecordTypeType,
         "TTL": int,
     },
 )
 
-DnsRecordOutputTypeDef = TypedDict(
-    "DnsRecordOutputTypeDef",
-    {
-        "Type": RecordTypeType,
-        "TTL": int,
-    },
-)
-
-SOAOutputTypeDef = TypedDict(
-    "SOAOutputTypeDef",
+SOATypeDef = TypedDict(
+    "SOATypeDef",
     {
         "TTL": int,
     },
 )
 
 GetInstanceRequestRequestTypeDef = TypedDict(
     "GetInstanceRequestRequestTypeDef",
@@ -347,42 +334,14 @@
 GetServiceRequestRequestTypeDef = TypedDict(
     "GetServiceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-_RequiredHealthCheckConfigOutputTypeDef = TypedDict(
-    "_RequiredHealthCheckConfigOutputTypeDef",
-    {
-        "Type": HealthCheckTypeType,
-    },
-)
-_OptionalHealthCheckConfigOutputTypeDef = TypedDict(
-    "_OptionalHealthCheckConfigOutputTypeDef",
-    {
-        "ResourcePath": str,
-        "FailureThreshold": int,
-    },
-    total=False,
-)
-
-class HealthCheckConfigOutputTypeDef(
-    _RequiredHealthCheckConfigOutputTypeDef, _OptionalHealthCheckConfigOutputTypeDef
-):
-    pass
-
-HealthCheckCustomConfigOutputTypeDef = TypedDict(
-    "HealthCheckCustomConfigOutputTypeDef",
-    {
-        "FailureThreshold": int,
-    },
-    total=False,
-)
-
 HttpNamespaceChangeTypeDef = TypedDict(
     "HttpNamespaceChangeTypeDef",
     {
         "Description": str,
     },
 )
 
@@ -499,36 +458,21 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 SOAChangeTypeDef = TypedDict(
     "SOAChangeTypeDef",
     {
         "TTL": int,
     },
 )
 
-SOATypeDef = TypedDict(
-    "SOATypeDef",
-    {
-        "TTL": int,
-    },
-)
-
 _RequiredRegisterInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterInstanceRequestRequestTypeDef",
     {
         "ServiceId": str,
         "InstanceId": str,
         "Attributes": Mapping[str, str],
     },
@@ -645,14 +589,22 @@
     {
         "Status": Dict[str, HealthStatusType],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RegisterInstanceResponseTypeDef = TypedDict(
     "RegisterInstanceResponseTypeDef",
     {
         "OperationId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -700,59 +652,73 @@
 DnsConfigChangeTypeDef = TypedDict(
     "DnsConfigChangeTypeDef",
     {
         "DnsRecords": Sequence[DnsRecordTypeDef],
     },
 )
 
-_RequiredDnsConfigTypeDef = TypedDict(
-    "_RequiredDnsConfigTypeDef",
+_RequiredDnsConfigOutputTypeDef = TypedDict(
+    "_RequiredDnsConfigOutputTypeDef",
     {
-        "DnsRecords": Sequence[DnsRecordTypeDef],
+        "DnsRecords": List[DnsRecordTypeDef],
     },
 )
-_OptionalDnsConfigTypeDef = TypedDict(
-    "_OptionalDnsConfigTypeDef",
+_OptionalDnsConfigOutputTypeDef = TypedDict(
+    "_OptionalDnsConfigOutputTypeDef",
     {
         "NamespaceId": str,
         "RoutingPolicy": RoutingPolicyType,
     },
     total=False,
 )
 
-class DnsConfigTypeDef(_RequiredDnsConfigTypeDef, _OptionalDnsConfigTypeDef):
+class DnsConfigOutputTypeDef(_RequiredDnsConfigOutputTypeDef, _OptionalDnsConfigOutputTypeDef):
     pass
 
-_RequiredDnsConfigOutputTypeDef = TypedDict(
-    "_RequiredDnsConfigOutputTypeDef",
+_RequiredDnsConfigTypeDef = TypedDict(
+    "_RequiredDnsConfigTypeDef",
     {
-        "DnsRecords": List[DnsRecordOutputTypeDef],
+        "DnsRecords": Sequence[DnsRecordTypeDef],
     },
 )
-_OptionalDnsConfigOutputTypeDef = TypedDict(
-    "_OptionalDnsConfigOutputTypeDef",
+_OptionalDnsConfigTypeDef = TypedDict(
+    "_OptionalDnsConfigTypeDef",
     {
         "NamespaceId": str,
         "RoutingPolicy": RoutingPolicyType,
     },
     total=False,
 )
 
-class DnsConfigOutputTypeDef(_RequiredDnsConfigOutputTypeDef, _OptionalDnsConfigOutputTypeDef):
+class DnsConfigTypeDef(_RequiredDnsConfigTypeDef, _OptionalDnsConfigTypeDef):
     pass
 
 DnsPropertiesTypeDef = TypedDict(
     "DnsPropertiesTypeDef",
     {
         "HostedZoneId": str,
-        "SOA": SOAOutputTypeDef,
+        "SOA": SOATypeDef,
     },
     total=False,
 )
 
+PrivateDnsPropertiesMutableTypeDef = TypedDict(
+    "PrivateDnsPropertiesMutableTypeDef",
+    {
+        "SOA": SOATypeDef,
+    },
+)
+
+PublicDnsPropertiesMutableTypeDef = TypedDict(
+    "PublicDnsPropertiesMutableTypeDef",
+    {
+        "SOA": SOATypeDef,
+    },
+)
+
 GetInstanceResponseTypeDef = TypedDict(
     "GetInstanceResponseTypeDef",
     {
         "Instance": InstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -877,56 +843,70 @@
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[ServiceFilterTypeDef],
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PrivateDnsPropertiesMutableChangeTypeDef = TypedDict(
     "PrivateDnsPropertiesMutableChangeTypeDef",
     {
         "SOA": SOAChangeTypeDef,
     },
 )
 
 PublicDnsPropertiesMutableChangeTypeDef = TypedDict(
     "PublicDnsPropertiesMutableChangeTypeDef",
     {
         "SOA": SOAChangeTypeDef,
     },
 )
 
-PrivateDnsPropertiesMutableTypeDef = TypedDict(
-    "PrivateDnsPropertiesMutableTypeDef",
+ServiceChangeTypeDef = TypedDict(
+    "ServiceChangeTypeDef",
     {
-        "SOA": SOATypeDef,
+        "Description": str,
+        "DnsConfig": DnsConfigChangeTypeDef,
+        "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
+    total=False,
 )
 
-PublicDnsPropertiesMutableTypeDef = TypedDict(
-    "PublicDnsPropertiesMutableTypeDef",
+ServiceSummaryTypeDef = TypedDict(
+    "ServiceSummaryTypeDef",
     {
-        "SOA": SOATypeDef,
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Type": ServiceTypeType,
+        "Description": str,
+        "InstanceCount": int,
+        "DnsConfig": DnsConfigOutputTypeDef,
+        "HealthCheckConfig": HealthCheckConfigTypeDef,
+        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
+        "CreateDate": datetime,
     },
+    total=False,
 )
 
-ServiceChangeTypeDef = TypedDict(
-    "ServiceChangeTypeDef",
+ServiceTypeDef = TypedDict(
+    "ServiceTypeDef",
     {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "NamespaceId": str,
         "Description": str,
-        "DnsConfig": DnsConfigChangeTypeDef,
+        "InstanceCount": int,
+        "DnsConfig": DnsConfigOutputTypeDef,
+        "Type": ServiceTypeType,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
+        "HealthCheckCustomConfig": HealthCheckCustomConfigTypeDef,
+        "CreateDate": datetime,
+        "CreatorRequestId": str,
     },
     total=False,
 )
 
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
@@ -949,57 +929,35 @@
 )
 
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
-ServiceSummaryTypeDef = TypedDict(
-    "ServiceSummaryTypeDef",
+NamespacePropertiesTypeDef = TypedDict(
+    "NamespacePropertiesTypeDef",
     {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Type": ServiceTypeType,
-        "Description": str,
-        "InstanceCount": int,
-        "DnsConfig": DnsConfigOutputTypeDef,
-        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
-        "HealthCheckCustomConfig": HealthCheckCustomConfigOutputTypeDef,
-        "CreateDate": datetime,
+        "DnsProperties": DnsPropertiesTypeDef,
+        "HttpProperties": HttpPropertiesTypeDef,
     },
     total=False,
 )
 
-ServiceTypeDef = TypedDict(
-    "ServiceTypeDef",
+PrivateDnsNamespacePropertiesTypeDef = TypedDict(
+    "PrivateDnsNamespacePropertiesTypeDef",
     {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "NamespaceId": str,
-        "Description": str,
-        "InstanceCount": int,
-        "DnsConfig": DnsConfigOutputTypeDef,
-        "Type": ServiceTypeType,
-        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
-        "HealthCheckCustomConfig": HealthCheckCustomConfigOutputTypeDef,
-        "CreateDate": datetime,
-        "CreatorRequestId": str,
+        "DnsProperties": PrivateDnsPropertiesMutableTypeDef,
     },
-    total=False,
 )
 
-NamespacePropertiesTypeDef = TypedDict(
-    "NamespacePropertiesTypeDef",
+PublicDnsNamespacePropertiesTypeDef = TypedDict(
+    "PublicDnsNamespacePropertiesTypeDef",
     {
-        "DnsProperties": DnsPropertiesTypeDef,
-        "HttpProperties": HttpPropertiesTypeDef,
+        "DnsProperties": PublicDnsPropertiesMutableTypeDef,
     },
-    total=False,
 )
 
 PrivateDnsNamespacePropertiesChangeTypeDef = TypedDict(
     "PrivateDnsNamespacePropertiesChangeTypeDef",
     {
         "DnsProperties": PrivateDnsPropertiesMutableChangeTypeDef,
     },
@@ -1008,28 +966,14 @@
 PublicDnsNamespacePropertiesChangeTypeDef = TypedDict(
     "PublicDnsNamespacePropertiesChangeTypeDef",
     {
         "DnsProperties": PublicDnsPropertiesMutableChangeTypeDef,
     },
 )
 
-PrivateDnsNamespacePropertiesTypeDef = TypedDict(
-    "PrivateDnsNamespacePropertiesTypeDef",
-    {
-        "DnsProperties": PrivateDnsPropertiesMutableTypeDef,
-    },
-)
-
-PublicDnsNamespacePropertiesTypeDef = TypedDict(
-    "PublicDnsNamespacePropertiesTypeDef",
-    {
-        "DnsProperties": PublicDnsPropertiesMutableTypeDef,
-    },
-)
-
 UpdateServiceRequestRequestTypeDef = TypedDict(
     "UpdateServiceRequestRequestTypeDef",
     {
         "Id": str,
         "Service": ServiceChangeTypeDef,
     },
 )
@@ -1086,32 +1030,14 @@
         "Properties": NamespacePropertiesTypeDef,
         "CreateDate": datetime,
         "CreatorRequestId": str,
     },
     total=False,
 )
 
-PrivateDnsNamespaceChangeTypeDef = TypedDict(
-    "PrivateDnsNamespaceChangeTypeDef",
-    {
-        "Description": str,
-        "Properties": PrivateDnsNamespacePropertiesChangeTypeDef,
-    },
-    total=False,
-)
-
-PublicDnsNamespaceChangeTypeDef = TypedDict(
-    "PublicDnsNamespaceChangeTypeDef",
-    {
-        "Description": str,
-        "Properties": PublicDnsNamespacePropertiesChangeTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreatePrivateDnsNamespaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePrivateDnsNamespaceRequestRequestTypeDef",
     {
         "Name": str,
         "Vpc": str,
     },
 )
@@ -1151,14 +1077,32 @@
 
 class CreatePublicDnsNamespaceRequestRequestTypeDef(
     _RequiredCreatePublicDnsNamespaceRequestRequestTypeDef,
     _OptionalCreatePublicDnsNamespaceRequestRequestTypeDef,
 ):
     pass
 
+PrivateDnsNamespaceChangeTypeDef = TypedDict(
+    "PrivateDnsNamespaceChangeTypeDef",
+    {
+        "Description": str,
+        "Properties": PrivateDnsNamespacePropertiesChangeTypeDef,
+    },
+    total=False,
+)
+
+PublicDnsNamespaceChangeTypeDef = TypedDict(
+    "PublicDnsNamespaceChangeTypeDef",
+    {
+        "Description": str,
+        "Properties": PublicDnsNamespacePropertiesChangeTypeDef,
+    },
+    total=False,
+)
+
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "Namespaces": List[NamespaceSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/PKG-INFO` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicediscovery
-Version: 1.28.12
-Summary: Type annotations for boto3.ServiceDiscovery 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ServiceDiscovery 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicediscovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicediscovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicediscovery)](https://pepy.tech/project/mypy-boto3-servicediscovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceDiscovery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
+[boto3.ServiceDiscovery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#ServiceDiscovery)
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
 [mypy-boto3-servicediscovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicediscovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,96 +357,91 @@
     HealthCheckCustomConfigTypeDef,
     DeleteNamespaceRequestRequestTypeDef,
     DeleteServiceRequestRequestTypeDef,
     DeregisterInstanceRequestRequestTypeDef,
     DiscoverInstancesRequestRequestTypeDef,
     HttpInstanceSummaryTypeDef,
     DnsRecordTypeDef,
-    DnsRecordOutputTypeDef,
-    SOAOutputTypeDef,
+    SOATypeDef,
     GetInstanceRequestRequestTypeDef,
     InstanceTypeDef,
     GetInstancesHealthStatusRequestRequestTypeDef,
     GetNamespaceRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     OperationTypeDef,
     GetServiceRequestRequestTypeDef,
-    HealthCheckConfigOutputTypeDef,
-    HealthCheckCustomConfigOutputTypeDef,
     HttpNamespaceChangeTypeDef,
     HttpPropertiesTypeDef,
     InstanceSummaryTypeDef,
     PaginatorConfigTypeDef,
     ListInstancesRequestRequestTypeDef,
     NamespaceFilterTypeDef,
     OperationFilterTypeDef,
     OperationSummaryTypeDef,
     ServiceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     SOAChangeTypeDef,
-    SOATypeDef,
     RegisterInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateInstanceCustomHealthStatusRequestRequestTypeDef,
     CreateHttpNamespaceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateHttpNamespaceResponseTypeDef,
     CreatePrivateDnsNamespaceResponseTypeDef,
     CreatePublicDnsNamespaceResponseTypeDef,
     DeleteNamespaceResponseTypeDef,
     DeregisterInstanceResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetInstancesHealthStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RegisterInstanceResponseTypeDef,
     UpdateHttpNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceResponseTypeDef,
     UpdatePublicDnsNamespaceResponseTypeDef,
     UpdateServiceResponseTypeDef,
     DiscoverInstancesResponseTypeDef,
     DnsConfigChangeTypeDef,
-    DnsConfigTypeDef,
     DnsConfigOutputTypeDef,
+    DnsConfigTypeDef,
     DnsPropertiesTypeDef,
+    PrivateDnsPropertiesMutableTypeDef,
+    PublicDnsPropertiesMutableTypeDef,
     GetInstanceResponseTypeDef,
     GetOperationResponseTypeDef,
     UpdateHttpNamespaceRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListOperationsRequestListOperationsPaginateTypeDef,
     ListOperationsRequestRequestTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PrivateDnsPropertiesMutableChangeTypeDef,
     PublicDnsPropertiesMutableChangeTypeDef,
-    PrivateDnsPropertiesMutableTypeDef,
-    PublicDnsPropertiesMutableTypeDef,
     ServiceChangeTypeDef,
-    CreateServiceRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ServiceTypeDef,
+    CreateServiceRequestRequestTypeDef,
     NamespacePropertiesTypeDef,
-    PrivateDnsNamespacePropertiesChangeTypeDef,
-    PublicDnsNamespacePropertiesChangeTypeDef,
     PrivateDnsNamespacePropertiesTypeDef,
     PublicDnsNamespacePropertiesTypeDef,
+    PrivateDnsNamespacePropertiesChangeTypeDef,
+    PublicDnsNamespacePropertiesChangeTypeDef,
     UpdateServiceRequestRequestTypeDef,
     ListServicesResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceResponseTypeDef,
     NamespaceSummaryTypeDef,
     NamespaceTypeDef,
-    PrivateDnsNamespaceChangeTypeDef,
-    PublicDnsNamespaceChangeTypeDef,
     CreatePrivateDnsNamespaceRequestRequestTypeDef,
     CreatePublicDnsNamespaceRequestRequestTypeDef,
+    PrivateDnsNamespaceChangeTypeDef,
+    PublicDnsNamespaceChangeTypeDef,
     ListNamespacesResponseTypeDef,
     GetNamespaceResponseTypeDef,
     UpdatePrivateDnsNamespaceRequestRequestTypeDef,
     UpdatePublicDnsNamespaceRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-servicediscovery-1.28.12/mypy_boto3_servicediscovery.egg-info/SOURCES.txt` & `mypy-boto3-servicediscovery-1.28.15/mypy_boto3_servicediscovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicediscovery-1.28.12/setup.py` & `mypy-boto3-servicediscovery-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-servicediscovery",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_servicediscovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServiceDiscovery 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ServiceDiscovery 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

