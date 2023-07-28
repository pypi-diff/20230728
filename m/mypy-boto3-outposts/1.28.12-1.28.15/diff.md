# Comparing `tmp/mypy-boto3-outposts-1.28.12.tar.gz` & `tmp/mypy-boto3-outposts-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-outposts-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
+gzip compressed data, was "mypy-boto3-outposts-1.28.15.tar", last modified: Fri Jul 28 20:43:25 2023, max compression
```

## Comparing `mypy-boto3-outposts-1.28.12.tar` & `mypy-boto3-outposts-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.817133 mypy-boto3-outposts-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-07-27 11:49:21.817133 mypy-boto3-outposts-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.805132 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21419 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21380 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25858 2023-07-27 11:41:10.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25833 2023-07-27 11:41:09.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.817133 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-07-27 11:49:21.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 11:49:21.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:21.000000 mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.817133 mypy-boto3-outposts-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:41:08.000000 mypy-boto3-outposts-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:25.101609 mypy-boto3-outposts-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:07.000000 mypy-boto3-outposts-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16327 2023-07-28 20:43:25.093609 mypy-boto3-outposts-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-07-28 20:33:07.000000 mypy-boto3-outposts-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:25.093609 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-28 20:33:07.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-28 20:33:07.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:33:07.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21419 2023-07-28 20:33:08.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21380 2023-07-28 20:33:07.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-07-28 20:33:08.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-07-28 20:33:08.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-28 20:33:08.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-07-28 20:33:08.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:07.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24584 2023-07-28 20:33:09.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24561 2023-07-28 20:33:08.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:07.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:25.093609 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16327 2023-07-28 20:43:24.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:43:24.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:24.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:24.000000 mypy-boto3-outposts-1.28.15/mypy_boto3_outposts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:25.101609 mypy-boto3-outposts-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:33:07.000000 mypy-boto3-outposts-1.28.15/setup.py
```

### Comparing `mypy-boto3-outposts-1.28.12/LICENSE` & `mypy-boto3-outposts-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.12/PKG-INFO` & `mypy-boto3-outposts-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-outposts
-Version: 1.28.12
-Summary: Type annotations for boto3.Outposts 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Outposts 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-outposts)](https://pepy.tech/project/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [mypy-boto3-outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,15 +360,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_outposts.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_outposts.type_defs import (
-    AddressOutputTypeDef,
     AddressTypeDef,
     AssetLocationTypeDef,
     ComputeAttributesTypeDef,
     CancelOrderInputRequestTypeDef,
     EC2CapacityTypeDef,
     ConnectionDetailsTypeDef,
     LineItemRequestTypeDef,
@@ -392,15 +391,14 @@
     ListAssetsInputRequestTypeDef,
     ListCatalogItemsInputRequestTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
     ListOutpostsInputRequestTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RackPhysicalPropertiesOutputTypeDef,
     StartConnectionRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
     UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     UpdateSiteAddressInputRequestTypeDef,
@@ -413,39 +411,39 @@
     StartConnectionResponseTypeDef,
     UpdateSiteAddressOutputTypeDef,
     CreateOutpostOutputTypeDef,
     GetOutpostOutputTypeDef,
     ListOutpostsOutputTypeDef,
     UpdateOutpostOutputTypeDef,
     CreateSiteInputRequestTypeDef,
+    SiteTypeDef,
     GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
     ListAssetsInputListAssetsPaginateTypeDef,
     ListCatalogItemsInputListCatalogItemsPaginateTypeDef,
     ListOrdersInputListOrdersPaginateTypeDef,
     ListOutpostsInputListOutpostsPaginateTypeDef,
     ListSitesInputListSitesPaginateTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
     LineItemTypeDef,
     ListOrdersOutputTypeDef,
-    SiteTypeDef,
     ListAssetsOutputTypeDef,
     GetCatalogItemOutputTypeDef,
     ListCatalogItemsOutputTypeDef,
-    OrderTypeDef,
     CreateSiteOutputTypeDef,
     GetSiteOutputTypeDef,
     ListSitesOutputTypeDef,
     UpdateSiteOutputTypeDef,
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
+    OrderTypeDef,
     CreateOrderOutputTypeDef,
     GetOrderOutputTypeDef,
 )
 
 
-def get_structure() -> AddressOutputTypeDef:
+def get_structure() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-outposts-1.28.12/README.md` & `mypy-boto3-outposts-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-outposts)](https://pepy.tech/project/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [mypy-boto3-outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,15 +328,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_outposts.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_outposts.type_defs import (
-    AddressOutputTypeDef,
     AddressTypeDef,
     AssetLocationTypeDef,
     ComputeAttributesTypeDef,
     CancelOrderInputRequestTypeDef,
     EC2CapacityTypeDef,
     ConnectionDetailsTypeDef,
     LineItemRequestTypeDef,
@@ -360,15 +359,14 @@
     ListAssetsInputRequestTypeDef,
     ListCatalogItemsInputRequestTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
     ListOutpostsInputRequestTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RackPhysicalPropertiesOutputTypeDef,
     StartConnectionRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
     UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     UpdateSiteAddressInputRequestTypeDef,
@@ -381,39 +379,39 @@
     StartConnectionResponseTypeDef,
     UpdateSiteAddressOutputTypeDef,
     CreateOutpostOutputTypeDef,
     GetOutpostOutputTypeDef,
     ListOutpostsOutputTypeDef,
     UpdateOutpostOutputTypeDef,
     CreateSiteInputRequestTypeDef,
+    SiteTypeDef,
     GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
     ListAssetsInputListAssetsPaginateTypeDef,
     ListCatalogItemsInputListCatalogItemsPaginateTypeDef,
     ListOrdersInputListOrdersPaginateTypeDef,
     ListOutpostsInputListOutpostsPaginateTypeDef,
     ListSitesInputListSitesPaginateTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
     LineItemTypeDef,
     ListOrdersOutputTypeDef,
-    SiteTypeDef,
     ListAssetsOutputTypeDef,
     GetCatalogItemOutputTypeDef,
     ListCatalogItemsOutputTypeDef,
-    OrderTypeDef,
     CreateSiteOutputTypeDef,
     GetSiteOutputTypeDef,
     ListSitesOutputTypeDef,
     UpdateSiteOutputTypeDef,
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
+    OrderTypeDef,
     CreateOrderOutputTypeDef,
     GetOrderOutputTypeDef,
 )
 
 
-def get_structure() -> AddressOutputTypeDef:
+def get_structure() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/__init__.py` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/__init__.pyi` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/__main__.py` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Outposts 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Outposts 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts\nOther"
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

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/client.py` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/client.pyi` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/literals.py` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/literals.pyi` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/paginator.py` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/paginator.pyi` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/type_defs.py` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for outposts service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_outposts.type_defs import AddressOutputTypeDef
+    from mypy_boto3_outposts.type_defs import AddressTypeDef
 
-    data: AddressOutputTypeDef = {...}
+    data: AddressTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -45,17 +45,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "AddressOutputTypeDef",
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
     "CancelOrderInputRequestTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
     "LineItemRequestTypeDef",
@@ -79,15 +77,14 @@
     "ListAssetsInputRequestTypeDef",
     "ListCatalogItemsInputRequestTypeDef",
     "ListOrdersInputRequestTypeDef",
     "OrderSummaryTypeDef",
     "ListOutpostsInputRequestTypeDef",
     "ListSitesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "RackPhysicalPropertiesOutputTypeDef",
     "StartConnectionRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateOutpostInputRequestTypeDef",
     "UpdateSiteInputRequestTypeDef",
     "UpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
     "UpdateSiteAddressInputRequestTypeDef",
@@ -100,65 +97,37 @@
     "StartConnectionResponseTypeDef",
     "UpdateSiteAddressOutputTypeDef",
     "CreateOutpostOutputTypeDef",
     "GetOutpostOutputTypeDef",
     "ListOutpostsOutputTypeDef",
     "UpdateOutpostOutputTypeDef",
     "CreateSiteInputRequestTypeDef",
+    "SiteTypeDef",
     "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
     "ListAssetsInputListAssetsPaginateTypeDef",
     "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
     "ListOrdersInputListOrdersPaginateTypeDef",
     "ListOutpostsInputListOutpostsPaginateTypeDef",
     "ListSitesInputListSitesPaginateTypeDef",
     "GetOutpostInstanceTypesOutputTypeDef",
     "LineItemTypeDef",
     "ListOrdersOutputTypeDef",
-    "SiteTypeDef",
     "ListAssetsOutputTypeDef",
     "GetCatalogItemOutputTypeDef",
     "ListCatalogItemsOutputTypeDef",
-    "OrderTypeDef",
     "CreateSiteOutputTypeDef",
     "GetSiteOutputTypeDef",
     "ListSitesOutputTypeDef",
     "UpdateSiteOutputTypeDef",
     "UpdateSiteRackPhysicalPropertiesOutputTypeDef",
+    "OrderTypeDef",
     "CreateOrderOutputTypeDef",
     "GetOrderOutputTypeDef",
 )
 
-_RequiredAddressOutputTypeDef = TypedDict(
-    "_RequiredAddressOutputTypeDef",
-    {
-        "AddressLine1": str,
-        "City": str,
-        "StateOrRegion": str,
-        "PostalCode": str,
-        "CountryCode": str,
-    },
-)
-_OptionalAddressOutputTypeDef = TypedDict(
-    "_OptionalAddressOutputTypeDef",
-    {
-        "ContactName": str,
-        "ContactPhoneNumber": str,
-        "AddressLine2": str,
-        "AddressLine3": str,
-        "DistrictOrCounty": str,
-        "Municipality": str,
-    },
-    total=False,
-)
-
-
-class AddressOutputTypeDef(_RequiredAddressOutputTypeDef, _OptionalAddressOutputTypeDef):
-    pass
-
-
 _RequiredAddressTypeDef = TypedDict(
     "_RequiredAddressTypeDef",
     {
         "AddressLine1": str,
         "City": str,
         "StateOrRegion": str,
         "PostalCode": str,
@@ -174,19 +143,17 @@
         "AddressLine3": str,
         "DistrictOrCounty": str,
         "Municipality": str,
     },
     total=False,
 )
 
-
 class AddressTypeDef(_RequiredAddressTypeDef, _OptionalAddressTypeDef):
     pass
 
-
 AssetLocationTypeDef = TypedDict(
     "AssetLocationTypeDef",
     {
         "RackElevation": float,
     },
     total=False,
 )
@@ -265,21 +232,19 @@
         "AvailabilityZoneId": str,
         "Tags": Mapping[str, str],
         "SupportedHardwareType": SupportedHardwareTypeType,
     },
     total=False,
 )
 
-
 class CreateOutpostInputRequestTypeDef(
     _RequiredCreateOutpostInputRequestTypeDef, _OptionalCreateOutpostInputRequestTypeDef
 ):
     pass
 
-
 OutpostTypeDef = TypedDict(
     "OutpostTypeDef",
     {
         "OutpostId": str,
         "OwnerId": str,
         "OutpostArn": str,
         "SiteId": str,
@@ -374,22 +339,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetOutpostInstanceTypesInputRequestTypeDef(
     _RequiredGetOutpostInstanceTypesInputRequestTypeDef,
     _OptionalGetOutpostInstanceTypesInputRequestTypeDef,
 ):
     pass
 
-
 InstanceTypeItemTypeDef = TypedDict(
     "InstanceTypeItemTypeDef",
     {
         "InstanceType": str,
     },
     total=False,
 )
@@ -440,21 +403,19 @@
         "MaxResults": int,
         "NextToken": str,
         "StatusFilter": Sequence[AssetStateType],
     },
     total=False,
 )
 
-
 class ListAssetsInputRequestTypeDef(
     _RequiredListAssetsInputRequestTypeDef, _OptionalListAssetsInputRequestTypeDef
 ):
     pass
 
-
 ListCatalogItemsInputRequestTypeDef = TypedDict(
     "ListCatalogItemsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ItemClassFilter": Sequence[CatalogItemClassType],
         "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
@@ -514,30 +475,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-RackPhysicalPropertiesOutputTypeDef = TypedDict(
-    "RackPhysicalPropertiesOutputTypeDef",
-    {
-        "PowerDrawKva": PowerDrawKvaType,
-        "PowerPhase": PowerPhaseType,
-        "PowerConnector": PowerConnectorType,
-        "PowerFeedDrop": PowerFeedDropType,
-        "UplinkGbps": UplinkGbpsType,
-        "UplinkCount": UplinkCountType,
-        "FiberOpticCableType": FiberOpticCableTypeType,
-        "OpticalStandard": OpticalStandardType,
-        "MaximumSupportedWeightLbs": MaximumSupportedWeightLbsType,
-    },
-    total=False,
-)
-
 StartConnectionRequestRequestTypeDef = TypedDict(
     "StartConnectionRequestRequestTypeDef",
     {
         "DeviceSerialNumber": str,
         "AssetId": str,
         "ClientPublicKey": str,
         "NetworkInterfaceDeviceIndex": int,
@@ -572,21 +517,19 @@
         "Name": str,
         "Description": str,
         "SupportedHardwareType": SupportedHardwareTypeType,
     },
     total=False,
 )
 
-
 class UpdateOutpostInputRequestTypeDef(
     _RequiredUpdateOutpostInputRequestTypeDef, _OptionalUpdateOutpostInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSiteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
 _OptionalUpdateSiteInputRequestTypeDef = TypedDict(
@@ -595,21 +538,19 @@
         "Name": str,
         "Description": str,
         "Notes": str,
     },
     total=False,
 )
 
-
 class UpdateSiteInputRequestTypeDef(
     _RequiredUpdateSiteInputRequestTypeDef, _OptionalUpdateSiteInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
 _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef = TypedDict(
@@ -624,22 +565,20 @@
         "FiberOpticCableType": FiberOpticCableTypeType,
         "OpticalStandard": OpticalStandardType,
         "MaximumSupportedWeightLbs": MaximumSupportedWeightLbsType,
     },
     total=False,
 )
 
-
 class UpdateSiteRackPhysicalPropertiesInputRequestTypeDef(
     _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
 ):
     pass
 
-
 UpdateSiteAddressInputRequestTypeDef = TypedDict(
     "UpdateSiteAddressInputRequestTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
         "Address": AddressTypeDef,
     },
@@ -683,36 +622,34 @@
     "_OptionalCreateOrderInputRequestTypeDef",
     {
         "PaymentTerm": PaymentTermType,
     },
     total=False,
 )
 
-
 class CreateOrderInputRequestTypeDef(
     _RequiredCreateOrderInputRequestTypeDef, _OptionalCreateOrderInputRequestTypeDef
 ):
     pass
 
-
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "ConnectionId": str,
         "ConnectionDetails": ConnectionDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSiteAddressOutputTypeDef = TypedDict(
     "GetSiteAddressOutputTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
-        "Address": AddressOutputTypeDef,
+        "Address": AddressTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
@@ -730,15 +667,15 @@
     },
 )
 
 UpdateSiteAddressOutputTypeDef = TypedDict(
     "UpdateSiteAddressOutputTypeDef",
     {
         "AddressType": AddressTypeType,
-        "Address": AddressOutputTypeDef,
+        "Address": AddressTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateOutpostOutputTypeDef = TypedDict(
     "CreateOutpostOutputTypeDef",
     {
@@ -787,20 +724,36 @@
         "OperatingAddress": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "RackPhysicalProperties": RackPhysicalPropertiesTypeDef,
     },
     total=False,
 )
 
-
 class CreateSiteInputRequestTypeDef(
     _RequiredCreateSiteInputRequestTypeDef, _OptionalCreateSiteInputRequestTypeDef
 ):
     pass
 
+SiteTypeDef = TypedDict(
+    "SiteTypeDef",
+    {
+        "SiteId": str,
+        "AccountId": str,
+        "Name": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "SiteArn": str,
+        "Notes": str,
+        "OperatingAddressCountryCode": str,
+        "OperatingAddressStateOrRegion": str,
+        "OperatingAddressCity": str,
+        "RackPhysicalProperties": RackPhysicalPropertiesTypeDef,
+    },
+    total=False,
+)
 
 _RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
     "_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
     {
         "OutpostId": str,
     },
 )
@@ -808,22 +761,20 @@
     "_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef(
     _RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
     _OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAssetsInputListAssetsPaginateTypeDef = TypedDict(
     "_RequiredListAssetsInputListAssetsPaginateTypeDef",
     {
         "OutpostIdentifier": str,
     },
 )
 _OptionalListAssetsInputListAssetsPaginateTypeDef = TypedDict(
@@ -832,22 +783,20 @@
         "HostIdFilter": Sequence[str],
         "StatusFilter": Sequence[AssetStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAssetsInputListAssetsPaginateTypeDef(
     _RequiredListAssetsInputListAssetsPaginateTypeDef,
     _OptionalListAssetsInputListAssetsPaginateTypeDef,
 ):
     pass
 
-
 ListCatalogItemsInputListCatalogItemsPaginateTypeDef = TypedDict(
     "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
     {
         "ItemClassFilter": Sequence[CatalogItemClassType],
         "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
         "EC2FamilyFilter": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -917,32 +866,14 @@
     {
         "Orders": List[OrderSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SiteTypeDef = TypedDict(
-    "SiteTypeDef",
-    {
-        "SiteId": str,
-        "AccountId": str,
-        "Name": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "SiteArn": str,
-        "Notes": str,
-        "OperatingAddressCountryCode": str,
-        "OperatingAddressStateOrRegion": str,
-        "OperatingAddressCity": str,
-        "RackPhysicalProperties": RackPhysicalPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 ListAssetsOutputTypeDef = TypedDict(
     "ListAssetsOutputTypeDef",
     {
         "Assets": List[AssetInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -961,30 +892,14 @@
     {
         "CatalogItems": List[CatalogItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OrderTypeDef = TypedDict(
-    "OrderTypeDef",
-    {
-        "OutpostId": str,
-        "OrderId": str,
-        "Status": OrderStatusType,
-        "LineItems": List[LineItemTypeDef],
-        "PaymentOption": PaymentOptionType,
-        "OrderSubmissionDate": datetime,
-        "OrderFulfilledDate": datetime,
-        "PaymentTerm": PaymentTermType,
-        "OrderType": OrderTypeType,
-    },
-    total=False,
-)
-
 CreateSiteOutputTypeDef = TypedDict(
     "CreateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1018,14 +933,30 @@
     "UpdateSiteRackPhysicalPropertiesOutputTypeDef",
     {
         "Site": SiteTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OrderTypeDef = TypedDict(
+    "OrderTypeDef",
+    {
+        "OutpostId": str,
+        "OrderId": str,
+        "Status": OrderStatusType,
+        "LineItems": List[LineItemTypeDef],
+        "PaymentOption": PaymentOptionType,
+        "OrderSubmissionDate": datetime,
+        "OrderFulfilledDate": datetime,
+        "PaymentTerm": PaymentTermType,
+        "OrderType": OrderTypeType,
+    },
+    total=False,
+)
+
 CreateOrderOutputTypeDef = TypedDict(
     "CreateOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts/type_defs.pyi` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for outposts service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_outposts.type_defs import AddressOutputTypeDef
+    from mypy_boto3_outposts.type_defs import AddressTypeDef
 
-    data: AddressOutputTypeDef = {...}
+    data: AddressTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -45,16 +45,16 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "AddressOutputTypeDef",
     "AddressTypeDef",
     "AssetLocationTypeDef",
     "ComputeAttributesTypeDef",
     "CancelOrderInputRequestTypeDef",
     "EC2CapacityTypeDef",
     "ConnectionDetailsTypeDef",
     "LineItemRequestTypeDef",
@@ -78,15 +78,14 @@
     "ListAssetsInputRequestTypeDef",
     "ListCatalogItemsInputRequestTypeDef",
     "ListOrdersInputRequestTypeDef",
     "OrderSummaryTypeDef",
     "ListOutpostsInputRequestTypeDef",
     "ListSitesInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "RackPhysicalPropertiesOutputTypeDef",
     "StartConnectionRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateOutpostInputRequestTypeDef",
     "UpdateSiteInputRequestTypeDef",
     "UpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
     "UpdateSiteAddressInputRequestTypeDef",
@@ -99,63 +98,37 @@
     "StartConnectionResponseTypeDef",
     "UpdateSiteAddressOutputTypeDef",
     "CreateOutpostOutputTypeDef",
     "GetOutpostOutputTypeDef",
     "ListOutpostsOutputTypeDef",
     "UpdateOutpostOutputTypeDef",
     "CreateSiteInputRequestTypeDef",
+    "SiteTypeDef",
     "GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
     "ListAssetsInputListAssetsPaginateTypeDef",
     "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
     "ListOrdersInputListOrdersPaginateTypeDef",
     "ListOutpostsInputListOutpostsPaginateTypeDef",
     "ListSitesInputListSitesPaginateTypeDef",
     "GetOutpostInstanceTypesOutputTypeDef",
     "LineItemTypeDef",
     "ListOrdersOutputTypeDef",
-    "SiteTypeDef",
     "ListAssetsOutputTypeDef",
     "GetCatalogItemOutputTypeDef",
     "ListCatalogItemsOutputTypeDef",
-    "OrderTypeDef",
     "CreateSiteOutputTypeDef",
     "GetSiteOutputTypeDef",
     "ListSitesOutputTypeDef",
     "UpdateSiteOutputTypeDef",
     "UpdateSiteRackPhysicalPropertiesOutputTypeDef",
+    "OrderTypeDef",
     "CreateOrderOutputTypeDef",
     "GetOrderOutputTypeDef",
 )
 
-_RequiredAddressOutputTypeDef = TypedDict(
-    "_RequiredAddressOutputTypeDef",
-    {
-        "AddressLine1": str,
-        "City": str,
-        "StateOrRegion": str,
-        "PostalCode": str,
-        "CountryCode": str,
-    },
-)
-_OptionalAddressOutputTypeDef = TypedDict(
-    "_OptionalAddressOutputTypeDef",
-    {
-        "ContactName": str,
-        "ContactPhoneNumber": str,
-        "AddressLine2": str,
-        "AddressLine3": str,
-        "DistrictOrCounty": str,
-        "Municipality": str,
-    },
-    total=False,
-)
-
-class AddressOutputTypeDef(_RequiredAddressOutputTypeDef, _OptionalAddressOutputTypeDef):
-    pass
-
 _RequiredAddressTypeDef = TypedDict(
     "_RequiredAddressTypeDef",
     {
         "AddressLine1": str,
         "City": str,
         "StateOrRegion": str,
         "PostalCode": str,
@@ -171,17 +144,19 @@
         "AddressLine3": str,
         "DistrictOrCounty": str,
         "Municipality": str,
     },
     total=False,
 )
 
+
 class AddressTypeDef(_RequiredAddressTypeDef, _OptionalAddressTypeDef):
     pass
 
+
 AssetLocationTypeDef = TypedDict(
     "AssetLocationTypeDef",
     {
         "RackElevation": float,
     },
     total=False,
 )
@@ -260,19 +235,21 @@
         "AvailabilityZoneId": str,
         "Tags": Mapping[str, str],
         "SupportedHardwareType": SupportedHardwareTypeType,
     },
     total=False,
 )
 
+
 class CreateOutpostInputRequestTypeDef(
     _RequiredCreateOutpostInputRequestTypeDef, _OptionalCreateOutpostInputRequestTypeDef
 ):
     pass
 
+
 OutpostTypeDef = TypedDict(
     "OutpostTypeDef",
     {
         "OutpostId": str,
         "OwnerId": str,
         "OutpostArn": str,
         "SiteId": str,
@@ -367,20 +344,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetOutpostInstanceTypesInputRequestTypeDef(
     _RequiredGetOutpostInstanceTypesInputRequestTypeDef,
     _OptionalGetOutpostInstanceTypesInputRequestTypeDef,
 ):
     pass
 
+
 InstanceTypeItemTypeDef = TypedDict(
     "InstanceTypeItemTypeDef",
     {
         "InstanceType": str,
     },
     total=False,
 )
@@ -431,19 +410,21 @@
         "MaxResults": int,
         "NextToken": str,
         "StatusFilter": Sequence[AssetStateType],
     },
     total=False,
 )
 
+
 class ListAssetsInputRequestTypeDef(
     _RequiredListAssetsInputRequestTypeDef, _OptionalListAssetsInputRequestTypeDef
 ):
     pass
 
+
 ListCatalogItemsInputRequestTypeDef = TypedDict(
     "ListCatalogItemsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ItemClassFilter": Sequence[CatalogItemClassType],
         "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
@@ -503,30 +484,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-RackPhysicalPropertiesOutputTypeDef = TypedDict(
-    "RackPhysicalPropertiesOutputTypeDef",
-    {
-        "PowerDrawKva": PowerDrawKvaType,
-        "PowerPhase": PowerPhaseType,
-        "PowerConnector": PowerConnectorType,
-        "PowerFeedDrop": PowerFeedDropType,
-        "UplinkGbps": UplinkGbpsType,
-        "UplinkCount": UplinkCountType,
-        "FiberOpticCableType": FiberOpticCableTypeType,
-        "OpticalStandard": OpticalStandardType,
-        "MaximumSupportedWeightLbs": MaximumSupportedWeightLbsType,
-    },
-    total=False,
-)
-
 StartConnectionRequestRequestTypeDef = TypedDict(
     "StartConnectionRequestRequestTypeDef",
     {
         "DeviceSerialNumber": str,
         "AssetId": str,
         "ClientPublicKey": str,
         "NetworkInterfaceDeviceIndex": int,
@@ -561,19 +526,21 @@
         "Name": str,
         "Description": str,
         "SupportedHardwareType": SupportedHardwareTypeType,
     },
     total=False,
 )
 
+
 class UpdateOutpostInputRequestTypeDef(
     _RequiredUpdateOutpostInputRequestTypeDef, _OptionalUpdateOutpostInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSiteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
 _OptionalUpdateSiteInputRequestTypeDef = TypedDict(
@@ -582,19 +549,21 @@
         "Name": str,
         "Description": str,
         "Notes": str,
     },
     total=False,
 )
 
+
 class UpdateSiteInputRequestTypeDef(
     _RequiredUpdateSiteInputRequestTypeDef, _OptionalUpdateSiteInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef",
     {
         "SiteId": str,
     },
 )
 _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef = TypedDict(
@@ -609,20 +578,22 @@
         "FiberOpticCableType": FiberOpticCableTypeType,
         "OpticalStandard": OpticalStandardType,
         "MaximumSupportedWeightLbs": MaximumSupportedWeightLbsType,
     },
     total=False,
 )
 
+
 class UpdateSiteRackPhysicalPropertiesInputRequestTypeDef(
     _RequiredUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     _OptionalUpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
 ):
     pass
 
+
 UpdateSiteAddressInputRequestTypeDef = TypedDict(
     "UpdateSiteAddressInputRequestTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
         "Address": AddressTypeDef,
     },
@@ -666,34 +637,36 @@
     "_OptionalCreateOrderInputRequestTypeDef",
     {
         "PaymentTerm": PaymentTermType,
     },
     total=False,
 )
 
+
 class CreateOrderInputRequestTypeDef(
     _RequiredCreateOrderInputRequestTypeDef, _OptionalCreateOrderInputRequestTypeDef
 ):
     pass
 
+
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "ConnectionId": str,
         "ConnectionDetails": ConnectionDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSiteAddressOutputTypeDef = TypedDict(
     "GetSiteAddressOutputTypeDef",
     {
         "SiteId": str,
         "AddressType": AddressTypeType,
-        "Address": AddressOutputTypeDef,
+        "Address": AddressTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
@@ -711,15 +684,15 @@
     },
 )
 
 UpdateSiteAddressOutputTypeDef = TypedDict(
     "UpdateSiteAddressOutputTypeDef",
     {
         "AddressType": AddressTypeType,
-        "Address": AddressOutputTypeDef,
+        "Address": AddressTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateOutpostOutputTypeDef = TypedDict(
     "CreateOutpostOutputTypeDef",
     {
@@ -768,39 +741,61 @@
         "OperatingAddress": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "RackPhysicalProperties": RackPhysicalPropertiesTypeDef,
     },
     total=False,
 )
 
+
 class CreateSiteInputRequestTypeDef(
     _RequiredCreateSiteInputRequestTypeDef, _OptionalCreateSiteInputRequestTypeDef
 ):
     pass
 
+
+SiteTypeDef = TypedDict(
+    "SiteTypeDef",
+    {
+        "SiteId": str,
+        "AccountId": str,
+        "Name": str,
+        "Description": str,
+        "Tags": Dict[str, str],
+        "SiteArn": str,
+        "Notes": str,
+        "OperatingAddressCountryCode": str,
+        "OperatingAddressStateOrRegion": str,
+        "OperatingAddressCity": str,
+        "RackPhysicalProperties": RackPhysicalPropertiesTypeDef,
+    },
+    total=False,
+)
+
 _RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
     "_RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
     {
         "OutpostId": str,
     },
 )
 _OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef = TypedDict(
     "_OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef(
     _RequiredGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
     _OptionalGetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAssetsInputListAssetsPaginateTypeDef = TypedDict(
     "_RequiredListAssetsInputListAssetsPaginateTypeDef",
     {
         "OutpostIdentifier": str,
     },
 )
 _OptionalListAssetsInputListAssetsPaginateTypeDef = TypedDict(
@@ -809,20 +804,22 @@
         "HostIdFilter": Sequence[str],
         "StatusFilter": Sequence[AssetStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAssetsInputListAssetsPaginateTypeDef(
     _RequiredListAssetsInputListAssetsPaginateTypeDef,
     _OptionalListAssetsInputListAssetsPaginateTypeDef,
 ):
     pass
 
+
 ListCatalogItemsInputListCatalogItemsPaginateTypeDef = TypedDict(
     "ListCatalogItemsInputListCatalogItemsPaginateTypeDef",
     {
         "ItemClassFilter": Sequence[CatalogItemClassType],
         "SupportedStorageFilter": Sequence[SupportedStorageEnumType],
         "EC2FamilyFilter": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -892,32 +889,14 @@
     {
         "Orders": List[OrderSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SiteTypeDef = TypedDict(
-    "SiteTypeDef",
-    {
-        "SiteId": str,
-        "AccountId": str,
-        "Name": str,
-        "Description": str,
-        "Tags": Dict[str, str],
-        "SiteArn": str,
-        "Notes": str,
-        "OperatingAddressCountryCode": str,
-        "OperatingAddressStateOrRegion": str,
-        "OperatingAddressCity": str,
-        "RackPhysicalProperties": RackPhysicalPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 ListAssetsOutputTypeDef = TypedDict(
     "ListAssetsOutputTypeDef",
     {
         "Assets": List[AssetInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -936,30 +915,14 @@
     {
         "CatalogItems": List[CatalogItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OrderTypeDef = TypedDict(
-    "OrderTypeDef",
-    {
-        "OutpostId": str,
-        "OrderId": str,
-        "Status": OrderStatusType,
-        "LineItems": List[LineItemTypeDef],
-        "PaymentOption": PaymentOptionType,
-        "OrderSubmissionDate": datetime,
-        "OrderFulfilledDate": datetime,
-        "PaymentTerm": PaymentTermType,
-        "OrderType": OrderTypeType,
-    },
-    total=False,
-)
-
 CreateSiteOutputTypeDef = TypedDict(
     "CreateSiteOutputTypeDef",
     {
         "Site": SiteTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -993,14 +956,30 @@
     "UpdateSiteRackPhysicalPropertiesOutputTypeDef",
     {
         "Site": SiteTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OrderTypeDef = TypedDict(
+    "OrderTypeDef",
+    {
+        "OutpostId": str,
+        "OrderId": str,
+        "Status": OrderStatusType,
+        "LineItems": List[LineItemTypeDef],
+        "PaymentOption": PaymentOptionType,
+        "OrderSubmissionDate": datetime,
+        "OrderFulfilledDate": datetime,
+        "PaymentTerm": PaymentTermType,
+        "OrderType": OrderTypeType,
+    },
+    total=False,
+)
+
 CreateOrderOutputTypeDef = TypedDict(
     "CreateOrderOutputTypeDef",
     {
         "Order": OrderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/PKG-INFO` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-outposts
-Version: 1.28.12
-Summary: Type annotations for boto3.Outposts 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Outposts 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-outposts)](https://pepy.tech/project/mypy-boto3-outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Outposts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
+[boto3.Outposts 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
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
 [mypy-boto3-outposts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_outposts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -360,15 +360,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_outposts.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_outposts.type_defs import (
-    AddressOutputTypeDef,
     AddressTypeDef,
     AssetLocationTypeDef,
     ComputeAttributesTypeDef,
     CancelOrderInputRequestTypeDef,
     EC2CapacityTypeDef,
     ConnectionDetailsTypeDef,
     LineItemRequestTypeDef,
@@ -392,15 +391,14 @@
     ListAssetsInputRequestTypeDef,
     ListCatalogItemsInputRequestTypeDef,
     ListOrdersInputRequestTypeDef,
     OrderSummaryTypeDef,
     ListOutpostsInputRequestTypeDef,
     ListSitesInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    RackPhysicalPropertiesOutputTypeDef,
     StartConnectionRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateOutpostInputRequestTypeDef,
     UpdateSiteInputRequestTypeDef,
     UpdateSiteRackPhysicalPropertiesInputRequestTypeDef,
     UpdateSiteAddressInputRequestTypeDef,
@@ -413,39 +411,39 @@
     StartConnectionResponseTypeDef,
     UpdateSiteAddressOutputTypeDef,
     CreateOutpostOutputTypeDef,
     GetOutpostOutputTypeDef,
     ListOutpostsOutputTypeDef,
     UpdateOutpostOutputTypeDef,
     CreateSiteInputRequestTypeDef,
+    SiteTypeDef,
     GetOutpostInstanceTypesInputGetOutpostInstanceTypesPaginateTypeDef,
     ListAssetsInputListAssetsPaginateTypeDef,
     ListCatalogItemsInputListCatalogItemsPaginateTypeDef,
     ListOrdersInputListOrdersPaginateTypeDef,
     ListOutpostsInputListOutpostsPaginateTypeDef,
     ListSitesInputListSitesPaginateTypeDef,
     GetOutpostInstanceTypesOutputTypeDef,
     LineItemTypeDef,
     ListOrdersOutputTypeDef,
-    SiteTypeDef,
     ListAssetsOutputTypeDef,
     GetCatalogItemOutputTypeDef,
     ListCatalogItemsOutputTypeDef,
-    OrderTypeDef,
     CreateSiteOutputTypeDef,
     GetSiteOutputTypeDef,
     ListSitesOutputTypeDef,
     UpdateSiteOutputTypeDef,
     UpdateSiteRackPhysicalPropertiesOutputTypeDef,
+    OrderTypeDef,
     CreateOrderOutputTypeDef,
     GetOrderOutputTypeDef,
 )
 
 
-def get_structure() -> AddressOutputTypeDef:
+def get_structure() -> AddressTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-outposts-1.28.12/mypy_boto3_outposts.egg-info/SOURCES.txt` & `mypy-boto3-outposts-1.28.15/mypy_boto3_outposts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-outposts-1.28.12/setup.py` & `mypy-boto3-outposts-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-outposts",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Outposts 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Outposts 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

