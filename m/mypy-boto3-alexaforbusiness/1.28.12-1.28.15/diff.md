# Comparing `tmp/mypy-boto3-alexaforbusiness-1.28.12.tar.gz` & `tmp/mypy-boto3-alexaforbusiness-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-alexaforbusiness-1.28.12.tar", last modified: Thu Jul 27 05:34:13 2023, max compression
+gzip compressed data, was "mypy-boto3-alexaforbusiness-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
```

## Comparing `mypy-boto3-alexaforbusiness-1.28.12.tar` & `mypy-boto3-alexaforbusiness-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.852594 mypy-boto3-alexaforbusiness-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24570 2023-07-27 05:34:13.848594 mypy-boto3-alexaforbusiness-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23047 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.844594 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-27 05:16:56.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    67327 2023-07-27 05:16:56.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-27 05:16:57.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-07-27 05:16:56.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16333 2023-07-27 05:16:56.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-07-27 05:16:56.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    73359 2023-07-27 05:16:58.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    73284 2023-07-27 05:16:57.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.848594 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24570 2023-07-27 05:34:13.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:34:13.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:13.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:13.000000 mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:13.852594 mypy-boto3-alexaforbusiness-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:16:55.000000 mypy-boto3-alexaforbusiness-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.724609 mypy-boto3-alexaforbusiness-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:42.000000 mypy-boto3-alexaforbusiness-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24236 2023-07-28 20:42:12.724609 mypy-boto3-alexaforbusiness-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22713 2023-07-28 20:18:42.000000 mypy-boto3-alexaforbusiness-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.712609 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-28 20:18:42.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-28 20:18:42.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 20:18:42.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-28 20:18:44.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67327 2023-07-28 20:18:43.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-28 20:18:44.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-07-28 20:18:44.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16333 2023-07-28 20:18:44.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-07-28 20:18:44.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:42.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71403 2023-07-28 20:18:46.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71328 2023-07-28 20:18:45.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:42.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.724609 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24236 2023-07-28 20:42:12.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:42:12.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:42:12.000000 mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.724609 mypy-boto3-alexaforbusiness-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 20:18:42.000000 mypy-boto3-alexaforbusiness-1.28.15/setup.py
```

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/LICENSE` & `mypy-boto3-alexaforbusiness-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/PKG-INFO` & `mypy-boto3-alexaforbusiness-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-alexaforbusiness
-Version: 1.28.12
-Summary: Type annotations for boto3.AlexaForBusiness 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AlexaForBusiness 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-alexaforbusiness)](https://pepy.tech/project/mypy-boto3-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AlexaForBusiness 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[boto3.AlexaForBusiness 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
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
 [mypy-boto3-alexaforbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,36 +408,28 @@
     AssociateContactWithAddressBookRequestRequestTypeDef,
     AssociateDeviceWithNetworkProfileRequestRequestTypeDef,
     AssociateDeviceWithRoomRequestRequestTypeDef,
     AssociateSkillGroupWithRoomRequestRequestTypeDef,
     AssociateSkillWithSkillGroupRequestRequestTypeDef,
     AssociateSkillWithUsersRequestRequestTypeDef,
     AudioTypeDef,
-    BusinessReportContentRangeOutputTypeDef,
     BusinessReportContentRangeTypeDef,
-    BusinessReportRecurrenceOutputTypeDef,
     BusinessReportRecurrenceTypeDef,
     BusinessReportS3LocationTypeDef,
     CategoryTypeDef,
-    ConferencePreferenceOutputTypeDef,
     ConferencePreferenceTypeDef,
-    IPDialInOutputTypeDef,
-    MeetingSettingOutputTypeDef,
-    PSTNDialInOutputTypeDef,
-    PhoneNumberOutputTypeDef,
-    SipAddressOutputTypeDef,
-    SsmlTypeDef,
-    TextTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
     IPDialInTypeDef,
     MeetingSettingTypeDef,
     PSTNDialInTypeDef,
     PhoneNumberTypeDef,
     SipAddressTypeDef,
+    SsmlTypeDef,
+    TextTypeDef,
+    TagTypeDef,
+    ResponseMetadataTypeDef,
     CreateEndOfMeetingReminderTypeDef,
     CreateInstantBookingTypeDef,
     CreateProactiveJoinTypeDef,
     CreateRequireCheckInTypeDef,
     DeleteAddressBookRequestRequestTypeDef,
     DeleteBusinessReportScheduleRequestRequestTypeDef,
     DeleteConferenceProviderRequestRequestTypeDef,
@@ -476,15 +468,15 @@
     GetGatewayRequestRequestTypeDef,
     GetNetworkProfileRequestRequestTypeDef,
     NetworkProfileTypeDef,
     GetProfileRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     RoomTypeDef,
     GetRoomSkillParameterRequestRequestTypeDef,
-    RoomSkillParameterOutputTypeDef,
+    RoomSkillParameterTypeDef,
     GetSkillGroupRequestRequestTypeDef,
     SkillGroupTypeDef,
     InstantBookingTypeDef,
     PaginatorConfigTypeDef,
     ListBusinessReportSchedulesRequestRequestTypeDef,
     ListConferenceProvidersRequestRequestTypeDef,
     ListDeviceEventsRequestRequestTypeDef,
@@ -493,21 +485,19 @@
     ListSkillsRequestRequestTypeDef,
     SkillSummaryTypeDef,
     ListSkillsStoreCategoriesRequestRequestTypeDef,
     ListSkillsStoreSkillsByCategoryRequestRequestTypeDef,
     ListSmartHomeAppliancesRequestRequestTypeDef,
     SmartHomeApplianceTypeDef,
     ListTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
     ProactiveJoinTypeDef,
     RequireCheckInTypeDef,
     NetworkProfileDataTypeDef,
     ProfileDataTypeDef,
     PutInvitationConfigurationRequestRequestTypeDef,
-    RoomSkillParameterTypeDef,
     PutSkillAuthorizationRequestRequestTypeDef,
     RejectSkillRequestRequestTypeDef,
     ResolveRoomRequestRequestTypeDef,
     RevokeInvitationRequestRequestTypeDef,
     RoomDataTypeDef,
     SortTypeDef,
     SkillGroupDataTypeDef,
@@ -527,19 +517,23 @@
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSkillGroupRequestRequestTypeDef,
     UpdateBusinessReportScheduleRequestRequestTypeDef,
     BusinessReportTypeDef,
     PutConferencePreferenceRequestRequestTypeDef,
     ConferenceProviderTypeDef,
+    UpdateConferenceProviderRequestRequestTypeDef,
     ContactDataTypeDef,
     ContactTypeDef,
+    UpdateContactRequestRequestTypeDef,
     ContentTypeDef,
     CreateAddressBookRequestRequestTypeDef,
     CreateBusinessReportScheduleRequestRequestTypeDef,
+    CreateConferenceProviderRequestRequestTypeDef,
+    CreateContactRequestRequestTypeDef,
     CreateGatewayGroupRequestRequestTypeDef,
     CreateNetworkProfileRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     CreateSkillGroupRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     RegisterAVSDeviceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -553,49 +547,45 @@
     CreateRoomResponseTypeDef,
     CreateSkillGroupResponseTypeDef,
     CreateUserResponseTypeDef,
     GetAddressBookResponseTypeDef,
     GetConferencePreferenceResponseTypeDef,
     GetInvitationConfigurationResponseTypeDef,
     ListSkillsStoreCategoriesResponseTypeDef,
+    ListTagsResponseTypeDef,
     RegisterAVSDeviceResponseTypeDef,
     SearchAddressBooksResponseTypeDef,
     SendAnnouncementResponseTypeDef,
-    CreateConferenceProviderRequestRequestTypeDef,
-    UpdateConferenceProviderRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
-    UpdateContactRequestRequestTypeDef,
     CreateMeetingRoomConfigurationTypeDef,
     SkillDetailsTypeDef,
     ListDeviceEventsResponseTypeDef,
     DeviceStatusInfoTypeDef,
     ListGatewayGroupsResponseTypeDef,
     GetGatewayGroupResponseTypeDef,
     ListGatewaysResponseTypeDef,
     GetGatewayResponseTypeDef,
     GetNetworkProfileResponseTypeDef,
     GetRoomResponseTypeDef,
     GetRoomSkillParameterResponseTypeDef,
+    PutRoomSkillParameterRequestRequestTypeDef,
     ResolveRoomResponseTypeDef,
     GetSkillGroupResponseTypeDef,
     ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef,
     ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef,
     ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     ListSkillsRequestListSkillsPaginateTypeDef,
     ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef,
     ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef,
     ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListSkillsResponseTypeDef,
     ListSmartHomeAppliancesResponseTypeDef,
-    ListTagsResponseTypeDef,
     MeetingRoomConfigurationTypeDef,
     SearchNetworkProfilesResponseTypeDef,
     SearchProfilesResponseTypeDef,
-    PutRoomSkillParameterRequestRequestTypeDef,
     SearchRoomsResponseTypeDef,
     SearchAddressBooksRequestRequestTypeDef,
     SearchContactsRequestRequestTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchNetworkProfilesRequestRequestTypeDef,
     SearchProfilesRequestRequestTypeDef,
```

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/README.md` & `mypy-boto3-alexaforbusiness-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-alexaforbusiness)](https://pepy.tech/project/mypy-boto3-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AlexaForBusiness 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[boto3.AlexaForBusiness 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
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
 [mypy-boto3-alexaforbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -376,36 +376,28 @@
     AssociateContactWithAddressBookRequestRequestTypeDef,
     AssociateDeviceWithNetworkProfileRequestRequestTypeDef,
     AssociateDeviceWithRoomRequestRequestTypeDef,
     AssociateSkillGroupWithRoomRequestRequestTypeDef,
     AssociateSkillWithSkillGroupRequestRequestTypeDef,
     AssociateSkillWithUsersRequestRequestTypeDef,
     AudioTypeDef,
-    BusinessReportContentRangeOutputTypeDef,
     BusinessReportContentRangeTypeDef,
-    BusinessReportRecurrenceOutputTypeDef,
     BusinessReportRecurrenceTypeDef,
     BusinessReportS3LocationTypeDef,
     CategoryTypeDef,
-    ConferencePreferenceOutputTypeDef,
     ConferencePreferenceTypeDef,
-    IPDialInOutputTypeDef,
-    MeetingSettingOutputTypeDef,
-    PSTNDialInOutputTypeDef,
-    PhoneNumberOutputTypeDef,
-    SipAddressOutputTypeDef,
-    SsmlTypeDef,
-    TextTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
     IPDialInTypeDef,
     MeetingSettingTypeDef,
     PSTNDialInTypeDef,
     PhoneNumberTypeDef,
     SipAddressTypeDef,
+    SsmlTypeDef,
+    TextTypeDef,
+    TagTypeDef,
+    ResponseMetadataTypeDef,
     CreateEndOfMeetingReminderTypeDef,
     CreateInstantBookingTypeDef,
     CreateProactiveJoinTypeDef,
     CreateRequireCheckInTypeDef,
     DeleteAddressBookRequestRequestTypeDef,
     DeleteBusinessReportScheduleRequestRequestTypeDef,
     DeleteConferenceProviderRequestRequestTypeDef,
@@ -444,15 +436,15 @@
     GetGatewayRequestRequestTypeDef,
     GetNetworkProfileRequestRequestTypeDef,
     NetworkProfileTypeDef,
     GetProfileRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     RoomTypeDef,
     GetRoomSkillParameterRequestRequestTypeDef,
-    RoomSkillParameterOutputTypeDef,
+    RoomSkillParameterTypeDef,
     GetSkillGroupRequestRequestTypeDef,
     SkillGroupTypeDef,
     InstantBookingTypeDef,
     PaginatorConfigTypeDef,
     ListBusinessReportSchedulesRequestRequestTypeDef,
     ListConferenceProvidersRequestRequestTypeDef,
     ListDeviceEventsRequestRequestTypeDef,
@@ -461,21 +453,19 @@
     ListSkillsRequestRequestTypeDef,
     SkillSummaryTypeDef,
     ListSkillsStoreCategoriesRequestRequestTypeDef,
     ListSkillsStoreSkillsByCategoryRequestRequestTypeDef,
     ListSmartHomeAppliancesRequestRequestTypeDef,
     SmartHomeApplianceTypeDef,
     ListTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
     ProactiveJoinTypeDef,
     RequireCheckInTypeDef,
     NetworkProfileDataTypeDef,
     ProfileDataTypeDef,
     PutInvitationConfigurationRequestRequestTypeDef,
-    RoomSkillParameterTypeDef,
     PutSkillAuthorizationRequestRequestTypeDef,
     RejectSkillRequestRequestTypeDef,
     ResolveRoomRequestRequestTypeDef,
     RevokeInvitationRequestRequestTypeDef,
     RoomDataTypeDef,
     SortTypeDef,
     SkillGroupDataTypeDef,
@@ -495,19 +485,23 @@
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSkillGroupRequestRequestTypeDef,
     UpdateBusinessReportScheduleRequestRequestTypeDef,
     BusinessReportTypeDef,
     PutConferencePreferenceRequestRequestTypeDef,
     ConferenceProviderTypeDef,
+    UpdateConferenceProviderRequestRequestTypeDef,
     ContactDataTypeDef,
     ContactTypeDef,
+    UpdateContactRequestRequestTypeDef,
     ContentTypeDef,
     CreateAddressBookRequestRequestTypeDef,
     CreateBusinessReportScheduleRequestRequestTypeDef,
+    CreateConferenceProviderRequestRequestTypeDef,
+    CreateContactRequestRequestTypeDef,
     CreateGatewayGroupRequestRequestTypeDef,
     CreateNetworkProfileRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     CreateSkillGroupRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     RegisterAVSDeviceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -521,49 +515,45 @@
     CreateRoomResponseTypeDef,
     CreateSkillGroupResponseTypeDef,
     CreateUserResponseTypeDef,
     GetAddressBookResponseTypeDef,
     GetConferencePreferenceResponseTypeDef,
     GetInvitationConfigurationResponseTypeDef,
     ListSkillsStoreCategoriesResponseTypeDef,
+    ListTagsResponseTypeDef,
     RegisterAVSDeviceResponseTypeDef,
     SearchAddressBooksResponseTypeDef,
     SendAnnouncementResponseTypeDef,
-    CreateConferenceProviderRequestRequestTypeDef,
-    UpdateConferenceProviderRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
-    UpdateContactRequestRequestTypeDef,
     CreateMeetingRoomConfigurationTypeDef,
     SkillDetailsTypeDef,
     ListDeviceEventsResponseTypeDef,
     DeviceStatusInfoTypeDef,
     ListGatewayGroupsResponseTypeDef,
     GetGatewayGroupResponseTypeDef,
     ListGatewaysResponseTypeDef,
     GetGatewayResponseTypeDef,
     GetNetworkProfileResponseTypeDef,
     GetRoomResponseTypeDef,
     GetRoomSkillParameterResponseTypeDef,
+    PutRoomSkillParameterRequestRequestTypeDef,
     ResolveRoomResponseTypeDef,
     GetSkillGroupResponseTypeDef,
     ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef,
     ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef,
     ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     ListSkillsRequestListSkillsPaginateTypeDef,
     ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef,
     ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef,
     ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListSkillsResponseTypeDef,
     ListSmartHomeAppliancesResponseTypeDef,
-    ListTagsResponseTypeDef,
     MeetingRoomConfigurationTypeDef,
     SearchNetworkProfilesResponseTypeDef,
     SearchProfilesResponseTypeDef,
-    PutRoomSkillParameterRequestRequestTypeDef,
     SearchRoomsResponseTypeDef,
     SearchAddressBooksRequestRequestTypeDef,
     SearchContactsRequestRequestTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchNetworkProfilesRequestRequestTypeDef,
     SearchProfilesRequestRequestTypeDef,
```

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/__init__.py` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/__init__.pyi` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/__main__.py` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AlexaForBusiness 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.AlexaForBusiness 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness\nOther"
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

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/client.py` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/client.pyi` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/literals.py` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/literals.pyi` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/paginator.py` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/paginator.pyi` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/type_defs.py` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,36 +59,28 @@
     "AssociateContactWithAddressBookRequestRequestTypeDef",
     "AssociateDeviceWithNetworkProfileRequestRequestTypeDef",
     "AssociateDeviceWithRoomRequestRequestTypeDef",
     "AssociateSkillGroupWithRoomRequestRequestTypeDef",
     "AssociateSkillWithSkillGroupRequestRequestTypeDef",
     "AssociateSkillWithUsersRequestRequestTypeDef",
     "AudioTypeDef",
-    "BusinessReportContentRangeOutputTypeDef",
     "BusinessReportContentRangeTypeDef",
-    "BusinessReportRecurrenceOutputTypeDef",
     "BusinessReportRecurrenceTypeDef",
     "BusinessReportS3LocationTypeDef",
     "CategoryTypeDef",
-    "ConferencePreferenceOutputTypeDef",
     "ConferencePreferenceTypeDef",
-    "IPDialInOutputTypeDef",
-    "MeetingSettingOutputTypeDef",
-    "PSTNDialInOutputTypeDef",
-    "PhoneNumberOutputTypeDef",
-    "SipAddressOutputTypeDef",
-    "SsmlTypeDef",
-    "TextTypeDef",
-    "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "IPDialInTypeDef",
     "MeetingSettingTypeDef",
     "PSTNDialInTypeDef",
     "PhoneNumberTypeDef",
     "SipAddressTypeDef",
+    "SsmlTypeDef",
+    "TextTypeDef",
+    "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateEndOfMeetingReminderTypeDef",
     "CreateInstantBookingTypeDef",
     "CreateProactiveJoinTypeDef",
     "CreateRequireCheckInTypeDef",
     "DeleteAddressBookRequestRequestTypeDef",
     "DeleteBusinessReportScheduleRequestRequestTypeDef",
     "DeleteConferenceProviderRequestRequestTypeDef",
@@ -127,15 +119,15 @@
     "GetGatewayRequestRequestTypeDef",
     "GetNetworkProfileRequestRequestTypeDef",
     "NetworkProfileTypeDef",
     "GetProfileRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "RoomTypeDef",
     "GetRoomSkillParameterRequestRequestTypeDef",
-    "RoomSkillParameterOutputTypeDef",
+    "RoomSkillParameterTypeDef",
     "GetSkillGroupRequestRequestTypeDef",
     "SkillGroupTypeDef",
     "InstantBookingTypeDef",
     "PaginatorConfigTypeDef",
     "ListBusinessReportSchedulesRequestRequestTypeDef",
     "ListConferenceProvidersRequestRequestTypeDef",
     "ListDeviceEventsRequestRequestTypeDef",
@@ -144,21 +136,19 @@
     "ListSkillsRequestRequestTypeDef",
     "SkillSummaryTypeDef",
     "ListSkillsStoreCategoriesRequestRequestTypeDef",
     "ListSkillsStoreSkillsByCategoryRequestRequestTypeDef",
     "ListSmartHomeAppliancesRequestRequestTypeDef",
     "SmartHomeApplianceTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ProactiveJoinTypeDef",
     "RequireCheckInTypeDef",
     "NetworkProfileDataTypeDef",
     "ProfileDataTypeDef",
     "PutInvitationConfigurationRequestRequestTypeDef",
-    "RoomSkillParameterTypeDef",
     "PutSkillAuthorizationRequestRequestTypeDef",
     "RejectSkillRequestRequestTypeDef",
     "ResolveRoomRequestRequestTypeDef",
     "RevokeInvitationRequestRequestTypeDef",
     "RoomDataTypeDef",
     "SortTypeDef",
     "SkillGroupDataTypeDef",
@@ -178,19 +168,23 @@
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSkillGroupRequestRequestTypeDef",
     "UpdateBusinessReportScheduleRequestRequestTypeDef",
     "BusinessReportTypeDef",
     "PutConferencePreferenceRequestRequestTypeDef",
     "ConferenceProviderTypeDef",
+    "UpdateConferenceProviderRequestRequestTypeDef",
     "ContactDataTypeDef",
     "ContactTypeDef",
+    "UpdateContactRequestRequestTypeDef",
     "ContentTypeDef",
     "CreateAddressBookRequestRequestTypeDef",
     "CreateBusinessReportScheduleRequestRequestTypeDef",
+    "CreateConferenceProviderRequestRequestTypeDef",
+    "CreateContactRequestRequestTypeDef",
     "CreateGatewayGroupRequestRequestTypeDef",
     "CreateNetworkProfileRequestRequestTypeDef",
     "CreateRoomRequestRequestTypeDef",
     "CreateSkillGroupRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "RegisterAVSDeviceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -204,49 +198,45 @@
     "CreateRoomResponseTypeDef",
     "CreateSkillGroupResponseTypeDef",
     "CreateUserResponseTypeDef",
     "GetAddressBookResponseTypeDef",
     "GetConferencePreferenceResponseTypeDef",
     "GetInvitationConfigurationResponseTypeDef",
     "ListSkillsStoreCategoriesResponseTypeDef",
+    "ListTagsResponseTypeDef",
     "RegisterAVSDeviceResponseTypeDef",
     "SearchAddressBooksResponseTypeDef",
     "SendAnnouncementResponseTypeDef",
-    "CreateConferenceProviderRequestRequestTypeDef",
-    "UpdateConferenceProviderRequestRequestTypeDef",
-    "CreateContactRequestRequestTypeDef",
-    "UpdateContactRequestRequestTypeDef",
     "CreateMeetingRoomConfigurationTypeDef",
     "SkillDetailsTypeDef",
     "ListDeviceEventsResponseTypeDef",
     "DeviceStatusInfoTypeDef",
     "ListGatewayGroupsResponseTypeDef",
     "GetGatewayGroupResponseTypeDef",
     "ListGatewaysResponseTypeDef",
     "GetGatewayResponseTypeDef",
     "GetNetworkProfileResponseTypeDef",
     "GetRoomResponseTypeDef",
     "GetRoomSkillParameterResponseTypeDef",
+    "PutRoomSkillParameterRequestRequestTypeDef",
     "ResolveRoomResponseTypeDef",
     "GetSkillGroupResponseTypeDef",
     "ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef",
     "ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef",
     "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     "ListSkillsRequestListSkillsPaginateTypeDef",
     "ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef",
     "ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef",
     "ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListSkillsResponseTypeDef",
     "ListSmartHomeAppliancesResponseTypeDef",
-    "ListTagsResponseTypeDef",
     "MeetingRoomConfigurationTypeDef",
     "SearchNetworkProfilesResponseTypeDef",
     "SearchProfilesResponseTypeDef",
-    "PutRoomSkillParameterRequestRequestTypeDef",
     "SearchRoomsResponseTypeDef",
     "SearchAddressBooksRequestRequestTypeDef",
     "SearchContactsRequestRequestTypeDef",
     "SearchDevicesRequestRequestTypeDef",
     "SearchDevicesRequestSearchDevicesPaginateTypeDef",
     "SearchNetworkProfilesRequestRequestTypeDef",
     "SearchProfilesRequestRequestTypeDef",
@@ -373,36 +363,21 @@
     "AudioTypeDef",
     {
         "Locale": Literal["en-US"],
         "Location": str,
     },
 )
 
-BusinessReportContentRangeOutputTypeDef = TypedDict(
-    "BusinessReportContentRangeOutputTypeDef",
-    {
-        "Interval": BusinessReportIntervalType,
-    },
-)
-
 BusinessReportContentRangeTypeDef = TypedDict(
     "BusinessReportContentRangeTypeDef",
     {
         "Interval": BusinessReportIntervalType,
     },
 )
 
-BusinessReportRecurrenceOutputTypeDef = TypedDict(
-    "BusinessReportRecurrenceOutputTypeDef",
-    {
-        "StartDate": str,
-    },
-    total=False,
-)
-
 BusinessReportRecurrenceTypeDef = TypedDict(
     "BusinessReportRecurrenceTypeDef",
     {
         "StartDate": str,
     },
     total=False,
 )
@@ -421,65 +396,57 @@
     {
         "CategoryId": int,
         "CategoryName": str,
     },
     total=False,
 )
 
-ConferencePreferenceOutputTypeDef = TypedDict(
-    "ConferencePreferenceOutputTypeDef",
-    {
-        "DefaultConferenceProviderArn": str,
-    },
-    total=False,
-)
-
 ConferencePreferenceTypeDef = TypedDict(
     "ConferencePreferenceTypeDef",
     {
         "DefaultConferenceProviderArn": str,
     },
     total=False,
 )
 
-IPDialInOutputTypeDef = TypedDict(
-    "IPDialInOutputTypeDef",
+IPDialInTypeDef = TypedDict(
+    "IPDialInTypeDef",
     {
         "Endpoint": str,
         "CommsProtocol": CommsProtocolType,
     },
 )
 
-MeetingSettingOutputTypeDef = TypedDict(
-    "MeetingSettingOutputTypeDef",
+MeetingSettingTypeDef = TypedDict(
+    "MeetingSettingTypeDef",
     {
         "RequirePin": RequirePinType,
     },
 )
 
-PSTNDialInOutputTypeDef = TypedDict(
-    "PSTNDialInOutputTypeDef",
+PSTNDialInTypeDef = TypedDict(
+    "PSTNDialInTypeDef",
     {
         "CountryCode": str,
         "PhoneNumber": str,
         "OneClickIdDelay": str,
         "OneClickPinDelay": str,
     },
 )
 
-PhoneNumberOutputTypeDef = TypedDict(
-    "PhoneNumberOutputTypeDef",
+PhoneNumberTypeDef = TypedDict(
+    "PhoneNumberTypeDef",
     {
         "Number": str,
         "Type": PhoneNumberTypeType,
     },
 )
 
-SipAddressOutputTypeDef = TypedDict(
-    "SipAddressOutputTypeDef",
+SipAddressTypeDef = TypedDict(
+    "SipAddressTypeDef",
     {
         "Uri": str,
         "Type": Literal["WORK"],
     },
 )
 
 SsmlTypeDef = TypedDict(
@@ -513,55 +480,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-IPDialInTypeDef = TypedDict(
-    "IPDialInTypeDef",
-    {
-        "Endpoint": str,
-        "CommsProtocol": CommsProtocolType,
-    },
-)
-
-MeetingSettingTypeDef = TypedDict(
-    "MeetingSettingTypeDef",
-    {
-        "RequirePin": RequirePinType,
-    },
-)
-
-PSTNDialInTypeDef = TypedDict(
-    "PSTNDialInTypeDef",
-    {
-        "CountryCode": str,
-        "PhoneNumber": str,
-        "OneClickIdDelay": str,
-        "OneClickPinDelay": str,
-    },
-)
-
-PhoneNumberTypeDef = TypedDict(
-    "PhoneNumberTypeDef",
-    {
-        "Number": str,
-        "Type": PhoneNumberTypeType,
-    },
-)
-
-SipAddressTypeDef = TypedDict(
-    "SipAddressTypeDef",
-    {
-        "Uri": str,
-        "Type": Literal["WORK"],
-    },
-)
-
 CreateEndOfMeetingReminderTypeDef = TypedDict(
     "CreateEndOfMeetingReminderTypeDef",
     {
         "ReminderAtMinutes": Sequence[int],
         "ReminderType": EndOfMeetingReminderTypeType,
         "Enabled": bool,
     },
@@ -1014,16 +940,16 @@
 class GetRoomSkillParameterRequestRequestTypeDef(
     _RequiredGetRoomSkillParameterRequestRequestTypeDef,
     _OptionalGetRoomSkillParameterRequestRequestTypeDef,
 ):
     pass
 
 
-RoomSkillParameterOutputTypeDef = TypedDict(
-    "RoomSkillParameterOutputTypeDef",
+RoomSkillParameterTypeDef = TypedDict(
+    "RoomSkillParameterTypeDef",
     {
         "ParameterKey": str,
         "ParameterValue": str,
     },
 )
 
 GetSkillGroupRequestRequestTypeDef = TypedDict(
@@ -1230,22 +1156,14 @@
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
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
 ProactiveJoinTypeDef = TypedDict(
     "ProactiveJoinTypeDef",
     {
         "EnabledByMotion": bool,
     },
     total=False,
 )
@@ -1308,22 +1226,14 @@
 class PutInvitationConfigurationRequestRequestTypeDef(
     _RequiredPutInvitationConfigurationRequestRequestTypeDef,
     _OptionalPutInvitationConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-RoomSkillParameterTypeDef = TypedDict(
-    "RoomSkillParameterTypeDef",
-    {
-        "ParameterKey": str,
-        "ParameterValue": str,
-    },
-)
-
 _RequiredPutSkillAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredPutSkillAuthorizationRequestRequestTypeDef",
     {
         "AuthorizationResult": Mapping[str, str],
         "SkillId": str,
     },
 )
@@ -1664,49 +1574,100 @@
 
 ConferenceProviderTypeDef = TypedDict(
     "ConferenceProviderTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": ConferenceProviderTypeType,
-        "IPDialIn": IPDialInOutputTypeDef,
-        "PSTNDialIn": PSTNDialInOutputTypeDef,
-        "MeetingSetting": MeetingSettingOutputTypeDef,
+        "IPDialIn": IPDialInTypeDef,
+        "PSTNDialIn": PSTNDialInTypeDef,
+        "MeetingSetting": MeetingSettingTypeDef,
+    },
+    total=False,
+)
+
+_RequiredUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConferenceProviderRequestRequestTypeDef",
+    {
+        "ConferenceProviderArn": str,
+        "ConferenceProviderType": ConferenceProviderTypeType,
+        "MeetingSetting": MeetingSettingTypeDef,
+    },
+)
+_OptionalUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConferenceProviderRequestRequestTypeDef",
+    {
+        "IPDialIn": IPDialInTypeDef,
+        "PSTNDialIn": PSTNDialInTypeDef,
     },
     total=False,
 )
 
+
+class UpdateConferenceProviderRequestRequestTypeDef(
+    _RequiredUpdateConferenceProviderRequestRequestTypeDef,
+    _OptionalUpdateConferenceProviderRequestRequestTypeDef,
+):
+    pass
+
+
 ContactDataTypeDef = TypedDict(
     "ContactDataTypeDef",
     {
         "ContactArn": str,
         "DisplayName": str,
         "FirstName": str,
         "LastName": str,
         "PhoneNumber": str,
-        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
-        "SipAddresses": List[SipAddressOutputTypeDef],
+        "PhoneNumbers": List[PhoneNumberTypeDef],
+        "SipAddresses": List[SipAddressTypeDef],
     },
     total=False,
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "ContactArn": str,
         "DisplayName": str,
         "FirstName": str,
         "LastName": str,
         "PhoneNumber": str,
-        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
-        "SipAddresses": List[SipAddressOutputTypeDef],
+        "PhoneNumbers": List[PhoneNumberTypeDef],
+        "SipAddresses": List[SipAddressTypeDef],
+    },
+    total=False,
+)
+
+_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateContactRequestRequestTypeDef",
+    {
+        "ContactArn": str,
+    },
+)
+_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateContactRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "FirstName": str,
+        "LastName": str,
+        "PhoneNumber": str,
+        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
+        "SipAddresses": Sequence[SipAddressTypeDef],
     },
     total=False,
 )
 
+
+class UpdateContactRequestRequestTypeDef(
+    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
+):
+    pass
+
+
 ContentTypeDef = TypedDict(
     "ContentTypeDef",
     {
         "TextList": Sequence[TextTypeDef],
         "SsmlList": Sequence[SsmlTypeDef],
         "AudioList": Sequence[AudioTypeDef],
     },
@@ -1760,14 +1721,68 @@
 class CreateBusinessReportScheduleRequestRequestTypeDef(
     _RequiredCreateBusinessReportScheduleRequestRequestTypeDef,
     _OptionalCreateBusinessReportScheduleRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredCreateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConferenceProviderRequestRequestTypeDef",
+    {
+        "ConferenceProviderName": str,
+        "ConferenceProviderType": ConferenceProviderTypeType,
+        "MeetingSetting": MeetingSettingTypeDef,
+    },
+)
+_OptionalCreateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConferenceProviderRequestRequestTypeDef",
+    {
+        "IPDialIn": IPDialInTypeDef,
+        "PSTNDialIn": PSTNDialInTypeDef,
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateConferenceProviderRequestRequestTypeDef(
+    _RequiredCreateConferenceProviderRequestRequestTypeDef,
+    _OptionalCreateConferenceProviderRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateContactRequestRequestTypeDef",
+    {
+        "FirstName": str,
+    },
+)
+_OptionalCreateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateContactRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "LastName": str,
+        "PhoneNumber": str,
+        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
+        "SipAddresses": Sequence[SipAddressTypeDef],
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateContactRequestRequestTypeDef(
+    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateGatewayGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayGroupRequestRequestTypeDef",
     {
         "Name": str,
         "ClientRequestToken": str,
     },
 )
@@ -2013,15 +2028,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConferencePreferenceResponseTypeDef = TypedDict(
     "GetConferencePreferenceResponseTypeDef",
     {
-        "Preference": ConferencePreferenceOutputTypeDef,
+        "Preference": ConferencePreferenceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInvitationConfigurationResponseTypeDef = TypedDict(
     "GetInvitationConfigurationResponseTypeDef",
     {
@@ -2037,14 +2052,23 @@
     {
         "CategoryList": List[CategoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RegisterAVSDeviceResponseTypeDef = TypedDict(
     "RegisterAVSDeviceResponseTypeDef",
     {
         "DeviceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2063,119 +2087,14 @@
     "SendAnnouncementResponseTypeDef",
     {
         "AnnouncementArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConferenceProviderRequestRequestTypeDef",
-    {
-        "ConferenceProviderName": str,
-        "ConferenceProviderType": ConferenceProviderTypeType,
-        "MeetingSetting": MeetingSettingTypeDef,
-    },
-)
-_OptionalCreateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConferenceProviderRequestRequestTypeDef",
-    {
-        "IPDialIn": IPDialInTypeDef,
-        "PSTNDialIn": PSTNDialInTypeDef,
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateConferenceProviderRequestRequestTypeDef(
-    _RequiredCreateConferenceProviderRequestRequestTypeDef,
-    _OptionalCreateConferenceProviderRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConferenceProviderRequestRequestTypeDef",
-    {
-        "ConferenceProviderArn": str,
-        "ConferenceProviderType": ConferenceProviderTypeType,
-        "MeetingSetting": MeetingSettingTypeDef,
-    },
-)
-_OptionalUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConferenceProviderRequestRequestTypeDef",
-    {
-        "IPDialIn": IPDialInTypeDef,
-        "PSTNDialIn": PSTNDialInTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateConferenceProviderRequestRequestTypeDef(
-    _RequiredUpdateConferenceProviderRequestRequestTypeDef,
-    _OptionalUpdateConferenceProviderRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateContactRequestRequestTypeDef",
-    {
-        "FirstName": str,
-    },
-)
-_OptionalCreateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateContactRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "LastName": str,
-        "PhoneNumber": str,
-        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
-        "SipAddresses": Sequence[SipAddressTypeDef],
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateContactRequestRequestTypeDef(
-    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateContactRequestRequestTypeDef",
-    {
-        "ContactArn": str,
-    },
-)
-_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateContactRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "FirstName": str,
-        "LastName": str,
-        "PhoneNumber": str,
-        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
-        "SipAddresses": Sequence[SipAddressTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateContactRequestRequestTypeDef(
-    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
-):
-    pass
-
-
 CreateMeetingRoomConfigurationTypeDef = TypedDict(
     "CreateMeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": CreateEndOfMeetingReminderTypeDef,
         "InstantBooking": CreateInstantBookingTypeDef,
         "RequireCheckIn": CreateRequireCheckInTypeDef,
@@ -2269,25 +2188,48 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoomSkillParameterResponseTypeDef = TypedDict(
     "GetRoomSkillParameterResponseTypeDef",
     {
-        "RoomSkillParameter": RoomSkillParameterOutputTypeDef,
+        "RoomSkillParameter": RoomSkillParameterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRoomSkillParameterRequestRequestTypeDef",
+    {
+        "SkillId": str,
+        "RoomSkillParameter": RoomSkillParameterTypeDef,
+    },
+)
+_OptionalPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRoomSkillParameterRequestRequestTypeDef",
+    {
+        "RoomArn": str,
+    },
+    total=False,
+)
+
+
+class PutRoomSkillParameterRequestRequestTypeDef(
+    _RequiredPutRoomSkillParameterRequestRequestTypeDef,
+    _OptionalPutRoomSkillParameterRequestRequestTypeDef,
+):
+    pass
+
+
 ResolveRoomResponseTypeDef = TypedDict(
     "ResolveRoomResponseTypeDef",
     {
         "RoomArn": str,
         "RoomName": str,
-        "RoomSkillParameters": List[RoomSkillParameterOutputTypeDef],
+        "RoomSkillParameters": List[RoomSkillParameterTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSkillGroupResponseTypeDef = TypedDict(
     "GetSkillGroupResponseTypeDef",
     {
@@ -2433,23 +2375,14 @@
     {
         "SmartHomeAppliances": List[SmartHomeApplianceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 MeetingRoomConfigurationTypeDef = TypedDict(
     "MeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": EndOfMeetingReminderTypeDef,
         "InstantBooking": InstantBookingTypeDef,
         "RequireCheckIn": RequireCheckInTypeDef,
@@ -2474,37 +2407,14 @@
         "Profiles": List[ProfileDataTypeDef],
         "NextToken": str,
         "TotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRoomSkillParameterRequestRequestTypeDef",
-    {
-        "SkillId": str,
-        "RoomSkillParameter": RoomSkillParameterTypeDef,
-    },
-)
-_OptionalPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRoomSkillParameterRequestRequestTypeDef",
-    {
-        "RoomArn": str,
-    },
-    total=False,
-)
-
-
-class PutRoomSkillParameterRequestRequestTypeDef(
-    _RequiredPutRoomSkillParameterRequestRequestTypeDef,
-    _OptionalPutRoomSkillParameterRequestRequestTypeDef,
-):
-    pass
-
-
 SearchRoomsResponseTypeDef = TypedDict(
     "SearchRoomsResponseTypeDef",
     {
         "Rooms": List[RoomDataTypeDef],
         "NextToken": str,
         "TotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2685,16 +2595,16 @@
     "BusinessReportScheduleTypeDef",
     {
         "ScheduleArn": str,
         "ScheduleName": str,
         "S3BucketName": str,
         "S3KeyPrefix": str,
         "Format": BusinessReportFormatType,
-        "ContentRange": BusinessReportContentRangeOutputTypeDef,
-        "Recurrence": BusinessReportRecurrenceOutputTypeDef,
+        "ContentRange": BusinessReportContentRangeTypeDef,
+        "Recurrence": BusinessReportRecurrenceTypeDef,
         "LastBusinessReport": BusinessReportTypeDef,
     },
     total=False,
 )
 
 GetConferenceProviderResponseTypeDef = TypedDict(
     "GetConferenceProviderResponseTypeDef",
```

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness/type_defs.pyi` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -58,36 +58,28 @@
     "AssociateContactWithAddressBookRequestRequestTypeDef",
     "AssociateDeviceWithNetworkProfileRequestRequestTypeDef",
     "AssociateDeviceWithRoomRequestRequestTypeDef",
     "AssociateSkillGroupWithRoomRequestRequestTypeDef",
     "AssociateSkillWithSkillGroupRequestRequestTypeDef",
     "AssociateSkillWithUsersRequestRequestTypeDef",
     "AudioTypeDef",
-    "BusinessReportContentRangeOutputTypeDef",
     "BusinessReportContentRangeTypeDef",
-    "BusinessReportRecurrenceOutputTypeDef",
     "BusinessReportRecurrenceTypeDef",
     "BusinessReportS3LocationTypeDef",
     "CategoryTypeDef",
-    "ConferencePreferenceOutputTypeDef",
     "ConferencePreferenceTypeDef",
-    "IPDialInOutputTypeDef",
-    "MeetingSettingOutputTypeDef",
-    "PSTNDialInOutputTypeDef",
-    "PhoneNumberOutputTypeDef",
-    "SipAddressOutputTypeDef",
-    "SsmlTypeDef",
-    "TextTypeDef",
-    "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "IPDialInTypeDef",
     "MeetingSettingTypeDef",
     "PSTNDialInTypeDef",
     "PhoneNumberTypeDef",
     "SipAddressTypeDef",
+    "SsmlTypeDef",
+    "TextTypeDef",
+    "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateEndOfMeetingReminderTypeDef",
     "CreateInstantBookingTypeDef",
     "CreateProactiveJoinTypeDef",
     "CreateRequireCheckInTypeDef",
     "DeleteAddressBookRequestRequestTypeDef",
     "DeleteBusinessReportScheduleRequestRequestTypeDef",
     "DeleteConferenceProviderRequestRequestTypeDef",
@@ -126,15 +118,15 @@
     "GetGatewayRequestRequestTypeDef",
     "GetNetworkProfileRequestRequestTypeDef",
     "NetworkProfileTypeDef",
     "GetProfileRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "RoomTypeDef",
     "GetRoomSkillParameterRequestRequestTypeDef",
-    "RoomSkillParameterOutputTypeDef",
+    "RoomSkillParameterTypeDef",
     "GetSkillGroupRequestRequestTypeDef",
     "SkillGroupTypeDef",
     "InstantBookingTypeDef",
     "PaginatorConfigTypeDef",
     "ListBusinessReportSchedulesRequestRequestTypeDef",
     "ListConferenceProvidersRequestRequestTypeDef",
     "ListDeviceEventsRequestRequestTypeDef",
@@ -143,21 +135,19 @@
     "ListSkillsRequestRequestTypeDef",
     "SkillSummaryTypeDef",
     "ListSkillsStoreCategoriesRequestRequestTypeDef",
     "ListSkillsStoreSkillsByCategoryRequestRequestTypeDef",
     "ListSmartHomeAppliancesRequestRequestTypeDef",
     "SmartHomeApplianceTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ProactiveJoinTypeDef",
     "RequireCheckInTypeDef",
     "NetworkProfileDataTypeDef",
     "ProfileDataTypeDef",
     "PutInvitationConfigurationRequestRequestTypeDef",
-    "RoomSkillParameterTypeDef",
     "PutSkillAuthorizationRequestRequestTypeDef",
     "RejectSkillRequestRequestTypeDef",
     "ResolveRoomRequestRequestTypeDef",
     "RevokeInvitationRequestRequestTypeDef",
     "RoomDataTypeDef",
     "SortTypeDef",
     "SkillGroupDataTypeDef",
@@ -177,19 +167,23 @@
     "UpdateNetworkProfileRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSkillGroupRequestRequestTypeDef",
     "UpdateBusinessReportScheduleRequestRequestTypeDef",
     "BusinessReportTypeDef",
     "PutConferencePreferenceRequestRequestTypeDef",
     "ConferenceProviderTypeDef",
+    "UpdateConferenceProviderRequestRequestTypeDef",
     "ContactDataTypeDef",
     "ContactTypeDef",
+    "UpdateContactRequestRequestTypeDef",
     "ContentTypeDef",
     "CreateAddressBookRequestRequestTypeDef",
     "CreateBusinessReportScheduleRequestRequestTypeDef",
+    "CreateConferenceProviderRequestRequestTypeDef",
+    "CreateContactRequestRequestTypeDef",
     "CreateGatewayGroupRequestRequestTypeDef",
     "CreateNetworkProfileRequestRequestTypeDef",
     "CreateRoomRequestRequestTypeDef",
     "CreateSkillGroupRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "RegisterAVSDeviceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -203,49 +197,45 @@
     "CreateRoomResponseTypeDef",
     "CreateSkillGroupResponseTypeDef",
     "CreateUserResponseTypeDef",
     "GetAddressBookResponseTypeDef",
     "GetConferencePreferenceResponseTypeDef",
     "GetInvitationConfigurationResponseTypeDef",
     "ListSkillsStoreCategoriesResponseTypeDef",
+    "ListTagsResponseTypeDef",
     "RegisterAVSDeviceResponseTypeDef",
     "SearchAddressBooksResponseTypeDef",
     "SendAnnouncementResponseTypeDef",
-    "CreateConferenceProviderRequestRequestTypeDef",
-    "UpdateConferenceProviderRequestRequestTypeDef",
-    "CreateContactRequestRequestTypeDef",
-    "UpdateContactRequestRequestTypeDef",
     "CreateMeetingRoomConfigurationTypeDef",
     "SkillDetailsTypeDef",
     "ListDeviceEventsResponseTypeDef",
     "DeviceStatusInfoTypeDef",
     "ListGatewayGroupsResponseTypeDef",
     "GetGatewayGroupResponseTypeDef",
     "ListGatewaysResponseTypeDef",
     "GetGatewayResponseTypeDef",
     "GetNetworkProfileResponseTypeDef",
     "GetRoomResponseTypeDef",
     "GetRoomSkillParameterResponseTypeDef",
+    "PutRoomSkillParameterRequestRequestTypeDef",
     "ResolveRoomResponseTypeDef",
     "GetSkillGroupResponseTypeDef",
     "ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef",
     "ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef",
     "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
     "ListSkillsRequestListSkillsPaginateTypeDef",
     "ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef",
     "ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef",
     "ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListSkillsResponseTypeDef",
     "ListSmartHomeAppliancesResponseTypeDef",
-    "ListTagsResponseTypeDef",
     "MeetingRoomConfigurationTypeDef",
     "SearchNetworkProfilesResponseTypeDef",
     "SearchProfilesResponseTypeDef",
-    "PutRoomSkillParameterRequestRequestTypeDef",
     "SearchRoomsResponseTypeDef",
     "SearchAddressBooksRequestRequestTypeDef",
     "SearchContactsRequestRequestTypeDef",
     "SearchDevicesRequestRequestTypeDef",
     "SearchDevicesRequestSearchDevicesPaginateTypeDef",
     "SearchNetworkProfilesRequestRequestTypeDef",
     "SearchProfilesRequestRequestTypeDef",
@@ -370,36 +360,21 @@
     "AudioTypeDef",
     {
         "Locale": Literal["en-US"],
         "Location": str,
     },
 )
 
-BusinessReportContentRangeOutputTypeDef = TypedDict(
-    "BusinessReportContentRangeOutputTypeDef",
-    {
-        "Interval": BusinessReportIntervalType,
-    },
-)
-
 BusinessReportContentRangeTypeDef = TypedDict(
     "BusinessReportContentRangeTypeDef",
     {
         "Interval": BusinessReportIntervalType,
     },
 )
 
-BusinessReportRecurrenceOutputTypeDef = TypedDict(
-    "BusinessReportRecurrenceOutputTypeDef",
-    {
-        "StartDate": str,
-    },
-    total=False,
-)
-
 BusinessReportRecurrenceTypeDef = TypedDict(
     "BusinessReportRecurrenceTypeDef",
     {
         "StartDate": str,
     },
     total=False,
 )
@@ -418,65 +393,57 @@
     {
         "CategoryId": int,
         "CategoryName": str,
     },
     total=False,
 )
 
-ConferencePreferenceOutputTypeDef = TypedDict(
-    "ConferencePreferenceOutputTypeDef",
-    {
-        "DefaultConferenceProviderArn": str,
-    },
-    total=False,
-)
-
 ConferencePreferenceTypeDef = TypedDict(
     "ConferencePreferenceTypeDef",
     {
         "DefaultConferenceProviderArn": str,
     },
     total=False,
 )
 
-IPDialInOutputTypeDef = TypedDict(
-    "IPDialInOutputTypeDef",
+IPDialInTypeDef = TypedDict(
+    "IPDialInTypeDef",
     {
         "Endpoint": str,
         "CommsProtocol": CommsProtocolType,
     },
 )
 
-MeetingSettingOutputTypeDef = TypedDict(
-    "MeetingSettingOutputTypeDef",
+MeetingSettingTypeDef = TypedDict(
+    "MeetingSettingTypeDef",
     {
         "RequirePin": RequirePinType,
     },
 )
 
-PSTNDialInOutputTypeDef = TypedDict(
-    "PSTNDialInOutputTypeDef",
+PSTNDialInTypeDef = TypedDict(
+    "PSTNDialInTypeDef",
     {
         "CountryCode": str,
         "PhoneNumber": str,
         "OneClickIdDelay": str,
         "OneClickPinDelay": str,
     },
 )
 
-PhoneNumberOutputTypeDef = TypedDict(
-    "PhoneNumberOutputTypeDef",
+PhoneNumberTypeDef = TypedDict(
+    "PhoneNumberTypeDef",
     {
         "Number": str,
         "Type": PhoneNumberTypeType,
     },
 )
 
-SipAddressOutputTypeDef = TypedDict(
-    "SipAddressOutputTypeDef",
+SipAddressTypeDef = TypedDict(
+    "SipAddressTypeDef",
     {
         "Uri": str,
         "Type": Literal["WORK"],
     },
 )
 
 SsmlTypeDef = TypedDict(
@@ -510,55 +477,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-IPDialInTypeDef = TypedDict(
-    "IPDialInTypeDef",
-    {
-        "Endpoint": str,
-        "CommsProtocol": CommsProtocolType,
-    },
-)
-
-MeetingSettingTypeDef = TypedDict(
-    "MeetingSettingTypeDef",
-    {
-        "RequirePin": RequirePinType,
-    },
-)
-
-PSTNDialInTypeDef = TypedDict(
-    "PSTNDialInTypeDef",
-    {
-        "CountryCode": str,
-        "PhoneNumber": str,
-        "OneClickIdDelay": str,
-        "OneClickPinDelay": str,
-    },
-)
-
-PhoneNumberTypeDef = TypedDict(
-    "PhoneNumberTypeDef",
-    {
-        "Number": str,
-        "Type": PhoneNumberTypeType,
-    },
-)
-
-SipAddressTypeDef = TypedDict(
-    "SipAddressTypeDef",
-    {
-        "Uri": str,
-        "Type": Literal["WORK"],
-    },
-)
-
 CreateEndOfMeetingReminderTypeDef = TypedDict(
     "CreateEndOfMeetingReminderTypeDef",
     {
         "ReminderAtMinutes": Sequence[int],
         "ReminderType": EndOfMeetingReminderTypeType,
         "Enabled": bool,
     },
@@ -1001,16 +927,16 @@
 
 class GetRoomSkillParameterRequestRequestTypeDef(
     _RequiredGetRoomSkillParameterRequestRequestTypeDef,
     _OptionalGetRoomSkillParameterRequestRequestTypeDef,
 ):
     pass
 
-RoomSkillParameterOutputTypeDef = TypedDict(
-    "RoomSkillParameterOutputTypeDef",
+RoomSkillParameterTypeDef = TypedDict(
+    "RoomSkillParameterTypeDef",
     {
         "ParameterKey": str,
         "ParameterValue": str,
     },
 )
 
 GetSkillGroupRequestRequestTypeDef = TypedDict(
@@ -1209,22 +1135,14 @@
 )
 
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
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
 ProactiveJoinTypeDef = TypedDict(
     "ProactiveJoinTypeDef",
     {
         "EnabledByMotion": bool,
     },
     total=False,
 )
@@ -1285,22 +1203,14 @@
 
 class PutInvitationConfigurationRequestRequestTypeDef(
     _RequiredPutInvitationConfigurationRequestRequestTypeDef,
     _OptionalPutInvitationConfigurationRequestRequestTypeDef,
 ):
     pass
 
-RoomSkillParameterTypeDef = TypedDict(
-    "RoomSkillParameterTypeDef",
-    {
-        "ParameterKey": str,
-        "ParameterValue": str,
-    },
-)
-
 _RequiredPutSkillAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredPutSkillAuthorizationRequestRequestTypeDef",
     {
         "AuthorizationResult": Mapping[str, str],
         "SkillId": str,
     },
 )
@@ -1627,49 +1537,96 @@
 
 ConferenceProviderTypeDef = TypedDict(
     "ConferenceProviderTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": ConferenceProviderTypeType,
-        "IPDialIn": IPDialInOutputTypeDef,
-        "PSTNDialIn": PSTNDialInOutputTypeDef,
-        "MeetingSetting": MeetingSettingOutputTypeDef,
+        "IPDialIn": IPDialInTypeDef,
+        "PSTNDialIn": PSTNDialInTypeDef,
+        "MeetingSetting": MeetingSettingTypeDef,
+    },
+    total=False,
+)
+
+_RequiredUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConferenceProviderRequestRequestTypeDef",
+    {
+        "ConferenceProviderArn": str,
+        "ConferenceProviderType": ConferenceProviderTypeType,
+        "MeetingSetting": MeetingSettingTypeDef,
+    },
+)
+_OptionalUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConferenceProviderRequestRequestTypeDef",
+    {
+        "IPDialIn": IPDialInTypeDef,
+        "PSTNDialIn": PSTNDialInTypeDef,
     },
     total=False,
 )
 
+class UpdateConferenceProviderRequestRequestTypeDef(
+    _RequiredUpdateConferenceProviderRequestRequestTypeDef,
+    _OptionalUpdateConferenceProviderRequestRequestTypeDef,
+):
+    pass
+
 ContactDataTypeDef = TypedDict(
     "ContactDataTypeDef",
     {
         "ContactArn": str,
         "DisplayName": str,
         "FirstName": str,
         "LastName": str,
         "PhoneNumber": str,
-        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
-        "SipAddresses": List[SipAddressOutputTypeDef],
+        "PhoneNumbers": List[PhoneNumberTypeDef],
+        "SipAddresses": List[SipAddressTypeDef],
     },
     total=False,
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "ContactArn": str,
         "DisplayName": str,
         "FirstName": str,
         "LastName": str,
         "PhoneNumber": str,
-        "PhoneNumbers": List[PhoneNumberOutputTypeDef],
-        "SipAddresses": List[SipAddressOutputTypeDef],
+        "PhoneNumbers": List[PhoneNumberTypeDef],
+        "SipAddresses": List[SipAddressTypeDef],
     },
     total=False,
 )
 
+_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateContactRequestRequestTypeDef",
+    {
+        "ContactArn": str,
+    },
+)
+_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateContactRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "FirstName": str,
+        "LastName": str,
+        "PhoneNumber": str,
+        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
+        "SipAddresses": Sequence[SipAddressTypeDef],
+    },
+    total=False,
+)
+
+class UpdateContactRequestRequestTypeDef(
+    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
+):
+    pass
+
 ContentTypeDef = TypedDict(
     "ContentTypeDef",
     {
         "TextList": Sequence[TextTypeDef],
         "SsmlList": Sequence[SsmlTypeDef],
         "AudioList": Sequence[AudioTypeDef],
     },
@@ -1719,14 +1676,64 @@
 
 class CreateBusinessReportScheduleRequestRequestTypeDef(
     _RequiredCreateBusinessReportScheduleRequestRequestTypeDef,
     _OptionalCreateBusinessReportScheduleRequestRequestTypeDef,
 ):
     pass
 
+_RequiredCreateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConferenceProviderRequestRequestTypeDef",
+    {
+        "ConferenceProviderName": str,
+        "ConferenceProviderType": ConferenceProviderTypeType,
+        "MeetingSetting": MeetingSettingTypeDef,
+    },
+)
+_OptionalCreateConferenceProviderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConferenceProviderRequestRequestTypeDef",
+    {
+        "IPDialIn": IPDialInTypeDef,
+        "PSTNDialIn": PSTNDialInTypeDef,
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateConferenceProviderRequestRequestTypeDef(
+    _RequiredCreateConferenceProviderRequestRequestTypeDef,
+    _OptionalCreateConferenceProviderRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateContactRequestRequestTypeDef",
+    {
+        "FirstName": str,
+    },
+)
+_OptionalCreateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateContactRequestRequestTypeDef",
+    {
+        "DisplayName": str,
+        "LastName": str,
+        "PhoneNumber": str,
+        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
+        "SipAddresses": Sequence[SipAddressTypeDef],
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateContactRequestRequestTypeDef(
+    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateGatewayGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayGroupRequestRequestTypeDef",
     {
         "Name": str,
         "ClientRequestToken": str,
     },
 )
@@ -1960,15 +1967,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConferencePreferenceResponseTypeDef = TypedDict(
     "GetConferencePreferenceResponseTypeDef",
     {
-        "Preference": ConferencePreferenceOutputTypeDef,
+        "Preference": ConferencePreferenceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInvitationConfigurationResponseTypeDef = TypedDict(
     "GetInvitationConfigurationResponseTypeDef",
     {
@@ -1984,14 +1991,23 @@
     {
         "CategoryList": List[CategoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RegisterAVSDeviceResponseTypeDef = TypedDict(
     "RegisterAVSDeviceResponseTypeDef",
     {
         "DeviceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2010,111 +2026,14 @@
     "SendAnnouncementResponseTypeDef",
     {
         "AnnouncementArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConferenceProviderRequestRequestTypeDef",
-    {
-        "ConferenceProviderName": str,
-        "ConferenceProviderType": ConferenceProviderTypeType,
-        "MeetingSetting": MeetingSettingTypeDef,
-    },
-)
-_OptionalCreateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConferenceProviderRequestRequestTypeDef",
-    {
-        "IPDialIn": IPDialInTypeDef,
-        "PSTNDialIn": PSTNDialInTypeDef,
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateConferenceProviderRequestRequestTypeDef(
-    _RequiredCreateConferenceProviderRequestRequestTypeDef,
-    _OptionalCreateConferenceProviderRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConferenceProviderRequestRequestTypeDef",
-    {
-        "ConferenceProviderArn": str,
-        "ConferenceProviderType": ConferenceProviderTypeType,
-        "MeetingSetting": MeetingSettingTypeDef,
-    },
-)
-_OptionalUpdateConferenceProviderRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConferenceProviderRequestRequestTypeDef",
-    {
-        "IPDialIn": IPDialInTypeDef,
-        "PSTNDialIn": PSTNDialInTypeDef,
-    },
-    total=False,
-)
-
-class UpdateConferenceProviderRequestRequestTypeDef(
-    _RequiredUpdateConferenceProviderRequestRequestTypeDef,
-    _OptionalUpdateConferenceProviderRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateContactRequestRequestTypeDef",
-    {
-        "FirstName": str,
-    },
-)
-_OptionalCreateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateContactRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "LastName": str,
-        "PhoneNumber": str,
-        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
-        "SipAddresses": Sequence[SipAddressTypeDef],
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateContactRequestRequestTypeDef(
-    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateContactRequestRequestTypeDef",
-    {
-        "ContactArn": str,
-    },
-)
-_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateContactRequestRequestTypeDef",
-    {
-        "DisplayName": str,
-        "FirstName": str,
-        "LastName": str,
-        "PhoneNumber": str,
-        "PhoneNumbers": Sequence[PhoneNumberTypeDef],
-        "SipAddresses": Sequence[SipAddressTypeDef],
-    },
-    total=False,
-)
-
-class UpdateContactRequestRequestTypeDef(
-    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
-):
-    pass
-
 CreateMeetingRoomConfigurationTypeDef = TypedDict(
     "CreateMeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": CreateEndOfMeetingReminderTypeDef,
         "InstantBooking": CreateInstantBookingTypeDef,
         "RequireCheckIn": CreateRequireCheckInTypeDef,
@@ -2208,25 +2127,46 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoomSkillParameterResponseTypeDef = TypedDict(
     "GetRoomSkillParameterResponseTypeDef",
     {
-        "RoomSkillParameter": RoomSkillParameterOutputTypeDef,
+        "RoomSkillParameter": RoomSkillParameterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRoomSkillParameterRequestRequestTypeDef",
+    {
+        "SkillId": str,
+        "RoomSkillParameter": RoomSkillParameterTypeDef,
+    },
+)
+_OptionalPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRoomSkillParameterRequestRequestTypeDef",
+    {
+        "RoomArn": str,
+    },
+    total=False,
+)
+
+class PutRoomSkillParameterRequestRequestTypeDef(
+    _RequiredPutRoomSkillParameterRequestRequestTypeDef,
+    _OptionalPutRoomSkillParameterRequestRequestTypeDef,
+):
+    pass
+
 ResolveRoomResponseTypeDef = TypedDict(
     "ResolveRoomResponseTypeDef",
     {
         "RoomArn": str,
         "RoomName": str,
-        "RoomSkillParameters": List[RoomSkillParameterOutputTypeDef],
+        "RoomSkillParameters": List[RoomSkillParameterTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSkillGroupResponseTypeDef = TypedDict(
     "GetSkillGroupResponseTypeDef",
     {
@@ -2364,23 +2304,14 @@
     {
         "SmartHomeAppliances": List[SmartHomeApplianceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 MeetingRoomConfigurationTypeDef = TypedDict(
     "MeetingRoomConfigurationTypeDef",
     {
         "RoomUtilizationMetricsEnabled": bool,
         "EndOfMeetingReminder": EndOfMeetingReminderTypeDef,
         "InstantBooking": InstantBookingTypeDef,
         "RequireCheckIn": RequireCheckInTypeDef,
@@ -2405,35 +2336,14 @@
         "Profiles": List[ProfileDataTypeDef],
         "NextToken": str,
         "TotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRoomSkillParameterRequestRequestTypeDef",
-    {
-        "SkillId": str,
-        "RoomSkillParameter": RoomSkillParameterTypeDef,
-    },
-)
-_OptionalPutRoomSkillParameterRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRoomSkillParameterRequestRequestTypeDef",
-    {
-        "RoomArn": str,
-    },
-    total=False,
-)
-
-class PutRoomSkillParameterRequestRequestTypeDef(
-    _RequiredPutRoomSkillParameterRequestRequestTypeDef,
-    _OptionalPutRoomSkillParameterRequestRequestTypeDef,
-):
-    pass
-
 SearchRoomsResponseTypeDef = TypedDict(
     "SearchRoomsResponseTypeDef",
     {
         "Rooms": List[RoomDataTypeDef],
         "NextToken": str,
         "TotalCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2614,16 +2524,16 @@
     "BusinessReportScheduleTypeDef",
     {
         "ScheduleArn": str,
         "ScheduleName": str,
         "S3BucketName": str,
         "S3KeyPrefix": str,
         "Format": BusinessReportFormatType,
-        "ContentRange": BusinessReportContentRangeOutputTypeDef,
-        "Recurrence": BusinessReportRecurrenceOutputTypeDef,
+        "ContentRange": BusinessReportContentRangeTypeDef,
+        "Recurrence": BusinessReportRecurrenceTypeDef,
         "LastBusinessReport": BusinessReportTypeDef,
     },
     total=False,
 )
 
 GetConferenceProviderResponseTypeDef = TypedDict(
     "GetConferenceProviderResponseTypeDef",
```

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/PKG-INFO` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-alexaforbusiness
-Version: 1.28.12
-Summary: Type annotations for boto3.AlexaForBusiness 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AlexaForBusiness 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-alexaforbusiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-alexaforbusiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-alexaforbusiness)](https://pepy.tech/project/mypy-boto3-alexaforbusiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AlexaForBusiness 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
+[boto3.AlexaForBusiness 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
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
 [mypy-boto3-alexaforbusiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_alexaforbusiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -408,36 +408,28 @@
     AssociateContactWithAddressBookRequestRequestTypeDef,
     AssociateDeviceWithNetworkProfileRequestRequestTypeDef,
     AssociateDeviceWithRoomRequestRequestTypeDef,
     AssociateSkillGroupWithRoomRequestRequestTypeDef,
     AssociateSkillWithSkillGroupRequestRequestTypeDef,
     AssociateSkillWithUsersRequestRequestTypeDef,
     AudioTypeDef,
-    BusinessReportContentRangeOutputTypeDef,
     BusinessReportContentRangeTypeDef,
-    BusinessReportRecurrenceOutputTypeDef,
     BusinessReportRecurrenceTypeDef,
     BusinessReportS3LocationTypeDef,
     CategoryTypeDef,
-    ConferencePreferenceOutputTypeDef,
     ConferencePreferenceTypeDef,
-    IPDialInOutputTypeDef,
-    MeetingSettingOutputTypeDef,
-    PSTNDialInOutputTypeDef,
-    PhoneNumberOutputTypeDef,
-    SipAddressOutputTypeDef,
-    SsmlTypeDef,
-    TextTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
     IPDialInTypeDef,
     MeetingSettingTypeDef,
     PSTNDialInTypeDef,
     PhoneNumberTypeDef,
     SipAddressTypeDef,
+    SsmlTypeDef,
+    TextTypeDef,
+    TagTypeDef,
+    ResponseMetadataTypeDef,
     CreateEndOfMeetingReminderTypeDef,
     CreateInstantBookingTypeDef,
     CreateProactiveJoinTypeDef,
     CreateRequireCheckInTypeDef,
     DeleteAddressBookRequestRequestTypeDef,
     DeleteBusinessReportScheduleRequestRequestTypeDef,
     DeleteConferenceProviderRequestRequestTypeDef,
@@ -476,15 +468,15 @@
     GetGatewayRequestRequestTypeDef,
     GetNetworkProfileRequestRequestTypeDef,
     NetworkProfileTypeDef,
     GetProfileRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     RoomTypeDef,
     GetRoomSkillParameterRequestRequestTypeDef,
-    RoomSkillParameterOutputTypeDef,
+    RoomSkillParameterTypeDef,
     GetSkillGroupRequestRequestTypeDef,
     SkillGroupTypeDef,
     InstantBookingTypeDef,
     PaginatorConfigTypeDef,
     ListBusinessReportSchedulesRequestRequestTypeDef,
     ListConferenceProvidersRequestRequestTypeDef,
     ListDeviceEventsRequestRequestTypeDef,
@@ -493,21 +485,19 @@
     ListSkillsRequestRequestTypeDef,
     SkillSummaryTypeDef,
     ListSkillsStoreCategoriesRequestRequestTypeDef,
     ListSkillsStoreSkillsByCategoryRequestRequestTypeDef,
     ListSmartHomeAppliancesRequestRequestTypeDef,
     SmartHomeApplianceTypeDef,
     ListTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
     ProactiveJoinTypeDef,
     RequireCheckInTypeDef,
     NetworkProfileDataTypeDef,
     ProfileDataTypeDef,
     PutInvitationConfigurationRequestRequestTypeDef,
-    RoomSkillParameterTypeDef,
     PutSkillAuthorizationRequestRequestTypeDef,
     RejectSkillRequestRequestTypeDef,
     ResolveRoomRequestRequestTypeDef,
     RevokeInvitationRequestRequestTypeDef,
     RoomDataTypeDef,
     SortTypeDef,
     SkillGroupDataTypeDef,
@@ -527,19 +517,23 @@
     UpdateNetworkProfileRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSkillGroupRequestRequestTypeDef,
     UpdateBusinessReportScheduleRequestRequestTypeDef,
     BusinessReportTypeDef,
     PutConferencePreferenceRequestRequestTypeDef,
     ConferenceProviderTypeDef,
+    UpdateConferenceProviderRequestRequestTypeDef,
     ContactDataTypeDef,
     ContactTypeDef,
+    UpdateContactRequestRequestTypeDef,
     ContentTypeDef,
     CreateAddressBookRequestRequestTypeDef,
     CreateBusinessReportScheduleRequestRequestTypeDef,
+    CreateConferenceProviderRequestRequestTypeDef,
+    CreateContactRequestRequestTypeDef,
     CreateGatewayGroupRequestRequestTypeDef,
     CreateNetworkProfileRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     CreateSkillGroupRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     RegisterAVSDeviceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -553,49 +547,45 @@
     CreateRoomResponseTypeDef,
     CreateSkillGroupResponseTypeDef,
     CreateUserResponseTypeDef,
     GetAddressBookResponseTypeDef,
     GetConferencePreferenceResponseTypeDef,
     GetInvitationConfigurationResponseTypeDef,
     ListSkillsStoreCategoriesResponseTypeDef,
+    ListTagsResponseTypeDef,
     RegisterAVSDeviceResponseTypeDef,
     SearchAddressBooksResponseTypeDef,
     SendAnnouncementResponseTypeDef,
-    CreateConferenceProviderRequestRequestTypeDef,
-    UpdateConferenceProviderRequestRequestTypeDef,
-    CreateContactRequestRequestTypeDef,
-    UpdateContactRequestRequestTypeDef,
     CreateMeetingRoomConfigurationTypeDef,
     SkillDetailsTypeDef,
     ListDeviceEventsResponseTypeDef,
     DeviceStatusInfoTypeDef,
     ListGatewayGroupsResponseTypeDef,
     GetGatewayGroupResponseTypeDef,
     ListGatewaysResponseTypeDef,
     GetGatewayResponseTypeDef,
     GetNetworkProfileResponseTypeDef,
     GetRoomResponseTypeDef,
     GetRoomSkillParameterResponseTypeDef,
+    PutRoomSkillParameterRequestRequestTypeDef,
     ResolveRoomResponseTypeDef,
     GetSkillGroupResponseTypeDef,
     ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef,
     ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef,
     ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
     ListSkillsRequestListSkillsPaginateTypeDef,
     ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef,
     ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef,
     ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef,
     ListTagsRequestListTagsPaginateTypeDef,
     ListSkillsResponseTypeDef,
     ListSmartHomeAppliancesResponseTypeDef,
-    ListTagsResponseTypeDef,
     MeetingRoomConfigurationTypeDef,
     SearchNetworkProfilesResponseTypeDef,
     SearchProfilesResponseTypeDef,
-    PutRoomSkillParameterRequestRequestTypeDef,
     SearchRoomsResponseTypeDef,
     SearchAddressBooksRequestRequestTypeDef,
     SearchContactsRequestRequestTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchNetworkProfilesRequestRequestTypeDef,
     SearchProfilesRequestRequestTypeDef,
```

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/mypy_boto3_alexaforbusiness.egg-info/SOURCES.txt` & `mypy-boto3-alexaforbusiness-1.28.15/mypy_boto3_alexaforbusiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-alexaforbusiness-1.28.12/setup.py` & `mypy-boto3-alexaforbusiness-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-alexaforbusiness",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_alexaforbusiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AlexaForBusiness 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.AlexaForBusiness 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

