# Comparing `tmp/mypy-boto3-license-manager-linux-subscriptions-1.28.12.tar.gz` & `tmp/mypy-boto3-license-manager-linux-subscriptions-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-linux-subscriptions-1.28.12.tar", last modified: Thu Jul 27 05:34:56 2023, max compression
+gzip compressed data, was "mypy-boto3-license-manager-linux-subscriptions-1.28.15.tar", last modified: Fri Jul 28 20:43:08 2023, max compression
```

## Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12.tar` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.096459 mypy-boto3-license-manager-linux-subscriptions-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-27 05:34:56.096459 mypy-boto3-license-manager-linux-subscriptions-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.088459 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-27 05:25:21.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.096459 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-27 05:34:55.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-27 05:34:55.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:55.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 05:34:55.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:56.096459 mypy-boto3-license-manager-linux-subscriptions-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.901386 mypy-boto3-license-manager-linux-subscriptions-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-28 20:43:08.893386 mypy-boto3-license-manager-linux-subscriptions-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.885386 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-07-28 20:30:11.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.893386 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 20:43:08.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:08.901386 mypy-boto3-license-manager-linux-subscriptions-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-28 20:30:10.000000 mypy-boto3-license-manager-linux-subscriptions-1.28.15/setup.py
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/LICENSE` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/PKG-INFO` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-linux-subscriptions
-Version: 1.28.12
-Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-linux-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-linux-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerLinuxSubscriptions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
+[boto3.LicenseManagerLinuxSubscriptions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
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
 [mypy-boto3-license-manager-linux-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,27 +345,27 @@
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_linux_subscriptions.type_defs import (
     FilterTypeDef,
     LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
+    ResponseMetadataTypeDef,
     InstanceTypeDef,
     LinuxSubscriptionsDiscoverySettingsTypeDef,
-    SubscriptionTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
+    SubscriptionTypeDef,
     ListLinuxSubscriptionInstancesRequestRequestTypeDef,
-    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
     UpdateServiceSettingsResponseTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
     UpdateServiceSettingsRequestRequestTypeDef,
+    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
+    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
 )
 
 
 def get_structure() -> FilterTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/README.md` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-linux-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-linux-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerLinuxSubscriptions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
+[boto3.LicenseManagerLinuxSubscriptions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
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
 [mypy-boto3-license-manager-linux-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,27 +313,27 @@
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_linux_subscriptions.type_defs import (
     FilterTypeDef,
     LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
+    ResponseMetadataTypeDef,
     InstanceTypeDef,
     LinuxSubscriptionsDiscoverySettingsTypeDef,
-    SubscriptionTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
+    SubscriptionTypeDef,
     ListLinuxSubscriptionInstancesRequestRequestTypeDef,
-    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
     UpdateServiceSettingsResponseTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
     UpdateServiceSettingsRequestRequestTypeDef,
+    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
+    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
 )
 
 
 def get_structure() -> FilterTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/__init__.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/__main__.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions\nOther"
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

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/client.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/client.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/literals.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/literals.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/paginator.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptioninstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLinuxSubscriptionInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Paginator.ListLinuxSubscriptionInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptioninstancespaginator)
         """
 
 
@@ -69,13 +69,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLinuxSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Paginator.ListLinuxSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptionspaginator)
         """
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptioninstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLinuxSubscriptionInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Paginator.ListLinuxSubscriptionInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptioninstancespaginator)
         """
 
 class ListLinuxSubscriptionsPaginator(Paginator):
@@ -65,13 +65,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLinuxSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Paginator.ListLinuxSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/paginators/#listlinuxsubscriptionspaginator)
         """
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/type_defs.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,27 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FilterTypeDef",
     "LinuxSubscriptionsDiscoverySettingsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "InstanceTypeDef",
     "LinuxSubscriptionsDiscoverySettingsTypeDef",
-    "SubscriptionTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
+    "SubscriptionTypeDef",
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
-    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsRequestRequestTypeDef",
     "GetServiceSettingsResponseTypeDef",
     "UpdateServiceSettingsResponseTypeDef",
     "ListLinuxSubscriptionInstancesResponseTypeDef",
     "UpdateServiceSettingsRequestRequestTypeDef",
+    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
+    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsResponseTypeDef",
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
@@ -60,14 +60,25 @@
     "LinuxSubscriptionsDiscoverySettingsOutputTypeDef",
     {
         "OrganizationIntegration": OrganizationIntegrationType,
         "SourceRegions": List[str],
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "AccountID": str,
         "AmiId": str,
         "InstanceID": str,
         "InstanceType": str,
@@ -85,73 +96,44 @@
     "LinuxSubscriptionsDiscoverySettingsTypeDef",
     {
         "OrganizationIntegration": OrganizationIntegrationType,
         "SourceRegions": Sequence[str],
     },
 )
 
-SubscriptionTypeDef = TypedDict(
-    "SubscriptionTypeDef",
-    {
-        "InstanceCount": int,
-        "Name": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
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
-ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef = TypedDict(
-    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
+SubscriptionTypeDef = TypedDict(
+    "SubscriptionTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "InstanceCount": int,
+        "Name": str,
+        "Type": str,
     },
     total=False,
 )
 
 ListLinuxSubscriptionInstancesRequestRequestTypeDef = TypedDict(
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef = TypedDict(
-    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLinuxSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListLinuxSubscriptionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -162,36 +144,36 @@
     "GetServiceSettingsResponseTypeDef",
     {
         "HomeRegions": List[str],
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
         "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
         "Status": StatusType,
         "StatusMessage": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceSettingsResponseTypeDef = TypedDict(
     "UpdateServiceSettingsResponseTypeDef",
     {
         "HomeRegions": List[str],
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
         "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
         "Status": StatusType,
         "StatusMessage": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLinuxSubscriptionInstancesResponseTypeDef = TypedDict(
     "ListLinuxSubscriptionInstancesResponseTypeDef",
     {
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceSettingsRequestRequestTypeDef",
     {
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
@@ -210,15 +192,33 @@
 class UpdateServiceSettingsRequestRequestTypeDef(
     _RequiredUpdateServiceSettingsRequestRequestTypeDef,
     _OptionalUpdateServiceSettingsRequestRequestTypeDef,
 ):
     pass
 
 
+ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef = TypedDict(
+    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef = TypedDict(
+    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListLinuxSubscriptionsResponseTypeDef = TypedDict(
     "ListLinuxSubscriptionsResponseTypeDef",
     {
         "NextToken": str,
         "Subscriptions": List[SubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,27 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FilterTypeDef",
     "LinuxSubscriptionsDiscoverySettingsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "InstanceTypeDef",
     "LinuxSubscriptionsDiscoverySettingsTypeDef",
-    "SubscriptionTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
+    "SubscriptionTypeDef",
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
-    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsRequestRequestTypeDef",
     "GetServiceSettingsResponseTypeDef",
     "UpdateServiceSettingsResponseTypeDef",
     "ListLinuxSubscriptionInstancesResponseTypeDef",
     "UpdateServiceSettingsRequestRequestTypeDef",
+    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
+    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsResponseTypeDef",
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
@@ -59,14 +59,25 @@
     "LinuxSubscriptionsDiscoverySettingsOutputTypeDef",
     {
         "OrganizationIntegration": OrganizationIntegrationType,
         "SourceRegions": List[str],
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "AccountID": str,
         "AmiId": str,
         "InstanceID": str,
         "InstanceType": str,
@@ -84,73 +95,44 @@
     "LinuxSubscriptionsDiscoverySettingsTypeDef",
     {
         "OrganizationIntegration": OrganizationIntegrationType,
         "SourceRegions": Sequence[str],
     },
 )
 
-SubscriptionTypeDef = TypedDict(
-    "SubscriptionTypeDef",
-    {
-        "InstanceCount": int,
-        "Name": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
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
-ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef = TypedDict(
-    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
+SubscriptionTypeDef = TypedDict(
+    "SubscriptionTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "InstanceCount": int,
+        "Name": str,
+        "Type": str,
     },
     total=False,
 )
 
 ListLinuxSubscriptionInstancesRequestRequestTypeDef = TypedDict(
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef = TypedDict(
-    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLinuxSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListLinuxSubscriptionsRequestRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -161,36 +143,36 @@
     "GetServiceSettingsResponseTypeDef",
     {
         "HomeRegions": List[str],
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
         "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
         "Status": StatusType,
         "StatusMessage": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceSettingsResponseTypeDef = TypedDict(
     "UpdateServiceSettingsResponseTypeDef",
     {
         "HomeRegions": List[str],
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
         "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
         "Status": StatusType,
         "StatusMessage": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLinuxSubscriptionInstancesResponseTypeDef = TypedDict(
     "ListLinuxSubscriptionInstancesResponseTypeDef",
     {
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceSettingsRequestRequestTypeDef",
     {
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
@@ -207,15 +189,33 @@
 
 class UpdateServiceSettingsRequestRequestTypeDef(
     _RequiredUpdateServiceSettingsRequestRequestTypeDef,
     _OptionalUpdateServiceSettingsRequestRequestTypeDef,
 ):
     pass
 
+ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef = TypedDict(
+    "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef = TypedDict(
+    "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListLinuxSubscriptionsResponseTypeDef = TypedDict(
     "ListLinuxSubscriptionsResponseTypeDef",
     {
         "NextToken": str,
         "Subscriptions": List[SubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager-linux-subscriptions
-Version: 1.28.12
-Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager-linux-subscriptions.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager-linux-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager-linux-subscriptions)](https://pepy.tech/project/mypy-boto3-license-manager-linux-subscriptions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManagerLinuxSubscriptions 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
+[boto3.LicenseManagerLinuxSubscriptions 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
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
 [mypy-boto3-license-manager-linux-subscriptions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager_linux_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,27 +345,27 @@
 structures and shapes assembled to typed dictionaries for additional type
 checking.
 
 ```python
 from mypy_boto3_license_manager_linux_subscriptions.type_defs import (
     FilterTypeDef,
     LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
+    ResponseMetadataTypeDef,
     InstanceTypeDef,
     LinuxSubscriptionsDiscoverySettingsTypeDef,
-    SubscriptionTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
+    SubscriptionTypeDef,
     ListLinuxSubscriptionInstancesRequestRequestTypeDef,
-    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsRequestRequestTypeDef,
     GetServiceSettingsResponseTypeDef,
     UpdateServiceSettingsResponseTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
     UpdateServiceSettingsRequestRequestTypeDef,
+    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
+    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
 )
 
 
 def get_structure() -> FilterTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/mypy_boto3_license_manager_linux_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-linux-subscriptions-1.28.12/setup.py` & `mypy-boto3-license-manager-linux-subscriptions-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager-linux-subscriptions",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_license_manager_linux_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.LicenseManagerLinuxSubscriptions 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

