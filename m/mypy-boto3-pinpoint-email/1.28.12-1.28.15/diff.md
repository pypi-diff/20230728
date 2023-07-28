# Comparing `tmp/mypy-boto3-pinpoint-email-1.28.12.tar.gz` & `tmp/mypy-boto3-pinpoint-email-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-email-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-email-1.28.15.tar", last modified: Fri Jul 28 20:43:27 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-email-1.28.12.tar` & `mypy-boto3-pinpoint-email-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-email-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18826 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-email-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17312 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-07-27 11:41:34.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32917 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-27 11:41:34.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-27 11:41:34.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-27 11:41:34.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-27 11:41:34.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37666 2023-07-27 11:41:35.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37632 2023-07-27 11:41:35.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18826 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-email-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:27.789646 mypy-boto3-pinpoint-email-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-07-28 20:43:27.773645 mypy-boto3-pinpoint-email-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:27.773645 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-07-28 20:33:25.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32917 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-28 20:33:26.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-28 20:33:26.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-28 20:33:25.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-28 20:33:25.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36033 2023-07-28 20:33:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35999 2023-07-28 20:33:26.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:27.773645 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:27.000000 mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:27.789646 mypy-boto3-pinpoint-email-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:33:23.000000 mypy-boto3-pinpoint-email-1.28.15/setup.py
```

### Comparing `mypy-boto3-pinpoint-email-1.28.12/LICENSE` & `mypy-boto3-pinpoint-email-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.12/PKG-INFO` & `mypy-boto3-pinpoint-email-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-email
-Version: 1.28.12
-Summary: Type annotations for boto3.PinpointEmail 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.PinpointEmail 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-email)](https://pepy.tech/project/mypy-boto3-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointEmail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[boto3.PinpointEmail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,15 +354,14 @@
 `mypy_boto3_pinpoint_email.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_email.type_defs import (
     BlacklistEntryTypeDef,
     ContentTypeDef,
-    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     ResponseMetadataTypeDef,
@@ -371,35 +370,28 @@
     VolumeStatisticsTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
-    DeliveryOptionsOutputTypeDef,
     DestinationTypeDef,
     DomainDeliverabilityCampaignTypeDef,
     InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
     RawMessageTypeDef,
     TemplateTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
-    KinesisFirehoseDestinationOutputTypeDef,
-    PinpointDestinationOutputTypeDef,
-    SnsDestinationOutputTypeDef,
     SendQuotaTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
     ReputationOptionsOutputTypeDef,
-    SendingOptionsOutputTypeDef,
-    TagOutputTypeDef,
-    TrackingOptionsOutputTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
@@ -432,27 +424,27 @@
     CreateEmailIdentityRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SendEmailResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     GetAccountResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
     GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
     ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
     ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
     ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     IspPlacementTypeDef,
```

### Comparing `mypy-boto3-pinpoint-email-1.28.12/README.md` & `mypy-boto3-pinpoint-email-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-email)](https://pepy.tech/project/mypy-boto3-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointEmail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[boto3.PinpointEmail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,15 +322,14 @@
 `mypy_boto3_pinpoint_email.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_email.type_defs import (
     BlacklistEntryTypeDef,
     ContentTypeDef,
-    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     ResponseMetadataTypeDef,
@@ -339,35 +338,28 @@
     VolumeStatisticsTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
-    DeliveryOptionsOutputTypeDef,
     DestinationTypeDef,
     DomainDeliverabilityCampaignTypeDef,
     InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
     RawMessageTypeDef,
     TemplateTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
-    KinesisFirehoseDestinationOutputTypeDef,
-    PinpointDestinationOutputTypeDef,
-    SnsDestinationOutputTypeDef,
     SendQuotaTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
     ReputationOptionsOutputTypeDef,
-    SendingOptionsOutputTypeDef,
-    TagOutputTypeDef,
-    TrackingOptionsOutputTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
@@ -400,27 +392,27 @@
     CreateEmailIdentityRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SendEmailResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     GetAccountResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
     GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
     ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
     ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
     ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     IspPlacementTypeDef,
```

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/__init__.py` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/__init__.pyi` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/__main__.py` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PinpointEmail 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.PinpointEmail 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail\nOther"
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

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/client.py` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/client.pyi` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/literals.py` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/literals.pyi` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/paginator.py` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/paginator.pyi` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/type_defs.py` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,17 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlacklistEntryTypeDef",
     "ContentTypeDef",
-    "CloudWatchDimensionConfigurationOutputTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "DeliveryOptionsTypeDef",
     "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "ResponseMetadataTypeDef",
@@ -52,35 +50,28 @@
     "VolumeStatisticsTypeDef",
     "DedicatedIpTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
-    "DeliveryOptionsOutputTypeDef",
     "DestinationTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
     "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
     "RawMessageTypeDef",
     "TemplateTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
-    "KinesisFirehoseDestinationOutputTypeDef",
-    "PinpointDestinationOutputTypeDef",
-    "SnsDestinationOutputTypeDef",
     "SendQuotaTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
     "ReputationOptionsOutputTypeDef",
-    "SendingOptionsOutputTypeDef",
-    "TagOutputTypeDef",
-    "TrackingOptionsOutputTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     "GetDomainStatisticsReportRequestRequestTypeDef",
@@ -113,27 +104,27 @@
     "CreateEmailIdentityRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "CreateDeliverabilityTestReportResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "ListConfigurationSetsResponseTypeDef",
     "ListDedicatedIpPoolsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "SendEmailResponseTypeDef",
     "CreateEmailIdentityResponseTypeDef",
     "DailyVolumeTypeDef",
     "OverallVolumeTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "GetAccountResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
     "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
     "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
     "IspPlacementTypeDef",
@@ -174,28 +165,17 @@
     "_OptionalContentTypeDef",
     {
         "Charset": str,
     },
     total=False,
 )
 
-
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
-
-CloudWatchDimensionConfigurationOutputTypeDef = TypedDict(
-    "CloudWatchDimensionConfigurationOutputTypeDef",
-    {
-        "DimensionName": str,
-        "DimensionValueSource": DimensionValueSourceType,
-        "DefaultDimensionValue": str,
-    },
-)
-
 CloudWatchDimensionConfigurationTypeDef = TypedDict(
     "CloudWatchDimensionConfigurationTypeDef",
     {
         "DimensionName": str,
         "DimensionValueSource": DimensionValueSourceType,
         "DefaultDimensionValue": str,
     },
@@ -298,19 +278,17 @@
     "_OptionalDedicatedIpTypeDef",
     {
         "PoolName": str,
     },
     total=False,
 )
 
-
 class DedicatedIpTypeDef(_RequiredDedicatedIpTypeDef, _OptionalDedicatedIpTypeDef):
     pass
 
-
 DeleteConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -345,23 +323,14 @@
         "FromEmailAddress": str,
         "CreateDate": datetime,
         "DeliverabilityTestStatus": DeliverabilityTestStatusType,
     },
     total=False,
 )
 
-DeliveryOptionsOutputTypeDef = TypedDict(
-    "DeliveryOptionsOutputTypeDef",
-    {
-        "TlsPolicy": TlsPolicyType,
-        "SendingPoolName": str,
-    },
-    total=False,
-)
-
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "ToAddresses": Sequence[str],
         "CcAddresses": Sequence[str],
         "BccAddresses": Sequence[str],
     },
@@ -442,37 +411,14 @@
 SnsDestinationTypeDef = TypedDict(
     "SnsDestinationTypeDef",
     {
         "TopicArn": str,
     },
 )
 
-KinesisFirehoseDestinationOutputTypeDef = TypedDict(
-    "KinesisFirehoseDestinationOutputTypeDef",
-    {
-        "IamRoleArn": str,
-        "DeliveryStreamArn": str,
-    },
-)
-
-PinpointDestinationOutputTypeDef = TypedDict(
-    "PinpointDestinationOutputTypeDef",
-    {
-        "ApplicationArn": str,
-    },
-    total=False,
-)
-
-SnsDestinationOutputTypeDef = TypedDict(
-    "SnsDestinationOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-
 SendQuotaTypeDef = TypedDict(
     "SendQuotaTypeDef",
     {
         "Max24HourSend": float,
         "MaxSendRate": float,
         "SentLast24Hours": float,
     },
@@ -505,37 +451,14 @@
     {
         "ReputationMetricsEnabled": bool,
         "LastFreshStart": datetime,
     },
     total=False,
 )
 
-SendingOptionsOutputTypeDef = TypedDict(
-    "SendingOptionsOutputTypeDef",
-    {
-        "SendingEnabled": bool,
-    },
-    total=False,
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-TrackingOptionsOutputTypeDef = TypedDict(
-    "TrackingOptionsOutputTypeDef",
-    {
-        "CustomRedirectDomain": str,
-    },
-)
-
 GetDedicatedIpRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpRequestRequestTypeDef",
     {
         "Ip": str,
     },
 )
 
@@ -660,22 +583,20 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-
 class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
     _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
 ):
     pass
 
-
 ListEmailIdentitiesRequestRequestTypeDef = TypedDict(
     "ListEmailIdentitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -723,88 +644,80 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
     },
     total=False,
 )
 
-
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ReputationMetricsEnabled": bool,
     },
     total=False,
 )
 
-
 class PutConfigurationSetReputationOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
 
-
 class PutConfigurationSetSendingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "CustomRedirectDomain": str,
     },
     total=False,
 )
 
-
 class PutConfigurationSetTrackingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 PutDedicatedIpInPoolRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
@@ -827,44 +740,40 @@
     "_OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "SigningEnabled": bool,
     },
     total=False,
 )
 
-
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailForwardingEnabled": bool,
     },
     total=False,
 )
 
-
 class PutEmailIdentityFeedbackAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
@@ -872,22 +781,20 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMxFailure": BehaviorOnMxFailureType,
     },
     total=False,
 )
 
-
 class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -900,15 +807,15 @@
     },
     total=False,
 )
 
 CloudWatchDestinationOutputTypeDef = TypedDict(
     "CloudWatchDestinationOutputTypeDef",
     {
-        "DimensionConfigurations": List[CloudWatchDimensionConfigurationOutputTypeDef],
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
@@ -925,44 +832,40 @@
     "_OptionalCreateDedicatedIpPoolRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDedicatedIpPoolRequestRequestTypeDef(
     _RequiredCreateDedicatedIpPoolRequestRequestTypeDef,
     _OptionalCreateDedicatedIpPoolRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_OptionalCreateEmailIdentityRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateEmailIdentityRequestRequestTypeDef(
     _RequiredCreateEmailIdentityRequestRequestTypeDef,
     _OptionalCreateEmailIdentityRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -981,22 +884,20 @@
         "ReputationOptions": ReputationOptionsTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
-
 CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
     "CreateDeliverabilityTestReportResponseTypeDef",
     {
         "ReportId": str,
         "DeliverabilityTestStatus": DeliverabilityTestStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1024,14 +925,22 @@
     {
         "DedicatedIpPools": List[str],
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
 SendEmailResponseTypeDef = TypedDict(
     "SendEmailResponseTypeDef",
     {
         "MessageId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1137,31 +1046,23 @@
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetConfigurationSetResponseTypeDef = TypedDict(
     "GetConfigurationSetResponseTypeDef",
     {
         "ConfigurationSetName": str,
-        "TrackingOptions": TrackingOptionsOutputTypeDef,
-        "DeliveryOptions": DeliveryOptionsOutputTypeDef,
+        "TrackingOptions": TrackingOptionsTypeDef,
+        "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsOutputTypeDef,
-        "SendingOptions": SendingOptionsOutputTypeDef,
-        "Tags": List[TagOutputTypeDef],
+        "SendingOptions": SendingOptionsTypeDef,
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = TypedDict(
     "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     {
@@ -1216,15 +1117,15 @@
     "GetEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEmailIdentitiesResponseTypeDef = TypedDict(
     "ListEmailIdentitiesResponseTypeDef",
     {
@@ -1249,27 +1150,25 @@
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationTypeDef = TypedDict(
     "_OptionalEventDestinationTypeDef",
     {
         "Enabled": bool,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
-        "SnsDestination": SnsDestinationOutputTypeDef,
-        "PinpointDestination": PinpointDestinationOutputTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+        "PinpointDestination": PinpointDestinationTypeDef,
     },
     total=False,
 )
 
-
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
-
 EventDestinationDefinitionTypeDef = TypedDict(
     "EventDestinationDefinitionTypeDef",
     {
         "Enabled": bool,
         "MatchingEventTypes": Sequence[EventTypeType],
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationTypeDef,
@@ -1310,30 +1209,28 @@
     "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
         "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
     },
     total=False,
 )
 
-
 class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
     _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
     _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
 ):
     pass
 
-
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
@@ -1382,22 +1279,20 @@
     {
         "ReportName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDeliverabilityTestReportRequestRequestTypeDef(
     _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef,
     _OptionalCreateDeliverabilityTestReportRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Destination": DestinationTypeDef,
         "Content": EmailContentTypeDef,
     },
 )
@@ -1409,12 +1304,11 @@
         "FeedbackForwardingEmailAddress": str,
         "EmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/type_defs.pyi` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,18 +31,18 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BlacklistEntryTypeDef",
     "ContentTypeDef",
-    "CloudWatchDimensionConfigurationOutputTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "DeliveryOptionsTypeDef",
     "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "ResponseMetadataTypeDef",
@@ -51,35 +51,28 @@
     "VolumeStatisticsTypeDef",
     "DedicatedIpTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
-    "DeliveryOptionsOutputTypeDef",
     "DestinationTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
     "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
     "RawMessageTypeDef",
     "TemplateTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
-    "KinesisFirehoseDestinationOutputTypeDef",
-    "PinpointDestinationOutputTypeDef",
-    "SnsDestinationOutputTypeDef",
     "SendQuotaTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
     "ReputationOptionsOutputTypeDef",
-    "SendingOptionsOutputTypeDef",
-    "TagOutputTypeDef",
-    "TrackingOptionsOutputTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     "GetDomainStatisticsReportRequestRequestTypeDef",
@@ -112,27 +105,27 @@
     "CreateEmailIdentityRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "CreateDeliverabilityTestReportResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "ListConfigurationSetsResponseTypeDef",
     "ListDedicatedIpPoolsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "SendEmailResponseTypeDef",
     "CreateEmailIdentityResponseTypeDef",
     "DailyVolumeTypeDef",
     "OverallVolumeTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "GetAccountResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "GetConfigurationSetResponseTypeDef",
     "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
     "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
     "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
     "IspPlacementTypeDef",
@@ -173,25 +166,18 @@
     "_OptionalContentTypeDef",
     {
         "Charset": str,
     },
     total=False,
 )
 
+
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
-CloudWatchDimensionConfigurationOutputTypeDef = TypedDict(
-    "CloudWatchDimensionConfigurationOutputTypeDef",
-    {
-        "DimensionName": str,
-        "DimensionValueSource": DimensionValueSourceType,
-        "DefaultDimensionValue": str,
-    },
-)
 
 CloudWatchDimensionConfigurationTypeDef = TypedDict(
     "CloudWatchDimensionConfigurationTypeDef",
     {
         "DimensionName": str,
         "DimensionValueSource": DimensionValueSourceType,
         "DefaultDimensionValue": str,
@@ -295,17 +281,19 @@
     "_OptionalDedicatedIpTypeDef",
     {
         "PoolName": str,
     },
     total=False,
 )
 
+
 class DedicatedIpTypeDef(_RequiredDedicatedIpTypeDef, _OptionalDedicatedIpTypeDef):
     pass
 
+
 DeleteConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -340,23 +328,14 @@
         "FromEmailAddress": str,
         "CreateDate": datetime,
         "DeliverabilityTestStatus": DeliverabilityTestStatusType,
     },
     total=False,
 )
 
-DeliveryOptionsOutputTypeDef = TypedDict(
-    "DeliveryOptionsOutputTypeDef",
-    {
-        "TlsPolicy": TlsPolicyType,
-        "SendingPoolName": str,
-    },
-    total=False,
-)
-
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "ToAddresses": Sequence[str],
         "CcAddresses": Sequence[str],
         "BccAddresses": Sequence[str],
     },
@@ -437,37 +416,14 @@
 SnsDestinationTypeDef = TypedDict(
     "SnsDestinationTypeDef",
     {
         "TopicArn": str,
     },
 )
 
-KinesisFirehoseDestinationOutputTypeDef = TypedDict(
-    "KinesisFirehoseDestinationOutputTypeDef",
-    {
-        "IamRoleArn": str,
-        "DeliveryStreamArn": str,
-    },
-)
-
-PinpointDestinationOutputTypeDef = TypedDict(
-    "PinpointDestinationOutputTypeDef",
-    {
-        "ApplicationArn": str,
-    },
-    total=False,
-)
-
-SnsDestinationOutputTypeDef = TypedDict(
-    "SnsDestinationOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-
 SendQuotaTypeDef = TypedDict(
     "SendQuotaTypeDef",
     {
         "Max24HourSend": float,
         "MaxSendRate": float,
         "SentLast24Hours": float,
     },
@@ -500,37 +456,14 @@
     {
         "ReputationMetricsEnabled": bool,
         "LastFreshStart": datetime,
     },
     total=False,
 )
 
-SendingOptionsOutputTypeDef = TypedDict(
-    "SendingOptionsOutputTypeDef",
-    {
-        "SendingEnabled": bool,
-    },
-    total=False,
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-TrackingOptionsOutputTypeDef = TypedDict(
-    "TrackingOptionsOutputTypeDef",
-    {
-        "CustomRedirectDomain": str,
-    },
-)
-
 GetDedicatedIpRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpRequestRequestTypeDef",
     {
         "Ip": str,
     },
 )
 
@@ -655,20 +588,22 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+
 class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
     _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
 ):
     pass
 
+
 ListEmailIdentitiesRequestRequestTypeDef = TypedDict(
     "ListEmailIdentitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -716,80 +651,88 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
     },
     total=False,
 )
 
+
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ReputationMetricsEnabled": bool,
     },
     total=False,
 )
 
+
 class PutConfigurationSetReputationOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
 
+
 class PutConfigurationSetSendingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "CustomRedirectDomain": str,
     },
     total=False,
 )
 
+
 class PutConfigurationSetTrackingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 PutDedicatedIpInPoolRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
@@ -812,40 +755,44 @@
     "_OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "SigningEnabled": bool,
     },
     total=False,
 )
 
+
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailForwardingEnabled": bool,
     },
     total=False,
 )
 
+
 class PutEmailIdentityFeedbackAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
@@ -853,20 +800,22 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMxFailure": BehaviorOnMxFailureType,
     },
     total=False,
 )
 
+
 class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -879,15 +828,15 @@
     },
     total=False,
 )
 
 CloudWatchDestinationOutputTypeDef = TypedDict(
     "CloudWatchDestinationOutputTypeDef",
     {
-        "DimensionConfigurations": List[CloudWatchDimensionConfigurationOutputTypeDef],
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
@@ -904,40 +853,44 @@
     "_OptionalCreateDedicatedIpPoolRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDedicatedIpPoolRequestRequestTypeDef(
     _RequiredCreateDedicatedIpPoolRequestRequestTypeDef,
     _OptionalCreateDedicatedIpPoolRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_OptionalCreateEmailIdentityRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateEmailIdentityRequestRequestTypeDef(
     _RequiredCreateEmailIdentityRequestRequestTypeDef,
     _OptionalCreateEmailIdentityRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -956,20 +909,22 @@
         "ReputationOptions": ReputationOptionsTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
+
 CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
     "CreateDeliverabilityTestReportResponseTypeDef",
     {
         "ReportId": str,
         "DeliverabilityTestStatus": DeliverabilityTestStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -997,14 +952,22 @@
     {
         "DedicatedIpPools": List[str],
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
 SendEmailResponseTypeDef = TypedDict(
     "SendEmailResponseTypeDef",
     {
         "MessageId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1110,31 +1073,23 @@
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetConfigurationSetResponseTypeDef = TypedDict(
     "GetConfigurationSetResponseTypeDef",
     {
         "ConfigurationSetName": str,
-        "TrackingOptions": TrackingOptionsOutputTypeDef,
-        "DeliveryOptions": DeliveryOptionsOutputTypeDef,
+        "TrackingOptions": TrackingOptionsTypeDef,
+        "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsOutputTypeDef,
-        "SendingOptions": SendingOptionsOutputTypeDef,
-        "Tags": List[TagOutputTypeDef],
+        "SendingOptions": SendingOptionsTypeDef,
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = TypedDict(
     "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     {
@@ -1189,15 +1144,15 @@
     "GetEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEmailIdentitiesResponseTypeDef = TypedDict(
     "ListEmailIdentitiesResponseTypeDef",
     {
@@ -1222,25 +1177,27 @@
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationTypeDef = TypedDict(
     "_OptionalEventDestinationTypeDef",
     {
         "Enabled": bool,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
-        "SnsDestination": SnsDestinationOutputTypeDef,
-        "PinpointDestination": PinpointDestinationOutputTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+        "PinpointDestination": PinpointDestinationTypeDef,
     },
     total=False,
 )
 
+
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
+
 EventDestinationDefinitionTypeDef = TypedDict(
     "EventDestinationDefinitionTypeDef",
     {
         "Enabled": bool,
         "MatchingEventTypes": Sequence[EventTypeType],
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationTypeDef,
@@ -1281,28 +1238,30 @@
     "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
         "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
     },
     total=False,
 )
 
+
 class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
     _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
     _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
 ):
     pass
 
+
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
@@ -1351,20 +1310,22 @@
     {
         "ReportName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDeliverabilityTestReportRequestRequestTypeDef(
     _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef,
     _OptionalCreateDeliverabilityTestReportRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Destination": DestinationTypeDef,
         "Content": EmailContentTypeDef,
     },
 )
@@ -1376,11 +1337,12 @@
         "FeedbackForwardingEmailAddress": str,
         "EmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-email
-Version: 1.28.12
-Summary: Type annotations for boto3.PinpointEmail 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.PinpointEmail 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-email)](https://pepy.tech/project/mypy-boto3-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointEmail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[boto3.PinpointEmail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,15 +354,14 @@
 `mypy_boto3_pinpoint_email.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_email.type_defs import (
     BlacklistEntryTypeDef,
     ContentTypeDef,
-    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     ResponseMetadataTypeDef,
@@ -371,35 +370,28 @@
     VolumeStatisticsTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
-    DeliveryOptionsOutputTypeDef,
     DestinationTypeDef,
     DomainDeliverabilityCampaignTypeDef,
     InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
     RawMessageTypeDef,
     TemplateTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
-    KinesisFirehoseDestinationOutputTypeDef,
-    PinpointDestinationOutputTypeDef,
-    SnsDestinationOutputTypeDef,
     SendQuotaTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
     ReputationOptionsOutputTypeDef,
-    SendingOptionsOutputTypeDef,
-    TagOutputTypeDef,
-    TrackingOptionsOutputTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
@@ -432,27 +424,27 @@
     CreateEmailIdentityRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     CreateDeliverabilityTestReportResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     SendEmailResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     GetAccountResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
     GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
     ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
     ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
     ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     IspPlacementTypeDef,
```

### Comparing `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-email-1.28.15/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.12/setup.py` & `mypy-boto3-pinpoint-email-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint-email",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_pinpoint_email"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PinpointEmail 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.PinpointEmail 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

