# Comparing `tmp/mypy-boto3-workmail-1.28.12.tar.gz` & `tmp/mypy-boto3-workmail-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workmail-1.28.12.tar", last modified: Thu Jul 27 11:49:50 2023, max compression
+gzip compressed data, was "mypy-boto3-workmail-1.28.15.tar", last modified: Fri Jul 28 20:43:57 2023, max compression
```

## Comparing `mypy-boto3-workmail-1.28.12.tar` & `mypy-boto3-workmail-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:50.277499 mypy-boto3-workmail-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:54.000000 mypy-boto3-workmail-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21327 2023-07-27 11:49:50.277499 mypy-boto3-workmail-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19836 2023-07-27 11:48:54.000000 mypy-boto3-workmail-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:50.265499 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-27 11:48:54.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57101 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    57005 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:55.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61470 2023-07-27 11:48:57.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    61387 2023-07-27 11:48:56.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:54.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:50.277499 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21327 2023-07-27 11:49:50.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 11:49:50.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:50.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:50.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:50.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:50.000000 mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:50.277499 mypy-boto3-workmail-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:48:54.000000 mypy-boto3-workmail-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:57.930059 mypy-boto3-workmail-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21189 2023-07-28 20:43:57.930059 mypy-boto3-workmail-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19698 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:57.930059 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57101 2023-07-28 20:41:37.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57005 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-07-28 20:41:37.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-07-28 20:41:37.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-28 20:41:37.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-07-28 20:41:37.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60313 2023-07-28 20:41:39.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60232 2023-07-28 20:41:38.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:57.930059 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21189 2023-07-28 20:43:57.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:43:57.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:57.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:57.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:57.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:57.000000 mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:57.930059 mypy-boto3-workmail-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:41:36.000000 mypy-boto3-workmail-1.28.15/setup.py
```

### Comparing `mypy-boto3-workmail-1.28.12/LICENSE` & `mypy-boto3-workmail-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.12/PKG-INFO` & `mypy-boto3-workmail-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workmail
-Version: 1.28.12
-Summary: Type annotations for boto3.WorkMail 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.WorkMail 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workmail.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workmail)](https://pepy.tech/project/mypy-boto3-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkMail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[boto3.WorkMail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
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
 [mypy-boto3-workmail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,22 +371,20 @@
 ```python
 from mypy_boto3_workmail.type_defs import (
     AccessControlRuleTypeDef,
     AssociateDelegateToResourceRequestRequestTypeDef,
     AssociateMemberToGroupRequestRequestTypeDef,
     AssumeImpersonationRoleRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    LambdaAvailabilityProviderOutputTypeDef,
+    LambdaAvailabilityProviderTypeDef,
     RedactedEwsAvailabilityProviderTypeDef,
-    BookingOptionsOutputTypeDef,
     BookingOptionsTypeDef,
     CancelMailboxExportJobRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     EwsAvailabilityProviderTypeDef,
-    LambdaAvailabilityProviderTypeDef,
     CreateGroupRequestRequestTypeDef,
     ImpersonationRuleTypeDef,
     CreateMobileDeviceAccessRuleRequestRequestTypeDef,
     DomainTypeDef,
     CreateResourceRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DelegateTypeDef,
@@ -411,15 +409,14 @@
     DescribeMailboxExportJobRequestRequestTypeDef,
     DescribeOrganizationRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
     DescribeUserRequestRequestTypeDef,
     DisassociateDelegateFromResourceRequestRequestTypeDef,
     DisassociateMemberFromGroupRequestRequestTypeDef,
     DnsRecordTypeDef,
-    FolderConfigurationOutputTypeDef,
     FolderConfigurationTypeDef,
     GetAccessControlEffectRequestRequestTypeDef,
     GetDefaultRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectRequestRequestTypeDef,
     ImpersonationMatchedRuleTypeDef,
     GetImpersonationRoleRequestRequestTypeDef,
     ImpersonationRuleOutputTypeDef,
@@ -450,27 +447,26 @@
     MobileDeviceAccessRuleTypeDef,
     ListOrganizationsRequestRequestTypeDef,
     OrganizationSummaryTypeDef,
     ListResourceDelegatesRequestRequestTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
     PutAccessControlRuleRequestRequestTypeDef,
     PutEmailMonitoringConfigurationRequestRequestTypeDef,
     PutInboundDmarcSettingsRequestRequestTypeDef,
     PutMailboxPermissionsRequestRequestTypeDef,
     PutMobileDeviceAccessOverrideRequestRequestTypeDef,
     RegisterMailDomainRequestRequestTypeDef,
     RegisterToWorkMailRequestRequestTypeDef,
     ResetPasswordRequestRequestTypeDef,
     StartMailboxExportJobRequestRequestTypeDef,
-    TagTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDefaultMailDomainRequestRequestTypeDef,
     UpdateMailboxQuotaRequestRequestTypeDef,
     UpdateMobileDeviceAccessRuleRequestRequestTypeDef,
     UpdatePrimaryEmailAddressRequestRequestTypeDef,
     AssumeImpersonationRoleResponseTypeDef,
     CreateGroupResponseTypeDef,
@@ -525,16 +521,16 @@
     ListMailboxExportJobsResponseTypeDef,
     ListMailboxPermissionsResponseTypeDef,
     ListMobileDeviceAccessOverridesResponseTypeDef,
     ListMobileDeviceAccessRulesResponseTypeDef,
     ListOrganizationsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ListUsersResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    ListUsersResponseTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
 )
 
 
 def get_structure() -> AccessControlRuleTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-workmail-1.28.12/README.md` & `mypy-boto3-workmail-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workmail.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workmail)](https://pepy.tech/project/mypy-boto3-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkMail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[boto3.WorkMail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
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
 [mypy-boto3-workmail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,22 +339,20 @@
 ```python
 from mypy_boto3_workmail.type_defs import (
     AccessControlRuleTypeDef,
     AssociateDelegateToResourceRequestRequestTypeDef,
     AssociateMemberToGroupRequestRequestTypeDef,
     AssumeImpersonationRoleRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    LambdaAvailabilityProviderOutputTypeDef,
+    LambdaAvailabilityProviderTypeDef,
     RedactedEwsAvailabilityProviderTypeDef,
-    BookingOptionsOutputTypeDef,
     BookingOptionsTypeDef,
     CancelMailboxExportJobRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     EwsAvailabilityProviderTypeDef,
-    LambdaAvailabilityProviderTypeDef,
     CreateGroupRequestRequestTypeDef,
     ImpersonationRuleTypeDef,
     CreateMobileDeviceAccessRuleRequestRequestTypeDef,
     DomainTypeDef,
     CreateResourceRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DelegateTypeDef,
@@ -379,15 +377,14 @@
     DescribeMailboxExportJobRequestRequestTypeDef,
     DescribeOrganizationRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
     DescribeUserRequestRequestTypeDef,
     DisassociateDelegateFromResourceRequestRequestTypeDef,
     DisassociateMemberFromGroupRequestRequestTypeDef,
     DnsRecordTypeDef,
-    FolderConfigurationOutputTypeDef,
     FolderConfigurationTypeDef,
     GetAccessControlEffectRequestRequestTypeDef,
     GetDefaultRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectRequestRequestTypeDef,
     ImpersonationMatchedRuleTypeDef,
     GetImpersonationRoleRequestRequestTypeDef,
     ImpersonationRuleOutputTypeDef,
@@ -418,27 +415,26 @@
     MobileDeviceAccessRuleTypeDef,
     ListOrganizationsRequestRequestTypeDef,
     OrganizationSummaryTypeDef,
     ListResourceDelegatesRequestRequestTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
     PutAccessControlRuleRequestRequestTypeDef,
     PutEmailMonitoringConfigurationRequestRequestTypeDef,
     PutInboundDmarcSettingsRequestRequestTypeDef,
     PutMailboxPermissionsRequestRequestTypeDef,
     PutMobileDeviceAccessOverrideRequestRequestTypeDef,
     RegisterMailDomainRequestRequestTypeDef,
     RegisterToWorkMailRequestRequestTypeDef,
     ResetPasswordRequestRequestTypeDef,
     StartMailboxExportJobRequestRequestTypeDef,
-    TagTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDefaultMailDomainRequestRequestTypeDef,
     UpdateMailboxQuotaRequestRequestTypeDef,
     UpdateMobileDeviceAccessRuleRequestRequestTypeDef,
     UpdatePrimaryEmailAddressRequestRequestTypeDef,
     AssumeImpersonationRoleResponseTypeDef,
     CreateGroupResponseTypeDef,
@@ -493,16 +489,16 @@
     ListMailboxExportJobsResponseTypeDef,
     ListMailboxPermissionsResponseTypeDef,
     ListMobileDeviceAccessOverridesResponseTypeDef,
     ListMobileDeviceAccessRulesResponseTypeDef,
     ListOrganizationsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ListUsersResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    ListUsersResponseTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
 )
 
 
 def get_structure() -> AccessControlRuleTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/__init__.py` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/__init__.pyi` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/__main__.py` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkMail 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.WorkMail 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail\nOther"
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

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/client.py` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/client.pyi` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/literals.py` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/literals.pyi` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/paginator.py` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/paginator.pyi` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/type_defs.py` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,29 +33,26 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessControlRuleTypeDef",
     "AssociateDelegateToResourceRequestRequestTypeDef",
     "AssociateMemberToGroupRequestRequestTypeDef",
     "AssumeImpersonationRoleRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "LambdaAvailabilityProviderOutputTypeDef",
+    "LambdaAvailabilityProviderTypeDef",
     "RedactedEwsAvailabilityProviderTypeDef",
-    "BookingOptionsOutputTypeDef",
     "BookingOptionsTypeDef",
     "CancelMailboxExportJobRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "EwsAvailabilityProviderTypeDef",
-    "LambdaAvailabilityProviderTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "ImpersonationRuleTypeDef",
     "CreateMobileDeviceAccessRuleRequestRequestTypeDef",
     "DomainTypeDef",
     "CreateResourceRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DelegateTypeDef",
@@ -80,15 +77,14 @@
     "DescribeMailboxExportJobRequestRequestTypeDef",
     "DescribeOrganizationRequestRequestTypeDef",
     "DescribeResourceRequestRequestTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "DisassociateDelegateFromResourceRequestRequestTypeDef",
     "DisassociateMemberFromGroupRequestRequestTypeDef",
     "DnsRecordTypeDef",
-    "FolderConfigurationOutputTypeDef",
     "FolderConfigurationTypeDef",
     "GetAccessControlEffectRequestRequestTypeDef",
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectRequestRequestTypeDef",
     "ImpersonationMatchedRuleTypeDef",
     "GetImpersonationRoleRequestRequestTypeDef",
     "ImpersonationRuleOutputTypeDef",
@@ -119,27 +115,26 @@
     "MobileDeviceAccessRuleTypeDef",
     "ListOrganizationsRequestRequestTypeDef",
     "OrganizationSummaryTypeDef",
     "ListResourceDelegatesRequestRequestTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserTypeDef",
     "PutAccessControlRuleRequestRequestTypeDef",
     "PutEmailMonitoringConfigurationRequestRequestTypeDef",
     "PutInboundDmarcSettingsRequestRequestTypeDef",
     "PutMailboxPermissionsRequestRequestTypeDef",
     "PutMobileDeviceAccessOverrideRequestRequestTypeDef",
     "RegisterMailDomainRequestRequestTypeDef",
     "RegisterToWorkMailRequestRequestTypeDef",
     "ResetPasswordRequestRequestTypeDef",
     "StartMailboxExportJobRequestRequestTypeDef",
-    "TagTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDefaultMailDomainRequestRequestTypeDef",
     "UpdateMailboxQuotaRequestRequestTypeDef",
     "UpdateMobileDeviceAccessRuleRequestRequestTypeDef",
     "UpdatePrimaryEmailAddressRequestRequestTypeDef",
     "AssumeImpersonationRoleResponseTypeDef",
     "CreateGroupResponseTypeDef",
@@ -194,16 +189,16 @@
     "ListMailboxExportJobsResponseTypeDef",
     "ListMailboxPermissionsResponseTypeDef",
     "ListMobileDeviceAccessOverridesResponseTypeDef",
     "ListMobileDeviceAccessRulesResponseTypeDef",
     "ListOrganizationsResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ListUsersResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "ListUsersResponseTypeDef",
     "ListAvailabilityConfigurationsResponseTypeDef",
 )
 
 AccessControlRuleTypeDef = TypedDict(
     "AccessControlRuleTypeDef",
     {
         "Name": str,
@@ -256,40 +251,30 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-LambdaAvailabilityProviderOutputTypeDef = TypedDict(
-    "LambdaAvailabilityProviderOutputTypeDef",
+LambdaAvailabilityProviderTypeDef = TypedDict(
+    "LambdaAvailabilityProviderTypeDef",
     {
         "LambdaArn": str,
     },
 )
 
 RedactedEwsAvailabilityProviderTypeDef = TypedDict(
     "RedactedEwsAvailabilityProviderTypeDef",
     {
         "EwsEndpoint": str,
         "EwsUsername": str,
     },
     total=False,
 )
 
-BookingOptionsOutputTypeDef = TypedDict(
-    "BookingOptionsOutputTypeDef",
-    {
-        "AutoAcceptRequests": bool,
-        "AutoDeclineRecurringRequests": bool,
-        "AutoDeclineConflictingRequests": bool,
-    },
-    total=False,
-)
-
 BookingOptionsTypeDef = TypedDict(
     "BookingOptionsTypeDef",
     {
         "AutoAcceptRequests": bool,
         "AutoDeclineRecurringRequests": bool,
         "AutoDeclineConflictingRequests": bool,
     },
@@ -319,21 +304,14 @@
     {
         "EwsEndpoint": str,
         "EwsUsername": str,
         "EwsPassword": str,
     },
 )
 
-LambdaAvailabilityProviderTypeDef = TypedDict(
-    "LambdaAvailabilityProviderTypeDef",
-    {
-        "LambdaArn": str,
-    },
-)
-
 CreateGroupRequestRequestTypeDef = TypedDict(
     "CreateGroupRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
     },
 )
@@ -352,21 +330,19 @@
         "Description": str,
         "TargetUsers": Sequence[str],
         "NotTargetUsers": Sequence[str],
     },
     total=False,
 )
 
-
 class ImpersonationRuleTypeDef(
     _RequiredImpersonationRuleTypeDef, _OptionalImpersonationRuleTypeDef
 ):
     pass
 
-
 _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Effect": MobileDeviceAccessRuleEffectType,
     },
@@ -384,22 +360,20 @@
         "NotDeviceOperatingSystems": Sequence[str],
         "DeviceUserAgents": Sequence[str],
         "NotDeviceUserAgents": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateMobileDeviceAccessRuleRequestRequestTypeDef(
     _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef,
     _OptionalCreateMobileDeviceAccessRuleRequestRequestTypeDef,
 ):
     pass
 
-
 DomainTypeDef = TypedDict(
     "DomainTypeDef",
     {
         "DomainName": str,
         "HostedZoneId": str,
     },
     total=False,
@@ -517,22 +491,20 @@
     "_OptionalDeleteOrganizationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteOrganizationRequestRequestTypeDef(
     _RequiredDeleteOrganizationRequestRequestTypeDef,
     _OptionalDeleteOrganizationRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteResourceRequestRequestTypeDef = TypedDict(
     "DeleteResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ResourceId": str,
     },
 )
@@ -646,36 +618,14 @@
         "Type": str,
         "Hostname": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredFolderConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFolderConfigurationOutputTypeDef",
-    {
-        "Name": FolderNameType,
-        "Action": RetentionActionType,
-    },
-)
-_OptionalFolderConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFolderConfigurationOutputTypeDef",
-    {
-        "Period": int,
-    },
-    total=False,
-)
-
-
-class FolderConfigurationOutputTypeDef(
-    _RequiredFolderConfigurationOutputTypeDef, _OptionalFolderConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredFolderConfigurationTypeDef = TypedDict(
     "_RequiredFolderConfigurationTypeDef",
     {
         "Name": FolderNameType,
         "Action": RetentionActionType,
     },
 )
@@ -683,21 +633,19 @@
     "_OptionalFolderConfigurationTypeDef",
     {
         "Period": int,
     },
     total=False,
 )
 
-
 class FolderConfigurationTypeDef(
     _RequiredFolderConfigurationTypeDef, _OptionalFolderConfigurationTypeDef
 ):
     pass
 
-
 _RequiredGetAccessControlEffectRequestRequestTypeDef = TypedDict(
     "_RequiredGetAccessControlEffectRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "IpAddress": str,
         "Action": str,
     },
@@ -707,22 +655,20 @@
     {
         "UserId": str,
         "ImpersonationRoleId": str,
     },
     total=False,
 )
 
-
 class GetAccessControlEffectRequestRequestTypeDef(
     _RequiredGetAccessControlEffectRequestRequestTypeDef,
     _OptionalGetAccessControlEffectRequestRequestTypeDef,
 ):
     pass
 
-
 GetDefaultRetentionPolicyRequestRequestTypeDef = TypedDict(
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
@@ -766,21 +712,19 @@
         "Description": str,
         "TargetUsers": List[str],
         "NotTargetUsers": List[str],
     },
     total=False,
 )
 
-
 class ImpersonationRuleOutputTypeDef(
     _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
 ):
     pass
 
-
 GetMailDomainRequestRequestTypeDef = TypedDict(
     "GetMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -806,22 +750,20 @@
         "DeviceModel": str,
         "DeviceOperatingSystem": str,
         "DeviceUserAgent": str,
     },
     total=False,
 )
 
-
 class GetMobileDeviceAccessEffectRequestRequestTypeDef(
     _RequiredGetMobileDeviceAccessEffectRequestRequestTypeDef,
     _OptionalGetMobileDeviceAccessEffectRequestRequestTypeDef,
 ):
     pass
 
-
 MobileDeviceAccessMatchedRuleTypeDef = TypedDict(
     "MobileDeviceAccessMatchedRuleTypeDef",
     {
         "MobileDeviceAccessRuleId": str,
         "Name": str,
     },
     total=False,
@@ -890,21 +832,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListAliasesRequestRequestTypeDef(
     _RequiredListAliasesRequestRequestTypeDef, _OptionalListAliasesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListAvailabilityConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailabilityConfigurationsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListAvailabilityConfigurationsRequestRequestTypeDef = TypedDict(
@@ -912,22 +852,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAvailabilityConfigurationsRequestRequestTypeDef(
     _RequiredListAvailabilityConfigurationsRequestRequestTypeDef,
     _OptionalListAvailabilityConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListGroupMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembersRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "GroupId": str,
     },
 )
@@ -936,21 +874,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListGroupMembersRequestRequestTypeDef(
     _RequiredListGroupMembersRequestRequestTypeDef, _OptionalListGroupMembersRequestRequestTypeDef
 ):
     pass
 
-
 MemberTypeDef = TypedDict(
     "MemberTypeDef",
     {
         "Id": str,
         "Name": str,
         "Type": MemberTypeType,
         "State": EntityStateType,
@@ -971,21 +907,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListGroupsRequestRequestTypeDef(
     _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListImpersonationRolesRequestRequestTypeDef = TypedDict(
     "_RequiredListImpersonationRolesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListImpersonationRolesRequestRequestTypeDef = TypedDict(
@@ -993,22 +927,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListImpersonationRolesRequestRequestTypeDef(
     _RequiredListImpersonationRolesRequestRequestTypeDef,
     _OptionalListImpersonationRolesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListMailDomainsRequestRequestTypeDef = TypedDict(
     "_RequiredListMailDomainsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListMailDomainsRequestRequestTypeDef = TypedDict(
@@ -1016,21 +948,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListMailDomainsRequestRequestTypeDef(
     _RequiredListMailDomainsRequestRequestTypeDef, _OptionalListMailDomainsRequestRequestTypeDef
 ):
     pass
 
-
 MailDomainSummaryTypeDef = TypedDict(
     "MailDomainSummaryTypeDef",
     {
         "DomainName": str,
         "DefaultDomain": bool,
     },
     total=False,
@@ -1047,22 +977,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListMailboxExportJobsRequestRequestTypeDef(
     _RequiredListMailboxExportJobsRequestRequestTypeDef,
     _OptionalListMailboxExportJobsRequestRequestTypeDef,
 ):
     pass
 
-
 MailboxExportJobTypeDef = TypedDict(
     "MailboxExportJobTypeDef",
     {
         "JobId": str,
         "EntityId": str,
         "Description": str,
         "S3BucketName": str,
@@ -1087,22 +1015,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListMailboxPermissionsRequestRequestTypeDef(
     _RequiredListMailboxPermissionsRequestRequestTypeDef,
     _OptionalListMailboxPermissionsRequestRequestTypeDef,
 ):
     pass
 
-
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "GranteeId": str,
         "GranteeType": MemberTypeType,
         "PermissionValues": List[PermissionTypeType],
     },
@@ -1121,22 +1047,20 @@
         "DeviceId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListMobileDeviceAccessOverridesRequestRequestTypeDef(
     _RequiredListMobileDeviceAccessOverridesRequestRequestTypeDef,
     _OptionalListMobileDeviceAccessOverridesRequestRequestTypeDef,
 ):
     pass
 
-
 MobileDeviceAccessOverrideTypeDef = TypedDict(
     "MobileDeviceAccessOverrideTypeDef",
     {
         "UserId": str,
         "DeviceId": str,
         "Effect": MobileDeviceAccessRuleEffectType,
         "Description": str,
@@ -1207,22 +1131,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListResourceDelegatesRequestRequestTypeDef(
     _RequiredListResourceDelegatesRequestRequestTypeDef,
     _OptionalListResourceDelegatesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -1230,21 +1152,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListResourcesRequestRequestTypeDef(
     _RequiredListResourcesRequestRequestTypeDef, _OptionalListResourcesRequestRequestTypeDef
 ):
     pass
 
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Id": str,
         "Email": str,
         "Name": str,
         "Type": ResourceTypeType,
@@ -1258,16 +1178,16 @@
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
 
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
@@ -1281,21 +1201,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "Id": str,
         "Email": str,
         "Name": str,
         "DisplayName": str,
@@ -1327,22 +1245,20 @@
         "NotUserIds": Sequence[str],
         "ImpersonationRoleIds": Sequence[str],
         "NotImpersonationRoleIds": Sequence[str],
     },
     total=False,
 )
 
-
 class PutAccessControlRuleRequestRequestTypeDef(
     _RequiredPutAccessControlRuleRequestRequestTypeDef,
     _OptionalPutAccessControlRuleRequestRequestTypeDef,
 ):
     pass
 
-
 PutEmailMonitoringConfigurationRequestRequestTypeDef = TypedDict(
     "PutEmailMonitoringConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "RoleArn": str,
         "LogGroupArn": str,
     },
@@ -1379,22 +1295,20 @@
     "_OptionalPutMobileDeviceAccessOverrideRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class PutMobileDeviceAccessOverrideRequestRequestTypeDef(
     _RequiredPutMobileDeviceAccessOverrideRequestRequestTypeDef,
     _OptionalPutMobileDeviceAccessOverrideRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRegisterMailDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1402,22 +1316,20 @@
     "_OptionalRegisterMailDomainRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class RegisterMailDomainRequestRequestTypeDef(
     _RequiredRegisterMailDomainRequestRequestTypeDef,
     _OptionalRegisterMailDomainRequestRequestTypeDef,
 ):
     pass
 
-
 RegisterToWorkMailRequestRequestTypeDef = TypedDict(
     "RegisterToWorkMailRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
         "Email": str,
     },
@@ -1448,30 +1360,20 @@
     "_OptionalStartMailboxExportJobRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class StartMailboxExportJobRequestRequestTypeDef(
     _RequiredStartMailboxExportJobRequestRequestTypeDef,
     _OptionalStartMailboxExportJobRequestRequestTypeDef,
 ):
     pass
 
-
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
@@ -1514,22 +1416,20 @@
         "NotDeviceOperatingSystems": Sequence[str],
         "DeviceUserAgents": Sequence[str],
         "NotDeviceUserAgents": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateMobileDeviceAccessRuleRequestRequestTypeDef(
     _RequiredUpdateMobileDeviceAccessRuleRequestRequestTypeDef,
     _OptionalUpdateMobileDeviceAccessRuleRequestRequestTypeDef,
 ):
     pass
 
-
 UpdatePrimaryEmailAddressRequestRequestTypeDef = TypedDict(
     "UpdatePrimaryEmailAddressRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
         "Email": str,
     },
@@ -1748,29 +1648,29 @@
 
 AvailabilityConfigurationTypeDef = TypedDict(
     "AvailabilityConfigurationTypeDef",
     {
         "DomainName": str,
         "ProviderType": AvailabilityProviderTypeType,
         "EwsProvider": RedactedEwsAvailabilityProviderTypeDef,
-        "LambdaProvider": LambdaAvailabilityProviderOutputTypeDef,
+        "LambdaProvider": LambdaAvailabilityProviderTypeDef,
         "DateCreated": datetime,
         "DateModified": datetime,
     },
     total=False,
 )
 
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceId": str,
         "Email": str,
         "Name": str,
         "Type": ResourceTypeType,
-        "BookingOptions": BookingOptionsOutputTypeDef,
+        "BookingOptions": BookingOptionsTypeDef,
         "State": EntityStateType,
         "EnabledDate": datetime,
         "DisabledDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1786,21 +1686,19 @@
     {
         "Name": str,
         "BookingOptions": BookingOptionsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateResourceRequestRequestTypeDef(
     _RequiredUpdateResourceRequestRequestTypeDef, _OptionalUpdateResourceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAvailabilityConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1810,22 +1708,20 @@
         "ClientToken": str,
         "EwsProvider": EwsAvailabilityProviderTypeDef,
         "LambdaProvider": LambdaAvailabilityProviderTypeDef,
     },
     total=False,
 )
 
-
 class CreateAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredCreateAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalCreateAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredTestAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredTestAvailabilityConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalTestAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
@@ -1834,22 +1730,20 @@
         "DomainName": str,
         "EwsProvider": EwsAvailabilityProviderTypeDef,
         "LambdaProvider": LambdaAvailabilityProviderTypeDef,
     },
     total=False,
 )
 
-
 class TestAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredTestAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalTestAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1858,22 +1752,20 @@
     {
         "EwsProvider": EwsAvailabilityProviderTypeDef,
         "LambdaProvider": LambdaAvailabilityProviderTypeDef,
     },
     total=False,
 )
 
-
 class UpdateAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalUpdateAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Type": ImpersonationRoleTypeType,
         "Rules": Sequence[ImpersonationRuleTypeDef],
@@ -1884,22 +1776,20 @@
     {
         "ClientToken": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateImpersonationRoleRequestRequestTypeDef(
     _RequiredCreateImpersonationRoleRequestRequestTypeDef,
     _OptionalCreateImpersonationRoleRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
         "Name": str,
         "Type": ImpersonationRoleTypeType,
@@ -1910,22 +1800,20 @@
     "_OptionalUpdateImpersonationRoleRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateImpersonationRoleRequestRequestTypeDef(
     _RequiredUpdateImpersonationRoleRequestRequestTypeDef,
     _OptionalUpdateImpersonationRoleRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOrganizationRequestRequestTypeDef",
     {
         "Alias": str,
     },
 )
 _OptionalCreateOrganizationRequestRequestTypeDef = TypedDict(
@@ -1936,22 +1824,20 @@
         "Domains": Sequence[DomainTypeDef],
         "KmsKeyArn": str,
         "EnableInteroperability": bool,
     },
     total=False,
 )
 
-
 class CreateOrganizationRequestRequestTypeDef(
     _RequiredCreateOrganizationRequestRequestTypeDef,
     _OptionalCreateOrganizationRequestRequestTypeDef,
 ):
     pass
 
-
 ListResourceDelegatesResponseTypeDef = TypedDict(
     "ListResourceDelegatesResponseTypeDef",
     {
         "Delegates": List[DelegateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1971,15 +1857,15 @@
 
 GetDefaultRetentionPolicyResponseTypeDef = TypedDict(
     "GetDefaultRetentionPolicyResponseTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
-        "FolderConfigurations": List[FolderConfigurationOutputTypeDef],
+        "FolderConfigurations": List[FolderConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRetentionPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutRetentionPolicyRequestRequestTypeDef",
     {
@@ -1993,22 +1879,20 @@
     {
         "Id": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class PutRetentionPolicyRequestRequestTypeDef(
     _RequiredPutRetentionPolicyRequestRequestTypeDef,
     _OptionalPutRetentionPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 GetImpersonationRoleEffectResponseTypeDef = TypedDict(
     "GetImpersonationRoleEffectResponseTypeDef",
     {
         "Type": ImpersonationRoleTypeType,
         "Effect": AccessEffectType,
         "MatchedRules": List[ImpersonationMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2067,44 +1951,40 @@
     "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAliasesRequestListAliasesPaginateTypeDef(
     _RequiredListAliasesRequestListAliasesPaginateTypeDef,
     _OptionalListAliasesRequestListAliasesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
     "_RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
     "_OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef(
     _RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     _OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef = TypedDict(
     "_RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef",
     {
         "OrganizationId": str,
         "GroupId": str,
     },
 )
@@ -2112,44 +1992,40 @@
     "_OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListGroupMembersRequestListGroupMembersPaginateTypeDef(
     _RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef,
     _OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
     "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
     "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListGroupsRequestListGroupsPaginateTypeDef(
     _RequiredListGroupsRequestListGroupsPaginateTypeDef,
     _OptionalListGroupsRequestListGroupsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = TypedDict(
     "_RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
     },
 )
@@ -2157,22 +2033,20 @@
     "_OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef(
     _RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
     _OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
 ):
     pass
 
-
 ListOrganizationsRequestListOrganizationsPaginateTypeDef = TypedDict(
     "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2188,66 +2062,60 @@
     "_OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef(
     _RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
     _OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
     "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
     "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListResourcesRequestListResourcesPaginateTypeDef(
     _RequiredListResourcesRequestListResourcesPaginateTypeDef,
     _OptionalListResourcesRequestListResourcesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
-
 ListGroupMembersResponseTypeDef = TypedDict(
     "ListGroupMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2314,36 +2182,36 @@
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
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 ListAvailabilityConfigurationsResponseTypeDef = TypedDict(
     "ListAvailabilityConfigurationsResponseTypeDef",
     {
         "AvailabilityConfigurations": List[AvailabilityConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail/type_defs.pyi` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,28 +33,27 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccessControlRuleTypeDef",
     "AssociateDelegateToResourceRequestRequestTypeDef",
     "AssociateMemberToGroupRequestRequestTypeDef",
     "AssumeImpersonationRoleRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "LambdaAvailabilityProviderOutputTypeDef",
+    "LambdaAvailabilityProviderTypeDef",
     "RedactedEwsAvailabilityProviderTypeDef",
-    "BookingOptionsOutputTypeDef",
     "BookingOptionsTypeDef",
     "CancelMailboxExportJobRequestRequestTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "EwsAvailabilityProviderTypeDef",
-    "LambdaAvailabilityProviderTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "ImpersonationRuleTypeDef",
     "CreateMobileDeviceAccessRuleRequestRequestTypeDef",
     "DomainTypeDef",
     "CreateResourceRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DelegateTypeDef",
@@ -79,15 +78,14 @@
     "DescribeMailboxExportJobRequestRequestTypeDef",
     "DescribeOrganizationRequestRequestTypeDef",
     "DescribeResourceRequestRequestTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "DisassociateDelegateFromResourceRequestRequestTypeDef",
     "DisassociateMemberFromGroupRequestRequestTypeDef",
     "DnsRecordTypeDef",
-    "FolderConfigurationOutputTypeDef",
     "FolderConfigurationTypeDef",
     "GetAccessControlEffectRequestRequestTypeDef",
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     "GetImpersonationRoleEffectRequestRequestTypeDef",
     "ImpersonationMatchedRuleTypeDef",
     "GetImpersonationRoleRequestRequestTypeDef",
     "ImpersonationRuleOutputTypeDef",
@@ -118,27 +116,26 @@
     "MobileDeviceAccessRuleTypeDef",
     "ListOrganizationsRequestRequestTypeDef",
     "OrganizationSummaryTypeDef",
     "ListResourceDelegatesRequestRequestTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserTypeDef",
     "PutAccessControlRuleRequestRequestTypeDef",
     "PutEmailMonitoringConfigurationRequestRequestTypeDef",
     "PutInboundDmarcSettingsRequestRequestTypeDef",
     "PutMailboxPermissionsRequestRequestTypeDef",
     "PutMobileDeviceAccessOverrideRequestRequestTypeDef",
     "RegisterMailDomainRequestRequestTypeDef",
     "RegisterToWorkMailRequestRequestTypeDef",
     "ResetPasswordRequestRequestTypeDef",
     "StartMailboxExportJobRequestRequestTypeDef",
-    "TagTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDefaultMailDomainRequestRequestTypeDef",
     "UpdateMailboxQuotaRequestRequestTypeDef",
     "UpdateMobileDeviceAccessRuleRequestRequestTypeDef",
     "UpdatePrimaryEmailAddressRequestRequestTypeDef",
     "AssumeImpersonationRoleResponseTypeDef",
     "CreateGroupResponseTypeDef",
@@ -193,16 +190,16 @@
     "ListMailboxExportJobsResponseTypeDef",
     "ListMailboxPermissionsResponseTypeDef",
     "ListMobileDeviceAccessOverridesResponseTypeDef",
     "ListMobileDeviceAccessRulesResponseTypeDef",
     "ListOrganizationsResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ListUsersResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "ListUsersResponseTypeDef",
     "ListAvailabilityConfigurationsResponseTypeDef",
 )
 
 AccessControlRuleTypeDef = TypedDict(
     "AccessControlRuleTypeDef",
     {
         "Name": str,
@@ -255,40 +252,30 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-LambdaAvailabilityProviderOutputTypeDef = TypedDict(
-    "LambdaAvailabilityProviderOutputTypeDef",
+LambdaAvailabilityProviderTypeDef = TypedDict(
+    "LambdaAvailabilityProviderTypeDef",
     {
         "LambdaArn": str,
     },
 )
 
 RedactedEwsAvailabilityProviderTypeDef = TypedDict(
     "RedactedEwsAvailabilityProviderTypeDef",
     {
         "EwsEndpoint": str,
         "EwsUsername": str,
     },
     total=False,
 )
 
-BookingOptionsOutputTypeDef = TypedDict(
-    "BookingOptionsOutputTypeDef",
-    {
-        "AutoAcceptRequests": bool,
-        "AutoDeclineRecurringRequests": bool,
-        "AutoDeclineConflictingRequests": bool,
-    },
-    total=False,
-)
-
 BookingOptionsTypeDef = TypedDict(
     "BookingOptionsTypeDef",
     {
         "AutoAcceptRequests": bool,
         "AutoDeclineRecurringRequests": bool,
         "AutoDeclineConflictingRequests": bool,
     },
@@ -318,21 +305,14 @@
     {
         "EwsEndpoint": str,
         "EwsUsername": str,
         "EwsPassword": str,
     },
 )
 
-LambdaAvailabilityProviderTypeDef = TypedDict(
-    "LambdaAvailabilityProviderTypeDef",
-    {
-        "LambdaArn": str,
-    },
-)
-
 CreateGroupRequestRequestTypeDef = TypedDict(
     "CreateGroupRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
     },
 )
@@ -351,19 +331,21 @@
         "Description": str,
         "TargetUsers": Sequence[str],
         "NotTargetUsers": Sequence[str],
     },
     total=False,
 )
 
+
 class ImpersonationRuleTypeDef(
     _RequiredImpersonationRuleTypeDef, _OptionalImpersonationRuleTypeDef
 ):
     pass
 
+
 _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Effect": MobileDeviceAccessRuleEffectType,
     },
@@ -381,20 +363,22 @@
         "NotDeviceOperatingSystems": Sequence[str],
         "DeviceUserAgents": Sequence[str],
         "NotDeviceUserAgents": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateMobileDeviceAccessRuleRequestRequestTypeDef(
     _RequiredCreateMobileDeviceAccessRuleRequestRequestTypeDef,
     _OptionalCreateMobileDeviceAccessRuleRequestRequestTypeDef,
 ):
     pass
 
+
 DomainTypeDef = TypedDict(
     "DomainTypeDef",
     {
         "DomainName": str,
         "HostedZoneId": str,
     },
     total=False,
@@ -512,20 +496,22 @@
     "_OptionalDeleteOrganizationRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteOrganizationRequestRequestTypeDef(
     _RequiredDeleteOrganizationRequestRequestTypeDef,
     _OptionalDeleteOrganizationRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteResourceRequestRequestTypeDef = TypedDict(
     "DeleteResourceRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ResourceId": str,
     },
 )
@@ -639,34 +625,14 @@
         "Type": str,
         "Hostname": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredFolderConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFolderConfigurationOutputTypeDef",
-    {
-        "Name": FolderNameType,
-        "Action": RetentionActionType,
-    },
-)
-_OptionalFolderConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFolderConfigurationOutputTypeDef",
-    {
-        "Period": int,
-    },
-    total=False,
-)
-
-class FolderConfigurationOutputTypeDef(
-    _RequiredFolderConfigurationOutputTypeDef, _OptionalFolderConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredFolderConfigurationTypeDef = TypedDict(
     "_RequiredFolderConfigurationTypeDef",
     {
         "Name": FolderNameType,
         "Action": RetentionActionType,
     },
 )
@@ -674,19 +640,21 @@
     "_OptionalFolderConfigurationTypeDef",
     {
         "Period": int,
     },
     total=False,
 )
 
+
 class FolderConfigurationTypeDef(
     _RequiredFolderConfigurationTypeDef, _OptionalFolderConfigurationTypeDef
 ):
     pass
 
+
 _RequiredGetAccessControlEffectRequestRequestTypeDef = TypedDict(
     "_RequiredGetAccessControlEffectRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "IpAddress": str,
         "Action": str,
     },
@@ -696,20 +664,22 @@
     {
         "UserId": str,
         "ImpersonationRoleId": str,
     },
     total=False,
 )
 
+
 class GetAccessControlEffectRequestRequestTypeDef(
     _RequiredGetAccessControlEffectRequestRequestTypeDef,
     _OptionalGetAccessControlEffectRequestRequestTypeDef,
 ):
     pass
 
+
 GetDefaultRetentionPolicyRequestRequestTypeDef = TypedDict(
     "GetDefaultRetentionPolicyRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 
@@ -753,19 +723,21 @@
         "Description": str,
         "TargetUsers": List[str],
         "NotTargetUsers": List[str],
     },
     total=False,
 )
 
+
 class ImpersonationRuleOutputTypeDef(
     _RequiredImpersonationRuleOutputTypeDef, _OptionalImpersonationRuleOutputTypeDef
 ):
     pass
 
+
 GetMailDomainRequestRequestTypeDef = TypedDict(
     "GetMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -791,20 +763,22 @@
         "DeviceModel": str,
         "DeviceOperatingSystem": str,
         "DeviceUserAgent": str,
     },
     total=False,
 )
 
+
 class GetMobileDeviceAccessEffectRequestRequestTypeDef(
     _RequiredGetMobileDeviceAccessEffectRequestRequestTypeDef,
     _OptionalGetMobileDeviceAccessEffectRequestRequestTypeDef,
 ):
     pass
 
+
 MobileDeviceAccessMatchedRuleTypeDef = TypedDict(
     "MobileDeviceAccessMatchedRuleTypeDef",
     {
         "MobileDeviceAccessRuleId": str,
         "Name": str,
     },
     total=False,
@@ -873,19 +847,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListAliasesRequestRequestTypeDef(
     _RequiredListAliasesRequestRequestTypeDef, _OptionalListAliasesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListAvailabilityConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAvailabilityConfigurationsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListAvailabilityConfigurationsRequestRequestTypeDef = TypedDict(
@@ -893,20 +869,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAvailabilityConfigurationsRequestRequestTypeDef(
     _RequiredListAvailabilityConfigurationsRequestRequestTypeDef,
     _OptionalListAvailabilityConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListGroupMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupMembersRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "GroupId": str,
     },
 )
@@ -915,19 +893,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListGroupMembersRequestRequestTypeDef(
     _RequiredListGroupMembersRequestRequestTypeDef, _OptionalListGroupMembersRequestRequestTypeDef
 ):
     pass
 
+
 MemberTypeDef = TypedDict(
     "MemberTypeDef",
     {
         "Id": str,
         "Name": str,
         "Type": MemberTypeType,
         "State": EntityStateType,
@@ -948,19 +928,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListGroupsRequestRequestTypeDef(
     _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListImpersonationRolesRequestRequestTypeDef = TypedDict(
     "_RequiredListImpersonationRolesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListImpersonationRolesRequestRequestTypeDef = TypedDict(
@@ -968,20 +950,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListImpersonationRolesRequestRequestTypeDef(
     _RequiredListImpersonationRolesRequestRequestTypeDef,
     _OptionalListImpersonationRolesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListMailDomainsRequestRequestTypeDef = TypedDict(
     "_RequiredListMailDomainsRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListMailDomainsRequestRequestTypeDef = TypedDict(
@@ -989,19 +973,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListMailDomainsRequestRequestTypeDef(
     _RequiredListMailDomainsRequestRequestTypeDef, _OptionalListMailDomainsRequestRequestTypeDef
 ):
     pass
 
+
 MailDomainSummaryTypeDef = TypedDict(
     "MailDomainSummaryTypeDef",
     {
         "DomainName": str,
         "DefaultDomain": bool,
     },
     total=False,
@@ -1018,20 +1004,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListMailboxExportJobsRequestRequestTypeDef(
     _RequiredListMailboxExportJobsRequestRequestTypeDef,
     _OptionalListMailboxExportJobsRequestRequestTypeDef,
 ):
     pass
 
+
 MailboxExportJobTypeDef = TypedDict(
     "MailboxExportJobTypeDef",
     {
         "JobId": str,
         "EntityId": str,
         "Description": str,
         "S3BucketName": str,
@@ -1056,20 +1044,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListMailboxPermissionsRequestRequestTypeDef(
     _RequiredListMailboxPermissionsRequestRequestTypeDef,
     _OptionalListMailboxPermissionsRequestRequestTypeDef,
 ):
     pass
 
+
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
         "GranteeId": str,
         "GranteeType": MemberTypeType,
         "PermissionValues": List[PermissionTypeType],
     },
@@ -1088,20 +1078,22 @@
         "DeviceId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListMobileDeviceAccessOverridesRequestRequestTypeDef(
     _RequiredListMobileDeviceAccessOverridesRequestRequestTypeDef,
     _OptionalListMobileDeviceAccessOverridesRequestRequestTypeDef,
 ):
     pass
 
+
 MobileDeviceAccessOverrideTypeDef = TypedDict(
     "MobileDeviceAccessOverrideTypeDef",
     {
         "UserId": str,
         "DeviceId": str,
         "Effect": MobileDeviceAccessRuleEffectType,
         "Description": str,
@@ -1172,20 +1164,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListResourceDelegatesRequestRequestTypeDef(
     _RequiredListResourceDelegatesRequestRequestTypeDef,
     _OptionalListResourceDelegatesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListResourcesRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListResourcesRequestRequestTypeDef = TypedDict(
@@ -1193,19 +1187,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListResourcesRequestRequestTypeDef(
     _RequiredListResourcesRequestRequestTypeDef, _OptionalListResourcesRequestRequestTypeDef
 ):
     pass
 
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Id": str,
         "Email": str,
         "Name": str,
         "Type": ResourceTypeType,
@@ -1219,16 +1215,16 @@
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
 
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
@@ -1242,19 +1238,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
+
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "Id": str,
         "Email": str,
         "Name": str,
         "DisplayName": str,
@@ -1286,20 +1284,22 @@
         "NotUserIds": Sequence[str],
         "ImpersonationRoleIds": Sequence[str],
         "NotImpersonationRoleIds": Sequence[str],
     },
     total=False,
 )
 
+
 class PutAccessControlRuleRequestRequestTypeDef(
     _RequiredPutAccessControlRuleRequestRequestTypeDef,
     _OptionalPutAccessControlRuleRequestRequestTypeDef,
 ):
     pass
 
+
 PutEmailMonitoringConfigurationRequestRequestTypeDef = TypedDict(
     "PutEmailMonitoringConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "RoleArn": str,
         "LogGroupArn": str,
     },
@@ -1336,20 +1336,22 @@
     "_OptionalPutMobileDeviceAccessOverrideRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class PutMobileDeviceAccessOverrideRequestRequestTypeDef(
     _RequiredPutMobileDeviceAccessOverrideRequestRequestTypeDef,
     _OptionalPutMobileDeviceAccessOverrideRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRegisterMailDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterMailDomainRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1357,20 +1359,22 @@
     "_OptionalRegisterMailDomainRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class RegisterMailDomainRequestRequestTypeDef(
     _RequiredRegisterMailDomainRequestRequestTypeDef,
     _OptionalRegisterMailDomainRequestRequestTypeDef,
 ):
     pass
 
+
 RegisterToWorkMailRequestRequestTypeDef = TypedDict(
     "RegisterToWorkMailRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
         "Email": str,
     },
@@ -1401,27 +1405,21 @@
     "_OptionalStartMailboxExportJobRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class StartMailboxExportJobRequestRequestTypeDef(
     _RequiredStartMailboxExportJobRequestRequestTypeDef,
     _OptionalStartMailboxExportJobRequestRequestTypeDef,
 ):
     pass
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
@@ -1465,20 +1463,22 @@
         "NotDeviceOperatingSystems": Sequence[str],
         "DeviceUserAgents": Sequence[str],
         "NotDeviceUserAgents": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateMobileDeviceAccessRuleRequestRequestTypeDef(
     _RequiredUpdateMobileDeviceAccessRuleRequestRequestTypeDef,
     _OptionalUpdateMobileDeviceAccessRuleRequestRequestTypeDef,
 ):
     pass
 
+
 UpdatePrimaryEmailAddressRequestRequestTypeDef = TypedDict(
     "UpdatePrimaryEmailAddressRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
         "Email": str,
     },
@@ -1697,29 +1697,29 @@
 
 AvailabilityConfigurationTypeDef = TypedDict(
     "AvailabilityConfigurationTypeDef",
     {
         "DomainName": str,
         "ProviderType": AvailabilityProviderTypeType,
         "EwsProvider": RedactedEwsAvailabilityProviderTypeDef,
-        "LambdaProvider": LambdaAvailabilityProviderOutputTypeDef,
+        "LambdaProvider": LambdaAvailabilityProviderTypeDef,
         "DateCreated": datetime,
         "DateModified": datetime,
     },
     total=False,
 )
 
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceId": str,
         "Email": str,
         "Name": str,
         "Type": ResourceTypeType,
-        "BookingOptions": BookingOptionsOutputTypeDef,
+        "BookingOptions": BookingOptionsTypeDef,
         "State": EntityStateType,
         "EnabledDate": datetime,
         "DisabledDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1735,19 +1735,21 @@
     {
         "Name": str,
         "BookingOptions": BookingOptionsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateResourceRequestRequestTypeDef(
     _RequiredUpdateResourceRequestRequestTypeDef, _OptionalUpdateResourceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAvailabilityConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1757,20 +1759,22 @@
         "ClientToken": str,
         "EwsProvider": EwsAvailabilityProviderTypeDef,
         "LambdaProvider": LambdaAvailabilityProviderTypeDef,
     },
     total=False,
 )
 
+
 class CreateAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredCreateAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalCreateAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredTestAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredTestAvailabilityConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalTestAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
@@ -1779,20 +1783,22 @@
         "DomainName": str,
         "EwsProvider": EwsAvailabilityProviderTypeDef,
         "LambdaProvider": LambdaAvailabilityProviderTypeDef,
     },
     total=False,
 )
 
+
 class TestAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredTestAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalTestAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "DomainName": str,
     },
 )
@@ -1801,20 +1807,22 @@
     {
         "EwsProvider": EwsAvailabilityProviderTypeDef,
         "LambdaProvider": LambdaAvailabilityProviderTypeDef,
     },
     total=False,
 )
 
+
 class UpdateAvailabilityConfigurationRequestRequestTypeDef(
     _RequiredUpdateAvailabilityConfigurationRequestRequestTypeDef,
     _OptionalUpdateAvailabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "Name": str,
         "Type": ImpersonationRoleTypeType,
         "Rules": Sequence[ImpersonationRuleTypeDef],
@@ -1825,20 +1833,22 @@
     {
         "ClientToken": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateImpersonationRoleRequestRequestTypeDef(
     _RequiredCreateImpersonationRoleRequestRequestTypeDef,
     _OptionalCreateImpersonationRoleRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateImpersonationRoleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImpersonationRoleRequestRequestTypeDef",
     {
         "OrganizationId": str,
         "ImpersonationRoleId": str,
         "Name": str,
         "Type": ImpersonationRoleTypeType,
@@ -1849,20 +1859,22 @@
     "_OptionalUpdateImpersonationRoleRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateImpersonationRoleRequestRequestTypeDef(
     _RequiredUpdateImpersonationRoleRequestRequestTypeDef,
     _OptionalUpdateImpersonationRoleRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateOrganizationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOrganizationRequestRequestTypeDef",
     {
         "Alias": str,
     },
 )
 _OptionalCreateOrganizationRequestRequestTypeDef = TypedDict(
@@ -1873,20 +1885,22 @@
         "Domains": Sequence[DomainTypeDef],
         "KmsKeyArn": str,
         "EnableInteroperability": bool,
     },
     total=False,
 )
 
+
 class CreateOrganizationRequestRequestTypeDef(
     _RequiredCreateOrganizationRequestRequestTypeDef,
     _OptionalCreateOrganizationRequestRequestTypeDef,
 ):
     pass
 
+
 ListResourceDelegatesResponseTypeDef = TypedDict(
     "ListResourceDelegatesResponseTypeDef",
     {
         "Delegates": List[DelegateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1906,15 +1920,15 @@
 
 GetDefaultRetentionPolicyResponseTypeDef = TypedDict(
     "GetDefaultRetentionPolicyResponseTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
-        "FolderConfigurations": List[FolderConfigurationOutputTypeDef],
+        "FolderConfigurations": List[FolderConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRetentionPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutRetentionPolicyRequestRequestTypeDef",
     {
@@ -1928,20 +1942,22 @@
     {
         "Id": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class PutRetentionPolicyRequestRequestTypeDef(
     _RequiredPutRetentionPolicyRequestRequestTypeDef,
     _OptionalPutRetentionPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 GetImpersonationRoleEffectResponseTypeDef = TypedDict(
     "GetImpersonationRoleEffectResponseTypeDef",
     {
         "Type": ImpersonationRoleTypeType,
         "Effect": AccessEffectType,
         "MatchedRules": List[ImpersonationMatchedRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2000,40 +2016,44 @@
     "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAliasesRequestListAliasesPaginateTypeDef(
     _RequiredListAliasesRequestListAliasesPaginateTypeDef,
     _OptionalListAliasesRequestListAliasesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
     "_RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef = TypedDict(
     "_OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef(
     _RequiredListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
     _OptionalListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef = TypedDict(
     "_RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef",
     {
         "OrganizationId": str,
         "GroupId": str,
     },
 )
@@ -2041,40 +2061,44 @@
     "_OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListGroupMembersRequestListGroupMembersPaginateTypeDef(
     _RequiredListGroupMembersRequestListGroupMembersPaginateTypeDef,
     _OptionalListGroupMembersRequestListGroupMembersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
     "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
     "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListGroupsRequestListGroupsPaginateTypeDef(
     _RequiredListGroupsRequestListGroupsPaginateTypeDef,
     _OptionalListGroupsRequestListGroupsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef = TypedDict(
     "_RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     {
         "OrganizationId": str,
         "EntityId": str,
     },
 )
@@ -2082,20 +2106,22 @@
     "_OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef(
     _RequiredListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
     _OptionalListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef,
 ):
     pass
 
+
 ListOrganizationsRequestListOrganizationsPaginateTypeDef = TypedDict(
     "ListOrganizationsRequestListOrganizationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2111,60 +2137,66 @@
     "_OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef(
     _RequiredListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
     _OptionalListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
     "_RequiredListResourcesRequestListResourcesPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListResourcesRequestListResourcesPaginateTypeDef = TypedDict(
     "_OptionalListResourcesRequestListResourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListResourcesRequestListResourcesPaginateTypeDef(
     _RequiredListResourcesRequestListResourcesPaginateTypeDef,
     _OptionalListResourcesRequestListResourcesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_RequiredListUsersRequestListUsersPaginateTypeDef",
     {
         "OrganizationId": str,
     },
 )
 _OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
     "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
+
 ListGroupMembersResponseTypeDef = TypedDict(
     "ListGroupMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2231,36 +2263,36 @@
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
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-)
-
 ListAvailabilityConfigurationsResponseTypeDef = TypedDict(
     "ListAvailabilityConfigurationsResponseTypeDef",
     {
         "AvailabilityConfigurations": List[AvailabilityConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/PKG-INFO` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workmail
-Version: 1.28.12
-Summary: Type annotations for boto3.WorkMail 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.WorkMail 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workmail.svg?color=blue)](https://pypi.org/project/mypy-boto3-workmail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workmail)](https://pepy.tech/project/mypy-boto3-workmail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkMail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
+[boto3.WorkMail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
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
 [mypy-boto3-workmail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workmail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,22 +371,20 @@
 ```python
 from mypy_boto3_workmail.type_defs import (
     AccessControlRuleTypeDef,
     AssociateDelegateToResourceRequestRequestTypeDef,
     AssociateMemberToGroupRequestRequestTypeDef,
     AssumeImpersonationRoleRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    LambdaAvailabilityProviderOutputTypeDef,
+    LambdaAvailabilityProviderTypeDef,
     RedactedEwsAvailabilityProviderTypeDef,
-    BookingOptionsOutputTypeDef,
     BookingOptionsTypeDef,
     CancelMailboxExportJobRequestRequestTypeDef,
     CreateAliasRequestRequestTypeDef,
     EwsAvailabilityProviderTypeDef,
-    LambdaAvailabilityProviderTypeDef,
     CreateGroupRequestRequestTypeDef,
     ImpersonationRuleTypeDef,
     CreateMobileDeviceAccessRuleRequestRequestTypeDef,
     DomainTypeDef,
     CreateResourceRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DelegateTypeDef,
@@ -411,15 +409,14 @@
     DescribeMailboxExportJobRequestRequestTypeDef,
     DescribeOrganizationRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
     DescribeUserRequestRequestTypeDef,
     DisassociateDelegateFromResourceRequestRequestTypeDef,
     DisassociateMemberFromGroupRequestRequestTypeDef,
     DnsRecordTypeDef,
-    FolderConfigurationOutputTypeDef,
     FolderConfigurationTypeDef,
     GetAccessControlEffectRequestRequestTypeDef,
     GetDefaultRetentionPolicyRequestRequestTypeDef,
     GetImpersonationRoleEffectRequestRequestTypeDef,
     ImpersonationMatchedRuleTypeDef,
     GetImpersonationRoleRequestRequestTypeDef,
     ImpersonationRuleOutputTypeDef,
@@ -450,27 +447,26 @@
     MobileDeviceAccessRuleTypeDef,
     ListOrganizationsRequestRequestTypeDef,
     OrganizationSummaryTypeDef,
     ListResourceDelegatesRequestRequestTypeDef,
     ListResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
     PutAccessControlRuleRequestRequestTypeDef,
     PutEmailMonitoringConfigurationRequestRequestTypeDef,
     PutInboundDmarcSettingsRequestRequestTypeDef,
     PutMailboxPermissionsRequestRequestTypeDef,
     PutMobileDeviceAccessOverrideRequestRequestTypeDef,
     RegisterMailDomainRequestRequestTypeDef,
     RegisterToWorkMailRequestRequestTypeDef,
     ResetPasswordRequestRequestTypeDef,
     StartMailboxExportJobRequestRequestTypeDef,
-    TagTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDefaultMailDomainRequestRequestTypeDef,
     UpdateMailboxQuotaRequestRequestTypeDef,
     UpdateMobileDeviceAccessRuleRequestRequestTypeDef,
     UpdatePrimaryEmailAddressRequestRequestTypeDef,
     AssumeImpersonationRoleResponseTypeDef,
     CreateGroupResponseTypeDef,
@@ -525,16 +521,16 @@
     ListMailboxExportJobsResponseTypeDef,
     ListMailboxPermissionsResponseTypeDef,
     ListMobileDeviceAccessOverridesResponseTypeDef,
     ListMobileDeviceAccessRulesResponseTypeDef,
     ListOrganizationsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ListUsersResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    ListUsersResponseTypeDef,
     ListAvailabilityConfigurationsResponseTypeDef,
 )
 
 
 def get_structure() -> AccessControlRuleTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-workmail-1.28.12/mypy_boto3_workmail.egg-info/SOURCES.txt` & `mypy-boto3-workmail-1.28.15/mypy_boto3_workmail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workmail-1.28.12/setup.py` & `mypy-boto3-workmail-1.28.15/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workmail",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_workmail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WorkMail 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.WorkMail 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

