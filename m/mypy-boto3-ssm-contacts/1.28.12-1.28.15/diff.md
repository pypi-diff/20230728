# Comparing `tmp/mypy-boto3-ssm-contacts-1.28.12.tar.gz` & `tmp/mypy-boto3-ssm-contacts-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-contacts-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-contacts-1.28.15.tar", last modified: Fri Jul 28 20:43:48 2023, max compression
```

## Comparing `mypy-boto3-ssm-contacts-1.28.12.tar` & `mypy-boto3-ssm-contacts-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.665320 mypy-boto3-ssm-contacts-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-07-27 11:49:41.657320 mypy-boto3-ssm-contacts-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.657320 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32233 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-07-27 11:47:29.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-27 11:47:29.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42975 2023-07-27 11:47:30.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42894 2023-07-27 11:47:29.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.657320 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-07-27 11:49:41.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 11:49:41.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:41.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 11:49:41.000000 mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.665320 mypy-boto3-ssm-contacts-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 11:47:28.000000 mypy-boto3-ssm-contacts-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:48.313927 mypy-boto3-ssm-contacts-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-07-28 20:43:48.301927 mypy-boto3-ssm-contacts-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:48.301927 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32233 2023-07-28 20:40:03.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-07-28 20:40:03.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-28 20:40:03.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-07-28 20:40:03.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-28 20:40:03.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40555 2023-07-28 20:40:04.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40478 2023-07-28 20:40:04.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:48.301927 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-07-28 20:43:48.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:43:48.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:48.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:48.000000 mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:48.313927 mypy-boto3-ssm-contacts-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 20:40:02.000000 mypy-boto3-ssm-contacts-1.28.15/setup.py
```

### Comparing `mypy-boto3-ssm-contacts-1.28.12/LICENSE` & `mypy-boto3-ssm-contacts-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.12/PKG-INFO` & `mypy-boto3-ssm-contacts-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-contacts
-Version: 1.28.12
-Summary: Type annotations for boto3.SSMContacts 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SSMContacts 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-contacts)](https://pepy.tech/project/mypy-boto3-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMContacts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[boto3.SSMContacts 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,22 +375,18 @@
 `mypy_boto3_ssm_contacts.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_contacts.type_defs import (
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
-    ChannelTargetInfoOutputTypeDef,
     ChannelTargetInfoTypeDef,
-    ContactChannelAddressOutputTypeDef,
     ContactChannelAddressTypeDef,
-    ContactTargetInfoOutputTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
-    HandOffTimeOutputTypeDef,
     HandOffTimeTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreateRotationOverrideRequestRequestTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
@@ -417,43 +413,39 @@
     ListPagesByEngagementRequestRequestTypeDef,
     PreviewOverrideTypeDef,
     ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
     ListRotationShiftsRequestRequestTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     PutContactPolicyRequestRequestTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
     StopEngagementRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ContactChannelTypeDef,
     CreateContactChannelRequestRequestTypeDef,
     UpdateContactChannelRequestRequestTypeDef,
-    TargetOutputTypeDef,
     TargetTypeDef,
-    CoverageTimeOutputTypeDef,
-    MonthlySettingOutputTypeDef,
-    WeeklySettingOutputTypeDef,
     CoverageTimeTypeDef,
     MonthlySettingTypeDef,
     WeeklySettingTypeDef,
     CreateContactChannelResultTypeDef,
     CreateContactResultTypeDef,
     CreateRotationOverrideResultTypeDef,
     CreateRotationResultTypeDef,
     DescribeEngagementResultTypeDef,
     DescribePageResultTypeDef,
     GetContactChannelResultTypeDef,
     GetContactPolicyResultTypeDef,
     GetRotationOverrideResultTypeDef,
     ListContactsResultTypeDef,
     StartEngagementResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEngagementsResultTypeDef,
     ListContactChannelsRequestListContactChannelsPaginateTypeDef,
     ListContactsRequestListContactsPaginateTypeDef,
     ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPagesByContactRequestListPagesByContactPaginateTypeDef,
@@ -464,15 +456,14 @@
     ListEngagementsRequestListEngagementsPaginateTypeDef,
     ListEngagementsRequestRequestTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
-    ListTagsForResourceResultTypeDef,
     RotationShiftTypeDef,
     ListContactChannelsResultTypeDef,
     StageOutputTypeDef,
     StageTypeDef,
     RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
```

### Comparing `mypy-boto3-ssm-contacts-1.28.12/README.md` & `mypy-boto3-ssm-contacts-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-contacts)](https://pepy.tech/project/mypy-boto3-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMContacts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[boto3.SSMContacts 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,22 +343,18 @@
 `mypy_boto3_ssm_contacts.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_contacts.type_defs import (
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
-    ChannelTargetInfoOutputTypeDef,
     ChannelTargetInfoTypeDef,
-    ContactChannelAddressOutputTypeDef,
     ContactChannelAddressTypeDef,
-    ContactTargetInfoOutputTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
-    HandOffTimeOutputTypeDef,
     HandOffTimeTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreateRotationOverrideRequestRequestTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
@@ -385,43 +381,39 @@
     ListPagesByEngagementRequestRequestTypeDef,
     PreviewOverrideTypeDef,
     ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
     ListRotationShiftsRequestRequestTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     PutContactPolicyRequestRequestTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
     StopEngagementRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ContactChannelTypeDef,
     CreateContactChannelRequestRequestTypeDef,
     UpdateContactChannelRequestRequestTypeDef,
-    TargetOutputTypeDef,
     TargetTypeDef,
-    CoverageTimeOutputTypeDef,
-    MonthlySettingOutputTypeDef,
-    WeeklySettingOutputTypeDef,
     CoverageTimeTypeDef,
     MonthlySettingTypeDef,
     WeeklySettingTypeDef,
     CreateContactChannelResultTypeDef,
     CreateContactResultTypeDef,
     CreateRotationOverrideResultTypeDef,
     CreateRotationResultTypeDef,
     DescribeEngagementResultTypeDef,
     DescribePageResultTypeDef,
     GetContactChannelResultTypeDef,
     GetContactPolicyResultTypeDef,
     GetRotationOverrideResultTypeDef,
     ListContactsResultTypeDef,
     StartEngagementResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEngagementsResultTypeDef,
     ListContactChannelsRequestListContactChannelsPaginateTypeDef,
     ListContactsRequestListContactsPaginateTypeDef,
     ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPagesByContactRequestListPagesByContactPaginateTypeDef,
@@ -432,15 +424,14 @@
     ListEngagementsRequestListEngagementsPaginateTypeDef,
     ListEngagementsRequestRequestTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
-    ListTagsForResourceResultTypeDef,
     RotationShiftTypeDef,
     ListContactChannelsResultTypeDef,
     StageOutputTypeDef,
     StageTypeDef,
     RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
```

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/__init__.py` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/__init__.pyi` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/__main__.py` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSMContacts 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.SSMContacts 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts\nOther"
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

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/client.py` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/client.pyi` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/literals.py` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/literals.pyi` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/paginator.py` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/paginator.pyi` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/type_defs.py` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,18 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptPageRequestRequestTypeDef",
     "ActivateContactChannelRequestRequestTypeDef",
-    "ChannelTargetInfoOutputTypeDef",
     "ChannelTargetInfoTypeDef",
-    "ContactChannelAddressOutputTypeDef",
     "ContactChannelAddressTypeDef",
-    "ContactTargetInfoOutputTypeDef",
     "ContactTargetInfoTypeDef",
     "ContactTypeDef",
-    "HandOffTimeOutputTypeDef",
     "HandOffTimeTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreateRotationOverrideRequestRequestTypeDef",
     "DeactivateContactChannelRequestRequestTypeDef",
     "DeleteContactChannelRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
@@ -73,43 +69,39 @@
     "ListPagesByEngagementRequestRequestTypeDef",
     "PreviewOverrideTypeDef",
     "ListRotationOverridesRequestRequestTypeDef",
     "RotationOverrideTypeDef",
     "ListRotationShiftsRequestRequestTypeDef",
     "ListRotationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "PutContactPolicyRequestRequestTypeDef",
     "ShiftDetailsTypeDef",
     "SendActivationCodeRequestRequestTypeDef",
     "StartEngagementRequestRequestTypeDef",
     "StopEngagementRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ContactChannelTypeDef",
     "CreateContactChannelRequestRequestTypeDef",
     "UpdateContactChannelRequestRequestTypeDef",
-    "TargetOutputTypeDef",
     "TargetTypeDef",
-    "CoverageTimeOutputTypeDef",
-    "MonthlySettingOutputTypeDef",
-    "WeeklySettingOutputTypeDef",
     "CoverageTimeTypeDef",
     "MonthlySettingTypeDef",
     "WeeklySettingTypeDef",
     "CreateContactChannelResultTypeDef",
     "CreateContactResultTypeDef",
     "CreateRotationOverrideResultTypeDef",
     "CreateRotationResultTypeDef",
     "DescribeEngagementResultTypeDef",
     "DescribePageResultTypeDef",
     "GetContactChannelResultTypeDef",
     "GetContactPolicyResultTypeDef",
     "GetRotationOverrideResultTypeDef",
     "ListContactsResultTypeDef",
     "StartEngagementResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEngagementsResultTypeDef",
     "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
     "ListContactsRequestListContactsPaginateTypeDef",
     "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
     "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
     "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
@@ -120,15 +112,14 @@
     "ListEngagementsRequestListEngagementsPaginateTypeDef",
     "ListEngagementsRequestRequestTypeDef",
     "ListPageReceiptsResultTypeDef",
     "ListPageResolutionsResultTypeDef",
     "ListPagesByContactResultTypeDef",
     "ListPagesByEngagementResultTypeDef",
     "ListRotationOverridesResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "RotationShiftTypeDef",
     "ListContactChannelsResultTypeDef",
     "StageOutputTypeDef",
     "StageTypeDef",
     "RecurrenceSettingsOutputTypeDef",
     "RecurrenceSettingsTypeDef",
     "ListPreviewRotationShiftsResultTypeDef",
@@ -176,35 +167,14 @@
     "ActivateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
         "ActivationCode": str,
     },
 )
 
-_RequiredChannelTargetInfoOutputTypeDef = TypedDict(
-    "_RequiredChannelTargetInfoOutputTypeDef",
-    {
-        "ContactChannelId": str,
-    },
-)
-_OptionalChannelTargetInfoOutputTypeDef = TypedDict(
-    "_OptionalChannelTargetInfoOutputTypeDef",
-    {
-        "RetryIntervalInMinutes": int,
-    },
-    total=False,
-)
-
-
-class ChannelTargetInfoOutputTypeDef(
-    _RequiredChannelTargetInfoOutputTypeDef, _OptionalChannelTargetInfoOutputTypeDef
-):
-    pass
-
-
 _RequiredChannelTargetInfoTypeDef = TypedDict(
     "_RequiredChannelTargetInfoTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 _OptionalChannelTargetInfoTypeDef = TypedDict(
@@ -218,51 +188,22 @@
 
 class ChannelTargetInfoTypeDef(
     _RequiredChannelTargetInfoTypeDef, _OptionalChannelTargetInfoTypeDef
 ):
     pass
 
 
-ContactChannelAddressOutputTypeDef = TypedDict(
-    "ContactChannelAddressOutputTypeDef",
-    {
-        "SimpleAddress": str,
-    },
-    total=False,
-)
-
 ContactChannelAddressTypeDef = TypedDict(
     "ContactChannelAddressTypeDef",
     {
         "SimpleAddress": str,
     },
     total=False,
 )
 
-_RequiredContactTargetInfoOutputTypeDef = TypedDict(
-    "_RequiredContactTargetInfoOutputTypeDef",
-    {
-        "IsEssential": bool,
-    },
-)
-_OptionalContactTargetInfoOutputTypeDef = TypedDict(
-    "_OptionalContactTargetInfoOutputTypeDef",
-    {
-        "ContactId": str,
-    },
-    total=False,
-)
-
-
-class ContactTargetInfoOutputTypeDef(
-    _RequiredContactTargetInfoOutputTypeDef, _OptionalContactTargetInfoOutputTypeDef
-):
-    pass
-
-
 _RequiredContactTargetInfoTypeDef = TypedDict(
     "_RequiredContactTargetInfoTypeDef",
     {
         "IsEssential": bool,
     },
 )
 _OptionalContactTargetInfoTypeDef = TypedDict(
@@ -297,22 +238,14 @@
 )
 
 
 class ContactTypeDef(_RequiredContactTypeDef, _OptionalContactTypeDef):
     pass
 
 
-HandOffTimeOutputTypeDef = TypedDict(
-    "HandOffTimeOutputTypeDef",
-    {
-        "HourOfDay": int,
-        "MinuteOfHour": int,
-    },
-)
-
 HandOffTimeTypeDef = TypedDict(
     "HandOffTimeTypeDef",
     {
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
 )
@@ -766,23 +699,14 @@
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
-    total=False,
-)
-
 PutContactPolicyRequestRequestTypeDef = TypedDict(
     "PutContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
         "Policy": str,
     },
 )
@@ -859,15 +783,15 @@
 
 _RequiredContactChannelTypeDef = TypedDict(
     "_RequiredContactChannelTypeDef",
     {
         "ContactChannelArn": str,
         "ContactArn": str,
         "Name": str,
-        "DeliveryAddress": ContactChannelAddressOutputTypeDef,
+        "DeliveryAddress": ContactChannelAddressTypeDef,
         "ActivationStatus": ActivationStatusType,
     },
 )
 _OptionalContactChannelTypeDef = TypedDict(
     "_OptionalContactChannelTypeDef",
     {
         "Type": ChannelTypeType,
@@ -925,57 +849,23 @@
 class UpdateContactChannelRequestRequestTypeDef(
     _RequiredUpdateContactChannelRequestRequestTypeDef,
     _OptionalUpdateContactChannelRequestRequestTypeDef,
 ):
     pass
 
 
-TargetOutputTypeDef = TypedDict(
-    "TargetOutputTypeDef",
-    {
-        "ChannelTargetInfo": ChannelTargetInfoOutputTypeDef,
-        "ContactTargetInfo": ContactTargetInfoOutputTypeDef,
-    },
-    total=False,
-)
-
 TargetTypeDef = TypedDict(
     "TargetTypeDef",
     {
         "ChannelTargetInfo": ChannelTargetInfoTypeDef,
         "ContactTargetInfo": ContactTargetInfoTypeDef,
     },
     total=False,
 )
 
-CoverageTimeOutputTypeDef = TypedDict(
-    "CoverageTimeOutputTypeDef",
-    {
-        "Start": HandOffTimeOutputTypeDef,
-        "End": HandOffTimeOutputTypeDef,
-    },
-    total=False,
-)
-
-MonthlySettingOutputTypeDef = TypedDict(
-    "MonthlySettingOutputTypeDef",
-    {
-        "DayOfMonth": int,
-        "HandOffTime": HandOffTimeOutputTypeDef,
-    },
-)
-
-WeeklySettingOutputTypeDef = TypedDict(
-    "WeeklySettingOutputTypeDef",
-    {
-        "DayOfWeek": DayOfWeekType,
-        "HandOffTime": HandOffTimeOutputTypeDef,
-    },
-)
-
 CoverageTimeTypeDef = TypedDict(
     "CoverageTimeTypeDef",
     {
         "Start": HandOffTimeTypeDef,
         "End": HandOffTimeTypeDef,
     },
     total=False,
@@ -1068,15 +958,15 @@
 GetContactChannelResultTypeDef = TypedDict(
     "GetContactChannelResultTypeDef",
     {
         "ContactArn": str,
         "ContactChannelArn": str,
         "Name": str,
         "Type": ChannelTypeType,
-        "DeliveryAddress": ContactChannelAddressOutputTypeDef,
+        "DeliveryAddress": ContactChannelAddressTypeDef,
         "ActivationStatus": ActivationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContactPolicyResultTypeDef = TypedDict(
     "GetContactPolicyResultTypeDef",
@@ -1113,14 +1003,22 @@
     "StartEngagementResultTypeDef",
     {
         "EngagementArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1373,22 +1271,14 @@
     {
         "RotationOverrides": List[RotationOverrideTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredRotationShiftTypeDef = TypedDict(
     "_RequiredRotationShiftTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
 )
@@ -1416,15 +1306,15 @@
     },
 )
 
 StageOutputTypeDef = TypedDict(
     "StageOutputTypeDef",
     {
         "DurationInMinutes": int,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
     },
 )
 
 StageTypeDef = TypedDict(
     "StageTypeDef",
     {
         "DurationInMinutes": int,
@@ -1438,18 +1328,18 @@
         "NumberOfOnCalls": int,
         "RecurrenceMultiplier": int,
     },
 )
 _OptionalRecurrenceSettingsOutputTypeDef = TypedDict(
     "_OptionalRecurrenceSettingsOutputTypeDef",
     {
-        "MonthlySettings": List[MonthlySettingOutputTypeDef],
-        "WeeklySettings": List[WeeklySettingOutputTypeDef],
-        "DailySettings": List[HandOffTimeOutputTypeDef],
-        "ShiftCoverages": Dict[DayOfWeekType, List[CoverageTimeOutputTypeDef]],
+        "MonthlySettings": List[MonthlySettingTypeDef],
+        "WeeklySettings": List[WeeklySettingTypeDef],
+        "DailySettings": List[HandOffTimeTypeDef],
+        "ShiftCoverages": Dict[DayOfWeekType, List[CoverageTimeTypeDef]],
     },
     total=False,
 )
 
 
 class RecurrenceSettingsOutputTypeDef(
     _RequiredRecurrenceSettingsOutputTypeDef, _OptionalRecurrenceSettingsOutputTypeDef
```

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts/type_defs.pyi` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -30,22 +30,18 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptPageRequestRequestTypeDef",
     "ActivateContactChannelRequestRequestTypeDef",
-    "ChannelTargetInfoOutputTypeDef",
     "ChannelTargetInfoTypeDef",
-    "ContactChannelAddressOutputTypeDef",
     "ContactChannelAddressTypeDef",
-    "ContactTargetInfoOutputTypeDef",
     "ContactTargetInfoTypeDef",
     "ContactTypeDef",
-    "HandOffTimeOutputTypeDef",
     "HandOffTimeTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "CreateRotationOverrideRequestRequestTypeDef",
     "DeactivateContactChannelRequestRequestTypeDef",
     "DeleteContactChannelRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
@@ -72,43 +68,39 @@
     "ListPagesByEngagementRequestRequestTypeDef",
     "PreviewOverrideTypeDef",
     "ListRotationOverridesRequestRequestTypeDef",
     "RotationOverrideTypeDef",
     "ListRotationShiftsRequestRequestTypeDef",
     "ListRotationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "PutContactPolicyRequestRequestTypeDef",
     "ShiftDetailsTypeDef",
     "SendActivationCodeRequestRequestTypeDef",
     "StartEngagementRequestRequestTypeDef",
     "StopEngagementRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ContactChannelTypeDef",
     "CreateContactChannelRequestRequestTypeDef",
     "UpdateContactChannelRequestRequestTypeDef",
-    "TargetOutputTypeDef",
     "TargetTypeDef",
-    "CoverageTimeOutputTypeDef",
-    "MonthlySettingOutputTypeDef",
-    "WeeklySettingOutputTypeDef",
     "CoverageTimeTypeDef",
     "MonthlySettingTypeDef",
     "WeeklySettingTypeDef",
     "CreateContactChannelResultTypeDef",
     "CreateContactResultTypeDef",
     "CreateRotationOverrideResultTypeDef",
     "CreateRotationResultTypeDef",
     "DescribeEngagementResultTypeDef",
     "DescribePageResultTypeDef",
     "GetContactChannelResultTypeDef",
     "GetContactPolicyResultTypeDef",
     "GetRotationOverrideResultTypeDef",
     "ListContactsResultTypeDef",
     "StartEngagementResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEngagementsResultTypeDef",
     "ListContactChannelsRequestListContactChannelsPaginateTypeDef",
     "ListContactsRequestListContactsPaginateTypeDef",
     "ListPageReceiptsRequestListPageReceiptsPaginateTypeDef",
     "ListPageResolutionsRequestListPageResolutionsPaginateTypeDef",
     "ListPagesByContactRequestListPagesByContactPaginateTypeDef",
@@ -119,15 +111,14 @@
     "ListEngagementsRequestListEngagementsPaginateTypeDef",
     "ListEngagementsRequestRequestTypeDef",
     "ListPageReceiptsResultTypeDef",
     "ListPageResolutionsResultTypeDef",
     "ListPagesByContactResultTypeDef",
     "ListPagesByEngagementResultTypeDef",
     "ListRotationOverridesResultTypeDef",
-    "ListTagsForResourceResultTypeDef",
     "RotationShiftTypeDef",
     "ListContactChannelsResultTypeDef",
     "StageOutputTypeDef",
     "StageTypeDef",
     "RecurrenceSettingsOutputTypeDef",
     "RecurrenceSettingsTypeDef",
     "ListPreviewRotationShiftsResultTypeDef",
@@ -173,33 +164,14 @@
     "ActivateContactChannelRequestRequestTypeDef",
     {
         "ContactChannelId": str,
         "ActivationCode": str,
     },
 )
 
-_RequiredChannelTargetInfoOutputTypeDef = TypedDict(
-    "_RequiredChannelTargetInfoOutputTypeDef",
-    {
-        "ContactChannelId": str,
-    },
-)
-_OptionalChannelTargetInfoOutputTypeDef = TypedDict(
-    "_OptionalChannelTargetInfoOutputTypeDef",
-    {
-        "RetryIntervalInMinutes": int,
-    },
-    total=False,
-)
-
-class ChannelTargetInfoOutputTypeDef(
-    _RequiredChannelTargetInfoOutputTypeDef, _OptionalChannelTargetInfoOutputTypeDef
-):
-    pass
-
 _RequiredChannelTargetInfoTypeDef = TypedDict(
     "_RequiredChannelTargetInfoTypeDef",
     {
         "ContactChannelId": str,
     },
 )
 _OptionalChannelTargetInfoTypeDef = TypedDict(
@@ -211,49 +183,22 @@
 )
 
 class ChannelTargetInfoTypeDef(
     _RequiredChannelTargetInfoTypeDef, _OptionalChannelTargetInfoTypeDef
 ):
     pass
 
-ContactChannelAddressOutputTypeDef = TypedDict(
-    "ContactChannelAddressOutputTypeDef",
-    {
-        "SimpleAddress": str,
-    },
-    total=False,
-)
-
 ContactChannelAddressTypeDef = TypedDict(
     "ContactChannelAddressTypeDef",
     {
         "SimpleAddress": str,
     },
     total=False,
 )
 
-_RequiredContactTargetInfoOutputTypeDef = TypedDict(
-    "_RequiredContactTargetInfoOutputTypeDef",
-    {
-        "IsEssential": bool,
-    },
-)
-_OptionalContactTargetInfoOutputTypeDef = TypedDict(
-    "_OptionalContactTargetInfoOutputTypeDef",
-    {
-        "ContactId": str,
-    },
-    total=False,
-)
-
-class ContactTargetInfoOutputTypeDef(
-    _RequiredContactTargetInfoOutputTypeDef, _OptionalContactTargetInfoOutputTypeDef
-):
-    pass
-
 _RequiredContactTargetInfoTypeDef = TypedDict(
     "_RequiredContactTargetInfoTypeDef",
     {
         "IsEssential": bool,
     },
 )
 _OptionalContactTargetInfoTypeDef = TypedDict(
@@ -284,22 +229,14 @@
     },
     total=False,
 )
 
 class ContactTypeDef(_RequiredContactTypeDef, _OptionalContactTypeDef):
     pass
 
-HandOffTimeOutputTypeDef = TypedDict(
-    "HandOffTimeOutputTypeDef",
-    {
-        "HourOfDay": int,
-        "MinuteOfHour": int,
-    },
-)
-
 HandOffTimeTypeDef = TypedDict(
     "HandOffTimeTypeDef",
     {
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
 )
@@ -729,23 +666,14 @@
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
-    total=False,
-)
-
 PutContactPolicyRequestRequestTypeDef = TypedDict(
     "PutContactPolicyRequestRequestTypeDef",
     {
         "ContactArn": str,
         "Policy": str,
     },
 )
@@ -818,15 +746,15 @@
 
 _RequiredContactChannelTypeDef = TypedDict(
     "_RequiredContactChannelTypeDef",
     {
         "ContactChannelArn": str,
         "ContactArn": str,
         "Name": str,
-        "DeliveryAddress": ContactChannelAddressOutputTypeDef,
+        "DeliveryAddress": ContactChannelAddressTypeDef,
         "ActivationStatus": ActivationStatusType,
     },
 )
 _OptionalContactChannelTypeDef = TypedDict(
     "_OptionalContactChannelTypeDef",
     {
         "Type": ChannelTypeType,
@@ -878,57 +806,23 @@
 
 class UpdateContactChannelRequestRequestTypeDef(
     _RequiredUpdateContactChannelRequestRequestTypeDef,
     _OptionalUpdateContactChannelRequestRequestTypeDef,
 ):
     pass
 
-TargetOutputTypeDef = TypedDict(
-    "TargetOutputTypeDef",
-    {
-        "ChannelTargetInfo": ChannelTargetInfoOutputTypeDef,
-        "ContactTargetInfo": ContactTargetInfoOutputTypeDef,
-    },
-    total=False,
-)
-
 TargetTypeDef = TypedDict(
     "TargetTypeDef",
     {
         "ChannelTargetInfo": ChannelTargetInfoTypeDef,
         "ContactTargetInfo": ContactTargetInfoTypeDef,
     },
     total=False,
 )
 
-CoverageTimeOutputTypeDef = TypedDict(
-    "CoverageTimeOutputTypeDef",
-    {
-        "Start": HandOffTimeOutputTypeDef,
-        "End": HandOffTimeOutputTypeDef,
-    },
-    total=False,
-)
-
-MonthlySettingOutputTypeDef = TypedDict(
-    "MonthlySettingOutputTypeDef",
-    {
-        "DayOfMonth": int,
-        "HandOffTime": HandOffTimeOutputTypeDef,
-    },
-)
-
-WeeklySettingOutputTypeDef = TypedDict(
-    "WeeklySettingOutputTypeDef",
-    {
-        "DayOfWeek": DayOfWeekType,
-        "HandOffTime": HandOffTimeOutputTypeDef,
-    },
-)
-
 CoverageTimeTypeDef = TypedDict(
     "CoverageTimeTypeDef",
     {
         "Start": HandOffTimeTypeDef,
         "End": HandOffTimeTypeDef,
     },
     total=False,
@@ -1021,15 +915,15 @@
 GetContactChannelResultTypeDef = TypedDict(
     "GetContactChannelResultTypeDef",
     {
         "ContactArn": str,
         "ContactChannelArn": str,
         "Name": str,
         "Type": ChannelTypeType,
-        "DeliveryAddress": ContactChannelAddressOutputTypeDef,
+        "DeliveryAddress": ContactChannelAddressTypeDef,
         "ActivationStatus": ActivationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContactPolicyResultTypeDef = TypedDict(
     "GetContactPolicyResultTypeDef",
@@ -1066,14 +960,22 @@
     "StartEngagementResultTypeDef",
     {
         "EngagementArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1312,22 +1214,14 @@
     {
         "RotationOverrides": List[RotationOverrideTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredRotationShiftTypeDef = TypedDict(
     "_RequiredRotationShiftTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
 )
@@ -1353,15 +1247,15 @@
     },
 )
 
 StageOutputTypeDef = TypedDict(
     "StageOutputTypeDef",
     {
         "DurationInMinutes": int,
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
     },
 )
 
 StageTypeDef = TypedDict(
     "StageTypeDef",
     {
         "DurationInMinutes": int,
@@ -1375,18 +1269,18 @@
         "NumberOfOnCalls": int,
         "RecurrenceMultiplier": int,
     },
 )
 _OptionalRecurrenceSettingsOutputTypeDef = TypedDict(
     "_OptionalRecurrenceSettingsOutputTypeDef",
     {
-        "MonthlySettings": List[MonthlySettingOutputTypeDef],
-        "WeeklySettings": List[WeeklySettingOutputTypeDef],
-        "DailySettings": List[HandOffTimeOutputTypeDef],
-        "ShiftCoverages": Dict[DayOfWeekType, List[CoverageTimeOutputTypeDef]],
+        "MonthlySettings": List[MonthlySettingTypeDef],
+        "WeeklySettings": List[WeeklySettingTypeDef],
+        "DailySettings": List[HandOffTimeTypeDef],
+        "ShiftCoverages": Dict[DayOfWeekType, List[CoverageTimeTypeDef]],
     },
     total=False,
 )
 
 class RecurrenceSettingsOutputTypeDef(
     _RequiredRecurrenceSettingsOutputTypeDef, _OptionalRecurrenceSettingsOutputTypeDef
 ):
```

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/PKG-INFO` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-contacts
-Version: 1.28.12
-Summary: Type annotations for boto3.SSMContacts 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SSMContacts 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-contacts.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-contacts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-contacts)](https://pepy.tech/project/mypy-boto3-ssm-contacts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMContacts 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
+[boto3.SSMContacts 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
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
 [mypy-boto3-ssm-contacts docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_contacts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,22 +375,18 @@
 `mypy_boto3_ssm_contacts.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_contacts.type_defs import (
     AcceptPageRequestRequestTypeDef,
     ActivateContactChannelRequestRequestTypeDef,
-    ChannelTargetInfoOutputTypeDef,
     ChannelTargetInfoTypeDef,
-    ContactChannelAddressOutputTypeDef,
     ContactChannelAddressTypeDef,
-    ContactTargetInfoOutputTypeDef,
     ContactTargetInfoTypeDef,
     ContactTypeDef,
-    HandOffTimeOutputTypeDef,
     HandOffTimeTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     CreateRotationOverrideRequestRequestTypeDef,
     DeactivateContactChannelRequestRequestTypeDef,
     DeleteContactChannelRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
@@ -417,43 +413,39 @@
     ListPagesByEngagementRequestRequestTypeDef,
     PreviewOverrideTypeDef,
     ListRotationOverridesRequestRequestTypeDef,
     RotationOverrideTypeDef,
     ListRotationShiftsRequestRequestTypeDef,
     ListRotationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     PutContactPolicyRequestRequestTypeDef,
     ShiftDetailsTypeDef,
     SendActivationCodeRequestRequestTypeDef,
     StartEngagementRequestRequestTypeDef,
     StopEngagementRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ContactChannelTypeDef,
     CreateContactChannelRequestRequestTypeDef,
     UpdateContactChannelRequestRequestTypeDef,
-    TargetOutputTypeDef,
     TargetTypeDef,
-    CoverageTimeOutputTypeDef,
-    MonthlySettingOutputTypeDef,
-    WeeklySettingOutputTypeDef,
     CoverageTimeTypeDef,
     MonthlySettingTypeDef,
     WeeklySettingTypeDef,
     CreateContactChannelResultTypeDef,
     CreateContactResultTypeDef,
     CreateRotationOverrideResultTypeDef,
     CreateRotationResultTypeDef,
     DescribeEngagementResultTypeDef,
     DescribePageResultTypeDef,
     GetContactChannelResultTypeDef,
     GetContactPolicyResultTypeDef,
     GetRotationOverrideResultTypeDef,
     ListContactsResultTypeDef,
     StartEngagementResultTypeDef,
+    ListTagsForResourceResultTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEngagementsResultTypeDef,
     ListContactChannelsRequestListContactChannelsPaginateTypeDef,
     ListContactsRequestListContactsPaginateTypeDef,
     ListPageReceiptsRequestListPageReceiptsPaginateTypeDef,
     ListPageResolutionsRequestListPageResolutionsPaginateTypeDef,
     ListPagesByContactRequestListPagesByContactPaginateTypeDef,
@@ -464,15 +456,14 @@
     ListEngagementsRequestListEngagementsPaginateTypeDef,
     ListEngagementsRequestRequestTypeDef,
     ListPageReceiptsResultTypeDef,
     ListPageResolutionsResultTypeDef,
     ListPagesByContactResultTypeDef,
     ListPagesByEngagementResultTypeDef,
     ListRotationOverridesResultTypeDef,
-    ListTagsForResourceResultTypeDef,
     RotationShiftTypeDef,
     ListContactChannelsResultTypeDef,
     StageOutputTypeDef,
     StageTypeDef,
     RecurrenceSettingsOutputTypeDef,
     RecurrenceSettingsTypeDef,
     ListPreviewRotationShiftsResultTypeDef,
```

### Comparing `mypy-boto3-ssm-contacts-1.28.12/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt` & `mypy-boto3-ssm-contacts-1.28.15/mypy_boto3_ssm_contacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-contacts-1.28.12/setup.py` & `mypy-boto3-ssm-contacts-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-contacts",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ssm_contacts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSMContacts 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.SSMContacts 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

