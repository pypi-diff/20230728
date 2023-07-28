# Comparing `tmp/mypy-boto3-chime-sdk-meetings-1.28.12.tar.gz` & `tmp/mypy-boto3-chime-sdk-meetings-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-meetings-1.28.12.tar", last modified: Thu Jul 27 05:34:23 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-meetings-1.28.15.tar", last modified: Fri Jul 28 20:42:22 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-meetings-1.28.12.tar` & `mypy-boto3-chime-sdk-meetings-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:23.036567 mypy-boto3-chime-sdk-meetings-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-27 05:34:23.036567 mypy-boto3-chime-sdk-meetings-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:23.036567 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:23.036567 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:23.036567 mypy-boto3-chime-sdk-meetings-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.528740 mypy-boto3-chime-sdk-meetings-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:37.000000 mypy-boto3-chime-sdk-meetings-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-28 20:42:22.528740 mypy-boto3-chime-sdk-meetings-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-07-28 20:20:37.000000 mypy-boto3-chime-sdk-meetings-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.528740 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-28 20:20:37.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-28 20:20:37.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-28 20:20:37.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-07-28 20:20:37.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-07-28 20:20:37.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-07-28 20:20:38.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-07-28 20:20:38.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:37.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14242 2023-07-28 20:20:38.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-07-28 20:20:38.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:37.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.528740 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 20:42:22.000000 mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:22.528740 mypy-boto3-chime-sdk-meetings-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-28 20:20:37.000000 mypy-boto3-chime-sdk-meetings-1.28.15/setup.py
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/LICENSE` & `mypy-boto3-chime-sdk-meetings-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/PKG-INFO` & `mypy-boto3-chime-sdk-meetings-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-meetings
-Version: 1.28.12
-Summary: Type annotations for boto3.ChimeSDKMeetings 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ChimeSDKMeetings 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-meetings)](https://pepy.tech/project/mypy-boto3-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMeetings 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[boto3.ChimeSDKMeetings 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
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
 [mypy-boto3-chime-sdk-meetings docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,63 +310,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime_sdk_meetings.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_meetings.type_defs import (
-    AttendeeCapabilitiesOutputTypeDef,
     AttendeeCapabilitiesTypeDef,
     AttendeeIdItemTypeDef,
-    AudioFeaturesOutputTypeDef,
     AudioFeaturesTypeDef,
     CreateAttendeeErrorTypeDef,
+    ResponseMetadataTypeDef,
     NotificationsConfigurationTypeDef,
     TagTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
     DeleteMeetingRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     MediaPlacementTypeDef,
-    ResponseMetadataTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     UpdateAttendeeCapabilitiesRequestRequestTypeDef,
     BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
-    MeetingFeaturesConfigurationOutputTypeDef,
     MeetingFeaturesConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TranscriptionConfigurationTypeDef,
-    ListTagsForResourceResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     UpdateAttendeeCapabilitiesResponseTypeDef,
     BatchCreateAttendeeRequestRequestTypeDef,
-    MeetingTypeDef,
     CreateMeetingRequestRequestTypeDef,
     CreateMeetingWithAttendeesRequestRequestTypeDef,
+    MeetingTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
 )
 
 
-def get_structure() -> AttendeeCapabilitiesOutputTypeDef:
+def get_structure() -> AttendeeCapabilitiesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/README.md` & `mypy-boto3-chime-sdk-meetings-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-meetings)](https://pepy.tech/project/mypy-boto3-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMeetings 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[boto3.ChimeSDKMeetings 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
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
 [mypy-boto3-chime-sdk-meetings docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -278,63 +278,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime_sdk_meetings.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_meetings.type_defs import (
-    AttendeeCapabilitiesOutputTypeDef,
     AttendeeCapabilitiesTypeDef,
     AttendeeIdItemTypeDef,
-    AudioFeaturesOutputTypeDef,
     AudioFeaturesTypeDef,
     CreateAttendeeErrorTypeDef,
+    ResponseMetadataTypeDef,
     NotificationsConfigurationTypeDef,
     TagTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
     DeleteMeetingRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     MediaPlacementTypeDef,
-    ResponseMetadataTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     UpdateAttendeeCapabilitiesRequestRequestTypeDef,
     BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
-    MeetingFeaturesConfigurationOutputTypeDef,
     MeetingFeaturesConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TranscriptionConfigurationTypeDef,
-    ListTagsForResourceResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     UpdateAttendeeCapabilitiesResponseTypeDef,
     BatchCreateAttendeeRequestRequestTypeDef,
-    MeetingTypeDef,
     CreateMeetingRequestRequestTypeDef,
     CreateMeetingWithAttendeesRequestRequestTypeDef,
+    MeetingTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
 )
 
 
-def get_structure() -> AttendeeCapabilitiesOutputTypeDef:
+def get_structure() -> AttendeeCapabilitiesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/__main__.py` & `mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMeetings 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMeetings 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings\nOther"
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

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/client.py` & `mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/client.pyi` & `mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/literals.py` & `mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/literals.pyi` & `mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/type_defs.py` & `mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for chime-sdk-meetings service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime_sdk_meetings.type_defs import AttendeeCapabilitiesOutputTypeDef
+    from mypy_boto3_chime_sdk_meetings.type_defs import AttendeeCapabilitiesTypeDef
 
-    data: AttendeeCapabilitiesOutputTypeDef = {...}
+    data: AttendeeCapabilitiesTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import (
     MediaCapabilitiesType,
@@ -33,70 +33,57 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AttendeeCapabilitiesOutputTypeDef",
     "AttendeeCapabilitiesTypeDef",
     "AttendeeIdItemTypeDef",
-    "AudioFeaturesOutputTypeDef",
     "AudioFeaturesTypeDef",
     "CreateAttendeeErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "NotificationsConfigurationTypeDef",
     "TagTypeDef",
     "DeleteAttendeeRequestRequestTypeDef",
     "DeleteMeetingRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "GetAttendeeRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "MediaPlacementTypeDef",
-    "ResponseMetadataTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeRequestItemTypeDef",
     "CreateAttendeeRequestRequestTypeDef",
     "UpdateAttendeeCapabilitiesRequestRequestTypeDef",
     "BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef",
-    "MeetingFeaturesConfigurationOutputTypeDef",
     "MeetingFeaturesConfigurationTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TranscriptionConfigurationTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
     "UpdateAttendeeCapabilitiesResponseTypeDef",
     "BatchCreateAttendeeRequestRequestTypeDef",
-    "MeetingTypeDef",
     "CreateMeetingRequestRequestTypeDef",
     "CreateMeetingWithAttendeesRequestRequestTypeDef",
+    "MeetingTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
 )
 
-AttendeeCapabilitiesOutputTypeDef = TypedDict(
-    "AttendeeCapabilitiesOutputTypeDef",
-    {
-        "Audio": MediaCapabilitiesType,
-        "Video": MediaCapabilitiesType,
-        "Content": MediaCapabilitiesType,
-    },
-)
-
 AttendeeCapabilitiesTypeDef = TypedDict(
     "AttendeeCapabilitiesTypeDef",
     {
         "Audio": MediaCapabilitiesType,
         "Video": MediaCapabilitiesType,
         "Content": MediaCapabilitiesType,
     },
@@ -105,22 +92,14 @@
 AttendeeIdItemTypeDef = TypedDict(
     "AttendeeIdItemTypeDef",
     {
         "AttendeeId": str,
     },
 )
 
-AudioFeaturesOutputTypeDef = TypedDict(
-    "AudioFeaturesOutputTypeDef",
-    {
-        "EchoReduction": MeetingFeatureStatusType,
-    },
-    total=False,
-)
-
 AudioFeaturesTypeDef = TypedDict(
     "AudioFeaturesTypeDef",
     {
         "EchoReduction": MeetingFeatureStatusType,
     },
     total=False,
 )
@@ -131,14 +110,25 @@
         "ExternalUserId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
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
 NotificationsConfigurationTypeDef = TypedDict(
     "NotificationsConfigurationTypeDef",
     {
         "LambdaFunctionArn": str,
         "SnsTopicArn": str,
         "SqsQueueArn": str,
     },
@@ -164,21 +154,14 @@
 DeleteMeetingRequestRequestTypeDef = TypedDict(
     "DeleteMeetingRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEngineTranscribeMedicalSettingsTypeDef = TypedDict(
     "_RequiredEngineTranscribeMedicalSettingsTypeDef",
     {
         "LanguageCode": Literal["en-US"],
         "Specialty": TranscribeMedicalSpecialtyType,
         "Type": TranscribeMedicalTypeType,
     },
@@ -263,22 +246,14 @@
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
-)
-
 MediaPlacementTypeDef = TypedDict(
     "MediaPlacementTypeDef",
     {
         "AudioHostUrl": str,
         "AudioFallbackUrl": str,
         "SignalingUrl": str,
         "TurnControlUrl": str,
@@ -286,25 +261,14 @@
         "ScreenViewingUrl": str,
         "ScreenSharingUrl": str,
         "EventIngestionUrl": str,
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
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
@@ -318,15 +282,15 @@
 
 AttendeeTypeDef = TypedDict(
     "AttendeeTypeDef",
     {
         "ExternalUserId": str,
         "AttendeeId": str,
         "JoinToken": str,
-        "Capabilities": AttendeeCapabilitiesOutputTypeDef,
+        "Capabilities": AttendeeCapabilitiesTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateAttendeeRequestItemTypeDef = TypedDict(
     "_RequiredCreateAttendeeRequestItemTypeDef",
     {
@@ -384,28 +348,35 @@
     {
         "MeetingId": str,
         "ExcludedAttendeeIds": Sequence[AttendeeIdItemTypeDef],
         "Capabilities": AttendeeCapabilitiesTypeDef,
     },
 )
 
-MeetingFeaturesConfigurationOutputTypeDef = TypedDict(
-    "MeetingFeaturesConfigurationOutputTypeDef",
+MeetingFeaturesConfigurationTypeDef = TypedDict(
+    "MeetingFeaturesConfigurationTypeDef",
     {
-        "Audio": AudioFeaturesOutputTypeDef,
+        "Audio": AudioFeaturesTypeDef,
     },
     total=False,
 )
 
-MeetingFeaturesConfigurationTypeDef = TypedDict(
-    "MeetingFeaturesConfigurationTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "Audio": AudioFeaturesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
@@ -417,88 +388,64 @@
     {
         "EngineTranscribeSettings": EngineTranscribeSettingsTypeDef,
         "EngineTranscribeMedicalSettings": EngineTranscribeMedicalSettingsTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchCreateAttendeeResponseTypeDef = TypedDict(
     "BatchCreateAttendeeResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAttendeeResponseTypeDef = TypedDict(
     "CreateAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAttendeeResponseTypeDef = TypedDict(
     "GetAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttendeesResponseTypeDef = TypedDict(
     "ListAttendeesResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAttendeeCapabilitiesResponseTypeDef = TypedDict(
     "UpdateAttendeeCapabilitiesResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateAttendeeRequestRequestTypeDef = TypedDict(
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
         "Attendees": Sequence[CreateAttendeeRequestItemTypeDef],
     },
 )
 
-MeetingTypeDef = TypedDict(
-    "MeetingTypeDef",
-    {
-        "MeetingId": str,
-        "MeetingHostId": str,
-        "ExternalMeetingId": str,
-        "MediaRegion": str,
-        "MediaPlacement": MediaPlacementTypeDef,
-        "MeetingFeatures": MeetingFeaturesConfigurationOutputTypeDef,
-        "PrimaryMeetingId": str,
-        "TenantIds": List[str],
-        "MeetingArn": str,
-    },
-    total=False,
-)
-
 _RequiredCreateMeetingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMeetingRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "MediaRegion": str,
         "ExternalMeetingId": str,
     },
@@ -549,40 +496,56 @@
 class CreateMeetingWithAttendeesRequestRequestTypeDef(
     _RequiredCreateMeetingWithAttendeesRequestRequestTypeDef,
     _OptionalCreateMeetingWithAttendeesRequestRequestTypeDef,
 ):
     pass
 
 
+MeetingTypeDef = TypedDict(
+    "MeetingTypeDef",
+    {
+        "MeetingId": str,
+        "MeetingHostId": str,
+        "ExternalMeetingId": str,
+        "MediaRegion": str,
+        "MediaPlacement": MediaPlacementTypeDef,
+        "MeetingFeatures": MeetingFeaturesConfigurationTypeDef,
+        "PrimaryMeetingId": str,
+        "TenantIds": List[str],
+        "MeetingArn": str,
+    },
+    total=False,
+)
+
 StartMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StartMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
         "TranscriptionConfiguration": TranscriptionConfigurationTypeDef,
     },
 )
 
 CreateMeetingResponseTypeDef = TypedDict(
     "CreateMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMeetingWithAttendeesResponseTypeDef = TypedDict(
     "CreateMeetingWithAttendeesResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMeetingResponseTypeDef = TypedDict(
     "GetMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/type_defs.pyi` & `mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for chime-sdk-meetings service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime_sdk_meetings.type_defs import AttendeeCapabilitiesOutputTypeDef
+    from mypy_boto3_chime_sdk_meetings.type_defs import AttendeeCapabilitiesTypeDef
 
-    data: AttendeeCapabilitiesOutputTypeDef = {...}
+    data: AttendeeCapabilitiesTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import (
     MediaCapabilitiesType,
@@ -32,70 +32,57 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AttendeeCapabilitiesOutputTypeDef",
     "AttendeeCapabilitiesTypeDef",
     "AttendeeIdItemTypeDef",
-    "AudioFeaturesOutputTypeDef",
     "AudioFeaturesTypeDef",
     "CreateAttendeeErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "NotificationsConfigurationTypeDef",
     "TagTypeDef",
     "DeleteAttendeeRequestRequestTypeDef",
     "DeleteMeetingRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "GetAttendeeRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "MediaPlacementTypeDef",
-    "ResponseMetadataTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeRequestItemTypeDef",
     "CreateAttendeeRequestRequestTypeDef",
     "UpdateAttendeeCapabilitiesRequestRequestTypeDef",
     "BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef",
-    "MeetingFeaturesConfigurationOutputTypeDef",
     "MeetingFeaturesConfigurationTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TranscriptionConfigurationTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
     "UpdateAttendeeCapabilitiesResponseTypeDef",
     "BatchCreateAttendeeRequestRequestTypeDef",
-    "MeetingTypeDef",
     "CreateMeetingRequestRequestTypeDef",
     "CreateMeetingWithAttendeesRequestRequestTypeDef",
+    "MeetingTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
 )
 
-AttendeeCapabilitiesOutputTypeDef = TypedDict(
-    "AttendeeCapabilitiesOutputTypeDef",
-    {
-        "Audio": MediaCapabilitiesType,
-        "Video": MediaCapabilitiesType,
-        "Content": MediaCapabilitiesType,
-    },
-)
-
 AttendeeCapabilitiesTypeDef = TypedDict(
     "AttendeeCapabilitiesTypeDef",
     {
         "Audio": MediaCapabilitiesType,
         "Video": MediaCapabilitiesType,
         "Content": MediaCapabilitiesType,
     },
@@ -104,22 +91,14 @@
 AttendeeIdItemTypeDef = TypedDict(
     "AttendeeIdItemTypeDef",
     {
         "AttendeeId": str,
     },
 )
 
-AudioFeaturesOutputTypeDef = TypedDict(
-    "AudioFeaturesOutputTypeDef",
-    {
-        "EchoReduction": MeetingFeatureStatusType,
-    },
-    total=False,
-)
-
 AudioFeaturesTypeDef = TypedDict(
     "AudioFeaturesTypeDef",
     {
         "EchoReduction": MeetingFeatureStatusType,
     },
     total=False,
 )
@@ -130,14 +109,25 @@
         "ExternalUserId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
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
 NotificationsConfigurationTypeDef = TypedDict(
     "NotificationsConfigurationTypeDef",
     {
         "LambdaFunctionArn": str,
         "SnsTopicArn": str,
         "SqsQueueArn": str,
     },
@@ -163,21 +153,14 @@
 DeleteMeetingRequestRequestTypeDef = TypedDict(
     "DeleteMeetingRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEngineTranscribeMedicalSettingsTypeDef = TypedDict(
     "_RequiredEngineTranscribeMedicalSettingsTypeDef",
     {
         "LanguageCode": Literal["en-US"],
         "Specialty": TranscribeMedicalSpecialtyType,
         "Type": TranscribeMedicalTypeType,
     },
@@ -258,22 +241,14 @@
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
-)
-
 MediaPlacementTypeDef = TypedDict(
     "MediaPlacementTypeDef",
     {
         "AudioHostUrl": str,
         "AudioFallbackUrl": str,
         "SignalingUrl": str,
         "TurnControlUrl": str,
@@ -281,25 +256,14 @@
         "ScreenViewingUrl": str,
         "ScreenSharingUrl": str,
         "EventIngestionUrl": str,
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
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
@@ -313,15 +277,15 @@
 
 AttendeeTypeDef = TypedDict(
     "AttendeeTypeDef",
     {
         "ExternalUserId": str,
         "AttendeeId": str,
         "JoinToken": str,
-        "Capabilities": AttendeeCapabilitiesOutputTypeDef,
+        "Capabilities": AttendeeCapabilitiesTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateAttendeeRequestItemTypeDef = TypedDict(
     "_RequiredCreateAttendeeRequestItemTypeDef",
     {
@@ -375,28 +339,35 @@
     {
         "MeetingId": str,
         "ExcludedAttendeeIds": Sequence[AttendeeIdItemTypeDef],
         "Capabilities": AttendeeCapabilitiesTypeDef,
     },
 )
 
-MeetingFeaturesConfigurationOutputTypeDef = TypedDict(
-    "MeetingFeaturesConfigurationOutputTypeDef",
+MeetingFeaturesConfigurationTypeDef = TypedDict(
+    "MeetingFeaturesConfigurationTypeDef",
     {
-        "Audio": AudioFeaturesOutputTypeDef,
+        "Audio": AudioFeaturesTypeDef,
     },
     total=False,
 )
 
-MeetingFeaturesConfigurationTypeDef = TypedDict(
-    "MeetingFeaturesConfigurationTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "Audio": AudioFeaturesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
@@ -408,88 +379,64 @@
     {
         "EngineTranscribeSettings": EngineTranscribeSettingsTypeDef,
         "EngineTranscribeMedicalSettings": EngineTranscribeMedicalSettingsTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchCreateAttendeeResponseTypeDef = TypedDict(
     "BatchCreateAttendeeResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAttendeeResponseTypeDef = TypedDict(
     "CreateAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAttendeeResponseTypeDef = TypedDict(
     "GetAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttendeesResponseTypeDef = TypedDict(
     "ListAttendeesResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAttendeeCapabilitiesResponseTypeDef = TypedDict(
     "UpdateAttendeeCapabilitiesResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateAttendeeRequestRequestTypeDef = TypedDict(
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
         "Attendees": Sequence[CreateAttendeeRequestItemTypeDef],
     },
 )
 
-MeetingTypeDef = TypedDict(
-    "MeetingTypeDef",
-    {
-        "MeetingId": str,
-        "MeetingHostId": str,
-        "ExternalMeetingId": str,
-        "MediaRegion": str,
-        "MediaPlacement": MediaPlacementTypeDef,
-        "MeetingFeatures": MeetingFeaturesConfigurationOutputTypeDef,
-        "PrimaryMeetingId": str,
-        "TenantIds": List[str],
-        "MeetingArn": str,
-    },
-    total=False,
-)
-
 _RequiredCreateMeetingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMeetingRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "MediaRegion": str,
         "ExternalMeetingId": str,
     },
@@ -536,40 +483,56 @@
 
 class CreateMeetingWithAttendeesRequestRequestTypeDef(
     _RequiredCreateMeetingWithAttendeesRequestRequestTypeDef,
     _OptionalCreateMeetingWithAttendeesRequestRequestTypeDef,
 ):
     pass
 
+MeetingTypeDef = TypedDict(
+    "MeetingTypeDef",
+    {
+        "MeetingId": str,
+        "MeetingHostId": str,
+        "ExternalMeetingId": str,
+        "MediaRegion": str,
+        "MediaPlacement": MediaPlacementTypeDef,
+        "MeetingFeatures": MeetingFeaturesConfigurationTypeDef,
+        "PrimaryMeetingId": str,
+        "TenantIds": List[str],
+        "MeetingArn": str,
+    },
+    total=False,
+)
+
 StartMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StartMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
         "TranscriptionConfiguration": TranscriptionConfigurationTypeDef,
     },
 )
 
 CreateMeetingResponseTypeDef = TypedDict(
     "CreateMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMeetingWithAttendeesResponseTypeDef = TypedDict(
     "CreateMeetingWithAttendeesResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMeetingResponseTypeDef = TypedDict(
     "GetMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-meetings
-Version: 1.28.12
-Summary: Type annotations for boto3.ChimeSDKMeetings 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ChimeSDKMeetings 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-meetings)](https://pepy.tech/project/mypy-boto3-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMeetings 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[boto3.ChimeSDKMeetings 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
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
 [mypy-boto3-chime-sdk-meetings docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,63 +310,59 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime_sdk_meetings.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_meetings.type_defs import (
-    AttendeeCapabilitiesOutputTypeDef,
     AttendeeCapabilitiesTypeDef,
     AttendeeIdItemTypeDef,
-    AudioFeaturesOutputTypeDef,
     AudioFeaturesTypeDef,
     CreateAttendeeErrorTypeDef,
+    ResponseMetadataTypeDef,
     NotificationsConfigurationTypeDef,
     TagTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
     DeleteMeetingRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     MediaPlacementTypeDef,
-    ResponseMetadataTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     UpdateAttendeeCapabilitiesRequestRequestTypeDef,
     BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
-    MeetingFeaturesConfigurationOutputTypeDef,
     MeetingFeaturesConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TranscriptionConfigurationTypeDef,
-    ListTagsForResourceResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     UpdateAttendeeCapabilitiesResponseTypeDef,
     BatchCreateAttendeeRequestRequestTypeDef,
-    MeetingTypeDef,
     CreateMeetingRequestRequestTypeDef,
     CreateMeetingWithAttendeesRequestRequestTypeDef,
+    MeetingTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
 )
 
 
-def get_structure() -> AttendeeCapabilitiesOutputTypeDef:
+def get_structure() -> AttendeeCapabilitiesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-meetings-1.28.15/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.12/setup.py` & `mypy-boto3-chime-sdk-meetings-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-meetings",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_chime_sdk_meetings"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMeetings 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ChimeSDKMeetings 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

