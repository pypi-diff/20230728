# Comparing `tmp/mypy-boto3-license-manager-user-subscriptions-1.28.12.tar.gz` & `tmp/mypy-boto3-license-manager-user-subscriptions-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-user-subscriptions-1.28.12.tar", last modified: Thu Jul 27 05:34:56 2023, max compression
+gzip compressed data, was "mypy-boto3-license-manager-user-subscriptions-1.28.15.tar", last modified: Fri Jul 28 20:43:09 2023, max compression
```

## Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12.tar` & `mypy-boto3-license-manager-user-subscriptions-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.940456 mypy-boto3-license-manager-user-subscriptions-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-07-27 05:34:56.940456 mypy-boto3-license-manager-user-subscriptions-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.932456 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-07-27 05:25:22.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16503 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.940456 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:56.940456 mypy-boto3-license-manager-user-subscriptions-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-user-subscriptions-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:09.037388 mypy-boto3-license-manager-user-subscriptions-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-07-28 20:43:09.033388 mypy-boto3-license-manager-user-subscriptions-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14635 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:09.033388 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-07-28 20:30:12.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-07-28 20:30:12.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:09.033388 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:09.037388 mypy-boto3-license-manager-user-subscriptions-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-user-subscriptions-1.28.15/setup.py
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/LICENSE` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/PKG-INFO` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-user-subscriptions
-Version: 1.28.12
-Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-user-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerUserSubscriptions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[boto3.LicenseManagerUserSubscriptions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,40 +346,38 @@
 
 `mypy_boto3_license_manager_user_subscriptions.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_user_subscriptions.type_defs import (
-    ActiveDirectoryIdentityProviderOutputTypeDef,
     ActiveDirectoryIdentityProviderTypeDef,
+    ResponseMetadataTypeDef,
     FilterTypeDef,
     SettingsOutputTypeDef,
     InstanceSummaryTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListIdentityProvidersRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    ListIdentityProvidersRequestRequestTypeDef,
     SettingsTypeDef,
-    ResponseMetadataTypeDef,
     UpdateSettingsTypeDef,
-    IdentityProviderOutputTypeDef,
     IdentityProviderTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
-    IdentityProviderSummaryTypeDef,
-    InstanceUserSummaryTypeDef,
-    ProductUserSummaryTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
+    IdentityProviderSummaryTypeDef,
+    InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
     ListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
     ListUserAssociationsRequestRequestTypeDef,
+    ProductUserSummaryTypeDef,
     RegisterIdentityProviderRequestRequestTypeDef,
     StartProductSubscriptionRequestRequestTypeDef,
     StopProductSubscriptionRequestRequestTypeDef,
     UpdateIdentityProviderSettingsRequestRequestTypeDef,
     DeregisterIdentityProviderResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
@@ -389,15 +387,15 @@
     ListUserAssociationsResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryIdentityProviderOutputTypeDef:
+def get_structure() -> ActiveDirectoryIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/README.md` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-user-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerUserSubscriptions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[boto3.LicenseManagerUserSubscriptions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,40 +314,38 @@
 
 `mypy_boto3_license_manager_user_subscriptions.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_user_subscriptions.type_defs import (
-    ActiveDirectoryIdentityProviderOutputTypeDef,
     ActiveDirectoryIdentityProviderTypeDef,
+    ResponseMetadataTypeDef,
     FilterTypeDef,
     SettingsOutputTypeDef,
     InstanceSummaryTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListIdentityProvidersRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    ListIdentityProvidersRequestRequestTypeDef,
     SettingsTypeDef,
-    ResponseMetadataTypeDef,
     UpdateSettingsTypeDef,
-    IdentityProviderOutputTypeDef,
     IdentityProviderTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
-    IdentityProviderSummaryTypeDef,
-    InstanceUserSummaryTypeDef,
-    ProductUserSummaryTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
+    IdentityProviderSummaryTypeDef,
+    InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
     ListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
     ListUserAssociationsRequestRequestTypeDef,
+    ProductUserSummaryTypeDef,
     RegisterIdentityProviderRequestRequestTypeDef,
     StartProductSubscriptionRequestRequestTypeDef,
     StopProductSubscriptionRequestRequestTypeDef,
     UpdateIdentityProviderSettingsRequestRequestTypeDef,
     DeregisterIdentityProviderResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
@@ -357,15 +355,15 @@
     ListUserAssociationsResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryIdentityProviderOutputTypeDef:
+def get_structure() -> ActiveDirectoryIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/__init__.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/__init__.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/__main__.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions\nOther"
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

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/client.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/client.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/literals.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/literals.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/paginator.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -42,89 +42,83 @@
 __all__ = (
     "ListIdentityProvidersPaginator",
     "ListInstancesPaginator",
     "ListProductSubscriptionsPaginator",
     "ListUserAssociationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListIdentityProvidersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listidentityproviderspaginator)
         """
 
-
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listinstancespaginator)
         """
 
-
 class ListProductSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListProductSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listproductsubscriptionspaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProductSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListProductSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listproductsubscriptionspaginator)
         """
 
-
 class ListUserAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListUserAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listuserassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUserAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListUserAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listuserassociationspaginator)
         """
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/paginator.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,83 +42,89 @@
 __all__ = (
     "ListIdentityProvidersPaginator",
     "ListInstancesPaginator",
     "ListProductSubscriptionsPaginator",
     "ListUserAssociationsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListIdentityProvidersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListIdentityProviders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listidentityproviderspaginator)
         """
 
+
 class ListInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listinstancespaginator)
         """
 
+
 class ListProductSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListProductSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listproductsubscriptionspaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProductSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListProductSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listproductsubscriptionspaginator)
         """
 
+
 class ListUserAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListUserAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listuserassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         InstanceId: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUserAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Paginator.ListUserAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/paginators/#listuserassociationspaginator)
         """
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/type_defs.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,55 +2,53 @@
 Type annotations for license-manager-user-subscriptions service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderOutputTypeDef
+    from mypy_boto3_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderTypeDef
 
-    data: ActiveDirectoryIdentityProviderOutputTypeDef = {...}
+    data: ActiveDirectoryIdentityProviderTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ActiveDirectoryIdentityProviderOutputTypeDef",
     "ActiveDirectoryIdentityProviderTypeDef",
+    "ResponseMetadataTypeDef",
     "FilterTypeDef",
     "SettingsOutputTypeDef",
     "InstanceSummaryTypeDef",
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    "ListIdentityProvidersRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "ListIdentityProvidersRequestRequestTypeDef",
     "SettingsTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateSettingsTypeDef",
-    "IdentityProviderOutputTypeDef",
     "IdentityProviderTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
-    "IdentityProviderSummaryTypeDef",
-    "InstanceUserSummaryTypeDef",
-    "ProductUserSummaryTypeDef",
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     "AssociateUserRequestRequestTypeDef",
     "DeregisterIdentityProviderRequestRequestTypeDef",
     "DisassociateUserRequestRequestTypeDef",
+    "IdentityProviderSummaryTypeDef",
+    "InstanceUserSummaryTypeDef",
     "ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     "ListProductSubscriptionsRequestRequestTypeDef",
     "ListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     "ListUserAssociationsRequestRequestTypeDef",
+    "ProductUserSummaryTypeDef",
     "RegisterIdentityProviderRequestRequestTypeDef",
     "StartProductSubscriptionRequestRequestTypeDef",
     "StopProductSubscriptionRequestRequestTypeDef",
     "UpdateIdentityProviderSettingsRequestRequestTypeDef",
     "DeregisterIdentityProviderResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "RegisterIdentityProviderResponseTypeDef",
@@ -59,28 +57,31 @@
     "DisassociateUserResponseTypeDef",
     "ListUserAssociationsResponseTypeDef",
     "ListProductSubscriptionsResponseTypeDef",
     "StartProductSubscriptionResponseTypeDef",
     "StopProductSubscriptionResponseTypeDef",
 )
 
-ActiveDirectoryIdentityProviderOutputTypeDef = TypedDict(
-    "ActiveDirectoryIdentityProviderOutputTypeDef",
+ActiveDirectoryIdentityProviderTypeDef = TypedDict(
+    "ActiveDirectoryIdentityProviderTypeDef",
     {
         "DirectoryId": str,
     },
     total=False,
 )
 
-ActiveDirectoryIdentityProviderTypeDef = TypedDict(
-    "ActiveDirectoryIdentityProviderTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "DirectoryId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Attribute": str,
         "Operation": str,
@@ -115,60 +116,41 @@
 )
 
 
 class InstanceSummaryTypeDef(_RequiredInstanceSummaryTypeDef, _OptionalInstanceSummaryTypeDef):
     pass
 
 
-ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListIdentityProvidersRequestRequestTypeDef = TypedDict(
     "ListIdentityProvidersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "SecurityGroupId": str,
         "Subnets": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredUpdateSettingsTypeDef = TypedDict(
     "_RequiredUpdateSettingsTypeDef",
     {
         "AddSubnets": Sequence[str],
         "RemoveSubnets": Sequence[str],
     },
 )
@@ -181,39 +163,22 @@
 )
 
 
 class UpdateSettingsTypeDef(_RequiredUpdateSettingsTypeDef, _OptionalUpdateSettingsTypeDef):
     pass
 
 
-IdentityProviderOutputTypeDef = TypedDict(
-    "IdentityProviderOutputTypeDef",
-    {
-        "ActiveDirectoryIdentityProvider": ActiveDirectoryIdentityProviderOutputTypeDef,
-    },
-    total=False,
-)
-
 IdentityProviderTypeDef = TypedDict(
     "IdentityProviderTypeDef",
     {
         "ActiveDirectoryIdentityProvider": ActiveDirectoryIdentityProviderTypeDef,
     },
     total=False,
 )
 
-ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "ListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInstancesRequestRequestTypeDef = TypedDict(
     "ListInstancesRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -221,146 +186,136 @@
 )
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "InstanceSummaries": List[InstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredIdentityProviderSummaryTypeDef = TypedDict(
-    "_RequiredIdentityProviderSummaryTypeDef",
+ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     {
-        "IdentityProvider": IdentityProviderOutputTypeDef,
-        "Product": str,
-        "Settings": SettingsOutputTypeDef,
-        "Status": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalIdentityProviderSummaryTypeDef = TypedDict(
-    "_OptionalIdentityProviderSummaryTypeDef",
+
+ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     {
-        "FailureMessage": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class IdentityProviderSummaryTypeDef(
-    _RequiredIdentityProviderSummaryTypeDef, _OptionalIdentityProviderSummaryTypeDef
-):
-    pass
-
-
-_RequiredInstanceUserSummaryTypeDef = TypedDict(
-    "_RequiredInstanceUserSummaryTypeDef",
+_RequiredAssociateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateUserRequestRequestTypeDef",
     {
-        "IdentityProvider": IdentityProviderOutputTypeDef,
+        "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
-        "Status": str,
         "Username": str,
     },
 )
-_OptionalInstanceUserSummaryTypeDef = TypedDict(
-    "_OptionalInstanceUserSummaryTypeDef",
+_OptionalAssociateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateUserRequestRequestTypeDef",
     {
-        "AssociationDate": str,
-        "DisassociationDate": str,
         "Domain": str,
-        "StatusMessage": str,
     },
     total=False,
 )
 
 
-class InstanceUserSummaryTypeDef(
-    _RequiredInstanceUserSummaryTypeDef, _OptionalInstanceUserSummaryTypeDef
+class AssociateUserRequestRequestTypeDef(
+    _RequiredAssociateUserRequestRequestTypeDef, _OptionalAssociateUserRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredProductUserSummaryTypeDef = TypedDict(
-    "_RequiredProductUserSummaryTypeDef",
+DeregisterIdentityProviderRequestRequestTypeDef = TypedDict(
+    "DeregisterIdentityProviderRequestRequestTypeDef",
     {
-        "IdentityProvider": IdentityProviderOutputTypeDef,
+        "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
-        "Status": str,
+    },
+)
+
+_RequiredDisassociateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateUserRequestRequestTypeDef",
+    {
+        "IdentityProvider": IdentityProviderTypeDef,
+        "InstanceId": str,
         "Username": str,
     },
 )
-_OptionalProductUserSummaryTypeDef = TypedDict(
-    "_OptionalProductUserSummaryTypeDef",
+_OptionalDisassociateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateUserRequestRequestTypeDef",
     {
         "Domain": str,
-        "StatusMessage": str,
-        "SubscriptionEndDate": str,
-        "SubscriptionStartDate": str,
     },
     total=False,
 )
 
 
-class ProductUserSummaryTypeDef(
-    _RequiredProductUserSummaryTypeDef, _OptionalProductUserSummaryTypeDef
+class DisassociateUserRequestRequestTypeDef(
+    _RequiredDisassociateUserRequestRequestTypeDef, _OptionalDisassociateUserRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredAssociateUserRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateUserRequestRequestTypeDef",
+_RequiredIdentityProviderSummaryTypeDef = TypedDict(
+    "_RequiredIdentityProviderSummaryTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
-        "InstanceId": str,
-        "Username": str,
+        "Product": str,
+        "Settings": SettingsOutputTypeDef,
+        "Status": str,
     },
 )
-_OptionalAssociateUserRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateUserRequestRequestTypeDef",
+_OptionalIdentityProviderSummaryTypeDef = TypedDict(
+    "_OptionalIdentityProviderSummaryTypeDef",
     {
-        "Domain": str,
+        "FailureMessage": str,
     },
     total=False,
 )
 
 
-class AssociateUserRequestRequestTypeDef(
-    _RequiredAssociateUserRequestRequestTypeDef, _OptionalAssociateUserRequestRequestTypeDef
+class IdentityProviderSummaryTypeDef(
+    _RequiredIdentityProviderSummaryTypeDef, _OptionalIdentityProviderSummaryTypeDef
 ):
     pass
 
 
-DeregisterIdentityProviderRequestRequestTypeDef = TypedDict(
-    "DeregisterIdentityProviderRequestRequestTypeDef",
-    {
-        "IdentityProvider": IdentityProviderTypeDef,
-        "Product": str,
-    },
-)
-
-_RequiredDisassociateUserRequestRequestTypeDef = TypedDict(
-    "_RequiredDisassociateUserRequestRequestTypeDef",
+_RequiredInstanceUserSummaryTypeDef = TypedDict(
+    "_RequiredInstanceUserSummaryTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
+        "Status": str,
         "Username": str,
     },
 )
-_OptionalDisassociateUserRequestRequestTypeDef = TypedDict(
-    "_OptionalDisassociateUserRequestRequestTypeDef",
+_OptionalInstanceUserSummaryTypeDef = TypedDict(
+    "_OptionalInstanceUserSummaryTypeDef",
     {
+        "AssociationDate": str,
+        "DisassociationDate": str,
         "Domain": str,
+        "StatusMessage": str,
     },
     total=False,
 )
 
 
-class DisassociateUserRequestRequestTypeDef(
-    _RequiredDisassociateUserRequestRequestTypeDef, _OptionalDisassociateUserRequestRequestTypeDef
+class InstanceUserSummaryTypeDef(
+    _RequiredInstanceUserSummaryTypeDef, _OptionalInstanceUserSummaryTypeDef
 ):
     pass
 
 
 _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef = TypedDict(
     "_RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     {
@@ -368,15 +323,15 @@
         "Product": str,
     },
 )
 _OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef = TypedDict(
     "_OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef(
     _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
@@ -417,15 +372,15 @@
         "InstanceId": str,
     },
 )
 _OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef = TypedDict(
     "_OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListUserAssociationsRequestListUserAssociationsPaginateTypeDef(
     _RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
@@ -455,14 +410,41 @@
 class ListUserAssociationsRequestRequestTypeDef(
     _RequiredListUserAssociationsRequestRequestTypeDef,
     _OptionalListUserAssociationsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredProductUserSummaryTypeDef = TypedDict(
+    "_RequiredProductUserSummaryTypeDef",
+    {
+        "IdentityProvider": IdentityProviderTypeDef,
+        "Product": str,
+        "Status": str,
+        "Username": str,
+    },
+)
+_OptionalProductUserSummaryTypeDef = TypedDict(
+    "_OptionalProductUserSummaryTypeDef",
+    {
+        "Domain": str,
+        "StatusMessage": str,
+        "SubscriptionEndDate": str,
+        "SubscriptionStartDate": str,
+    },
+    total=False,
+)
+
+
+class ProductUserSummaryTypeDef(
+    _RequiredProductUserSummaryTypeDef, _OptionalProductUserSummaryTypeDef
+):
+    pass
+
+
 _RequiredRegisterIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterIdentityProviderRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -539,85 +521,85 @@
     },
 )
 
 DeregisterIdentityProviderResponseTypeDef = TypedDict(
     "DeregisterIdentityProviderResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "IdentityProviderSummaries": List[IdentityProviderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterIdentityProviderResponseTypeDef = TypedDict(
     "RegisterIdentityProviderResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIdentityProviderSettingsResponseTypeDef = TypedDict(
     "UpdateIdentityProviderSettingsResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateUserResponseTypeDef = TypedDict(
     "AssociateUserResponseTypeDef",
     {
         "InstanceUserSummary": InstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateUserResponseTypeDef = TypedDict(
     "DisassociateUserResponseTypeDef",
     {
         "InstanceUserSummary": InstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserAssociationsResponseTypeDef = TypedDict(
     "ListUserAssociationsResponseTypeDef",
     {
         "InstanceUserSummaries": List[InstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProductSubscriptionsResponseTypeDef = TypedDict(
     "ListProductSubscriptionsResponseTypeDef",
     {
         "NextToken": str,
         "ProductUserSummaries": List[ProductUserSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartProductSubscriptionResponseTypeDef = TypedDict(
     "StartProductSubscriptionResponseTypeDef",
     {
         "ProductUserSummary": ProductUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopProductSubscriptionResponseTypeDef = TypedDict(
     "StopProductSubscriptionResponseTypeDef",
     {
         "ProductUserSummary": ProductUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,54 +2,52 @@
 Type annotations for license-manager-user-subscriptions service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderOutputTypeDef
+    from mypy_boto3_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderTypeDef
 
-    data: ActiveDirectoryIdentityProviderOutputTypeDef = {...}
+    data: ActiveDirectoryIdentityProviderTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ActiveDirectoryIdentityProviderOutputTypeDef",
     "ActiveDirectoryIdentityProviderTypeDef",
+    "ResponseMetadataTypeDef",
     "FilterTypeDef",
     "SettingsOutputTypeDef",
     "InstanceSummaryTypeDef",
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    "ListIdentityProvidersRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "ListIdentityProvidersRequestRequestTypeDef",
     "SettingsTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateSettingsTypeDef",
-    "IdentityProviderOutputTypeDef",
     "IdentityProviderTypeDef",
-    "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
-    "IdentityProviderSummaryTypeDef",
-    "InstanceUserSummaryTypeDef",
-    "ProductUserSummaryTypeDef",
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     "AssociateUserRequestRequestTypeDef",
     "DeregisterIdentityProviderRequestRequestTypeDef",
     "DisassociateUserRequestRequestTypeDef",
+    "IdentityProviderSummaryTypeDef",
+    "InstanceUserSummaryTypeDef",
     "ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     "ListProductSubscriptionsRequestRequestTypeDef",
     "ListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     "ListUserAssociationsRequestRequestTypeDef",
+    "ProductUserSummaryTypeDef",
     "RegisterIdentityProviderRequestRequestTypeDef",
     "StartProductSubscriptionRequestRequestTypeDef",
     "StopProductSubscriptionRequestRequestTypeDef",
     "UpdateIdentityProviderSettingsRequestRequestTypeDef",
     "DeregisterIdentityProviderResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "RegisterIdentityProviderResponseTypeDef",
@@ -58,28 +56,31 @@
     "DisassociateUserResponseTypeDef",
     "ListUserAssociationsResponseTypeDef",
     "ListProductSubscriptionsResponseTypeDef",
     "StartProductSubscriptionResponseTypeDef",
     "StopProductSubscriptionResponseTypeDef",
 )
 
-ActiveDirectoryIdentityProviderOutputTypeDef = TypedDict(
-    "ActiveDirectoryIdentityProviderOutputTypeDef",
+ActiveDirectoryIdentityProviderTypeDef = TypedDict(
+    "ActiveDirectoryIdentityProviderTypeDef",
     {
         "DirectoryId": str,
     },
     total=False,
 )
 
-ActiveDirectoryIdentityProviderTypeDef = TypedDict(
-    "ActiveDirectoryIdentityProviderTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "DirectoryId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Attribute": str,
         "Operation": str,
@@ -112,60 +113,41 @@
     },
     total=False,
 )
 
 class InstanceSummaryTypeDef(_RequiredInstanceSummaryTypeDef, _OptionalInstanceSummaryTypeDef):
     pass
 
-ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListIdentityProvidersRequestRequestTypeDef = TypedDict(
     "ListIdentityProvidersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "SecurityGroupId": str,
         "Subnets": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredUpdateSettingsTypeDef = TypedDict(
     "_RequiredUpdateSettingsTypeDef",
     {
         "AddSubnets": Sequence[str],
         "RemoveSubnets": Sequence[str],
     },
 )
@@ -176,39 +158,22 @@
     },
     total=False,
 )
 
 class UpdateSettingsTypeDef(_RequiredUpdateSettingsTypeDef, _OptionalUpdateSettingsTypeDef):
     pass
 
-IdentityProviderOutputTypeDef = TypedDict(
-    "IdentityProviderOutputTypeDef",
-    {
-        "ActiveDirectoryIdentityProvider": ActiveDirectoryIdentityProviderOutputTypeDef,
-    },
-    total=False,
-)
-
 IdentityProviderTypeDef = TypedDict(
     "IdentityProviderTypeDef",
     {
         "ActiveDirectoryIdentityProvider": ActiveDirectoryIdentityProviderTypeDef,
     },
     total=False,
 )
 
-ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
-    "ListInstancesRequestListInstancesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInstancesRequestRequestTypeDef = TypedDict(
     "ListInstancesRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -216,152 +181,144 @@
 )
 
 ListInstancesResponseTypeDef = TypedDict(
     "ListInstancesResponseTypeDef",
     {
         "InstanceSummaries": List[InstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredIdentityProviderSummaryTypeDef = TypedDict(
-    "_RequiredIdentityProviderSummaryTypeDef",
+ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     {
-        "IdentityProvider": IdentityProviderOutputTypeDef,
-        "Product": str,
-        "Settings": SettingsOutputTypeDef,
-        "Status": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalIdentityProviderSummaryTypeDef = TypedDict(
-    "_OptionalIdentityProviderSummaryTypeDef",
+
+ListInstancesRequestListInstancesPaginateTypeDef = TypedDict(
+    "ListInstancesRequestListInstancesPaginateTypeDef",
     {
-        "FailureMessage": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class IdentityProviderSummaryTypeDef(
-    _RequiredIdentityProviderSummaryTypeDef, _OptionalIdentityProviderSummaryTypeDef
-):
-    pass
-
-_RequiredInstanceUserSummaryTypeDef = TypedDict(
-    "_RequiredInstanceUserSummaryTypeDef",
+_RequiredAssociateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateUserRequestRequestTypeDef",
     {
-        "IdentityProvider": IdentityProviderOutputTypeDef,
+        "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
-        "Status": str,
         "Username": str,
     },
 )
-_OptionalInstanceUserSummaryTypeDef = TypedDict(
-    "_OptionalInstanceUserSummaryTypeDef",
+_OptionalAssociateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateUserRequestRequestTypeDef",
     {
-        "AssociationDate": str,
-        "DisassociationDate": str,
         "Domain": str,
-        "StatusMessage": str,
     },
     total=False,
 )
 
-class InstanceUserSummaryTypeDef(
-    _RequiredInstanceUserSummaryTypeDef, _OptionalInstanceUserSummaryTypeDef
+class AssociateUserRequestRequestTypeDef(
+    _RequiredAssociateUserRequestRequestTypeDef, _OptionalAssociateUserRequestRequestTypeDef
 ):
     pass
 
-_RequiredProductUserSummaryTypeDef = TypedDict(
-    "_RequiredProductUserSummaryTypeDef",
+DeregisterIdentityProviderRequestRequestTypeDef = TypedDict(
+    "DeregisterIdentityProviderRequestRequestTypeDef",
     {
-        "IdentityProvider": IdentityProviderOutputTypeDef,
+        "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
-        "Status": str,
-        "Username": str,
     },
 )
-_OptionalProductUserSummaryTypeDef = TypedDict(
-    "_OptionalProductUserSummaryTypeDef",
-    {
-        "Domain": str,
-        "StatusMessage": str,
-        "SubscriptionEndDate": str,
-        "SubscriptionStartDate": str,
-    },
-    total=False,
-)
-
-class ProductUserSummaryTypeDef(
-    _RequiredProductUserSummaryTypeDef, _OptionalProductUserSummaryTypeDef
-):
-    pass
 
-_RequiredAssociateUserRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateUserRequestRequestTypeDef",
+_RequiredDisassociateUserRequestRequestTypeDef = TypedDict(
+    "_RequiredDisassociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
         "Username": str,
     },
 )
-_OptionalAssociateUserRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateUserRequestRequestTypeDef",
+_OptionalDisassociateUserRequestRequestTypeDef = TypedDict(
+    "_OptionalDisassociateUserRequestRequestTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
-class AssociateUserRequestRequestTypeDef(
-    _RequiredAssociateUserRequestRequestTypeDef, _OptionalAssociateUserRequestRequestTypeDef
+class DisassociateUserRequestRequestTypeDef(
+    _RequiredDisassociateUserRequestRequestTypeDef, _OptionalDisassociateUserRequestRequestTypeDef
 ):
     pass
 
-DeregisterIdentityProviderRequestRequestTypeDef = TypedDict(
-    "DeregisterIdentityProviderRequestRequestTypeDef",
+_RequiredIdentityProviderSummaryTypeDef = TypedDict(
+    "_RequiredIdentityProviderSummaryTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
+        "Settings": SettingsOutputTypeDef,
+        "Status": str,
     },
 )
+_OptionalIdentityProviderSummaryTypeDef = TypedDict(
+    "_OptionalIdentityProviderSummaryTypeDef",
+    {
+        "FailureMessage": str,
+    },
+    total=False,
+)
 
-_RequiredDisassociateUserRequestRequestTypeDef = TypedDict(
-    "_RequiredDisassociateUserRequestRequestTypeDef",
+class IdentityProviderSummaryTypeDef(
+    _RequiredIdentityProviderSummaryTypeDef, _OptionalIdentityProviderSummaryTypeDef
+):
+    pass
+
+_RequiredInstanceUserSummaryTypeDef = TypedDict(
+    "_RequiredInstanceUserSummaryTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
+        "Status": str,
         "Username": str,
     },
 )
-_OptionalDisassociateUserRequestRequestTypeDef = TypedDict(
-    "_OptionalDisassociateUserRequestRequestTypeDef",
+_OptionalInstanceUserSummaryTypeDef = TypedDict(
+    "_OptionalInstanceUserSummaryTypeDef",
     {
+        "AssociationDate": str,
+        "DisassociationDate": str,
         "Domain": str,
+        "StatusMessage": str,
     },
     total=False,
 )
 
-class DisassociateUserRequestRequestTypeDef(
-    _RequiredDisassociateUserRequestRequestTypeDef, _OptionalDisassociateUserRequestRequestTypeDef
+class InstanceUserSummaryTypeDef(
+    _RequiredInstanceUserSummaryTypeDef, _OptionalInstanceUserSummaryTypeDef
 ):
     pass
 
 _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef = TypedDict(
     "_RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
 _OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef = TypedDict(
     "_OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef(
     _RequiredListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     _OptionalListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
@@ -398,15 +355,15 @@
         "InstanceId": str,
     },
 )
 _OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef = TypedDict(
     "_OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListUserAssociationsRequestListUserAssociationsPaginateTypeDef(
     _RequiredListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
     _OptionalListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
@@ -432,14 +389,39 @@
 
 class ListUserAssociationsRequestRequestTypeDef(
     _RequiredListUserAssociationsRequestRequestTypeDef,
     _OptionalListUserAssociationsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredProductUserSummaryTypeDef = TypedDict(
+    "_RequiredProductUserSummaryTypeDef",
+    {
+        "IdentityProvider": IdentityProviderTypeDef,
+        "Product": str,
+        "Status": str,
+        "Username": str,
+    },
+)
+_OptionalProductUserSummaryTypeDef = TypedDict(
+    "_OptionalProductUserSummaryTypeDef",
+    {
+        "Domain": str,
+        "StatusMessage": str,
+        "SubscriptionEndDate": str,
+        "SubscriptionStartDate": str,
+    },
+    total=False,
+)
+
+class ProductUserSummaryTypeDef(
+    _RequiredProductUserSummaryTypeDef, _OptionalProductUserSummaryTypeDef
+):
+    pass
+
 _RequiredRegisterIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterIdentityProviderRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
     },
 )
@@ -510,85 +492,85 @@
     },
 )
 
 DeregisterIdentityProviderResponseTypeDef = TypedDict(
     "DeregisterIdentityProviderResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "IdentityProviderSummaries": List[IdentityProviderSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterIdentityProviderResponseTypeDef = TypedDict(
     "RegisterIdentityProviderResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIdentityProviderSettingsResponseTypeDef = TypedDict(
     "UpdateIdentityProviderSettingsResponseTypeDef",
     {
         "IdentityProviderSummary": IdentityProviderSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateUserResponseTypeDef = TypedDict(
     "AssociateUserResponseTypeDef",
     {
         "InstanceUserSummary": InstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateUserResponseTypeDef = TypedDict(
     "DisassociateUserResponseTypeDef",
     {
         "InstanceUserSummary": InstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserAssociationsResponseTypeDef = TypedDict(
     "ListUserAssociationsResponseTypeDef",
     {
         "InstanceUserSummaries": List[InstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProductSubscriptionsResponseTypeDef = TypedDict(
     "ListProductSubscriptionsResponseTypeDef",
     {
         "NextToken": str,
         "ProductUserSummaries": List[ProductUserSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartProductSubscriptionResponseTypeDef = TypedDict(
     "StartProductSubscriptionResponseTypeDef",
     {
         "ProductUserSummary": ProductUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopProductSubscriptionResponseTypeDef = TypedDict(
     "StopProductSubscriptionResponseTypeDef",
     {
         "ProductUserSummary": ProductUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-user-subscriptions
-Version: 1.28.12
-Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-user-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-user-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerUserSubscriptions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
+[boto3.LicenseManagerUserSubscriptions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions)
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
 [mypy-boto3-license-manager-user-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,40 +346,38 @@
 
 `mypy_boto3_license_manager_user_subscriptions.type_defs` module contains
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_user_subscriptions.type_defs import (
-    ActiveDirectoryIdentityProviderOutputTypeDef,
     ActiveDirectoryIdentityProviderTypeDef,
+    ResponseMetadataTypeDef,
     FilterTypeDef,
     SettingsOutputTypeDef,
     InstanceSummaryTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListIdentityProvidersRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    ListIdentityProvidersRequestRequestTypeDef,
     SettingsTypeDef,
-    ResponseMetadataTypeDef,
     UpdateSettingsTypeDef,
-    IdentityProviderOutputTypeDef,
     IdentityProviderTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListInstancesResponseTypeDef,
-    IdentityProviderSummaryTypeDef,
-    InstanceUserSummaryTypeDef,
-    ProductUserSummaryTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    ListInstancesRequestListInstancesPaginateTypeDef,
     AssociateUserRequestRequestTypeDef,
     DeregisterIdentityProviderRequestRequestTypeDef,
     DisassociateUserRequestRequestTypeDef,
+    IdentityProviderSummaryTypeDef,
+    InstanceUserSummaryTypeDef,
     ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
     ListProductSubscriptionsRequestRequestTypeDef,
     ListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
     ListUserAssociationsRequestRequestTypeDef,
+    ProductUserSummaryTypeDef,
     RegisterIdentityProviderRequestRequestTypeDef,
     StartProductSubscriptionRequestRequestTypeDef,
     StopProductSubscriptionRequestRequestTypeDef,
     UpdateIdentityProviderSettingsRequestRequestTypeDef,
     DeregisterIdentityProviderResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
@@ -389,15 +387,15 @@
     ListUserAssociationsResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveDirectoryIdentityProviderOutputTypeDef:
+def get_structure() -> ActiveDirectoryIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/mypy_boto3_license_manager_user_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-user-subscriptions-1.28.12/setup.py` & `mypy-boto3-license-manager-user-subscriptions-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager-user-subscriptions",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_license_manager_user_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.LicenseManagerUserSubscriptions 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

