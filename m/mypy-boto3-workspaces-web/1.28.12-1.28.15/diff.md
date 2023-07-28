# Comparing `tmp/mypy-boto3-workspaces-web-1.28.12.tar.gz` & `tmp/mypy-boto3-workspaces-web-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-web-1.28.12.tar", last modified: Thu Jul 27 11:49:51 2023, max compression
+gzip compressed data, was "mypy-boto3-workspaces-web-1.28.15.tar", last modified: Fri Jul 28 20:43:58 2023, max compression
```

## Comparing `mypy-boto3-workspaces-web-1.28.12.tar` & `mypy-boto3-workspaces-web-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.197507 mypy-boto3-workspaces-web-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17486 2023-07-27 11:49:51.197507 mypy-boto3-workspaces-web-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15972 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.197507 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37970 2023-07-27 11:49:03.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37906 2023-07-27 11:49:03.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-07-27 11:49:03.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-27 11:49:03.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41836 2023-07-27 11:49:04.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41783 2023-07-27 11:49:03.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:51.197507 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17486 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:51.000000 mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:51.197507 mypy-boto3-workspaces-web-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 11:49:02.000000 mypy-boto3-workspaces-web-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:58.202062 mypy-boto3-workspaces-web-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:47.000000 mypy-boto3-workspaces-web-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17439 2023-07-28 20:43:58.202062 mypy-boto3-workspaces-web-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15925 2023-07-28 20:41:47.000000 mypy-boto3-workspaces-web-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:58.202062 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-28 20:41:47.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-28 20:41:47.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:41:47.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37970 2023-07-28 20:41:47.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37906 2023-07-28 20:41:47.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-07-28 20:41:47.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-28 20:41:47.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:47.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41306 2023-07-28 20:41:48.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41255 2023-07-28 20:41:48.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:47.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:58.202062 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17439 2023-07-28 20:43:58.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-28 20:43:58.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:58.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:58.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:58.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:58.000000 mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:58.202062 mypy-boto3-workspaces-web-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:41:47.000000 mypy-boto3-workspaces-web-1.28.15/setup.py
```

### Comparing `mypy-boto3-workspaces-web-1.28.12/LICENSE` & `mypy-boto3-workspaces-web-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.12/PKG-INFO` & `mypy-boto3-workspaces-web-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces-web
-Version: 1.28.12
-Summary: Type annotations for boto3.WorkSpacesWeb 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.WorkSpacesWeb 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-web)](https://pepy.tech/project/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,24 +349,22 @@
     TrustStoreTypeDef,
     GetUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsTypeDef,
     GetUserSettingsRequestRequestTypeDef,
     UserSettingsTypeDef,
     IdentityProviderSummaryTypeDef,
     IpAccessSettingsSummaryTypeDef,
-    IpRuleOutputTypeDef,
     ListBrowserSettingsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ListIpAccessSettingsRequestRequestTypeDef,
     ListNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsSummaryTypeDef,
     ListPortalsRequestRequestTypeDef,
     PortalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListTrustStoreCertificatesRequestRequestTypeDef,
     ListTrustStoresRequestRequestTypeDef,
     TrustStoreSummaryTypeDef,
     ListUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsSummaryTypeDef,
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
@@ -401,34 +399,34 @@
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
     CreatePortalRequestRequestTypeDef,
     CreateTrustStoreRequestRequestTypeDef,
     CreateUserAccessLoggingSettingsRequestRequestTypeDef,
     CreateUserSettingsRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIpAccessSettingsRequestRequestTypeDef,
+    IpAccessSettingsTypeDef,
     UpdateIpAccessSettingsRequestRequestTypeDef,
     GetIdentityProviderResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     GetNetworkSettingsResponseTypeDef,
     UpdateNetworkSettingsResponseTypeDef,
     GetPortalResponseTypeDef,
     UpdatePortalResponseTypeDef,
     GetTrustStoreResponseTypeDef,
     GetUserAccessLoggingSettingsResponseTypeDef,
     UpdateUserAccessLoggingSettingsResponseTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListIpAccessSettingsResponseTypeDef,
-    IpAccessSettingsTypeDef,
     ListNetworkSettingsResponseTypeDef,
     ListPortalsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTrustStoresResponseTypeDef,
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     GetIpAccessSettingsResponseTypeDef,
     UpdateIpAccessSettingsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-workspaces-web-1.28.12/README.md` & `mypy-boto3-workspaces-web-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-web)](https://pepy.tech/project/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,24 +317,22 @@
     TrustStoreTypeDef,
     GetUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsTypeDef,
     GetUserSettingsRequestRequestTypeDef,
     UserSettingsTypeDef,
     IdentityProviderSummaryTypeDef,
     IpAccessSettingsSummaryTypeDef,
-    IpRuleOutputTypeDef,
     ListBrowserSettingsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ListIpAccessSettingsRequestRequestTypeDef,
     ListNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsSummaryTypeDef,
     ListPortalsRequestRequestTypeDef,
     PortalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListTrustStoreCertificatesRequestRequestTypeDef,
     ListTrustStoresRequestRequestTypeDef,
     TrustStoreSummaryTypeDef,
     ListUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsSummaryTypeDef,
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
@@ -369,34 +367,34 @@
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
     CreatePortalRequestRequestTypeDef,
     CreateTrustStoreRequestRequestTypeDef,
     CreateUserAccessLoggingSettingsRequestRequestTypeDef,
     CreateUserSettingsRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIpAccessSettingsRequestRequestTypeDef,
+    IpAccessSettingsTypeDef,
     UpdateIpAccessSettingsRequestRequestTypeDef,
     GetIdentityProviderResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     GetNetworkSettingsResponseTypeDef,
     UpdateNetworkSettingsResponseTypeDef,
     GetPortalResponseTypeDef,
     UpdatePortalResponseTypeDef,
     GetTrustStoreResponseTypeDef,
     GetUserAccessLoggingSettingsResponseTypeDef,
     UpdateUserAccessLoggingSettingsResponseTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListIpAccessSettingsResponseTypeDef,
-    IpAccessSettingsTypeDef,
     ListNetworkSettingsResponseTypeDef,
     ListPortalsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTrustStoresResponseTypeDef,
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     GetIpAccessSettingsResponseTypeDef,
     UpdateIpAccessSettingsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/__main__.py` & `mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkSpacesWeb 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.WorkSpacesWeb 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb\nOther"
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

### Comparing `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/client.py` & `mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/client.pyi` & `mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/literals.py` & `mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/literals.pyi` & `mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/type_defs.py` & `mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateBrowserSettingsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpAccessSettingsRequestRequestTypeDef",
     "AssociateNetworkSettingsRequestRequestTypeDef",
     "AssociateTrustStoreRequestRequestTypeDef",
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
@@ -77,24 +76,22 @@
     "TrustStoreTypeDef",
     "GetUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsTypeDef",
     "GetUserSettingsRequestRequestTypeDef",
     "UserSettingsTypeDef",
     "IdentityProviderSummaryTypeDef",
     "IpAccessSettingsSummaryTypeDef",
-    "IpRuleOutputTypeDef",
     "ListBrowserSettingsRequestRequestTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
     "ListIpAccessSettingsRequestRequestTypeDef",
     "ListNetworkSettingsRequestRequestTypeDef",
     "NetworkSettingsSummaryTypeDef",
     "ListPortalsRequestRequestTypeDef",
     "PortalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListTrustStoreCertificatesRequestRequestTypeDef",
     "ListTrustStoresRequestRequestTypeDef",
     "TrustStoreSummaryTypeDef",
     "ListUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsSummaryTypeDef",
     "ListUserSettingsRequestRequestTypeDef",
     "UserSettingsSummaryTypeDef",
@@ -129,34 +126,34 @@
     "GetTrustStoreCertificateResponseTypeDef",
     "CreateBrowserSettingsRequestRequestTypeDef",
     "CreateNetworkSettingsRequestRequestTypeDef",
     "CreatePortalRequestRequestTypeDef",
     "CreateTrustStoreRequestRequestTypeDef",
     "CreateUserAccessLoggingSettingsRequestRequestTypeDef",
     "CreateUserSettingsRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIpAccessSettingsRequestRequestTypeDef",
+    "IpAccessSettingsTypeDef",
     "UpdateIpAccessSettingsRequestRequestTypeDef",
     "GetIdentityProviderResponseTypeDef",
     "UpdateIdentityProviderResponseTypeDef",
     "GetNetworkSettingsResponseTypeDef",
     "UpdateNetworkSettingsResponseTypeDef",
     "GetPortalResponseTypeDef",
     "UpdatePortalResponseTypeDef",
     "GetTrustStoreResponseTypeDef",
     "GetUserAccessLoggingSettingsResponseTypeDef",
     "UpdateUserAccessLoggingSettingsResponseTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "ListIpAccessSettingsResponseTypeDef",
-    "IpAccessSettingsTypeDef",
     "ListNetworkSettingsResponseTypeDef",
     "ListPortalsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTrustStoresResponseTypeDef",
     "ListUserAccessLoggingSettingsResponseTypeDef",
     "ListUserSettingsResponseTypeDef",
     "GetIpAccessSettingsResponseTypeDef",
     "UpdateIpAccessSettingsResponseTypeDef",
 )
 
@@ -238,19 +235,17 @@
     {
         "associatedPortalArns": List[str],
         "browserPolicy": str,
     },
     total=False,
 )
 
-
 class BrowserSettingsTypeDef(_RequiredBrowserSettingsTypeDef, _OptionalBrowserSettingsTypeDef):
     pass
 
-
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "issuer": str,
         "notValidAfter": datetime,
         "notValidBefore": datetime,
         "subject": str,
@@ -293,41 +288,37 @@
     "_OptionalCreateIdentityProviderRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredIpRuleTypeDef = TypedDict(
     "_RequiredIpRuleTypeDef",
     {
         "ipRange": str,
     },
 )
 _OptionalIpRuleTypeDef = TypedDict(
     "_OptionalIpRuleTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class IpRuleTypeDef(_RequiredIpRuleTypeDef, _OptionalIpRuleTypeDef):
     pass
 
-
 DeleteBrowserSettingsRequestRequestTypeDef = TypedDict(
     "DeleteBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
     },
 )
 
@@ -448,19 +439,17 @@
         "identityProviderDetails": Dict[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
     total=False,
 )
 
-
 class IdentityProviderTypeDef(_RequiredIdentityProviderTypeDef, _OptionalIdentityProviderTypeDef):
     pass
 
-
 GetIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "GetIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
     },
 )
 
@@ -484,19 +473,17 @@
         "securityGroupIds": List[str],
         "subnetIds": List[str],
         "vpcId": str,
     },
     total=False,
 )
 
-
 class NetworkSettingsTypeDef(_RequiredNetworkSettingsTypeDef, _OptionalNetworkSettingsTypeDef):
     pass
 
-
 GetPortalRequestRequestTypeDef = TypedDict(
     "GetPortalRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
@@ -571,21 +558,19 @@
     {
         "associatedPortalArns": List[str],
         "kinesisStreamArn": str,
     },
     total=False,
 )
 
-
 class UserAccessLoggingSettingsTypeDef(
     _RequiredUserAccessLoggingSettingsTypeDef, _OptionalUserAccessLoggingSettingsTypeDef
 ):
     pass
 
-
 GetUserSettingsRequestRequestTypeDef = TypedDict(
     "GetUserSettingsRequestRequestTypeDef",
     {
         "userSettingsArn": str,
     },
 )
 
@@ -606,19 +591,17 @@
         "pasteAllowed": EnabledTypeType,
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
     },
     total=False,
 )
 
-
 class UserSettingsTypeDef(_RequiredUserSettingsTypeDef, _OptionalUserSettingsTypeDef):
     pass
 
-
 IdentityProviderSummaryTypeDef = TypedDict(
     "IdentityProviderSummaryTypeDef",
     {
         "identityProviderArn": str,
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
@@ -632,33 +615,14 @@
         "description": str,
         "displayName": str,
         "ipAccessSettingsArn": str,
     },
     total=False,
 )
 
-_RequiredIpRuleOutputTypeDef = TypedDict(
-    "_RequiredIpRuleOutputTypeDef",
-    {
-        "ipRange": str,
-    },
-)
-_OptionalIpRuleOutputTypeDef = TypedDict(
-    "_OptionalIpRuleOutputTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-
-class IpRuleOutputTypeDef(_RequiredIpRuleOutputTypeDef, _OptionalIpRuleOutputTypeDef):
-    pass
-
-
 ListBrowserSettingsRequestRequestTypeDef = TypedDict(
     "ListBrowserSettingsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -675,22 +639,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListIdentityProvidersRequestRequestTypeDef(
     _RequiredListIdentityProvidersRequestRequestTypeDef,
     _OptionalListIdentityProvidersRequestRequestTypeDef,
 ):
     pass
 
-
 ListIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "ListIpAccessSettingsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -747,22 +709,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
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
 _RequiredListTrustStoreCertificatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTrustStoreCertificatesRequestRequestTypeDef",
     {
         "trustStoreArn": str,
     },
 )
 _OptionalListTrustStoreCertificatesRequestRequestTypeDef = TypedDict(
@@ -770,22 +724,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTrustStoreCertificatesRequestRequestTypeDef(
     _RequiredListTrustStoreCertificatesRequestRequestTypeDef,
     _OptionalListTrustStoreCertificatesRequestRequestTypeDef,
 ):
     pass
 
-
 ListTrustStoresRequestRequestTypeDef = TypedDict(
     "ListTrustStoresRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -860,22 +812,20 @@
     {
         "browserPolicy": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateBrowserSettingsRequestRequestTypeDef(
     _RequiredUpdateBrowserSettingsRequestRequestTypeDef,
     _OptionalUpdateBrowserSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentityProviderRequestRequestTypeDef",
     {
         "identityProviderArn": str,
     },
 )
 _OptionalUpdateIdentityProviderRequestRequestTypeDef = TypedDict(
@@ -885,22 +835,20 @@
         "identityProviderDetails": Mapping[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
     total=False,
 )
 
-
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
     },
 )
 _OptionalUpdateNetworkSettingsRequestRequestTypeDef = TypedDict(
@@ -910,22 +858,20 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "vpcId": str,
     },
     total=False,
 )
 
-
 class UpdateNetworkSettingsRequestRequestTypeDef(
     _RequiredUpdateNetworkSettingsRequestRequestTypeDef,
     _OptionalUpdateNetworkSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdatePortalRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePortalRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 _OptionalUpdatePortalRequestRequestTypeDef = TypedDict(
@@ -933,21 +879,19 @@
     {
         "authenticationType": AuthenticationTypeType,
         "displayName": str,
     },
     total=False,
 )
 
-
 class UpdatePortalRequestRequestTypeDef(
     _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateTrustStoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrustStoreRequestRequestTypeDef",
     {
         "trustStoreArn": str,
     },
 )
 _OptionalUpdateTrustStoreRequestRequestTypeDef = TypedDict(
@@ -956,21 +900,19 @@
         "certificatesToAdd": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
         "certificatesToDelete": Sequence[str],
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateTrustStoreRequestRequestTypeDef(
     _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "userAccessLoggingSettingsArn": str,
     },
 )
 _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -978,22 +920,20 @@
     {
         "clientToken": str,
         "kinesisStreamArn": str,
     },
     total=False,
 )
 
-
 class UpdateUserAccessLoggingSettingsRequestRequestTypeDef(
     _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateUserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserSettingsRequestRequestTypeDef",
     {
         "userSettingsArn": str,
     },
 )
 _OptionalUpdateUserSettingsRequestRequestTypeDef = TypedDict(
@@ -1007,22 +947,20 @@
         "pasteAllowed": EnabledTypeType,
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
     },
     total=False,
 )
 
-
 class UpdateUserSettingsRequestRequestTypeDef(
     _RequiredUpdateUserSettingsRequestRequestTypeDef,
     _OptionalUpdateUserSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 AssociateBrowserSettingsResponseTypeDef = TypedDict(
     "AssociateBrowserSettingsResponseTypeDef",
     {
         "browserSettingsArn": str,
         "portalArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1212,22 +1150,20 @@
         "clientToken": str,
         "customerManagedKey": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateBrowserSettingsRequestRequestTypeDef(
     _RequiredCreateBrowserSettingsRequestRequestTypeDef,
     _OptionalCreateBrowserSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkSettingsRequestRequestTypeDef",
     {
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "vpcId": str,
     },
@@ -1237,22 +1173,20 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateNetworkSettingsRequestRequestTypeDef(
     _RequiredCreateNetworkSettingsRequestRequestTypeDef,
     _OptionalCreateNetworkSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 CreatePortalRequestRequestTypeDef = TypedDict(
     "CreatePortalRequestRequestTypeDef",
     {
         "additionalEncryptionContext": Mapping[str, str],
         "authenticationType": AuthenticationTypeType,
         "clientToken": str,
         "customerManagedKey": str,
@@ -1273,21 +1207,19 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateTrustStoreRequestRequestTypeDef(
     _RequiredCreateTrustStoreRequestRequestTypeDef, _OptionalCreateTrustStoreRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "kinesisStreamArn": str,
     },
 )
 _OptionalCreateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -1295,22 +1227,20 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateUserAccessLoggingSettingsRequestRequestTypeDef(
     _RequiredCreateUserAccessLoggingSettingsRequestRequestTypeDef,
     _OptionalCreateUserAccessLoggingSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateUserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserSettingsRequestRequestTypeDef",
     {
         "copyAllowed": EnabledTypeType,
         "downloadAllowed": EnabledTypeType,
         "pasteAllowed": EnabledTypeType,
         "printAllowed": EnabledTypeType,
@@ -1324,21 +1254,27 @@
         "disconnectTimeoutInMinutes": int,
         "idleDisconnectTimeoutInMinutes": int,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateUserSettingsRequestRequestTypeDef(
     _RequiredCreateUserSettingsRequestRequestTypeDef,
     _OptionalCreateUserSettingsRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
@@ -1347,21 +1283,19 @@
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipRules": Sequence[IpRuleTypeDef],
     },
 )
 _OptionalCreateIpAccessSettingsRequestRequestTypeDef = TypedDict(
@@ -1373,21 +1307,40 @@
         "description": str,
         "displayName": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateIpAccessSettingsRequestRequestTypeDef(
     _RequiredCreateIpAccessSettingsRequestRequestTypeDef,
     _OptionalCreateIpAccessSettingsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredIpAccessSettingsTypeDef = TypedDict(
+    "_RequiredIpAccessSettingsTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+    },
+)
+_OptionalIpAccessSettingsTypeDef = TypedDict(
+    "_OptionalIpAccessSettingsTypeDef",
+    {
+        "associatedPortalArns": List[str],
+        "creationDate": datetime,
+        "description": str,
+        "displayName": str,
+        "ipRules": List[IpRuleTypeDef],
+    },
+    total=False,
+)
+
+class IpAccessSettingsTypeDef(_RequiredIpAccessSettingsTypeDef, _OptionalIpAccessSettingsTypeDef):
+    pass
 
 _RequiredUpdateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
     },
 )
@@ -1398,22 +1351,20 @@
         "description": str,
         "displayName": str,
         "ipRules": Sequence[IpRuleTypeDef],
     },
     total=False,
 )
 
-
 class UpdateIpAccessSettingsRequestRequestTypeDef(
     _RequiredUpdateIpAccessSettingsRequestRequestTypeDef,
     _OptionalUpdateIpAccessSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 GetIdentityProviderResponseTypeDef = TypedDict(
     "GetIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1512,37 +1463,14 @@
     {
         "ipAccessSettings": List[IpAccessSettingsSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredIpAccessSettingsTypeDef = TypedDict(
-    "_RequiredIpAccessSettingsTypeDef",
-    {
-        "ipAccessSettingsArn": str,
-    },
-)
-_OptionalIpAccessSettingsTypeDef = TypedDict(
-    "_OptionalIpAccessSettingsTypeDef",
-    {
-        "associatedPortalArns": List[str],
-        "creationDate": datetime,
-        "description": str,
-        "displayName": str,
-        "ipRules": List[IpRuleOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class IpAccessSettingsTypeDef(_RequiredIpAccessSettingsTypeDef, _OptionalIpAccessSettingsTypeDef):
-    pass
-
-
 ListNetworkSettingsResponseTypeDef = TypedDict(
     "ListNetworkSettingsResponseTypeDef",
     {
         "networkSettings": List[NetworkSettingsSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1553,22 +1481,14 @@
     {
         "nextToken": str,
         "portals": List[PortalSummaryTypeDef],
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
 ListTrustStoresResponseTypeDef = TypedDict(
     "ListTrustStoresResponseTypeDef",
     {
         "nextToken": str,
         "trustStores": List[TrustStoreSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web/type_defs.pyi` & `mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateBrowserSettingsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpAccessSettingsRequestRequestTypeDef",
     "AssociateNetworkSettingsRequestRequestTypeDef",
     "AssociateTrustStoreRequestRequestTypeDef",
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
@@ -76,24 +77,22 @@
     "TrustStoreTypeDef",
     "GetUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsTypeDef",
     "GetUserSettingsRequestRequestTypeDef",
     "UserSettingsTypeDef",
     "IdentityProviderSummaryTypeDef",
     "IpAccessSettingsSummaryTypeDef",
-    "IpRuleOutputTypeDef",
     "ListBrowserSettingsRequestRequestTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
     "ListIpAccessSettingsRequestRequestTypeDef",
     "ListNetworkSettingsRequestRequestTypeDef",
     "NetworkSettingsSummaryTypeDef",
     "ListPortalsRequestRequestTypeDef",
     "PortalSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListTrustStoreCertificatesRequestRequestTypeDef",
     "ListTrustStoresRequestRequestTypeDef",
     "TrustStoreSummaryTypeDef",
     "ListUserAccessLoggingSettingsRequestRequestTypeDef",
     "UserAccessLoggingSettingsSummaryTypeDef",
     "ListUserSettingsRequestRequestTypeDef",
     "UserSettingsSummaryTypeDef",
@@ -128,34 +127,34 @@
     "GetTrustStoreCertificateResponseTypeDef",
     "CreateBrowserSettingsRequestRequestTypeDef",
     "CreateNetworkSettingsRequestRequestTypeDef",
     "CreatePortalRequestRequestTypeDef",
     "CreateTrustStoreRequestRequestTypeDef",
     "CreateUserAccessLoggingSettingsRequestRequestTypeDef",
     "CreateUserSettingsRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIpAccessSettingsRequestRequestTypeDef",
+    "IpAccessSettingsTypeDef",
     "UpdateIpAccessSettingsRequestRequestTypeDef",
     "GetIdentityProviderResponseTypeDef",
     "UpdateIdentityProviderResponseTypeDef",
     "GetNetworkSettingsResponseTypeDef",
     "UpdateNetworkSettingsResponseTypeDef",
     "GetPortalResponseTypeDef",
     "UpdatePortalResponseTypeDef",
     "GetTrustStoreResponseTypeDef",
     "GetUserAccessLoggingSettingsResponseTypeDef",
     "UpdateUserAccessLoggingSettingsResponseTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsResponseTypeDef",
     "ListIdentityProvidersResponseTypeDef",
     "ListIpAccessSettingsResponseTypeDef",
-    "IpAccessSettingsTypeDef",
     "ListNetworkSettingsResponseTypeDef",
     "ListPortalsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTrustStoresResponseTypeDef",
     "ListUserAccessLoggingSettingsResponseTypeDef",
     "ListUserSettingsResponseTypeDef",
     "GetIpAccessSettingsResponseTypeDef",
     "UpdateIpAccessSettingsResponseTypeDef",
 )
 
@@ -237,17 +236,19 @@
     {
         "associatedPortalArns": List[str],
         "browserPolicy": str,
     },
     total=False,
 )
 
+
 class BrowserSettingsTypeDef(_RequiredBrowserSettingsTypeDef, _OptionalBrowserSettingsTypeDef):
     pass
 
+
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "issuer": str,
         "notValidAfter": datetime,
         "notValidBefore": datetime,
         "subject": str,
@@ -290,37 +291,41 @@
     "_OptionalCreateIdentityProviderRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredIpRuleTypeDef = TypedDict(
     "_RequiredIpRuleTypeDef",
     {
         "ipRange": str,
     },
 )
 _OptionalIpRuleTypeDef = TypedDict(
     "_OptionalIpRuleTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class IpRuleTypeDef(_RequiredIpRuleTypeDef, _OptionalIpRuleTypeDef):
     pass
 
+
 DeleteBrowserSettingsRequestRequestTypeDef = TypedDict(
     "DeleteBrowserSettingsRequestRequestTypeDef",
     {
         "browserSettingsArn": str,
     },
 )
 
@@ -441,17 +446,19 @@
         "identityProviderDetails": Dict[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
     total=False,
 )
 
+
 class IdentityProviderTypeDef(_RequiredIdentityProviderTypeDef, _OptionalIdentityProviderTypeDef):
     pass
 
+
 GetIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "GetIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
     },
 )
 
@@ -475,17 +482,19 @@
         "securityGroupIds": List[str],
         "subnetIds": List[str],
         "vpcId": str,
     },
     total=False,
 )
 
+
 class NetworkSettingsTypeDef(_RequiredNetworkSettingsTypeDef, _OptionalNetworkSettingsTypeDef):
     pass
 
+
 GetPortalRequestRequestTypeDef = TypedDict(
     "GetPortalRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 
@@ -560,19 +569,21 @@
     {
         "associatedPortalArns": List[str],
         "kinesisStreamArn": str,
     },
     total=False,
 )
 
+
 class UserAccessLoggingSettingsTypeDef(
     _RequiredUserAccessLoggingSettingsTypeDef, _OptionalUserAccessLoggingSettingsTypeDef
 ):
     pass
 
+
 GetUserSettingsRequestRequestTypeDef = TypedDict(
     "GetUserSettingsRequestRequestTypeDef",
     {
         "userSettingsArn": str,
     },
 )
 
@@ -593,17 +604,19 @@
         "pasteAllowed": EnabledTypeType,
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
     },
     total=False,
 )
 
+
 class UserSettingsTypeDef(_RequiredUserSettingsTypeDef, _OptionalUserSettingsTypeDef):
     pass
 
+
 IdentityProviderSummaryTypeDef = TypedDict(
     "IdentityProviderSummaryTypeDef",
     {
         "identityProviderArn": str,
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
@@ -617,31 +630,14 @@
         "description": str,
         "displayName": str,
         "ipAccessSettingsArn": str,
     },
     total=False,
 )
 
-_RequiredIpRuleOutputTypeDef = TypedDict(
-    "_RequiredIpRuleOutputTypeDef",
-    {
-        "ipRange": str,
-    },
-)
-_OptionalIpRuleOutputTypeDef = TypedDict(
-    "_OptionalIpRuleOutputTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-class IpRuleOutputTypeDef(_RequiredIpRuleOutputTypeDef, _OptionalIpRuleOutputTypeDef):
-    pass
-
 ListBrowserSettingsRequestRequestTypeDef = TypedDict(
     "ListBrowserSettingsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -658,20 +654,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListIdentityProvidersRequestRequestTypeDef(
     _RequiredListIdentityProvidersRequestRequestTypeDef,
     _OptionalListIdentityProvidersRequestRequestTypeDef,
 ):
     pass
 
+
 ListIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "ListIpAccessSettingsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -728,22 +726,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
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
 _RequiredListTrustStoreCertificatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTrustStoreCertificatesRequestRequestTypeDef",
     {
         "trustStoreArn": str,
     },
 )
 _OptionalListTrustStoreCertificatesRequestRequestTypeDef = TypedDict(
@@ -751,20 +741,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTrustStoreCertificatesRequestRequestTypeDef(
     _RequiredListTrustStoreCertificatesRequestRequestTypeDef,
     _OptionalListTrustStoreCertificatesRequestRequestTypeDef,
 ):
     pass
 
+
 ListTrustStoresRequestRequestTypeDef = TypedDict(
     "ListTrustStoresRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -839,20 +831,22 @@
     {
         "browserPolicy": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateBrowserSettingsRequestRequestTypeDef(
     _RequiredUpdateBrowserSettingsRequestRequestTypeDef,
     _OptionalUpdateBrowserSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentityProviderRequestRequestTypeDef",
     {
         "identityProviderArn": str,
     },
 )
 _OptionalUpdateIdentityProviderRequestRequestTypeDef = TypedDict(
@@ -862,20 +856,22 @@
         "identityProviderDetails": Mapping[str, str],
         "identityProviderName": str,
         "identityProviderType": IdentityProviderTypeType,
     },
     total=False,
 )
 
+
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkSettingsRequestRequestTypeDef",
     {
         "networkSettingsArn": str,
     },
 )
 _OptionalUpdateNetworkSettingsRequestRequestTypeDef = TypedDict(
@@ -885,20 +881,22 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "vpcId": str,
     },
     total=False,
 )
 
+
 class UpdateNetworkSettingsRequestRequestTypeDef(
     _RequiredUpdateNetworkSettingsRequestRequestTypeDef,
     _OptionalUpdateNetworkSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdatePortalRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePortalRequestRequestTypeDef",
     {
         "portalArn": str,
     },
 )
 _OptionalUpdatePortalRequestRequestTypeDef = TypedDict(
@@ -906,19 +904,21 @@
     {
         "authenticationType": AuthenticationTypeType,
         "displayName": str,
     },
     total=False,
 )
 
+
 class UpdatePortalRequestRequestTypeDef(
     _RequiredUpdatePortalRequestRequestTypeDef, _OptionalUpdatePortalRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateTrustStoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrustStoreRequestRequestTypeDef",
     {
         "trustStoreArn": str,
     },
 )
 _OptionalUpdateTrustStoreRequestRequestTypeDef = TypedDict(
@@ -927,19 +927,21 @@
         "certificatesToAdd": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
         "certificatesToDelete": Sequence[str],
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateTrustStoreRequestRequestTypeDef(
     _RequiredUpdateTrustStoreRequestRequestTypeDef, _OptionalUpdateTrustStoreRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "userAccessLoggingSettingsArn": str,
     },
 )
 _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -947,20 +949,22 @@
     {
         "clientToken": str,
         "kinesisStreamArn": str,
     },
     total=False,
 )
 
+
 class UpdateUserAccessLoggingSettingsRequestRequestTypeDef(
     _RequiredUpdateUserAccessLoggingSettingsRequestRequestTypeDef,
     _OptionalUpdateUserAccessLoggingSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateUserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserSettingsRequestRequestTypeDef",
     {
         "userSettingsArn": str,
     },
 )
 _OptionalUpdateUserSettingsRequestRequestTypeDef = TypedDict(
@@ -974,20 +978,22 @@
         "pasteAllowed": EnabledTypeType,
         "printAllowed": EnabledTypeType,
         "uploadAllowed": EnabledTypeType,
     },
     total=False,
 )
 
+
 class UpdateUserSettingsRequestRequestTypeDef(
     _RequiredUpdateUserSettingsRequestRequestTypeDef,
     _OptionalUpdateUserSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 AssociateBrowserSettingsResponseTypeDef = TypedDict(
     "AssociateBrowserSettingsResponseTypeDef",
     {
         "browserSettingsArn": str,
         "portalArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1177,20 +1183,22 @@
         "clientToken": str,
         "customerManagedKey": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateBrowserSettingsRequestRequestTypeDef(
     _RequiredCreateBrowserSettingsRequestRequestTypeDef,
     _OptionalCreateBrowserSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateNetworkSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateNetworkSettingsRequestRequestTypeDef",
     {
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "vpcId": str,
     },
@@ -1200,20 +1208,22 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateNetworkSettingsRequestRequestTypeDef(
     _RequiredCreateNetworkSettingsRequestRequestTypeDef,
     _OptionalCreateNetworkSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 CreatePortalRequestRequestTypeDef = TypedDict(
     "CreatePortalRequestRequestTypeDef",
     {
         "additionalEncryptionContext": Mapping[str, str],
         "authenticationType": AuthenticationTypeType,
         "clientToken": str,
         "customerManagedKey": str,
@@ -1234,19 +1244,21 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateTrustStoreRequestRequestTypeDef(
     _RequiredCreateTrustStoreRequestRequestTypeDef, _OptionalCreateTrustStoreRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "kinesisStreamArn": str,
     },
 )
 _OptionalCreateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
@@ -1254,20 +1266,22 @@
     {
         "clientToken": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateUserAccessLoggingSettingsRequestRequestTypeDef(
     _RequiredCreateUserAccessLoggingSettingsRequestRequestTypeDef,
     _OptionalCreateUserAccessLoggingSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateUserSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserSettingsRequestRequestTypeDef",
     {
         "copyAllowed": EnabledTypeType,
         "downloadAllowed": EnabledTypeType,
         "pasteAllowed": EnabledTypeType,
         "printAllowed": EnabledTypeType,
@@ -1281,20 +1295,30 @@
         "disconnectTimeoutInMinutes": int,
         "idleDisconnectTimeoutInMinutes": int,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateUserSettingsRequestRequestTypeDef(
     _RequiredCreateUserSettingsRequestRequestTypeDef,
     _OptionalCreateUserSettingsRequestRequestTypeDef,
 ):
     pass
 
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1302,19 +1326,21 @@
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipRules": Sequence[IpRuleTypeDef],
     },
 )
 _OptionalCreateIpAccessSettingsRequestRequestTypeDef = TypedDict(
@@ -1326,20 +1352,45 @@
         "description": str,
         "displayName": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateIpAccessSettingsRequestRequestTypeDef(
     _RequiredCreateIpAccessSettingsRequestRequestTypeDef,
     _OptionalCreateIpAccessSettingsRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredIpAccessSettingsTypeDef = TypedDict(
+    "_RequiredIpAccessSettingsTypeDef",
+    {
+        "ipAccessSettingsArn": str,
+    },
+)
+_OptionalIpAccessSettingsTypeDef = TypedDict(
+    "_OptionalIpAccessSettingsTypeDef",
+    {
+        "associatedPortalArns": List[str],
+        "creationDate": datetime,
+        "description": str,
+        "displayName": str,
+        "ipRules": List[IpRuleTypeDef],
+    },
+    total=False,
+)
+
+
+class IpAccessSettingsTypeDef(_RequiredIpAccessSettingsTypeDef, _OptionalIpAccessSettingsTypeDef):
+    pass
+
+
 _RequiredUpdateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
     },
 )
 _OptionalUpdateIpAccessSettingsRequestRequestTypeDef = TypedDict(
@@ -1349,20 +1400,22 @@
         "description": str,
         "displayName": str,
         "ipRules": Sequence[IpRuleTypeDef],
     },
     total=False,
 )
 
+
 class UpdateIpAccessSettingsRequestRequestTypeDef(
     _RequiredUpdateIpAccessSettingsRequestRequestTypeDef,
     _OptionalUpdateIpAccessSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 GetIdentityProviderResponseTypeDef = TypedDict(
     "GetIdentityProviderResponseTypeDef",
     {
         "identityProvider": IdentityProviderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1461,35 +1514,14 @@
     {
         "ipAccessSettings": List[IpAccessSettingsSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredIpAccessSettingsTypeDef = TypedDict(
-    "_RequiredIpAccessSettingsTypeDef",
-    {
-        "ipAccessSettingsArn": str,
-    },
-)
-_OptionalIpAccessSettingsTypeDef = TypedDict(
-    "_OptionalIpAccessSettingsTypeDef",
-    {
-        "associatedPortalArns": List[str],
-        "creationDate": datetime,
-        "description": str,
-        "displayName": str,
-        "ipRules": List[IpRuleOutputTypeDef],
-    },
-    total=False,
-)
-
-class IpAccessSettingsTypeDef(_RequiredIpAccessSettingsTypeDef, _OptionalIpAccessSettingsTypeDef):
-    pass
-
 ListNetworkSettingsResponseTypeDef = TypedDict(
     "ListNetworkSettingsResponseTypeDef",
     {
         "networkSettings": List[NetworkSettingsSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1500,22 +1532,14 @@
     {
         "nextToken": str,
         "portals": List[PortalSummaryTypeDef],
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
 ListTrustStoresResponseTypeDef = TypedDict(
     "ListTrustStoresResponseTypeDef",
     {
         "nextToken": str,
         "trustStores": List[TrustStoreSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/PKG-INFO` & `mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces-web
-Version: 1.28.12
-Summary: Type annotations for boto3.WorkSpacesWeb 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.WorkSpacesWeb 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-web)](https://pepy.tech/project/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
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
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,24 +349,22 @@
     TrustStoreTypeDef,
     GetUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsTypeDef,
     GetUserSettingsRequestRequestTypeDef,
     UserSettingsTypeDef,
     IdentityProviderSummaryTypeDef,
     IpAccessSettingsSummaryTypeDef,
-    IpRuleOutputTypeDef,
     ListBrowserSettingsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ListIpAccessSettingsRequestRequestTypeDef,
     ListNetworkSettingsRequestRequestTypeDef,
     NetworkSettingsSummaryTypeDef,
     ListPortalsRequestRequestTypeDef,
     PortalSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListTrustStoreCertificatesRequestRequestTypeDef,
     ListTrustStoresRequestRequestTypeDef,
     TrustStoreSummaryTypeDef,
     ListUserAccessLoggingSettingsRequestRequestTypeDef,
     UserAccessLoggingSettingsSummaryTypeDef,
     ListUserSettingsRequestRequestTypeDef,
     UserSettingsSummaryTypeDef,
@@ -401,34 +399,34 @@
     GetTrustStoreCertificateResponseTypeDef,
     CreateBrowserSettingsRequestRequestTypeDef,
     CreateNetworkSettingsRequestRequestTypeDef,
     CreatePortalRequestRequestTypeDef,
     CreateTrustStoreRequestRequestTypeDef,
     CreateUserAccessLoggingSettingsRequestRequestTypeDef,
     CreateUserSettingsRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIpAccessSettingsRequestRequestTypeDef,
+    IpAccessSettingsTypeDef,
     UpdateIpAccessSettingsRequestRequestTypeDef,
     GetIdentityProviderResponseTypeDef,
     UpdateIdentityProviderResponseTypeDef,
     GetNetworkSettingsResponseTypeDef,
     UpdateNetworkSettingsResponseTypeDef,
     GetPortalResponseTypeDef,
     UpdatePortalResponseTypeDef,
     GetTrustStoreResponseTypeDef,
     GetUserAccessLoggingSettingsResponseTypeDef,
     UpdateUserAccessLoggingSettingsResponseTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsResponseTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListIpAccessSettingsResponseTypeDef,
-    IpAccessSettingsTypeDef,
     ListNetworkSettingsResponseTypeDef,
     ListPortalsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTrustStoresResponseTypeDef,
     ListUserAccessLoggingSettingsResponseTypeDef,
     ListUserSettingsResponseTypeDef,
     GetIpAccessSettingsResponseTypeDef,
     UpdateIpAccessSettingsResponseTypeDef,
 )
```

### Comparing `mypy-boto3-workspaces-web-1.28.12/mypy_boto3_workspaces_web.egg-info/SOURCES.txt` & `mypy-boto3-workspaces-web-1.28.15/mypy_boto3_workspaces_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.28.12/setup.py` & `mypy-boto3-workspaces-web-1.28.15/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workspaces-web",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_workspaces_web"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkSpacesWeb 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.WorkSpacesWeb 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

