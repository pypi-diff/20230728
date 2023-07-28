# Comparing `tmp/mypy-boto3-sso-admin-1.28.12.tar.gz` & `tmp/mypy-boto3-sso-admin-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sso-admin-1.28.12.tar", last modified: Thu Jul 27 11:49:43 2023, max compression
+gzip compressed data, was "mypy-boto3-sso-admin-1.28.15.tar", last modified: Fri Jul 28 20:43:49 2023, max compression
```

## Comparing `mypy-boto3-sso-admin-1.28.12.tar` & `mypy-boto3-sso-admin-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.753340 mypy-boto3-sso-admin-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20614 2023-07-27 11:49:43.753340 mypy-boto3-sso-admin-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19120 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.753340 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34841 2023-07-27 11:47:37.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34786 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-07-27 11:47:37.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-07-27 11:47:37.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-07-27 11:47:37.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-07-27 11:47:37.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41509 2023-07-27 11:47:38.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41458 2023-07-27 11:47:37.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:43.753340 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20614 2023-07-27 11:49:43.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 11:49:43.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:43.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:43.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 11:49:43.000000 mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:43.753340 mypy-boto3-sso-admin-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-27 11:47:36.000000 mypy-boto3-sso-admin-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.305940 mypy-boto3-sso-admin-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-07-28 20:43:49.305940 mypy-boto3-sso-admin-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19011 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.293940 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34841 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34786 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-07-28 20:40:14.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40501 2023-07-28 20:40:14.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40452 2023-07-28 20:40:14.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.305940 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-07-28 20:43:49.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:49.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:49.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:49.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:49.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:43:49.000000 mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:49.305940 mypy-boto3-sso-admin-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-28 20:40:13.000000 mypy-boto3-sso-admin-1.28.15/setup.py
```

### Comparing `mypy-boto3-sso-admin-1.28.12/LICENSE` & `mypy-boto3-sso-admin-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.12/PKG-INFO` & `mypy-boto3-sso-admin-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-admin
-Version: 1.28.12
-Summary: Type annotations for boto3.SSOAdmin 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SSOAdmin 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso-admin)](https://pepy.tech/project/mypy-boto3-sso-admin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOAdmin 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
+[boto3.SSOAdmin 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
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
 [mypy-boto3-sso-admin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -388,15 +388,14 @@
     CustomerManagedPolicyReferenceTypeDef,
     AttachManagedPolicyToPermissionSetRequestRequestTypeDef,
     AttachedManagedPolicyTypeDef,
     CreateAccountAssignmentRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     PermissionSetTypeDef,
-    CustomerManagedPolicyReferenceOutputTypeDef,
     DeleteAccountAssignmentRequestRequestTypeDef,
     DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef,
     DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DeletePermissionSetRequestRequestTypeDef,
     DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef,
     DescribeAccountAssignmentCreationStatusRequestRequestTypeDef,
     DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef,
@@ -415,15 +414,14 @@
     ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListManagedPoliciesInPermissionSetRequestRequestTypeDef,
     PermissionSetProvisioningStatusMetadataTypeDef,
     ListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
     ListPermissionSetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ProvisionPermissionSetRequestRequestTypeDef,
     PutInlinePolicyToPermissionSetRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePermissionSetRequestRequestTypeDef,
     AccessControlAttributeOutputTypeDef,
     AccessControlAttributeTypeDef,
     AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
@@ -434,23 +432,23 @@
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
     GetInlinePolicyForPermissionSetResponseTypeDef,
     ListAccountAssignmentCreationStatusResponseTypeDef,
     ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
     ListAccountsForProvisionedPermissionSetResponseTypeDef,
+    ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
     ListManagedPoliciesInPermissionSetResponseTypeDef,
     ListPermissionSetsProvisionedToAccountResponseTypeDef,
     ListPermissionSetsResponseTypeDef,
     CreatePermissionSetRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreatePermissionSetResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
-    ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
-    PermissionsBoundaryOutputTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     ProvisionPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListAccountAssignmentCreationStatusRequestRequestTypeDef,
     ListAccountAssignmentDeletionStatusRequestRequestTypeDef,
     ListPermissionSetProvisioningStatusRequestRequestTypeDef,
     ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
@@ -461,19 +459,18 @@
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
     ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
     ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
     ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListPermissionSetProvisioningStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     InstanceAccessControlAttributeConfigurationOutputTypeDef,
     InstanceAccessControlAttributeConfigurationTypeDef,
-    PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef,
     GetPermissionsBoundaryForPermissionSetResponseTypeDef,
+    PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
     CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AccessControlAttributeValueOutputTypeDef:
```

### Comparing `mypy-boto3-sso-admin-1.28.12/README.md` & `mypy-boto3-sso-admin-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso-admin)](https://pepy.tech/project/mypy-boto3-sso-admin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOAdmin 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
+[boto3.SSOAdmin 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
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
 [mypy-boto3-sso-admin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,15 +356,14 @@
     CustomerManagedPolicyReferenceTypeDef,
     AttachManagedPolicyToPermissionSetRequestRequestTypeDef,
     AttachedManagedPolicyTypeDef,
     CreateAccountAssignmentRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     PermissionSetTypeDef,
-    CustomerManagedPolicyReferenceOutputTypeDef,
     DeleteAccountAssignmentRequestRequestTypeDef,
     DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef,
     DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DeletePermissionSetRequestRequestTypeDef,
     DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef,
     DescribeAccountAssignmentCreationStatusRequestRequestTypeDef,
     DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef,
@@ -383,15 +382,14 @@
     ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListManagedPoliciesInPermissionSetRequestRequestTypeDef,
     PermissionSetProvisioningStatusMetadataTypeDef,
     ListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
     ListPermissionSetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ProvisionPermissionSetRequestRequestTypeDef,
     PutInlinePolicyToPermissionSetRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePermissionSetRequestRequestTypeDef,
     AccessControlAttributeOutputTypeDef,
     AccessControlAttributeTypeDef,
     AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
@@ -402,23 +400,23 @@
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
     GetInlinePolicyForPermissionSetResponseTypeDef,
     ListAccountAssignmentCreationStatusResponseTypeDef,
     ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
     ListAccountsForProvisionedPermissionSetResponseTypeDef,
+    ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
     ListManagedPoliciesInPermissionSetResponseTypeDef,
     ListPermissionSetsProvisionedToAccountResponseTypeDef,
     ListPermissionSetsResponseTypeDef,
     CreatePermissionSetRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreatePermissionSetResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
-    ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
-    PermissionsBoundaryOutputTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     ProvisionPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListAccountAssignmentCreationStatusRequestRequestTypeDef,
     ListAccountAssignmentDeletionStatusRequestRequestTypeDef,
     ListPermissionSetProvisioningStatusRequestRequestTypeDef,
     ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
@@ -429,19 +427,18 @@
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
     ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
     ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
     ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListPermissionSetProvisioningStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     InstanceAccessControlAttributeConfigurationOutputTypeDef,
     InstanceAccessControlAttributeConfigurationTypeDef,
-    PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef,
     GetPermissionsBoundaryForPermissionSetResponseTypeDef,
+    PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
     CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AccessControlAttributeValueOutputTypeDef:
```

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/__init__.py` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/__init__.pyi` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/__main__.py` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSOAdmin 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.SSOAdmin 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin\nOther"
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

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/client.py` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/client.pyi` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/literals.py` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/literals.pyi` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/paginator.py` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/paginator.pyi` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/type_defs.py` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     "CustomerManagedPolicyReferenceTypeDef",
     "AttachManagedPolicyToPermissionSetRequestRequestTypeDef",
     "AttachedManagedPolicyTypeDef",
     "CreateAccountAssignmentRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "PermissionSetTypeDef",
-    "CustomerManagedPolicyReferenceOutputTypeDef",
     "DeleteAccountAssignmentRequestRequestTypeDef",
     "DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef",
     "DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "DeletePermissionSetRequestRequestTypeDef",
     "DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef",
     "DescribeAccountAssignmentCreationStatusRequestRequestTypeDef",
     "DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef",
@@ -69,15 +68,14 @@
     "ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListManagedPoliciesInPermissionSetRequestRequestTypeDef",
     "PermissionSetProvisioningStatusMetadataTypeDef",
     "ListPermissionSetsProvisionedToAccountRequestRequestTypeDef",
     "ListPermissionSetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ProvisionPermissionSetRequestRequestTypeDef",
     "PutInlinePolicyToPermissionSetRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePermissionSetRequestRequestTypeDef",
     "AccessControlAttributeOutputTypeDef",
     "AccessControlAttributeTypeDef",
     "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
@@ -88,23 +86,23 @@
     "DescribeAccountAssignmentCreationStatusResponseTypeDef",
     "DescribeAccountAssignmentDeletionStatusResponseTypeDef",
     "GetInlinePolicyForPermissionSetResponseTypeDef",
     "ListAccountAssignmentCreationStatusResponseTypeDef",
     "ListAccountAssignmentDeletionStatusResponseTypeDef",
     "ListAccountAssignmentsResponseTypeDef",
     "ListAccountsForProvisionedPermissionSetResponseTypeDef",
+    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
     "ListManagedPoliciesInPermissionSetResponseTypeDef",
     "ListPermissionSetsProvisionedToAccountResponseTypeDef",
     "ListPermissionSetsResponseTypeDef",
     "CreatePermissionSetRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreatePermissionSetResponseTypeDef",
     "DescribePermissionSetResponseTypeDef",
-    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
-    "PermissionsBoundaryOutputTypeDef",
     "DescribePermissionSetProvisioningStatusResponseTypeDef",
     "ProvisionPermissionSetResponseTypeDef",
     "ListInstancesResponseTypeDef",
     "ListAccountAssignmentCreationStatusRequestRequestTypeDef",
     "ListAccountAssignmentDeletionStatusRequestRequestTypeDef",
     "ListPermissionSetProvisioningStatusRequestRequestTypeDef",
     "ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
@@ -115,19 +113,18 @@
     "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
     "ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     "ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
     "ListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListPermissionSetProvisioningStatusResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "InstanceAccessControlAttributeConfigurationOutputTypeDef",
     "InstanceAccessControlAttributeConfigurationTypeDef",
-    "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
     "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
+    "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
     "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
 )
 
 AccessControlAttributeValueOutputTypeDef = TypedDict(
     "AccessControlAttributeValueOutputTypeDef",
@@ -259,36 +256,14 @@
         "CreatedDate": datetime,
         "SessionDuration": str,
         "RelayState": str,
     },
     total=False,
 )
 
-_RequiredCustomerManagedPolicyReferenceOutputTypeDef = TypedDict(
-    "_RequiredCustomerManagedPolicyReferenceOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCustomerManagedPolicyReferenceOutputTypeDef = TypedDict(
-    "_OptionalCustomerManagedPolicyReferenceOutputTypeDef",
-    {
-        "Path": str,
-    },
-    total=False,
-)
-
-
-class CustomerManagedPolicyReferenceOutputTypeDef(
-    _RequiredCustomerManagedPolicyReferenceOutputTypeDef,
-    _OptionalCustomerManagedPolicyReferenceOutputTypeDef,
-):
-    pass
-
-
 DeleteAccountAssignmentRequestRequestTypeDef = TypedDict(
     "DeleteAccountAssignmentRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "TargetId": str,
         "TargetType": Literal["AWS_ACCOUNT"],
         "PermissionSetArn": str,
@@ -616,22 +591,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredProvisionPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
         "TargetType": ProvisionTargetTypeType,
     },
@@ -810,14 +777,23 @@
     {
         "AccountIds": List[str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef = TypedDict(
+    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
+    {
+        "CustomerManagedPolicyReferences": List[CustomerManagedPolicyReferenceTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListManagedPoliciesInPermissionSetResponseTypeDef = TypedDict(
     "ListManagedPoliciesInPermissionSetResponseTypeDef",
     {
         "AttachedManagedPolicies": List[AttachedManagedPolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -863,14 +839,23 @@
 class CreatePermissionSetRequestRequestTypeDef(
     _RequiredCreatePermissionSetRequestRequestTypeDef,
     _OptionalCreatePermissionSetRequestRequestTypeDef,
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -888,32 +873,14 @@
     "DescribePermissionSetResponseTypeDef",
     {
         "PermissionSet": PermissionSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef = TypedDict(
-    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
-    {
-        "CustomerManagedPolicyReferences": List[CustomerManagedPolicyReferenceOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PermissionsBoundaryOutputTypeDef = TypedDict(
-    "PermissionsBoundaryOutputTypeDef",
-    {
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceOutputTypeDef,
-        "ManagedPolicyArn": str,
-    },
-    total=False,
-)
-
 DescribePermissionSetProvisioningStatusResponseTypeDef = TypedDict(
     "DescribePermissionSetProvisioningStatusResponseTypeDef",
     {
         "PermissionSetProvisioningStatus": PermissionSetProvisioningStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1252,51 +1219,42 @@
     {
         "PermissionSetsProvisioningStatus": List[PermissionSetProvisioningStatusMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 InstanceAccessControlAttributeConfigurationOutputTypeDef = TypedDict(
     "InstanceAccessControlAttributeConfigurationOutputTypeDef",
     {
         "AccessControlAttributes": List[AccessControlAttributeOutputTypeDef],
     },
 )
 
 InstanceAccessControlAttributeConfigurationTypeDef = TypedDict(
     "InstanceAccessControlAttributeConfigurationTypeDef",
     {
         "AccessControlAttributes": Sequence[AccessControlAttributeTypeDef],
     },
 )
 
-PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef = TypedDict(
-    "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
+GetPermissionsBoundaryForPermissionSetResponseTypeDef = TypedDict(
+    "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
         "PermissionsBoundary": PermissionsBoundaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetPermissionsBoundaryForPermissionSetResponseTypeDef = TypedDict(
-    "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
+PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef = TypedDict(
+    "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
     {
-        "PermissionsBoundary": PermissionsBoundaryOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+        "PermissionsBoundary": PermissionsBoundaryTypeDef,
     },
 )
 
 DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef = TypedDict(
     "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     {
         "Status": InstanceAccessControlAttributeConfigurationStatusType,
```

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin/type_defs.pyi` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     "CustomerManagedPolicyReferenceTypeDef",
     "AttachManagedPolicyToPermissionSetRequestRequestTypeDef",
     "AttachedManagedPolicyTypeDef",
     "CreateAccountAssignmentRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "PermissionSetTypeDef",
-    "CustomerManagedPolicyReferenceOutputTypeDef",
     "DeleteAccountAssignmentRequestRequestTypeDef",
     "DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef",
     "DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "DeletePermissionSetRequestRequestTypeDef",
     "DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef",
     "DescribeAccountAssignmentCreationStatusRequestRequestTypeDef",
     "DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef",
@@ -68,15 +67,14 @@
     "ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListManagedPoliciesInPermissionSetRequestRequestTypeDef",
     "PermissionSetProvisioningStatusMetadataTypeDef",
     "ListPermissionSetsProvisionedToAccountRequestRequestTypeDef",
     "ListPermissionSetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ProvisionPermissionSetRequestRequestTypeDef",
     "PutInlinePolicyToPermissionSetRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePermissionSetRequestRequestTypeDef",
     "AccessControlAttributeOutputTypeDef",
     "AccessControlAttributeTypeDef",
     "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
@@ -87,23 +85,23 @@
     "DescribeAccountAssignmentCreationStatusResponseTypeDef",
     "DescribeAccountAssignmentDeletionStatusResponseTypeDef",
     "GetInlinePolicyForPermissionSetResponseTypeDef",
     "ListAccountAssignmentCreationStatusResponseTypeDef",
     "ListAccountAssignmentDeletionStatusResponseTypeDef",
     "ListAccountAssignmentsResponseTypeDef",
     "ListAccountsForProvisionedPermissionSetResponseTypeDef",
+    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
     "ListManagedPoliciesInPermissionSetResponseTypeDef",
     "ListPermissionSetsProvisionedToAccountResponseTypeDef",
     "ListPermissionSetsResponseTypeDef",
     "CreatePermissionSetRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreatePermissionSetResponseTypeDef",
     "DescribePermissionSetResponseTypeDef",
-    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
-    "PermissionsBoundaryOutputTypeDef",
     "DescribePermissionSetProvisioningStatusResponseTypeDef",
     "ProvisionPermissionSetResponseTypeDef",
     "ListInstancesResponseTypeDef",
     "ListAccountAssignmentCreationStatusRequestRequestTypeDef",
     "ListAccountAssignmentDeletionStatusRequestRequestTypeDef",
     "ListPermissionSetProvisioningStatusRequestRequestTypeDef",
     "ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef",
@@ -114,19 +112,18 @@
     "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
     "ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     "ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
     "ListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListPermissionSetProvisioningStatusResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "InstanceAccessControlAttributeConfigurationOutputTypeDef",
     "InstanceAccessControlAttributeConfigurationTypeDef",
-    "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
     "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
+    "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
     "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
 )
 
 AccessControlAttributeValueOutputTypeDef = TypedDict(
     "AccessControlAttributeValueOutputTypeDef",
@@ -256,34 +253,14 @@
         "CreatedDate": datetime,
         "SessionDuration": str,
         "RelayState": str,
     },
     total=False,
 )
 
-_RequiredCustomerManagedPolicyReferenceOutputTypeDef = TypedDict(
-    "_RequiredCustomerManagedPolicyReferenceOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCustomerManagedPolicyReferenceOutputTypeDef = TypedDict(
-    "_OptionalCustomerManagedPolicyReferenceOutputTypeDef",
-    {
-        "Path": str,
-    },
-    total=False,
-)
-
-class CustomerManagedPolicyReferenceOutputTypeDef(
-    _RequiredCustomerManagedPolicyReferenceOutputTypeDef,
-    _OptionalCustomerManagedPolicyReferenceOutputTypeDef,
-):
-    pass
-
 DeleteAccountAssignmentRequestRequestTypeDef = TypedDict(
     "DeleteAccountAssignmentRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "TargetId": str,
         "TargetType": Literal["AWS_ACCOUNT"],
         "PermissionSetArn": str,
@@ -597,22 +574,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredProvisionPermissionSetRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionPermissionSetRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
         "TargetType": ProvisionTargetTypeType,
     },
@@ -787,14 +756,23 @@
     {
         "AccountIds": List[str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef = TypedDict(
+    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
+    {
+        "CustomerManagedPolicyReferences": List[CustomerManagedPolicyReferenceTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListManagedPoliciesInPermissionSetResponseTypeDef = TypedDict(
     "ListManagedPoliciesInPermissionSetResponseTypeDef",
     {
         "AttachedManagedPolicies": List[AttachedManagedPolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -838,14 +816,23 @@
 
 class CreatePermissionSetRequestRequestTypeDef(
     _RequiredCreatePermissionSetRequestRequestTypeDef,
     _OptionalCreatePermissionSetRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -863,32 +850,14 @@
     "DescribePermissionSetResponseTypeDef",
     {
         "PermissionSet": PermissionSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef = TypedDict(
-    "ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef",
-    {
-        "CustomerManagedPolicyReferences": List[CustomerManagedPolicyReferenceOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PermissionsBoundaryOutputTypeDef = TypedDict(
-    "PermissionsBoundaryOutputTypeDef",
-    {
-        "CustomerManagedPolicyReference": CustomerManagedPolicyReferenceOutputTypeDef,
-        "ManagedPolicyArn": str,
-    },
-    total=False,
-)
-
 DescribePermissionSetProvisioningStatusResponseTypeDef = TypedDict(
     "DescribePermissionSetProvisioningStatusResponseTypeDef",
     {
         "PermissionSetProvisioningStatus": PermissionSetProvisioningStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1201,51 +1170,42 @@
     {
         "PermissionSetsProvisioningStatus": List[PermissionSetProvisioningStatusMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 InstanceAccessControlAttributeConfigurationOutputTypeDef = TypedDict(
     "InstanceAccessControlAttributeConfigurationOutputTypeDef",
     {
         "AccessControlAttributes": List[AccessControlAttributeOutputTypeDef],
     },
 )
 
 InstanceAccessControlAttributeConfigurationTypeDef = TypedDict(
     "InstanceAccessControlAttributeConfigurationTypeDef",
     {
         "AccessControlAttributes": Sequence[AccessControlAttributeTypeDef],
     },
 )
 
-PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef = TypedDict(
-    "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
+GetPermissionsBoundaryForPermissionSetResponseTypeDef = TypedDict(
+    "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     {
-        "InstanceArn": str,
-        "PermissionSetArn": str,
         "PermissionsBoundary": PermissionsBoundaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetPermissionsBoundaryForPermissionSetResponseTypeDef = TypedDict(
-    "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
+PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef = TypedDict(
+    "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
     {
-        "PermissionsBoundary": PermissionsBoundaryOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "InstanceArn": str,
+        "PermissionSetArn": str,
+        "PermissionsBoundary": PermissionsBoundaryTypeDef,
     },
 )
 
 DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef = TypedDict(
     "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     {
         "Status": InstanceAccessControlAttributeConfigurationStatusType,
```

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/PKG-INFO` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sso-admin
-Version: 1.28.12
-Summary: Type annotations for boto3.SSOAdmin 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SSOAdmin 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sso-admin.svg?color=blue)](https://pypi.org/project/mypy-boto3-sso-admin)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sso-admin)](https://pepy.tech/project/mypy-boto3-sso-admin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSOAdmin 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
+[boto3.SSOAdmin 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
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
 [mypy-boto3-sso-admin docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sso_admin/).
 
 See how it helps to find and fix potential bugs:
 
@@ -388,15 +388,14 @@
     CustomerManagedPolicyReferenceTypeDef,
     AttachManagedPolicyToPermissionSetRequestRequestTypeDef,
     AttachedManagedPolicyTypeDef,
     CreateAccountAssignmentRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     PermissionSetTypeDef,
-    CustomerManagedPolicyReferenceOutputTypeDef,
     DeleteAccountAssignmentRequestRequestTypeDef,
     DeleteInlinePolicyFromPermissionSetRequestRequestTypeDef,
     DeleteInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     DeletePermissionSetRequestRequestTypeDef,
     DeletePermissionsBoundaryFromPermissionSetRequestRequestTypeDef,
     DescribeAccountAssignmentCreationStatusRequestRequestTypeDef,
     DescribeAccountAssignmentDeletionStatusRequestRequestTypeDef,
@@ -415,15 +414,14 @@
     ListCustomerManagedPolicyReferencesInPermissionSetRequestRequestTypeDef,
     ListInstancesRequestRequestTypeDef,
     ListManagedPoliciesInPermissionSetRequestRequestTypeDef,
     PermissionSetProvisioningStatusMetadataTypeDef,
     ListPermissionSetsProvisionedToAccountRequestRequestTypeDef,
     ListPermissionSetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ProvisionPermissionSetRequestRequestTypeDef,
     PutInlinePolicyToPermissionSetRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePermissionSetRequestRequestTypeDef,
     AccessControlAttributeOutputTypeDef,
     AccessControlAttributeTypeDef,
     AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef,
@@ -434,23 +432,23 @@
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
     GetInlinePolicyForPermissionSetResponseTypeDef,
     ListAccountAssignmentCreationStatusResponseTypeDef,
     ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
     ListAccountsForProvisionedPermissionSetResponseTypeDef,
+    ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
     ListManagedPoliciesInPermissionSetResponseTypeDef,
     ListPermissionSetsProvisionedToAccountResponseTypeDef,
     ListPermissionSetsResponseTypeDef,
     CreatePermissionSetRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreatePermissionSetResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
-    ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
-    PermissionsBoundaryOutputTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     ProvisionPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListAccountAssignmentCreationStatusRequestRequestTypeDef,
     ListAccountAssignmentDeletionStatusRequestRequestTypeDef,
     ListPermissionSetProvisioningStatusRequestRequestTypeDef,
     ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef,
@@ -461,19 +459,18 @@
     ListInstancesRequestListInstancesPaginateTypeDef,
     ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef,
     ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef,
     ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef,
     ListPermissionSetsRequestListPermissionSetsPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListPermissionSetProvisioningStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     InstanceAccessControlAttributeConfigurationOutputTypeDef,
     InstanceAccessControlAttributeConfigurationTypeDef,
-    PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef,
     GetPermissionsBoundaryForPermissionSetResponseTypeDef,
+    PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
     CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
     UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AccessControlAttributeValueOutputTypeDef:
```

### Comparing `mypy-boto3-sso-admin-1.28.12/mypy_boto3_sso_admin.egg-info/SOURCES.txt` & `mypy-boto3-sso-admin-1.28.15/mypy_boto3_sso_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sso-admin-1.28.12/setup.py` & `mypy-boto3-sso-admin-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sso-admin",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_sso_admin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSOAdmin 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.SSOAdmin 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

