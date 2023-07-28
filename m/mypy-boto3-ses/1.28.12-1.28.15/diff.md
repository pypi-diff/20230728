# Comparing `tmp/mypy-boto3-ses-1.28.12.tar.gz` & `tmp/mypy-boto3-ses-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ses-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
+gzip compressed data, was "mypy-boto3-ses-1.28.15.tar", last modified: Fri Jul 28 20:43:44 2023, max compression
```

## Comparing `mypy-boto3-ses-1.28.12.tar` & `mypy-boto3-ses-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.833293 mypy-boto3-ses-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21099 2023-07-27 11:49:38.833293 mypy-boto3-ses-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19628 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.829293 mypy-boto3-ses-1.28.12/mypy_boto3_ses/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49195 2023-07-27 11:46:50.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49111 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-07-27 11:46:52.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-07-27 11:46:52.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-27 11:46:50.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-27 11:46:50.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54975 2023-07-27 11:46:53.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54894 2023-07-27 11:46:52.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-27 11:46:50.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-27 11:46:50.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.833293 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21099 2023-07-27 11:49:38.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 11:49:38.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:38.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.833293 mypy-boto3-ses-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.829879 mypy-boto3-ses-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-07-28 20:43:44.829879 mypy-boto3-ses-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.829879 mypy-boto3-ses-1.28.15/mypy_boto3_ses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49195 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49111 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    49427 2023-07-28 20:39:23.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49360 2023-07-28 20:39:22.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-28 20:39:21.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:44.829879 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-07-28 20:43:44.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:43:44.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:44.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:44.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:44.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:44.000000 mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:44.829879 mypy-boto3-ses-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:39:20.000000 mypy-boto3-ses-1.28.15/setup.py
```

### Comparing `mypy-boto3-ses-1.28.12/LICENSE` & `mypy-boto3-ses-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.12/PKG-INFO` & `mypy-boto3-ses-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ses
-Version: 1.28.12
-Summary: Type annotations for boto3.SES 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SES 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ses)](https://pepy.tech/project/mypy-boto3-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SES 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[boto3.SES 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,26 +375,22 @@
 ### Typed dictionaries
 
 `mypy_boto3_ses.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ses.type_defs import (
-    AddHeaderActionOutputTypeDef,
     AddHeaderActionTypeDef,
     ContentTypeDef,
-    BounceActionOutputTypeDef,
     BounceActionTypeDef,
     BulkEmailDestinationStatusTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloneReceiptRuleSetRequestRequestTypeDef,
-    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
-    ConfigurationSetOutputTypeDef,
     ConfigurationSetTypeDef,
     TrackingOptionsTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
     CreateReceiptRuleSetRequestRequestTypeDef,
     TemplateTypeDef,
     CustomVerificationEmailTemplateTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
@@ -404,25 +400,21 @@
     DeleteIdentityPolicyRequestRequestTypeDef,
     DeleteIdentityRequestRequestTypeDef,
     DeleteReceiptFilterRequestRequestTypeDef,
     DeleteReceiptRuleRequestRequestTypeDef,
     DeleteReceiptRuleSetRequestRequestTypeDef,
     DeleteTemplateRequestRequestTypeDef,
     DeleteVerifiedEmailAddressRequestRequestTypeDef,
-    DeliveryOptionsOutputTypeDef,
     DeliveryOptionsTypeDef,
     ReceiptRuleSetMetadataTypeDef,
     ResponseMetadataTypeDef,
     DescribeConfigurationSetRequestRequestTypeDef,
     ReputationOptionsTypeDef,
-    TrackingOptionsOutputTypeDef,
     DescribeReceiptRuleRequestRequestTypeDef,
     DescribeReceiptRuleSetRequestRequestTypeDef,
-    KinesisFirehoseDestinationOutputTypeDef,
-    SNSDestinationOutputTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SNSDestinationTypeDef,
     ExtensionFieldTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
     GetIdentityDkimAttributesRequestRequestTypeDef,
     IdentityDkimAttributesTypeDef,
     GetIdentityMailFromDomainAttributesRequestRequestTypeDef,
@@ -431,36 +423,29 @@
     IdentityNotificationAttributesTypeDef,
     GetIdentityPoliciesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetIdentityVerificationAttributesRequestRequestTypeDef,
     IdentityVerificationAttributesTypeDef,
     SendDataPointTypeDef,
     GetTemplateRequestRequestTypeDef,
-    TemplateOutputTypeDef,
-    LambdaActionOutputTypeDef,
     LambdaActionTypeDef,
     PaginatorConfigTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListIdentitiesRequestRequestTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
     RawMessageTypeDef,
-    S3ActionOutputTypeDef,
-    SNSActionOutputTypeDef,
-    StopActionOutputTypeDef,
-    WorkmailActionOutputTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
-    ReceiptIpFilterOutputTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
     SetActiveReceiptRuleSetRequestRequestTypeDef,
     SetIdentityDkimEnabledRequestRequestTypeDef,
     SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef,
     SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef,
@@ -488,14 +473,15 @@
     UpdateTemplateRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityPoliciesResponseTypeDef,
     GetSendQuotaResponseTypeDef,
+    GetTemplateResponseTypeDef,
     ListConfigurationSetsResponseTypeDef,
     ListCustomVerificationEmailTemplatesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoliciesResponseTypeDef,
     ListReceiptRuleSetsResponseTypeDef,
     ListVerifiedEmailAddressesResponseTypeDef,
     SendBounceResponseTypeDef,
@@ -511,49 +497,46 @@
     RecipientDsnFieldsTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
-    GetTemplateResponseTypeDef,
     ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
     SendRawEmailRequestRequestTypeDef,
-    ReceiptActionOutputTypeDef,
     ReceiptActionTypeDef,
-    ReceiptFilterOutputTypeDef,
     ReceiptFilterTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
     EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     BouncedRecipientInfoTypeDef,
     ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
-    ListReceiptFiltersResponseTypeDef,
     CreateReceiptFilterRequestRequestTypeDef,
+    ListReceiptFiltersResponseTypeDef,
     SendEmailRequestRequestTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     SendBounceRequestRequestTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     CreateReceiptRuleRequestRequestTypeDef,
     UpdateReceiptRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddHeaderActionOutputTypeDef:
+def get_structure() -> AddHeaderActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ses-1.28.12/README.md` & `mypy-boto3-ses-1.28.15/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ses)](https://pepy.tech/project/mypy-boto3-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SES 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[boto3.SES 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,26 +343,22 @@
 ### Typed dictionaries
 
 `mypy_boto3_ses.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ses.type_defs import (
-    AddHeaderActionOutputTypeDef,
     AddHeaderActionTypeDef,
     ContentTypeDef,
-    BounceActionOutputTypeDef,
     BounceActionTypeDef,
     BulkEmailDestinationStatusTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloneReceiptRuleSetRequestRequestTypeDef,
-    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
-    ConfigurationSetOutputTypeDef,
     ConfigurationSetTypeDef,
     TrackingOptionsTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
     CreateReceiptRuleSetRequestRequestTypeDef,
     TemplateTypeDef,
     CustomVerificationEmailTemplateTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
@@ -372,25 +368,21 @@
     DeleteIdentityPolicyRequestRequestTypeDef,
     DeleteIdentityRequestRequestTypeDef,
     DeleteReceiptFilterRequestRequestTypeDef,
     DeleteReceiptRuleRequestRequestTypeDef,
     DeleteReceiptRuleSetRequestRequestTypeDef,
     DeleteTemplateRequestRequestTypeDef,
     DeleteVerifiedEmailAddressRequestRequestTypeDef,
-    DeliveryOptionsOutputTypeDef,
     DeliveryOptionsTypeDef,
     ReceiptRuleSetMetadataTypeDef,
     ResponseMetadataTypeDef,
     DescribeConfigurationSetRequestRequestTypeDef,
     ReputationOptionsTypeDef,
-    TrackingOptionsOutputTypeDef,
     DescribeReceiptRuleRequestRequestTypeDef,
     DescribeReceiptRuleSetRequestRequestTypeDef,
-    KinesisFirehoseDestinationOutputTypeDef,
-    SNSDestinationOutputTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SNSDestinationTypeDef,
     ExtensionFieldTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
     GetIdentityDkimAttributesRequestRequestTypeDef,
     IdentityDkimAttributesTypeDef,
     GetIdentityMailFromDomainAttributesRequestRequestTypeDef,
@@ -399,36 +391,29 @@
     IdentityNotificationAttributesTypeDef,
     GetIdentityPoliciesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetIdentityVerificationAttributesRequestRequestTypeDef,
     IdentityVerificationAttributesTypeDef,
     SendDataPointTypeDef,
     GetTemplateRequestRequestTypeDef,
-    TemplateOutputTypeDef,
-    LambdaActionOutputTypeDef,
     LambdaActionTypeDef,
     PaginatorConfigTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListIdentitiesRequestRequestTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
     RawMessageTypeDef,
-    S3ActionOutputTypeDef,
-    SNSActionOutputTypeDef,
-    StopActionOutputTypeDef,
-    WorkmailActionOutputTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
-    ReceiptIpFilterOutputTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
     SetActiveReceiptRuleSetRequestRequestTypeDef,
     SetIdentityDkimEnabledRequestRequestTypeDef,
     SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef,
     SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef,
@@ -456,14 +441,15 @@
     UpdateTemplateRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityPoliciesResponseTypeDef,
     GetSendQuotaResponseTypeDef,
+    GetTemplateResponseTypeDef,
     ListConfigurationSetsResponseTypeDef,
     ListCustomVerificationEmailTemplatesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoliciesResponseTypeDef,
     ListReceiptRuleSetsResponseTypeDef,
     ListVerifiedEmailAddressesResponseTypeDef,
     SendBounceResponseTypeDef,
@@ -479,49 +465,46 @@
     RecipientDsnFieldsTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
-    GetTemplateResponseTypeDef,
     ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
     SendRawEmailRequestRequestTypeDef,
-    ReceiptActionOutputTypeDef,
     ReceiptActionTypeDef,
-    ReceiptFilterOutputTypeDef,
     ReceiptFilterTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
     EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     BouncedRecipientInfoTypeDef,
     ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
-    ListReceiptFiltersResponseTypeDef,
     CreateReceiptFilterRequestRequestTypeDef,
+    ListReceiptFiltersResponseTypeDef,
     SendEmailRequestRequestTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     SendBounceRequestRequestTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     CreateReceiptRuleRequestRequestTypeDef,
     UpdateReceiptRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddHeaderActionOutputTypeDef:
+def get_structure() -> AddHeaderActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/__init__.py` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/__init__.pyi` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/__main__.py` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SES 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.SES 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES\nOther"
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

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/client.py` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/client.pyi` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/literals.py` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/literals.pyi` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/paginator.py` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/paginator.pyi` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/type_defs.py` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ses service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ses.type_defs import AddHeaderActionOutputTypeDef
+    from mypy_boto3_ses.type_defs import AddHeaderActionTypeDef
 
-    data: AddHeaderActionOutputTypeDef = {...}
+    data: AddHeaderActionTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -42,26 +42,22 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AddHeaderActionOutputTypeDef",
     "AddHeaderActionTypeDef",
     "ContentTypeDef",
-    "BounceActionOutputTypeDef",
     "BounceActionTypeDef",
     "BulkEmailDestinationStatusTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloneReceiptRuleSetRequestRequestTypeDef",
-    "CloudWatchDimensionConfigurationOutputTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
-    "ConfigurationSetOutputTypeDef",
     "ConfigurationSetTypeDef",
     "TrackingOptionsTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "CreateReceiptRuleSetRequestRequestTypeDef",
     "TemplateTypeDef",
     "CustomVerificationEmailTemplateTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
@@ -71,25 +67,21 @@
     "DeleteIdentityPolicyRequestRequestTypeDef",
     "DeleteIdentityRequestRequestTypeDef",
     "DeleteReceiptFilterRequestRequestTypeDef",
     "DeleteReceiptRuleRequestRequestTypeDef",
     "DeleteReceiptRuleSetRequestRequestTypeDef",
     "DeleteTemplateRequestRequestTypeDef",
     "DeleteVerifiedEmailAddressRequestRequestTypeDef",
-    "DeliveryOptionsOutputTypeDef",
     "DeliveryOptionsTypeDef",
     "ReceiptRuleSetMetadataTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeConfigurationSetRequestRequestTypeDef",
     "ReputationOptionsTypeDef",
-    "TrackingOptionsOutputTypeDef",
     "DescribeReceiptRuleRequestRequestTypeDef",
     "DescribeReceiptRuleSetRequestRequestTypeDef",
-    "KinesisFirehoseDestinationOutputTypeDef",
-    "SNSDestinationOutputTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SNSDestinationTypeDef",
     "ExtensionFieldTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     "IdentityDkimAttributesTypeDef",
     "GetIdentityMailFromDomainAttributesRequestRequestTypeDef",
@@ -98,36 +90,29 @@
     "IdentityNotificationAttributesTypeDef",
     "GetIdentityPoliciesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetIdentityVerificationAttributesRequestRequestTypeDef",
     "IdentityVerificationAttributesTypeDef",
     "SendDataPointTypeDef",
     "GetTemplateRequestRequestTypeDef",
-    "TemplateOutputTypeDef",
-    "LambdaActionOutputTypeDef",
     "LambdaActionTypeDef",
     "PaginatorConfigTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListIdentitiesRequestRequestTypeDef",
     "ListIdentityPoliciesRequestRequestTypeDef",
     "ListReceiptRuleSetsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateMetadataTypeDef",
     "PutIdentityPolicyRequestRequestTypeDef",
     "RawMessageTypeDef",
-    "S3ActionOutputTypeDef",
-    "SNSActionOutputTypeDef",
-    "StopActionOutputTypeDef",
-    "WorkmailActionOutputTypeDef",
     "S3ActionTypeDef",
     "SNSActionTypeDef",
     "StopActionTypeDef",
     "WorkmailActionTypeDef",
-    "ReceiptIpFilterOutputTypeDef",
     "ReceiptIpFilterTypeDef",
     "ReorderReceiptRuleSetRequestRequestTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     "SetIdentityDkimEnabledRequestRequestTypeDef",
     "SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef",
     "SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef",
@@ -155,14 +140,15 @@
     "UpdateTemplateRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAccountSendingEnabledResponseTypeDef",
     "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetIdentityPoliciesResponseTypeDef",
     "GetSendQuotaResponseTypeDef",
+    "GetTemplateResponseTypeDef",
     "ListConfigurationSetsResponseTypeDef",
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     "ListIdentitiesResponseTypeDef",
     "ListIdentityPoliciesResponseTypeDef",
     "ListReceiptRuleSetsResponseTypeDef",
     "ListVerifiedEmailAddressesResponseTypeDef",
     "SendBounceResponseTypeDef",
@@ -178,55 +164,44 @@
     "RecipientDsnFieldsTypeDef",
     "GetIdentityDkimAttributesResponseTypeDef",
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     "GetIdentityNotificationAttributesResponseTypeDef",
     "GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     "GetIdentityVerificationAttributesResponseTypeDef",
     "GetSendStatisticsResponseTypeDef",
-    "GetTemplateResponseTypeDef",
     "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
     "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
     "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
     "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesResponseTypeDef",
     "SendRawEmailRequestRequestTypeDef",
-    "ReceiptActionOutputTypeDef",
     "ReceiptActionTypeDef",
-    "ReceiptFilterOutputTypeDef",
     "ReceiptFilterTypeDef",
     "MessageTypeDef",
     "SendBulkTemplatedEmailRequestRequestTypeDef",
     "EventDestinationOutputTypeDef",
     "EventDestinationTypeDef",
     "BouncedRecipientInfoTypeDef",
     "ReceiptRuleOutputTypeDef",
     "ReceiptRuleTypeDef",
-    "ListReceiptFiltersResponseTypeDef",
     "CreateReceiptFilterRequestRequestTypeDef",
+    "ListReceiptFiltersResponseTypeDef",
     "SendEmailRequestRequestTypeDef",
     "DescribeConfigurationSetResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "SendBounceRequestRequestTypeDef",
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     "DescribeReceiptRuleResponseTypeDef",
     "DescribeReceiptRuleSetResponseTypeDef",
     "CreateReceiptRuleRequestRequestTypeDef",
     "UpdateReceiptRuleRequestRequestTypeDef",
 )
 
-AddHeaderActionOutputTypeDef = TypedDict(
-    "AddHeaderActionOutputTypeDef",
-    {
-        "HeaderName": str,
-        "HeaderValue": str,
-    },
-)
-
 AddHeaderActionTypeDef = TypedDict(
     "AddHeaderActionTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
@@ -246,38 +221,14 @@
 )
 
 
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
 
-_RequiredBounceActionOutputTypeDef = TypedDict(
-    "_RequiredBounceActionOutputTypeDef",
-    {
-        "SmtpReplyCode": str,
-        "Message": str,
-        "Sender": str,
-    },
-)
-_OptionalBounceActionOutputTypeDef = TypedDict(
-    "_OptionalBounceActionOutputTypeDef",
-    {
-        "TopicArn": str,
-        "StatusCode": str,
-    },
-    total=False,
-)
-
-
-class BounceActionOutputTypeDef(
-    _RequiredBounceActionOutputTypeDef, _OptionalBounceActionOutputTypeDef
-):
-    pass
-
-
 _RequiredBounceActionTypeDef = TypedDict(
     "_RequiredBounceActionTypeDef",
     {
         "SmtpReplyCode": str,
         "Message": str,
         "Sender": str,
     },
@@ -328,39 +279,23 @@
     "CloneReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "OriginalRuleSetName": str,
     },
 )
 
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
 )
 
-ConfigurationSetOutputTypeDef = TypedDict(
-    "ConfigurationSetOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 ConfigurationSetTypeDef = TypedDict(
     "ConfigurationSetTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -500,22 +435,14 @@
 DeleteVerifiedEmailAddressRequestRequestTypeDef = TypedDict(
     "DeleteVerifiedEmailAddressRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
-DeliveryOptionsOutputTypeDef = TypedDict(
-    "DeliveryOptionsOutputTypeDef",
-    {
-        "TlsPolicy": TlsPolicyType,
-    },
-    total=False,
-)
-
 DeliveryOptionsTypeDef = TypedDict(
     "DeliveryOptionsTypeDef",
     {
         "TlsPolicy": TlsPolicyType,
     },
     total=False,
 )
@@ -568,22 +495,14 @@
         "SendingEnabled": bool,
         "ReputationMetricsEnabled": bool,
         "LastFreshStart": datetime,
     },
     total=False,
 )
 
-TrackingOptionsOutputTypeDef = TypedDict(
-    "TrackingOptionsOutputTypeDef",
-    {
-        "CustomRedirectDomain": str,
-    },
-    total=False,
-)
-
 DescribeReceiptRuleRequestRequestTypeDef = TypedDict(
     "DescribeReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleName": str,
     },
 )
@@ -591,29 +510,14 @@
 DescribeReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "DescribeReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
 )
 
-KinesisFirehoseDestinationOutputTypeDef = TypedDict(
-    "KinesisFirehoseDestinationOutputTypeDef",
-    {
-        "IAMRoleARN": str,
-        "DeliveryStreamARN": str,
-    },
-)
-
-SNSDestinationOutputTypeDef = TypedDict(
-    "SNSDestinationOutputTypeDef",
-    {
-        "TopicARN": str,
-    },
-)
-
 KinesisFirehoseDestinationTypeDef = TypedDict(
     "KinesisFirehoseDestinationTypeDef",
     {
         "IAMRoleARN": str,
         "DeliveryStreamARN": str,
     },
 )
@@ -778,57 +682,14 @@
 GetTemplateRequestRequestTypeDef = TypedDict(
     "GetTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 
-_RequiredTemplateOutputTypeDef = TypedDict(
-    "_RequiredTemplateOutputTypeDef",
-    {
-        "TemplateName": str,
-    },
-)
-_OptionalTemplateOutputTypeDef = TypedDict(
-    "_OptionalTemplateOutputTypeDef",
-    {
-        "SubjectPart": str,
-        "TextPart": str,
-        "HtmlPart": str,
-    },
-    total=False,
-)
-
-
-class TemplateOutputTypeDef(_RequiredTemplateOutputTypeDef, _OptionalTemplateOutputTypeDef):
-    pass
-
-
-_RequiredLambdaActionOutputTypeDef = TypedDict(
-    "_RequiredLambdaActionOutputTypeDef",
-    {
-        "FunctionArn": str,
-    },
-)
-_OptionalLambdaActionOutputTypeDef = TypedDict(
-    "_OptionalLambdaActionOutputTypeDef",
-    {
-        "TopicArn": str,
-        "InvocationType": InvocationTypeType,
-    },
-    total=False,
-)
-
-
-class LambdaActionOutputTypeDef(
-    _RequiredLambdaActionOutputTypeDef, _OptionalLambdaActionOutputTypeDef
-):
-    pass
-
-
 _RequiredLambdaActionTypeDef = TypedDict(
     "_RequiredLambdaActionTypeDef",
     {
         "FunctionArn": str,
     },
 )
 _OptionalLambdaActionTypeDef = TypedDict(
@@ -928,94 +789,14 @@
 RawMessageTypeDef = TypedDict(
     "RawMessageTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-_RequiredS3ActionOutputTypeDef = TypedDict(
-    "_RequiredS3ActionOutputTypeDef",
-    {
-        "BucketName": str,
-    },
-)
-_OptionalS3ActionOutputTypeDef = TypedDict(
-    "_OptionalS3ActionOutputTypeDef",
-    {
-        "TopicArn": str,
-        "ObjectKeyPrefix": str,
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
-
-class S3ActionOutputTypeDef(_RequiredS3ActionOutputTypeDef, _OptionalS3ActionOutputTypeDef):
-    pass
-
-
-_RequiredSNSActionOutputTypeDef = TypedDict(
-    "_RequiredSNSActionOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-_OptionalSNSActionOutputTypeDef = TypedDict(
-    "_OptionalSNSActionOutputTypeDef",
-    {
-        "Encoding": SNSActionEncodingType,
-    },
-    total=False,
-)
-
-
-class SNSActionOutputTypeDef(_RequiredSNSActionOutputTypeDef, _OptionalSNSActionOutputTypeDef):
-    pass
-
-
-_RequiredStopActionOutputTypeDef = TypedDict(
-    "_RequiredStopActionOutputTypeDef",
-    {
-        "Scope": Literal["RuleSet"],
-    },
-)
-_OptionalStopActionOutputTypeDef = TypedDict(
-    "_OptionalStopActionOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-    total=False,
-)
-
-
-class StopActionOutputTypeDef(_RequiredStopActionOutputTypeDef, _OptionalStopActionOutputTypeDef):
-    pass
-
-
-_RequiredWorkmailActionOutputTypeDef = TypedDict(
-    "_RequiredWorkmailActionOutputTypeDef",
-    {
-        "OrganizationArn": str,
-    },
-)
-_OptionalWorkmailActionOutputTypeDef = TypedDict(
-    "_OptionalWorkmailActionOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-    total=False,
-)
-
-
-class WorkmailActionOutputTypeDef(
-    _RequiredWorkmailActionOutputTypeDef, _OptionalWorkmailActionOutputTypeDef
-):
-    pass
-
-
 _RequiredS3ActionTypeDef = TypedDict(
     "_RequiredS3ActionTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ActionTypeDef = TypedDict(
@@ -1086,22 +867,14 @@
 )
 
 
 class WorkmailActionTypeDef(_RequiredWorkmailActionTypeDef, _OptionalWorkmailActionTypeDef):
     pass
 
 
-ReceiptIpFilterOutputTypeDef = TypedDict(
-    "ReceiptIpFilterOutputTypeDef",
-    {
-        "Policy": ReceiptFilterPolicyType,
-        "Cidr": str,
-    },
-)
-
 ReceiptIpFilterTypeDef = TypedDict(
     "ReceiptIpFilterTypeDef",
     {
         "Policy": ReceiptFilterPolicyType,
         "Cidr": str,
     },
 )
@@ -1386,15 +1159,15 @@
 ):
     pass
 
 
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
@@ -1502,18 +1275,26 @@
         "Max24HourSend": float,
         "MaxSendRate": float,
         "SentLast24Hours": float,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "Template": TemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListConfigurationSetsResponseTypeDef = TypedDict(
     "ListConfigurationSetsResponseTypeDef",
     {
-        "ConfigurationSets": List[ConfigurationSetOutputTypeDef],
+        "ConfigurationSets": List[ConfigurationSetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
@@ -1734,22 +1515,14 @@
     "GetSendStatisticsResponseTypeDef",
     {
         "SendDataPoints": List[SendDataPointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "Template": TemplateOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
     "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1819,50 +1592,28 @@
 
 class SendRawEmailRequestRequestTypeDef(
     _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
 ):
     pass
 
 
-ReceiptActionOutputTypeDef = TypedDict(
-    "ReceiptActionOutputTypeDef",
-    {
-        "S3Action": S3ActionOutputTypeDef,
-        "BounceAction": BounceActionOutputTypeDef,
-        "WorkmailAction": WorkmailActionOutputTypeDef,
-        "LambdaAction": LambdaActionOutputTypeDef,
-        "StopAction": StopActionOutputTypeDef,
-        "AddHeaderAction": AddHeaderActionOutputTypeDef,
-        "SNSAction": SNSActionOutputTypeDef,
-    },
-    total=False,
-)
-
 ReceiptActionTypeDef = TypedDict(
     "ReceiptActionTypeDef",
     {
         "S3Action": S3ActionTypeDef,
         "BounceAction": BounceActionTypeDef,
         "WorkmailAction": WorkmailActionTypeDef,
         "LambdaAction": LambdaActionTypeDef,
         "StopAction": StopActionTypeDef,
         "AddHeaderAction": AddHeaderActionTypeDef,
         "SNSAction": SNSActionTypeDef,
     },
     total=False,
 )
 
-ReceiptFilterOutputTypeDef = TypedDict(
-    "ReceiptFilterOutputTypeDef",
-    {
-        "Name": str,
-        "IpFilter": ReceiptIpFilterOutputTypeDef,
-    },
-)
-
 ReceiptFilterTypeDef = TypedDict(
     "ReceiptFilterTypeDef",
     {
         "Name": str,
         "IpFilter": ReceiptIpFilterTypeDef,
     },
 )
@@ -1913,17 +1664,17 @@
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationOutputTypeDef = TypedDict(
     "_OptionalEventDestinationOutputTypeDef",
     {
         "Enabled": bool,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
-        "SNSDestination": SNSDestinationOutputTypeDef,
+        "SNSDestination": SNSDestinationTypeDef,
     },
     total=False,
 )
 
 
 class EventDestinationOutputTypeDef(
     _RequiredEventDestinationOutputTypeDef, _OptionalEventDestinationOutputTypeDef
@@ -1985,15 +1736,15 @@
 )
 _OptionalReceiptRuleOutputTypeDef = TypedDict(
     "_OptionalReceiptRuleOutputTypeDef",
     {
         "Enabled": bool,
         "TlsPolicy": TlsPolicyType,
         "Recipients": List[str],
-        "Actions": List[ReceiptActionOutputTypeDef],
+        "Actions": List[ReceiptActionTypeDef],
         "ScanEnabled": bool,
     },
     total=False,
 )
 
 
 class ReceiptRuleOutputTypeDef(
@@ -2021,26 +1772,26 @@
 )
 
 
 class ReceiptRuleTypeDef(_RequiredReceiptRuleTypeDef, _OptionalReceiptRuleTypeDef):
     pass
 
 
-ListReceiptFiltersResponseTypeDef = TypedDict(
-    "ListReceiptFiltersResponseTypeDef",
+CreateReceiptFilterRequestRequestTypeDef = TypedDict(
+    "CreateReceiptFilterRequestRequestTypeDef",
     {
-        "Filters": List[ReceiptFilterOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Filter": ReceiptFilterTypeDef,
     },
 )
 
-CreateReceiptFilterRequestRequestTypeDef = TypedDict(
-    "CreateReceiptFilterRequestRequestTypeDef",
+ListReceiptFiltersResponseTypeDef = TypedDict(
+    "ListReceiptFiltersResponseTypeDef",
     {
-        "Filter": ReceiptFilterTypeDef,
+        "Filters": List[ReceiptFilterTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Source": str,
@@ -2067,18 +1818,18 @@
 ):
     pass
 
 
 DescribeConfigurationSetResponseTypeDef = TypedDict(
     "DescribeConfigurationSetResponseTypeDef",
     {
-        "ConfigurationSet": ConfigurationSetOutputTypeDef,
+        "ConfigurationSet": ConfigurationSetTypeDef,
         "EventDestinations": List[EventDestinationOutputTypeDef],
-        "TrackingOptions": TrackingOptionsOutputTypeDef,
-        "DeliveryOptions": DeliveryOptionsOutputTypeDef,
+        "TrackingOptions": TrackingOptionsTypeDef,
+        "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
```

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/type_defs.pyi` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ses service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ses.type_defs import AddHeaderActionOutputTypeDef
+    from mypy_boto3_ses.type_defs import AddHeaderActionTypeDef
 
-    data: AddHeaderActionOutputTypeDef = {...}
+    data: AddHeaderActionTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -41,26 +41,22 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AddHeaderActionOutputTypeDef",
     "AddHeaderActionTypeDef",
     "ContentTypeDef",
-    "BounceActionOutputTypeDef",
     "BounceActionTypeDef",
     "BulkEmailDestinationStatusTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloneReceiptRuleSetRequestRequestTypeDef",
-    "CloudWatchDimensionConfigurationOutputTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
-    "ConfigurationSetOutputTypeDef",
     "ConfigurationSetTypeDef",
     "TrackingOptionsTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "CreateReceiptRuleSetRequestRequestTypeDef",
     "TemplateTypeDef",
     "CustomVerificationEmailTemplateTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
@@ -70,25 +66,21 @@
     "DeleteIdentityPolicyRequestRequestTypeDef",
     "DeleteIdentityRequestRequestTypeDef",
     "DeleteReceiptFilterRequestRequestTypeDef",
     "DeleteReceiptRuleRequestRequestTypeDef",
     "DeleteReceiptRuleSetRequestRequestTypeDef",
     "DeleteTemplateRequestRequestTypeDef",
     "DeleteVerifiedEmailAddressRequestRequestTypeDef",
-    "DeliveryOptionsOutputTypeDef",
     "DeliveryOptionsTypeDef",
     "ReceiptRuleSetMetadataTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeConfigurationSetRequestRequestTypeDef",
     "ReputationOptionsTypeDef",
-    "TrackingOptionsOutputTypeDef",
     "DescribeReceiptRuleRequestRequestTypeDef",
     "DescribeReceiptRuleSetRequestRequestTypeDef",
-    "KinesisFirehoseDestinationOutputTypeDef",
-    "SNSDestinationOutputTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SNSDestinationTypeDef",
     "ExtensionFieldTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     "IdentityDkimAttributesTypeDef",
     "GetIdentityMailFromDomainAttributesRequestRequestTypeDef",
@@ -97,36 +89,29 @@
     "IdentityNotificationAttributesTypeDef",
     "GetIdentityPoliciesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetIdentityVerificationAttributesRequestRequestTypeDef",
     "IdentityVerificationAttributesTypeDef",
     "SendDataPointTypeDef",
     "GetTemplateRequestRequestTypeDef",
-    "TemplateOutputTypeDef",
-    "LambdaActionOutputTypeDef",
     "LambdaActionTypeDef",
     "PaginatorConfigTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListIdentitiesRequestRequestTypeDef",
     "ListIdentityPoliciesRequestRequestTypeDef",
     "ListReceiptRuleSetsRequestRequestTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateMetadataTypeDef",
     "PutIdentityPolicyRequestRequestTypeDef",
     "RawMessageTypeDef",
-    "S3ActionOutputTypeDef",
-    "SNSActionOutputTypeDef",
-    "StopActionOutputTypeDef",
-    "WorkmailActionOutputTypeDef",
     "S3ActionTypeDef",
     "SNSActionTypeDef",
     "StopActionTypeDef",
     "WorkmailActionTypeDef",
-    "ReceiptIpFilterOutputTypeDef",
     "ReceiptIpFilterTypeDef",
     "ReorderReceiptRuleSetRequestRequestTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     "SetIdentityDkimEnabledRequestRequestTypeDef",
     "SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef",
     "SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef",
@@ -154,14 +139,15 @@
     "UpdateTemplateRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAccountSendingEnabledResponseTypeDef",
     "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetIdentityPoliciesResponseTypeDef",
     "GetSendQuotaResponseTypeDef",
+    "GetTemplateResponseTypeDef",
     "ListConfigurationSetsResponseTypeDef",
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     "ListIdentitiesResponseTypeDef",
     "ListIdentityPoliciesResponseTypeDef",
     "ListReceiptRuleSetsResponseTypeDef",
     "ListVerifiedEmailAddressesResponseTypeDef",
     "SendBounceResponseTypeDef",
@@ -177,55 +163,44 @@
     "RecipientDsnFieldsTypeDef",
     "GetIdentityDkimAttributesResponseTypeDef",
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     "GetIdentityNotificationAttributesResponseTypeDef",
     "GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     "GetIdentityVerificationAttributesResponseTypeDef",
     "GetSendStatisticsResponseTypeDef",
-    "GetTemplateResponseTypeDef",
     "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
     "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
     "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
     "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesResponseTypeDef",
     "SendRawEmailRequestRequestTypeDef",
-    "ReceiptActionOutputTypeDef",
     "ReceiptActionTypeDef",
-    "ReceiptFilterOutputTypeDef",
     "ReceiptFilterTypeDef",
     "MessageTypeDef",
     "SendBulkTemplatedEmailRequestRequestTypeDef",
     "EventDestinationOutputTypeDef",
     "EventDestinationTypeDef",
     "BouncedRecipientInfoTypeDef",
     "ReceiptRuleOutputTypeDef",
     "ReceiptRuleTypeDef",
-    "ListReceiptFiltersResponseTypeDef",
     "CreateReceiptFilterRequestRequestTypeDef",
+    "ListReceiptFiltersResponseTypeDef",
     "SendEmailRequestRequestTypeDef",
     "DescribeConfigurationSetResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "SendBounceRequestRequestTypeDef",
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     "DescribeReceiptRuleResponseTypeDef",
     "DescribeReceiptRuleSetResponseTypeDef",
     "CreateReceiptRuleRequestRequestTypeDef",
     "UpdateReceiptRuleRequestRequestTypeDef",
 )
 
-AddHeaderActionOutputTypeDef = TypedDict(
-    "AddHeaderActionOutputTypeDef",
-    {
-        "HeaderName": str,
-        "HeaderValue": str,
-    },
-)
-
 AddHeaderActionTypeDef = TypedDict(
     "AddHeaderActionTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
@@ -243,36 +218,14 @@
     },
     total=False,
 )
 
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
-_RequiredBounceActionOutputTypeDef = TypedDict(
-    "_RequiredBounceActionOutputTypeDef",
-    {
-        "SmtpReplyCode": str,
-        "Message": str,
-        "Sender": str,
-    },
-)
-_OptionalBounceActionOutputTypeDef = TypedDict(
-    "_OptionalBounceActionOutputTypeDef",
-    {
-        "TopicArn": str,
-        "StatusCode": str,
-    },
-    total=False,
-)
-
-class BounceActionOutputTypeDef(
-    _RequiredBounceActionOutputTypeDef, _OptionalBounceActionOutputTypeDef
-):
-    pass
-
 _RequiredBounceActionTypeDef = TypedDict(
     "_RequiredBounceActionTypeDef",
     {
         "SmtpReplyCode": str,
         "Message": str,
         "Sender": str,
     },
@@ -321,39 +274,23 @@
     "CloneReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "OriginalRuleSetName": str,
     },
 )
 
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
 )
 
-ConfigurationSetOutputTypeDef = TypedDict(
-    "ConfigurationSetOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 ConfigurationSetTypeDef = TypedDict(
     "ConfigurationSetTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -491,22 +428,14 @@
 DeleteVerifiedEmailAddressRequestRequestTypeDef = TypedDict(
     "DeleteVerifiedEmailAddressRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
-DeliveryOptionsOutputTypeDef = TypedDict(
-    "DeliveryOptionsOutputTypeDef",
-    {
-        "TlsPolicy": TlsPolicyType,
-    },
-    total=False,
-)
-
 DeliveryOptionsTypeDef = TypedDict(
     "DeliveryOptionsTypeDef",
     {
         "TlsPolicy": TlsPolicyType,
     },
     total=False,
 )
@@ -557,22 +486,14 @@
         "SendingEnabled": bool,
         "ReputationMetricsEnabled": bool,
         "LastFreshStart": datetime,
     },
     total=False,
 )
 
-TrackingOptionsOutputTypeDef = TypedDict(
-    "TrackingOptionsOutputTypeDef",
-    {
-        "CustomRedirectDomain": str,
-    },
-    total=False,
-)
-
 DescribeReceiptRuleRequestRequestTypeDef = TypedDict(
     "DescribeReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleName": str,
     },
 )
@@ -580,29 +501,14 @@
 DescribeReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "DescribeReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
 )
 
-KinesisFirehoseDestinationOutputTypeDef = TypedDict(
-    "KinesisFirehoseDestinationOutputTypeDef",
-    {
-        "IAMRoleARN": str,
-        "DeliveryStreamARN": str,
-    },
-)
-
-SNSDestinationOutputTypeDef = TypedDict(
-    "SNSDestinationOutputTypeDef",
-    {
-        "TopicARN": str,
-    },
-)
-
 KinesisFirehoseDestinationTypeDef = TypedDict(
     "KinesisFirehoseDestinationTypeDef",
     {
         "IAMRoleARN": str,
         "DeliveryStreamARN": str,
     },
 )
@@ -761,53 +667,14 @@
 GetTemplateRequestRequestTypeDef = TypedDict(
     "GetTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 
-_RequiredTemplateOutputTypeDef = TypedDict(
-    "_RequiredTemplateOutputTypeDef",
-    {
-        "TemplateName": str,
-    },
-)
-_OptionalTemplateOutputTypeDef = TypedDict(
-    "_OptionalTemplateOutputTypeDef",
-    {
-        "SubjectPart": str,
-        "TextPart": str,
-        "HtmlPart": str,
-    },
-    total=False,
-)
-
-class TemplateOutputTypeDef(_RequiredTemplateOutputTypeDef, _OptionalTemplateOutputTypeDef):
-    pass
-
-_RequiredLambdaActionOutputTypeDef = TypedDict(
-    "_RequiredLambdaActionOutputTypeDef",
-    {
-        "FunctionArn": str,
-    },
-)
-_OptionalLambdaActionOutputTypeDef = TypedDict(
-    "_OptionalLambdaActionOutputTypeDef",
-    {
-        "TopicArn": str,
-        "InvocationType": InvocationTypeType,
-    },
-    total=False,
-)
-
-class LambdaActionOutputTypeDef(
-    _RequiredLambdaActionOutputTypeDef, _OptionalLambdaActionOutputTypeDef
-):
-    pass
-
 _RequiredLambdaActionTypeDef = TypedDict(
     "_RequiredLambdaActionTypeDef",
     {
         "FunctionArn": str,
     },
 )
 _OptionalLambdaActionTypeDef = TypedDict(
@@ -905,86 +772,14 @@
 RawMessageTypeDef = TypedDict(
     "RawMessageTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-_RequiredS3ActionOutputTypeDef = TypedDict(
-    "_RequiredS3ActionOutputTypeDef",
-    {
-        "BucketName": str,
-    },
-)
-_OptionalS3ActionOutputTypeDef = TypedDict(
-    "_OptionalS3ActionOutputTypeDef",
-    {
-        "TopicArn": str,
-        "ObjectKeyPrefix": str,
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
-class S3ActionOutputTypeDef(_RequiredS3ActionOutputTypeDef, _OptionalS3ActionOutputTypeDef):
-    pass
-
-_RequiredSNSActionOutputTypeDef = TypedDict(
-    "_RequiredSNSActionOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-_OptionalSNSActionOutputTypeDef = TypedDict(
-    "_OptionalSNSActionOutputTypeDef",
-    {
-        "Encoding": SNSActionEncodingType,
-    },
-    total=False,
-)
-
-class SNSActionOutputTypeDef(_RequiredSNSActionOutputTypeDef, _OptionalSNSActionOutputTypeDef):
-    pass
-
-_RequiredStopActionOutputTypeDef = TypedDict(
-    "_RequiredStopActionOutputTypeDef",
-    {
-        "Scope": Literal["RuleSet"],
-    },
-)
-_OptionalStopActionOutputTypeDef = TypedDict(
-    "_OptionalStopActionOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-    total=False,
-)
-
-class StopActionOutputTypeDef(_RequiredStopActionOutputTypeDef, _OptionalStopActionOutputTypeDef):
-    pass
-
-_RequiredWorkmailActionOutputTypeDef = TypedDict(
-    "_RequiredWorkmailActionOutputTypeDef",
-    {
-        "OrganizationArn": str,
-    },
-)
-_OptionalWorkmailActionOutputTypeDef = TypedDict(
-    "_OptionalWorkmailActionOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-    total=False,
-)
-
-class WorkmailActionOutputTypeDef(
-    _RequiredWorkmailActionOutputTypeDef, _OptionalWorkmailActionOutputTypeDef
-):
-    pass
-
 _RequiredS3ActionTypeDef = TypedDict(
     "_RequiredS3ActionTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ActionTypeDef = TypedDict(
@@ -1047,22 +842,14 @@
     },
     total=False,
 )
 
 class WorkmailActionTypeDef(_RequiredWorkmailActionTypeDef, _OptionalWorkmailActionTypeDef):
     pass
 
-ReceiptIpFilterOutputTypeDef = TypedDict(
-    "ReceiptIpFilterOutputTypeDef",
-    {
-        "Policy": ReceiptFilterPolicyType,
-        "Cidr": str,
-    },
-)
-
 ReceiptIpFilterTypeDef = TypedDict(
     "ReceiptIpFilterTypeDef",
     {
         "Policy": ReceiptFilterPolicyType,
         "Cidr": str,
     },
 )
@@ -1333,15 +1120,15 @@
     _OptionalSendTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
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
@@ -1447,18 +1234,26 @@
         "Max24HourSend": float,
         "MaxSendRate": float,
         "SentLast24Hours": float,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "Template": TemplateTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListConfigurationSetsResponseTypeDef = TypedDict(
     "ListConfigurationSetsResponseTypeDef",
     {
-        "ConfigurationSets": List[ConfigurationSetOutputTypeDef],
+        "ConfigurationSets": List[ConfigurationSetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
@@ -1673,22 +1468,14 @@
     "GetSendStatisticsResponseTypeDef",
     {
         "SendDataPoints": List[SendDataPointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "Template": TemplateOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
     "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1756,50 +1543,28 @@
 )
 
 class SendRawEmailRequestRequestTypeDef(
     _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
 ):
     pass
 
-ReceiptActionOutputTypeDef = TypedDict(
-    "ReceiptActionOutputTypeDef",
-    {
-        "S3Action": S3ActionOutputTypeDef,
-        "BounceAction": BounceActionOutputTypeDef,
-        "WorkmailAction": WorkmailActionOutputTypeDef,
-        "LambdaAction": LambdaActionOutputTypeDef,
-        "StopAction": StopActionOutputTypeDef,
-        "AddHeaderAction": AddHeaderActionOutputTypeDef,
-        "SNSAction": SNSActionOutputTypeDef,
-    },
-    total=False,
-)
-
 ReceiptActionTypeDef = TypedDict(
     "ReceiptActionTypeDef",
     {
         "S3Action": S3ActionTypeDef,
         "BounceAction": BounceActionTypeDef,
         "WorkmailAction": WorkmailActionTypeDef,
         "LambdaAction": LambdaActionTypeDef,
         "StopAction": StopActionTypeDef,
         "AddHeaderAction": AddHeaderActionTypeDef,
         "SNSAction": SNSActionTypeDef,
     },
     total=False,
 )
 
-ReceiptFilterOutputTypeDef = TypedDict(
-    "ReceiptFilterOutputTypeDef",
-    {
-        "Name": str,
-        "IpFilter": ReceiptIpFilterOutputTypeDef,
-    },
-)
-
 ReceiptFilterTypeDef = TypedDict(
     "ReceiptFilterTypeDef",
     {
         "Name": str,
         "IpFilter": ReceiptIpFilterTypeDef,
     },
 )
@@ -1848,17 +1613,17 @@
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationOutputTypeDef = TypedDict(
     "_OptionalEventDestinationOutputTypeDef",
     {
         "Enabled": bool,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
-        "SNSDestination": SNSDestinationOutputTypeDef,
+        "SNSDestination": SNSDestinationTypeDef,
     },
     total=False,
 )
 
 class EventDestinationOutputTypeDef(
     _RequiredEventDestinationOutputTypeDef, _OptionalEventDestinationOutputTypeDef
 ):
@@ -1914,15 +1679,15 @@
 )
 _OptionalReceiptRuleOutputTypeDef = TypedDict(
     "_OptionalReceiptRuleOutputTypeDef",
     {
         "Enabled": bool,
         "TlsPolicy": TlsPolicyType,
         "Recipients": List[str],
-        "Actions": List[ReceiptActionOutputTypeDef],
+        "Actions": List[ReceiptActionTypeDef],
         "ScanEnabled": bool,
     },
     total=False,
 )
 
 class ReceiptRuleOutputTypeDef(
     _RequiredReceiptRuleOutputTypeDef, _OptionalReceiptRuleOutputTypeDef
@@ -1946,26 +1711,26 @@
     },
     total=False,
 )
 
 class ReceiptRuleTypeDef(_RequiredReceiptRuleTypeDef, _OptionalReceiptRuleTypeDef):
     pass
 
-ListReceiptFiltersResponseTypeDef = TypedDict(
-    "ListReceiptFiltersResponseTypeDef",
+CreateReceiptFilterRequestRequestTypeDef = TypedDict(
+    "CreateReceiptFilterRequestRequestTypeDef",
     {
-        "Filters": List[ReceiptFilterOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Filter": ReceiptFilterTypeDef,
     },
 )
 
-CreateReceiptFilterRequestRequestTypeDef = TypedDict(
-    "CreateReceiptFilterRequestRequestTypeDef",
+ListReceiptFiltersResponseTypeDef = TypedDict(
+    "ListReceiptFiltersResponseTypeDef",
     {
-        "Filter": ReceiptFilterTypeDef,
+        "Filters": List[ReceiptFilterTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Source": str,
@@ -1990,18 +1755,18 @@
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
 
 DescribeConfigurationSetResponseTypeDef = TypedDict(
     "DescribeConfigurationSetResponseTypeDef",
     {
-        "ConfigurationSet": ConfigurationSetOutputTypeDef,
+        "ConfigurationSet": ConfigurationSetTypeDef,
         "EventDestinations": List[EventDestinationOutputTypeDef],
-        "TrackingOptions": TrackingOptionsOutputTypeDef,
-        "DeliveryOptions": DeliveryOptionsOutputTypeDef,
+        "TrackingOptions": TrackingOptionsTypeDef,
+        "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
```

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/waiter.py` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses/waiter.pyi` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/PKG-INFO` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ses
-Version: 1.28.12
-Summary: Type annotations for boto3.SES 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SES 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ses)](https://pepy.tech/project/mypy-boto3-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SES 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[boto3.SES 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,26 +375,22 @@
 ### Typed dictionaries
 
 `mypy_boto3_ses.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ses.type_defs import (
-    AddHeaderActionOutputTypeDef,
     AddHeaderActionTypeDef,
     ContentTypeDef,
-    BounceActionOutputTypeDef,
     BounceActionTypeDef,
     BulkEmailDestinationStatusTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloneReceiptRuleSetRequestRequestTypeDef,
-    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
-    ConfigurationSetOutputTypeDef,
     ConfigurationSetTypeDef,
     TrackingOptionsTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
     CreateReceiptRuleSetRequestRequestTypeDef,
     TemplateTypeDef,
     CustomVerificationEmailTemplateTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
@@ -404,25 +400,21 @@
     DeleteIdentityPolicyRequestRequestTypeDef,
     DeleteIdentityRequestRequestTypeDef,
     DeleteReceiptFilterRequestRequestTypeDef,
     DeleteReceiptRuleRequestRequestTypeDef,
     DeleteReceiptRuleSetRequestRequestTypeDef,
     DeleteTemplateRequestRequestTypeDef,
     DeleteVerifiedEmailAddressRequestRequestTypeDef,
-    DeliveryOptionsOutputTypeDef,
     DeliveryOptionsTypeDef,
     ReceiptRuleSetMetadataTypeDef,
     ResponseMetadataTypeDef,
     DescribeConfigurationSetRequestRequestTypeDef,
     ReputationOptionsTypeDef,
-    TrackingOptionsOutputTypeDef,
     DescribeReceiptRuleRequestRequestTypeDef,
     DescribeReceiptRuleSetRequestRequestTypeDef,
-    KinesisFirehoseDestinationOutputTypeDef,
-    SNSDestinationOutputTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SNSDestinationTypeDef,
     ExtensionFieldTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
     GetIdentityDkimAttributesRequestRequestTypeDef,
     IdentityDkimAttributesTypeDef,
     GetIdentityMailFromDomainAttributesRequestRequestTypeDef,
@@ -431,36 +423,29 @@
     IdentityNotificationAttributesTypeDef,
     GetIdentityPoliciesRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetIdentityVerificationAttributesRequestRequestTypeDef,
     IdentityVerificationAttributesTypeDef,
     SendDataPointTypeDef,
     GetTemplateRequestRequestTypeDef,
-    TemplateOutputTypeDef,
-    LambdaActionOutputTypeDef,
     LambdaActionTypeDef,
     PaginatorConfigTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListIdentitiesRequestRequestTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
     RawMessageTypeDef,
-    S3ActionOutputTypeDef,
-    SNSActionOutputTypeDef,
-    StopActionOutputTypeDef,
-    WorkmailActionOutputTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
-    ReceiptIpFilterOutputTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
     SetActiveReceiptRuleSetRequestRequestTypeDef,
     SetIdentityDkimEnabledRequestRequestTypeDef,
     SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef,
     SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef,
@@ -488,14 +473,15 @@
     UpdateTemplateRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityPoliciesResponseTypeDef,
     GetSendQuotaResponseTypeDef,
+    GetTemplateResponseTypeDef,
     ListConfigurationSetsResponseTypeDef,
     ListCustomVerificationEmailTemplatesResponseTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoliciesResponseTypeDef,
     ListReceiptRuleSetsResponseTypeDef,
     ListVerifiedEmailAddressesResponseTypeDef,
     SendBounceResponseTypeDef,
@@ -511,49 +497,46 @@
     RecipientDsnFieldsTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
-    GetTemplateResponseTypeDef,
     ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
     SendRawEmailRequestRequestTypeDef,
-    ReceiptActionOutputTypeDef,
     ReceiptActionTypeDef,
-    ReceiptFilterOutputTypeDef,
     ReceiptFilterTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
     EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     BouncedRecipientInfoTypeDef,
     ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
-    ListReceiptFiltersResponseTypeDef,
     CreateReceiptFilterRequestRequestTypeDef,
+    ListReceiptFiltersResponseTypeDef,
     SendEmailRequestRequestTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     SendBounceRequestRequestTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     CreateReceiptRuleRequestRequestTypeDef,
     UpdateReceiptRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddHeaderActionOutputTypeDef:
+def get_structure() -> AddHeaderActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/SOURCES.txt` & `mypy-boto3-ses-1.28.15/mypy_boto3_ses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.12/setup.py` & `mypy-boto3-ses-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ses",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ses"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SES 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SES 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

