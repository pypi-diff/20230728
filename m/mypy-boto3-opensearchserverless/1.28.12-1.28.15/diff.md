# Comparing `tmp/mypy-boto3-opensearchserverless-1.28.12.tar.gz` & `tmp/mypy-boto3-opensearchserverless-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opensearchserverless-1.28.12.tar", last modified: Thu Jul 27 05:44:17 2023, max compression
+gzip compressed data, was "mypy-boto3-opensearchserverless-1.28.15.tar", last modified: Fri Jul 28 20:43:24 2023, max compression
```

## Comparing `mypy-boto3-opensearchserverless-1.28.12.tar` & `mypy-boto3-opensearchserverless-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.383381 mypy-boto3-opensearchserverless-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15955 2023-07-27 05:44:17.383381 mypy-boto3-opensearchserverless-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14409 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.383381 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23936 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23898 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:44:03.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.383381 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15955 2023-07-27 05:44:17.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-27 05:44:17.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:44:17.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 05:44:17.000000 mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:44:17.383381 mypy-boto3-opensearchserverless-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-27 05:44:02.000000 mypy-boto3-opensearchserverless-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.261597 mypy-boto3-opensearchserverless-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:52.000000 mypy-boto3-opensearchserverless-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-07-28 20:43:24.261597 mypy-boto3-opensearchserverless-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-07-28 20:32:52.000000 mypy-boto3-opensearchserverless-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.253597 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-28 20:32:52.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-28 20:32:52.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 20:32:52.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23936 2023-07-28 20:32:52.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23898 2023-07-28 20:32:52.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-07-28 20:32:52.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-28 20:32:52.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:52.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29351 2023-07-28 20:32:55.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29312 2023-07-28 20:32:55.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:52.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.261597 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-07-28 20:43:24.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-28 20:43:24.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:24.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 20:43:24.000000 mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:24.261597 mypy-boto3-opensearchserverless-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-28 20:32:51.000000 mypy-boto3-opensearchserverless-1.28.15/setup.py
```

### Comparing `mypy-boto3-opensearchserverless-1.28.12/LICENSE` & `mypy-boto3-opensearchserverless-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.28.12/PKG-INFO` & `mypy-boto3-opensearchserverless-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearchserverless
-Version: 1.28.12
-Summary: Type annotations for boto3.OpenSearchServiceServerless 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.OpenSearchServiceServerless 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearchserverless)](https://pepy.tech/project/mypy-boto3-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchServiceServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[boto3.OpenSearchServiceServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
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
 [mypy-boto3-opensearchserverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,23 +306,22 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearchserverless.type_defs import (
     AccessPolicyDetailTypeDef,
     AccessPolicyStatsTypeDef,
     AccessPolicySummaryTypeDef,
-    CapacityLimitsOutputTypeDef,
+    CapacityLimitsTypeDef,
     BatchGetCollectionRequestRequestTypeDef,
     CollectionDetailTypeDef,
     CollectionErrorDetailTypeDef,
     ResponseMetadataTypeDef,
     BatchGetVpcEndpointRequestRequestTypeDef,
     VpcEndpointDetailTypeDef,
     VpcEndpointErrorDetailTypeDef,
-    CapacityLimitsTypeDef,
     CollectionFiltersTypeDef,
     CollectionSummaryTypeDef,
     CreateAccessPolicyRequestRequestTypeDef,
     CreateCollectionDetailTypeDef,
     TagTypeDef,
     SamlConfigOptionsTypeDef,
     CreateSecurityPolicyRequestRequestTypeDef,
@@ -343,53 +342,51 @@
     GetSecurityPolicyRequestRequestTypeDef,
     ListAccessPoliciesRequestRequestTypeDef,
     ListSecurityConfigsRequestRequestTypeDef,
     SecurityConfigSummaryTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
     SecurityPolicySummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     VpcEndpointFiltersTypeDef,
     VpcEndpointSummaryTypeDef,
-    SamlConfigOptionsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     UpdateCollectionDetailTypeDef,
     UpdateCollectionRequestRequestTypeDef,
     UpdateSecurityPolicyRequestRequestTypeDef,
     UpdateVpcEndpointDetailTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     AccountSettingsDetailTypeDef,
+    UpdateAccountSettingsRequestRequestTypeDef,
     BatchGetCollectionResponseTypeDef,
     CreateAccessPolicyResponseTypeDef,
     GetAccessPolicyResponseTypeDef,
     ListAccessPoliciesResponseTypeDef,
     UpdateAccessPolicyResponseTypeDef,
     BatchGetVpcEndpointResponseTypeDef,
-    UpdateAccountSettingsRequestRequestTypeDef,
     ListCollectionsRequestRequestTypeDef,
     ListCollectionsResponseTypeDef,
     CreateCollectionResponseTypeDef,
     CreateCollectionRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSecurityConfigRequestRequestTypeDef,
+    SecurityConfigDetailTypeDef,
     UpdateSecurityConfigRequestRequestTypeDef,
     CreateSecurityPolicyResponseTypeDef,
     GetSecurityPolicyResponseTypeDef,
     UpdateSecurityPolicyResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DeleteCollectionResponseTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     GetPoliciesStatsResponseTypeDef,
     ListSecurityConfigsResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
     ListVpcEndpointsResponseTypeDef,
-    SecurityConfigDetailTypeDef,
     UpdateCollectionResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsResponseTypeDef,
     CreateSecurityConfigResponseTypeDef,
     GetSecurityConfigResponseTypeDef,
     UpdateSecurityConfigResponseTypeDef,
```

### Comparing `mypy-boto3-opensearchserverless-1.28.12/README.md` & `mypy-boto3-opensearchserverless-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearchserverless)](https://pepy.tech/project/mypy-boto3-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchServiceServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[boto3.OpenSearchServiceServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
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
 [mypy-boto3-opensearchserverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -274,23 +274,22 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearchserverless.type_defs import (
     AccessPolicyDetailTypeDef,
     AccessPolicyStatsTypeDef,
     AccessPolicySummaryTypeDef,
-    CapacityLimitsOutputTypeDef,
+    CapacityLimitsTypeDef,
     BatchGetCollectionRequestRequestTypeDef,
     CollectionDetailTypeDef,
     CollectionErrorDetailTypeDef,
     ResponseMetadataTypeDef,
     BatchGetVpcEndpointRequestRequestTypeDef,
     VpcEndpointDetailTypeDef,
     VpcEndpointErrorDetailTypeDef,
-    CapacityLimitsTypeDef,
     CollectionFiltersTypeDef,
     CollectionSummaryTypeDef,
     CreateAccessPolicyRequestRequestTypeDef,
     CreateCollectionDetailTypeDef,
     TagTypeDef,
     SamlConfigOptionsTypeDef,
     CreateSecurityPolicyRequestRequestTypeDef,
@@ -311,53 +310,51 @@
     GetSecurityPolicyRequestRequestTypeDef,
     ListAccessPoliciesRequestRequestTypeDef,
     ListSecurityConfigsRequestRequestTypeDef,
     SecurityConfigSummaryTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
     SecurityPolicySummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     VpcEndpointFiltersTypeDef,
     VpcEndpointSummaryTypeDef,
-    SamlConfigOptionsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     UpdateCollectionDetailTypeDef,
     UpdateCollectionRequestRequestTypeDef,
     UpdateSecurityPolicyRequestRequestTypeDef,
     UpdateVpcEndpointDetailTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     AccountSettingsDetailTypeDef,
+    UpdateAccountSettingsRequestRequestTypeDef,
     BatchGetCollectionResponseTypeDef,
     CreateAccessPolicyResponseTypeDef,
     GetAccessPolicyResponseTypeDef,
     ListAccessPoliciesResponseTypeDef,
     UpdateAccessPolicyResponseTypeDef,
     BatchGetVpcEndpointResponseTypeDef,
-    UpdateAccountSettingsRequestRequestTypeDef,
     ListCollectionsRequestRequestTypeDef,
     ListCollectionsResponseTypeDef,
     CreateCollectionResponseTypeDef,
     CreateCollectionRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSecurityConfigRequestRequestTypeDef,
+    SecurityConfigDetailTypeDef,
     UpdateSecurityConfigRequestRequestTypeDef,
     CreateSecurityPolicyResponseTypeDef,
     GetSecurityPolicyResponseTypeDef,
     UpdateSecurityPolicyResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DeleteCollectionResponseTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     GetPoliciesStatsResponseTypeDef,
     ListSecurityConfigsResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
     ListVpcEndpointsResponseTypeDef,
-    SecurityConfigDetailTypeDef,
     UpdateCollectionResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsResponseTypeDef,
     CreateSecurityConfigResponseTypeDef,
     GetSecurityConfigResponseTypeDef,
     UpdateSecurityConfigResponseTypeDef,
```

### Comparing `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/__init__.py` & `mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/__main__.py` & `mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchServiceServerless 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.OpenSearchServiceServerless 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless\nOther"
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

### Comparing `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/client.py` & `mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/client.pyi` & `mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/literals.py` & `mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/literals.pyi` & `mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/type_defs.py` & `mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,23 +31,22 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessPolicyDetailTypeDef",
     "AccessPolicyStatsTypeDef",
     "AccessPolicySummaryTypeDef",
-    "CapacityLimitsOutputTypeDef",
+    "CapacityLimitsTypeDef",
     "BatchGetCollectionRequestRequestTypeDef",
     "CollectionDetailTypeDef",
     "CollectionErrorDetailTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetVpcEndpointRequestRequestTypeDef",
     "VpcEndpointDetailTypeDef",
     "VpcEndpointErrorDetailTypeDef",
-    "CapacityLimitsTypeDef",
     "CollectionFiltersTypeDef",
     "CollectionSummaryTypeDef",
     "CreateAccessPolicyRequestRequestTypeDef",
     "CreateCollectionDetailTypeDef",
     "TagTypeDef",
     "SamlConfigOptionsTypeDef",
     "CreateSecurityPolicyRequestRequestTypeDef",
@@ -68,53 +67,51 @@
     "GetSecurityPolicyRequestRequestTypeDef",
     "ListAccessPoliciesRequestRequestTypeDef",
     "ListSecurityConfigsRequestRequestTypeDef",
     "SecurityConfigSummaryTypeDef",
     "ListSecurityPoliciesRequestRequestTypeDef",
     "SecurityPolicySummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "VpcEndpointFiltersTypeDef",
     "VpcEndpointSummaryTypeDef",
-    "SamlConfigOptionsOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessPolicyRequestRequestTypeDef",
     "UpdateCollectionDetailTypeDef",
     "UpdateCollectionRequestRequestTypeDef",
     "UpdateSecurityPolicyRequestRequestTypeDef",
     "UpdateVpcEndpointDetailTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
     "AccountSettingsDetailTypeDef",
+    "UpdateAccountSettingsRequestRequestTypeDef",
     "BatchGetCollectionResponseTypeDef",
     "CreateAccessPolicyResponseTypeDef",
     "GetAccessPolicyResponseTypeDef",
     "ListAccessPoliciesResponseTypeDef",
     "UpdateAccessPolicyResponseTypeDef",
     "BatchGetVpcEndpointResponseTypeDef",
-    "UpdateAccountSettingsRequestRequestTypeDef",
     "ListCollectionsRequestRequestTypeDef",
     "ListCollectionsResponseTypeDef",
     "CreateCollectionResponseTypeDef",
     "CreateCollectionRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSecurityConfigRequestRequestTypeDef",
+    "SecurityConfigDetailTypeDef",
     "UpdateSecurityConfigRequestRequestTypeDef",
     "CreateSecurityPolicyResponseTypeDef",
     "GetSecurityPolicyResponseTypeDef",
     "UpdateSecurityPolicyResponseTypeDef",
     "CreateVpcEndpointResponseTypeDef",
     "DeleteCollectionResponseTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "GetPoliciesStatsResponseTypeDef",
     "ListSecurityConfigsResponseTypeDef",
     "ListSecurityPoliciesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
     "ListVpcEndpointsResponseTypeDef",
-    "SecurityConfigDetailTypeDef",
     "UpdateCollectionResponseTypeDef",
     "UpdateVpcEndpointResponseTypeDef",
     "GetAccountSettingsResponseTypeDef",
     "UpdateAccountSettingsResponseTypeDef",
     "CreateSecurityConfigResponseTypeDef",
     "GetSecurityConfigResponseTypeDef",
     "UpdateSecurityConfigResponseTypeDef",
@@ -151,16 +148,16 @@
         "name": str,
         "policyVersion": str,
         "type": Literal["data"],
     },
     total=False,
 )
 
-CapacityLimitsOutputTypeDef = TypedDict(
-    "CapacityLimitsOutputTypeDef",
+CapacityLimitsTypeDef = TypedDict(
+    "CapacityLimitsTypeDef",
     {
         "maxIndexingCapacityInOCU": int,
         "maxSearchCapacityInOCU": int,
     },
     total=False,
 )
 
@@ -240,23 +237,14 @@
         "errorCode": str,
         "errorMessage": str,
         "id": str,
     },
     total=False,
 )
 
-CapacityLimitsTypeDef = TypedDict(
-    "CapacityLimitsTypeDef",
-    {
-        "maxIndexingCapacityInOCU": int,
-        "maxSearchCapacityInOCU": int,
-    },
-    total=False,
-)
-
 CollectionFiltersTypeDef = TypedDict(
     "CollectionFiltersTypeDef",
     {
         "name": str,
         "status": CollectionStatusType,
     },
     total=False,
@@ -688,22 +676,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 VpcEndpointFiltersTypeDef = TypedDict(
     "VpcEndpointFiltersTypeDef",
     {
         "status": VpcEndpointStatusType,
     },
     total=False,
 )
@@ -714,37 +694,14 @@
         "id": str,
         "name": str,
         "status": VpcEndpointStatusType,
     },
     total=False,
 )
 
-_RequiredSamlConfigOptionsOutputTypeDef = TypedDict(
-    "_RequiredSamlConfigOptionsOutputTypeDef",
-    {
-        "metadata": str,
-    },
-)
-_OptionalSamlConfigOptionsOutputTypeDef = TypedDict(
-    "_OptionalSamlConfigOptionsOutputTypeDef",
-    {
-        "groupAttribute": str,
-        "sessionTimeout": int,
-        "userAttribute": str,
-    },
-    total=False,
-)
-
-
-class SamlConfigOptionsOutputTypeDef(
-    _RequiredSamlConfigOptionsOutputTypeDef, _OptionalSamlConfigOptionsOutputTypeDef
-):
-    pass
-
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -875,15 +832,23 @@
 ):
     pass
 
 
 AccountSettingsDetailTypeDef = TypedDict(
     "AccountSettingsDetailTypeDef",
     {
-        "capacityLimits": CapacityLimitsOutputTypeDef,
+        "capacityLimits": CapacityLimitsTypeDef,
+    },
+    total=False,
+)
+
+UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateAccountSettingsRequestRequestTypeDef",
+    {
+        "capacityLimits": CapacityLimitsTypeDef,
     },
     total=False,
 )
 
 BatchGetCollectionResponseTypeDef = TypedDict(
     "BatchGetCollectionResponseTypeDef",
     {
@@ -931,22 +896,14 @@
     {
         "vpcEndpointDetails": List[VpcEndpointDetailTypeDef],
         "vpcEndpointErrorDetails": List[VpcEndpointErrorDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateAccountSettingsRequestRequestTypeDef",
-    {
-        "capacityLimits": CapacityLimitsTypeDef,
-    },
-    total=False,
-)
-
 ListCollectionsRequestRequestTypeDef = TypedDict(
     "ListCollectionsRequestRequestTypeDef",
     {
         "collectionFilters": CollectionFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
@@ -990,14 +947,22 @@
 
 class CreateCollectionRequestRequestTypeDef(
     _RequiredCreateCollectionRequestRequestTypeDef, _OptionalCreateCollectionRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1023,14 +988,28 @@
 class CreateSecurityConfigRequestRequestTypeDef(
     _RequiredCreateSecurityConfigRequestRequestTypeDef,
     _OptionalCreateSecurityConfigRequestRequestTypeDef,
 ):
     pass
 
 
+SecurityConfigDetailTypeDef = TypedDict(
+    "SecurityConfigDetailTypeDef",
+    {
+        "configVersion": str,
+        "createdDate": int,
+        "description": str,
+        "id": str,
+        "lastModifiedDate": int,
+        "samlOptions": SamlConfigOptionsTypeDef,
+        "type": Literal["saml"],
+    },
+    total=False,
+)
+
 _RequiredUpdateSecurityConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityConfigRequestRequestTypeDef",
     {
         "configVersion": str,
         "id": str,
     },
 )
@@ -1125,22 +1104,14 @@
     {
         "nextToken": str,
         "securityPolicySummaries": List[SecurityPolicySummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListVpcEndpointsRequestRequestTypeDef = TypedDict(
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "vpcEndpointFilters": VpcEndpointFiltersTypeDef,
     },
@@ -1152,28 +1123,14 @@
     {
         "nextToken": str,
         "vpcEndpointSummaries": List[VpcEndpointSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SecurityConfigDetailTypeDef = TypedDict(
-    "SecurityConfigDetailTypeDef",
-    {
-        "configVersion": str,
-        "createdDate": int,
-        "description": str,
-        "id": str,
-        "lastModifiedDate": int,
-        "samlOptions": SamlConfigOptionsOutputTypeDef,
-        "type": Literal["saml"],
-    },
-    total=False,
-)
-
 UpdateCollectionResponseTypeDef = TypedDict(
     "UpdateCollectionResponseTypeDef",
     {
         "updateCollectionDetail": UpdateCollectionDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless/type_defs.pyi` & `mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -30,23 +30,22 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessPolicyDetailTypeDef",
     "AccessPolicyStatsTypeDef",
     "AccessPolicySummaryTypeDef",
-    "CapacityLimitsOutputTypeDef",
+    "CapacityLimitsTypeDef",
     "BatchGetCollectionRequestRequestTypeDef",
     "CollectionDetailTypeDef",
     "CollectionErrorDetailTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetVpcEndpointRequestRequestTypeDef",
     "VpcEndpointDetailTypeDef",
     "VpcEndpointErrorDetailTypeDef",
-    "CapacityLimitsTypeDef",
     "CollectionFiltersTypeDef",
     "CollectionSummaryTypeDef",
     "CreateAccessPolicyRequestRequestTypeDef",
     "CreateCollectionDetailTypeDef",
     "TagTypeDef",
     "SamlConfigOptionsTypeDef",
     "CreateSecurityPolicyRequestRequestTypeDef",
@@ -67,53 +66,51 @@
     "GetSecurityPolicyRequestRequestTypeDef",
     "ListAccessPoliciesRequestRequestTypeDef",
     "ListSecurityConfigsRequestRequestTypeDef",
     "SecurityConfigSummaryTypeDef",
     "ListSecurityPoliciesRequestRequestTypeDef",
     "SecurityPolicySummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "VpcEndpointFiltersTypeDef",
     "VpcEndpointSummaryTypeDef",
-    "SamlConfigOptionsOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessPolicyRequestRequestTypeDef",
     "UpdateCollectionDetailTypeDef",
     "UpdateCollectionRequestRequestTypeDef",
     "UpdateSecurityPolicyRequestRequestTypeDef",
     "UpdateVpcEndpointDetailTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
     "AccountSettingsDetailTypeDef",
+    "UpdateAccountSettingsRequestRequestTypeDef",
     "BatchGetCollectionResponseTypeDef",
     "CreateAccessPolicyResponseTypeDef",
     "GetAccessPolicyResponseTypeDef",
     "ListAccessPoliciesResponseTypeDef",
     "UpdateAccessPolicyResponseTypeDef",
     "BatchGetVpcEndpointResponseTypeDef",
-    "UpdateAccountSettingsRequestRequestTypeDef",
     "ListCollectionsRequestRequestTypeDef",
     "ListCollectionsResponseTypeDef",
     "CreateCollectionResponseTypeDef",
     "CreateCollectionRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSecurityConfigRequestRequestTypeDef",
+    "SecurityConfigDetailTypeDef",
     "UpdateSecurityConfigRequestRequestTypeDef",
     "CreateSecurityPolicyResponseTypeDef",
     "GetSecurityPolicyResponseTypeDef",
     "UpdateSecurityPolicyResponseTypeDef",
     "CreateVpcEndpointResponseTypeDef",
     "DeleteCollectionResponseTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "GetPoliciesStatsResponseTypeDef",
     "ListSecurityConfigsResponseTypeDef",
     "ListSecurityPoliciesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
     "ListVpcEndpointsResponseTypeDef",
-    "SecurityConfigDetailTypeDef",
     "UpdateCollectionResponseTypeDef",
     "UpdateVpcEndpointResponseTypeDef",
     "GetAccountSettingsResponseTypeDef",
     "UpdateAccountSettingsResponseTypeDef",
     "CreateSecurityConfigResponseTypeDef",
     "GetSecurityConfigResponseTypeDef",
     "UpdateSecurityConfigResponseTypeDef",
@@ -150,16 +147,16 @@
         "name": str,
         "policyVersion": str,
         "type": Literal["data"],
     },
     total=False,
 )
 
-CapacityLimitsOutputTypeDef = TypedDict(
-    "CapacityLimitsOutputTypeDef",
+CapacityLimitsTypeDef = TypedDict(
+    "CapacityLimitsTypeDef",
     {
         "maxIndexingCapacityInOCU": int,
         "maxSearchCapacityInOCU": int,
     },
     total=False,
 )
 
@@ -239,23 +236,14 @@
         "errorCode": str,
         "errorMessage": str,
         "id": str,
     },
     total=False,
 )
 
-CapacityLimitsTypeDef = TypedDict(
-    "CapacityLimitsTypeDef",
-    {
-        "maxIndexingCapacityInOCU": int,
-        "maxSearchCapacityInOCU": int,
-    },
-    total=False,
-)
-
 CollectionFiltersTypeDef = TypedDict(
     "CollectionFiltersTypeDef",
     {
         "name": str,
         "status": CollectionStatusType,
     },
     total=False,
@@ -663,22 +651,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 VpcEndpointFiltersTypeDef = TypedDict(
     "VpcEndpointFiltersTypeDef",
     {
         "status": VpcEndpointStatusType,
     },
     total=False,
 )
@@ -689,35 +669,14 @@
         "id": str,
         "name": str,
         "status": VpcEndpointStatusType,
     },
     total=False,
 )
 
-_RequiredSamlConfigOptionsOutputTypeDef = TypedDict(
-    "_RequiredSamlConfigOptionsOutputTypeDef",
-    {
-        "metadata": str,
-    },
-)
-_OptionalSamlConfigOptionsOutputTypeDef = TypedDict(
-    "_OptionalSamlConfigOptionsOutputTypeDef",
-    {
-        "groupAttribute": str,
-        "sessionTimeout": int,
-        "userAttribute": str,
-    },
-    total=False,
-)
-
-class SamlConfigOptionsOutputTypeDef(
-    _RequiredSamlConfigOptionsOutputTypeDef, _OptionalSamlConfigOptionsOutputTypeDef
-):
-    pass
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -840,15 +799,23 @@
     _RequiredUpdateVpcEndpointRequestRequestTypeDef, _OptionalUpdateVpcEndpointRequestRequestTypeDef
 ):
     pass
 
 AccountSettingsDetailTypeDef = TypedDict(
     "AccountSettingsDetailTypeDef",
     {
-        "capacityLimits": CapacityLimitsOutputTypeDef,
+        "capacityLimits": CapacityLimitsTypeDef,
+    },
+    total=False,
+)
+
+UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateAccountSettingsRequestRequestTypeDef",
+    {
+        "capacityLimits": CapacityLimitsTypeDef,
     },
     total=False,
 )
 
 BatchGetCollectionResponseTypeDef = TypedDict(
     "BatchGetCollectionResponseTypeDef",
     {
@@ -896,22 +863,14 @@
     {
         "vpcEndpointDetails": List[VpcEndpointDetailTypeDef],
         "vpcEndpointErrorDetails": List[VpcEndpointErrorDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateAccountSettingsRequestRequestTypeDef",
-    {
-        "capacityLimits": CapacityLimitsTypeDef,
-    },
-    total=False,
-)
-
 ListCollectionsRequestRequestTypeDef = TypedDict(
     "ListCollectionsRequestRequestTypeDef",
     {
         "collectionFilters": CollectionFiltersTypeDef,
         "maxResults": int,
         "nextToken": str,
     },
@@ -953,14 +912,22 @@
 )
 
 class CreateCollectionRequestRequestTypeDef(
     _RequiredCreateCollectionRequestRequestTypeDef, _OptionalCreateCollectionRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -984,14 +951,28 @@
 
 class CreateSecurityConfigRequestRequestTypeDef(
     _RequiredCreateSecurityConfigRequestRequestTypeDef,
     _OptionalCreateSecurityConfigRequestRequestTypeDef,
 ):
     pass
 
+SecurityConfigDetailTypeDef = TypedDict(
+    "SecurityConfigDetailTypeDef",
+    {
+        "configVersion": str,
+        "createdDate": int,
+        "description": str,
+        "id": str,
+        "lastModifiedDate": int,
+        "samlOptions": SamlConfigOptionsTypeDef,
+        "type": Literal["saml"],
+    },
+    total=False,
+)
+
 _RequiredUpdateSecurityConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecurityConfigRequestRequestTypeDef",
     {
         "configVersion": str,
         "id": str,
     },
 )
@@ -1084,22 +1065,14 @@
     {
         "nextToken": str,
         "securityPolicySummaries": List[SecurityPolicySummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListVpcEndpointsRequestRequestTypeDef = TypedDict(
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "vpcEndpointFilters": VpcEndpointFiltersTypeDef,
     },
@@ -1111,28 +1084,14 @@
     {
         "nextToken": str,
         "vpcEndpointSummaries": List[VpcEndpointSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SecurityConfigDetailTypeDef = TypedDict(
-    "SecurityConfigDetailTypeDef",
-    {
-        "configVersion": str,
-        "createdDate": int,
-        "description": str,
-        "id": str,
-        "lastModifiedDate": int,
-        "samlOptions": SamlConfigOptionsOutputTypeDef,
-        "type": Literal["saml"],
-    },
-    total=False,
-)
-
 UpdateCollectionResponseTypeDef = TypedDict(
     "UpdateCollectionResponseTypeDef",
     {
         "updateCollectionDetail": UpdateCollectionDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/PKG-INFO` & `mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearchserverless
-Version: 1.28.12
-Summary: Type annotations for boto3.OpenSearchServiceServerless 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.OpenSearchServiceServerless 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearchserverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearchserverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearchserverless)](https://pepy.tech/project/mypy-boto3-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchServiceServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[boto3.OpenSearchServiceServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
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
 [mypy-boto3-opensearchserverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearchserverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,23 +306,22 @@
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearchserverless.type_defs import (
     AccessPolicyDetailTypeDef,
     AccessPolicyStatsTypeDef,
     AccessPolicySummaryTypeDef,
-    CapacityLimitsOutputTypeDef,
+    CapacityLimitsTypeDef,
     BatchGetCollectionRequestRequestTypeDef,
     CollectionDetailTypeDef,
     CollectionErrorDetailTypeDef,
     ResponseMetadataTypeDef,
     BatchGetVpcEndpointRequestRequestTypeDef,
     VpcEndpointDetailTypeDef,
     VpcEndpointErrorDetailTypeDef,
-    CapacityLimitsTypeDef,
     CollectionFiltersTypeDef,
     CollectionSummaryTypeDef,
     CreateAccessPolicyRequestRequestTypeDef,
     CreateCollectionDetailTypeDef,
     TagTypeDef,
     SamlConfigOptionsTypeDef,
     CreateSecurityPolicyRequestRequestTypeDef,
@@ -343,53 +342,51 @@
     GetSecurityPolicyRequestRequestTypeDef,
     ListAccessPoliciesRequestRequestTypeDef,
     ListSecurityConfigsRequestRequestTypeDef,
     SecurityConfigSummaryTypeDef,
     ListSecurityPoliciesRequestRequestTypeDef,
     SecurityPolicySummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     VpcEndpointFiltersTypeDef,
     VpcEndpointSummaryTypeDef,
-    SamlConfigOptionsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessPolicyRequestRequestTypeDef,
     UpdateCollectionDetailTypeDef,
     UpdateCollectionRequestRequestTypeDef,
     UpdateSecurityPolicyRequestRequestTypeDef,
     UpdateVpcEndpointDetailTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     AccountSettingsDetailTypeDef,
+    UpdateAccountSettingsRequestRequestTypeDef,
     BatchGetCollectionResponseTypeDef,
     CreateAccessPolicyResponseTypeDef,
     GetAccessPolicyResponseTypeDef,
     ListAccessPoliciesResponseTypeDef,
     UpdateAccessPolicyResponseTypeDef,
     BatchGetVpcEndpointResponseTypeDef,
-    UpdateAccountSettingsRequestRequestTypeDef,
     ListCollectionsRequestRequestTypeDef,
     ListCollectionsResponseTypeDef,
     CreateCollectionResponseTypeDef,
     CreateCollectionRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSecurityConfigRequestRequestTypeDef,
+    SecurityConfigDetailTypeDef,
     UpdateSecurityConfigRequestRequestTypeDef,
     CreateSecurityPolicyResponseTypeDef,
     GetSecurityPolicyResponseTypeDef,
     UpdateSecurityPolicyResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DeleteCollectionResponseTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     GetPoliciesStatsResponseTypeDef,
     ListSecurityConfigsResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
     ListVpcEndpointsResponseTypeDef,
-    SecurityConfigDetailTypeDef,
     UpdateCollectionResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsResponseTypeDef,
     CreateSecurityConfigResponseTypeDef,
     GetSecurityConfigResponseTypeDef,
     UpdateSecurityConfigResponseTypeDef,
```

### Comparing `mypy-boto3-opensearchserverless-1.28.12/mypy_boto3_opensearchserverless.egg-info/SOURCES.txt` & `mypy-boto3-opensearchserverless-1.28.15/mypy_boto3_opensearchserverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearchserverless-1.28.12/setup.py` & `mypy-boto3-opensearchserverless-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opensearchserverless",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_opensearchserverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchServiceServerless 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.OpenSearchServiceServerless 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

