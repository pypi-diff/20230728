# Comparing `tmp/mypy-boto3-groundstation-1.28.12.tar.gz` & `tmp/mypy-boto3-groundstation-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-groundstation-1.28.12.tar", last modified: Thu Jul 27 05:34:45 2023, max compression
+gzip compressed data, was "mypy-boto3-groundstation-1.28.15.tar", last modified: Fri Jul 28 20:42:53 2023, max compression
```

## Comparing `mypy-boto3-groundstation-1.28.12.tar` & `mypy-boto3-groundstation-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.144498 mypy-boto3-groundstation-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20170 2023-07-27 05:34:45.140498 mypy-boto3-groundstation-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18659 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.132498 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26848 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26800 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-27 05:23:11.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-27 05:23:11.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-27 05:23:10.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48959 2023-07-27 05:23:12.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48894 2023-07-27 05:23:11.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-27 05:23:10.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-27 05:23:10.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.140498 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20170 2023-07-27 05:34:44.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-27 05:34:44.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:44.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:44.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:44.000000 mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:45.144498 mypy-boto3-groundstation-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 05:23:09.000000 mypy-boto3-groundstation-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.345173 mypy-boto3-groundstation-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19321 2023-07-28 20:42:53.345173 mypy-boto3-groundstation-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17810 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.329172 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26848 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26800 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40795 2023-07-28 20:27:10.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40746 2023-07-28 20:27:10.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-28 20:27:09.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.345173 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19321 2023-07-28 20:42:53.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-28 20:42:53.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:53.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:53.000000 mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:53.345173 mypy-boto3-groundstation-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 20:27:08.000000 mypy-boto3-groundstation-1.28.15/setup.py
```

### Comparing `mypy-boto3-groundstation-1.28.12/LICENSE` & `mypy-boto3-groundstation-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.12/PKG-INFO` & `mypy-boto3-groundstation-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-groundstation
-Version: 1.28.12
-Summary: Type annotations for boto3.GroundStation 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.GroundStation 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-groundstation)](https://pepy.tech/project/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -387,146 +387,122 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_groundstation.type_defs import (
     ComponentVersionTypeDef,
     AggregateStatusTypeDef,
     AntennaDemodDecodeDetailsTypeDef,
-    DecodeConfigOutputTypeDef,
-    DemodulationConfigOutputTypeDef,
     DecodeConfigTypeDef,
     DemodulationConfigTypeDef,
-    EirpOutputTypeDef,
     EirpTypeDef,
     CancelContactRequestRequestTypeDef,
     ComponentStatusDataTypeDef,
     S3RecordingDetailsTypeDef,
-    ConfigIdResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConfigListItemTypeDef,
-    DataflowEndpointConfigOutputTypeDef,
-    S3RecordingConfigOutputTypeDef,
-    TrackingConfigOutputTypeDef,
-    UplinkEchoConfigOutputTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
-    SocketAddressOutputTypeDef,
     SocketAddressTypeDef,
     ElevationTypeDef,
-    ContactIdResponseTypeDef,
     KmsKeyTypeDef,
-    DataflowEndpointGroupIdResponseTypeDef,
     DataflowEndpointListItemTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeContactRequestRequestTypeDef,
     DescribeEphemerisRequestRequestTypeDef,
     DiscoveryDataTypeDef,
     SecurityDetailsOutputTypeDef,
     SecurityDetailsTypeDef,
-    S3ObjectOutputTypeDef,
-    EphemerisIdResponseTypeDef,
+    S3ObjectTypeDef,
     EphemerisMetaDataTypeDef,
-    FrequencyBandwidthOutputTypeDef,
     FrequencyBandwidthTypeDef,
-    FrequencyOutputTypeDef,
     FrequencyTypeDef,
     GetAgentConfigurationRequestRequestTypeDef,
-    GetAgentConfigurationResponseTypeDef,
     GetConfigRequestRequestTypeDef,
     GetDataflowEndpointGroupRequestRequestTypeDef,
     GetMinuteUsageRequestRequestTypeDef,
-    GetMinuteUsageResponseTypeDef,
     GetMissionProfileRequestRequestTypeDef,
-    KmsKeyOutputTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
-    IntegerRangeOutputTypeDef,
     IntegerRangeTypeDef,
-    ListConfigsRequestListConfigsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListConfigsRequestRequestTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
-    ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
-    ListEphemeridesRequestListEphemeridesPaginateTypeDef,
     ListEphemeridesRequestRequestTypeDef,
-    ListGroundStationsRequestListGroundStationsPaginateTypeDef,
     ListGroundStationsRequestRequestTypeDef,
-    ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
     ListMissionProfilesRequestRequestTypeDef,
     MissionProfileListItemTypeDef,
-    ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MissionProfileIdResponseTypeDef,
-    S3ObjectTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterAgentResponseTypeDef,
     ReserveContactRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAgentStatusResponseTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
     AgentDetailsTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
+    ConfigIdResponseTypeDef,
+    ContactIdResponseTypeDef,
+    DataflowEndpointGroupIdResponseTypeDef,
+    EphemerisIdResponseTypeDef,
+    GetAgentConfigurationResponseTypeDef,
+    GetMinuteUsageResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MissionProfileIdResponseTypeDef,
+    RegisterAgentResponseTypeDef,
+    UpdateAgentStatusResponseTypeDef,
     ListConfigsResponseTypeDef,
-    ConnectionDetailsOutputTypeDef,
-    DataflowEndpointOutputTypeDef,
     ConnectionDetailsTypeDef,
     DataflowEndpointTypeDef,
     ContactDataTypeDef,
     CreateMissionProfileRequestRequestTypeDef,
+    GetMissionProfileResponseTypeDef,
     UpdateMissionProfileRequestRequestTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     DescribeContactRequestContactScheduledWaitTypeDef,
     EphemerisDescriptionTypeDef,
     EphemerisItemTypeDef,
+    OEMEphemerisTypeDef,
     GetSatelliteResponseTypeDef,
     SatelliteListItemTypeDef,
-    SpectrumConfigOutputTypeDef,
-    UplinkSpectrumConfigOutputTypeDef,
     SpectrumConfigTypeDef,
     UplinkSpectrumConfigTypeDef,
-    GetMissionProfileResponseTypeDef,
     ListGroundStationsResponseTypeDef,
-    RangedSocketAddressOutputTypeDef,
     RangedSocketAddressTypeDef,
+    ListConfigsRequestListConfigsPaginateTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
+    ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
+    ListEphemeridesRequestListEphemeridesPaginateTypeDef,
+    ListGroundStationsRequestListGroundStationsPaginateTypeDef,
+    ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
+    ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListMissionProfilesResponseTypeDef,
-    OEMEphemerisTypeDef,
     TLEDataTypeDef,
     RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
-    AntennaDownlinkConfigOutputTypeDef,
-    AntennaDownlinkDemodDecodeConfigOutputTypeDef,
-    AntennaUplinkConfigOutputTypeDef,
     AntennaDownlinkConfigTypeDef,
     AntennaDownlinkDemodDecodeConfigTypeDef,
     AntennaUplinkConfigTypeDef,
-    RangedConnectionDetailsOutputTypeDef,
     RangedConnectionDetailsTypeDef,
     TLEEphemerisTypeDef,
     DescribeEphemerisResponseTypeDef,
-    ConfigTypeDataOutputTypeDef,
     ConfigTypeDataTypeDef,
-    AwsGroundStationAgentEndpointOutputTypeDef,
     AwsGroundStationAgentEndpointTypeDef,
     EphemerisDataTypeDef,
-    GetConfigResponseTypeDef,
     CreateConfigRequestRequestTypeDef,
+    GetConfigResponseTypeDef,
     UpdateConfigRequestRequestTypeDef,
     EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     CreateEphemerisRequestRequestTypeDef,
     ConfigDetailsTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
     CreateDataflowEndpointGroupRequestRequestTypeDef,
```

### Comparing `mypy-boto3-groundstation-1.28.12/README.md` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-groundstation
+Version: 1.28.15
+Summary: Type annotations for boto3.GroundStation 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 groundstation type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-groundstation"></a>
 
 # mypy-boto3-groundstation
 
 [![PyPI - mypy-boto3-groundstation](https://img.shields.io/pypi/v/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-groundstation)](https://pepy.tech/project/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,146 +387,122 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_groundstation.type_defs import (
     ComponentVersionTypeDef,
     AggregateStatusTypeDef,
     AntennaDemodDecodeDetailsTypeDef,
-    DecodeConfigOutputTypeDef,
-    DemodulationConfigOutputTypeDef,
     DecodeConfigTypeDef,
     DemodulationConfigTypeDef,
-    EirpOutputTypeDef,
     EirpTypeDef,
     CancelContactRequestRequestTypeDef,
     ComponentStatusDataTypeDef,
     S3RecordingDetailsTypeDef,
-    ConfigIdResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConfigListItemTypeDef,
-    DataflowEndpointConfigOutputTypeDef,
-    S3RecordingConfigOutputTypeDef,
-    TrackingConfigOutputTypeDef,
-    UplinkEchoConfigOutputTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
-    SocketAddressOutputTypeDef,
     SocketAddressTypeDef,
     ElevationTypeDef,
-    ContactIdResponseTypeDef,
     KmsKeyTypeDef,
-    DataflowEndpointGroupIdResponseTypeDef,
     DataflowEndpointListItemTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeContactRequestRequestTypeDef,
     DescribeEphemerisRequestRequestTypeDef,
     DiscoveryDataTypeDef,
     SecurityDetailsOutputTypeDef,
     SecurityDetailsTypeDef,
-    S3ObjectOutputTypeDef,
-    EphemerisIdResponseTypeDef,
+    S3ObjectTypeDef,
     EphemerisMetaDataTypeDef,
-    FrequencyBandwidthOutputTypeDef,
     FrequencyBandwidthTypeDef,
-    FrequencyOutputTypeDef,
     FrequencyTypeDef,
     GetAgentConfigurationRequestRequestTypeDef,
-    GetAgentConfigurationResponseTypeDef,
     GetConfigRequestRequestTypeDef,
     GetDataflowEndpointGroupRequestRequestTypeDef,
     GetMinuteUsageRequestRequestTypeDef,
-    GetMinuteUsageResponseTypeDef,
     GetMissionProfileRequestRequestTypeDef,
-    KmsKeyOutputTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
-    IntegerRangeOutputTypeDef,
     IntegerRangeTypeDef,
-    ListConfigsRequestListConfigsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListConfigsRequestRequestTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
-    ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
-    ListEphemeridesRequestListEphemeridesPaginateTypeDef,
     ListEphemeridesRequestRequestTypeDef,
-    ListGroundStationsRequestListGroundStationsPaginateTypeDef,
     ListGroundStationsRequestRequestTypeDef,
-    ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
     ListMissionProfilesRequestRequestTypeDef,
     MissionProfileListItemTypeDef,
-    ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MissionProfileIdResponseTypeDef,
-    S3ObjectTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterAgentResponseTypeDef,
     ReserveContactRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAgentStatusResponseTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
     AgentDetailsTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
+    ConfigIdResponseTypeDef,
+    ContactIdResponseTypeDef,
+    DataflowEndpointGroupIdResponseTypeDef,
+    EphemerisIdResponseTypeDef,
+    GetAgentConfigurationResponseTypeDef,
+    GetMinuteUsageResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MissionProfileIdResponseTypeDef,
+    RegisterAgentResponseTypeDef,
+    UpdateAgentStatusResponseTypeDef,
     ListConfigsResponseTypeDef,
-    ConnectionDetailsOutputTypeDef,
-    DataflowEndpointOutputTypeDef,
     ConnectionDetailsTypeDef,
     DataflowEndpointTypeDef,
     ContactDataTypeDef,
     CreateMissionProfileRequestRequestTypeDef,
+    GetMissionProfileResponseTypeDef,
     UpdateMissionProfileRequestRequestTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     DescribeContactRequestContactScheduledWaitTypeDef,
     EphemerisDescriptionTypeDef,
     EphemerisItemTypeDef,
+    OEMEphemerisTypeDef,
     GetSatelliteResponseTypeDef,
     SatelliteListItemTypeDef,
-    SpectrumConfigOutputTypeDef,
-    UplinkSpectrumConfigOutputTypeDef,
     SpectrumConfigTypeDef,
     UplinkSpectrumConfigTypeDef,
-    GetMissionProfileResponseTypeDef,
     ListGroundStationsResponseTypeDef,
-    RangedSocketAddressOutputTypeDef,
     RangedSocketAddressTypeDef,
+    ListConfigsRequestListConfigsPaginateTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
+    ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
+    ListEphemeridesRequestListEphemeridesPaginateTypeDef,
+    ListGroundStationsRequestListGroundStationsPaginateTypeDef,
+    ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
+    ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListMissionProfilesResponseTypeDef,
-    OEMEphemerisTypeDef,
     TLEDataTypeDef,
     RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
-    AntennaDownlinkConfigOutputTypeDef,
-    AntennaDownlinkDemodDecodeConfigOutputTypeDef,
-    AntennaUplinkConfigOutputTypeDef,
     AntennaDownlinkConfigTypeDef,
     AntennaDownlinkDemodDecodeConfigTypeDef,
     AntennaUplinkConfigTypeDef,
-    RangedConnectionDetailsOutputTypeDef,
     RangedConnectionDetailsTypeDef,
     TLEEphemerisTypeDef,
     DescribeEphemerisResponseTypeDef,
-    ConfigTypeDataOutputTypeDef,
     ConfigTypeDataTypeDef,
-    AwsGroundStationAgentEndpointOutputTypeDef,
     AwsGroundStationAgentEndpointTypeDef,
     EphemerisDataTypeDef,
-    GetConfigResponseTypeDef,
     CreateConfigRequestRequestTypeDef,
+    GetConfigResponseTypeDef,
     UpdateConfigRequestRequestTypeDef,
     EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     CreateEphemerisRequestRequestTypeDef,
     ConfigDetailsTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
     CreateDataflowEndpointGroupRequestRequestTypeDef,
```

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/__init__.py` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/__init__.pyi` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/__main__.py` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GroundStation 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.GroundStation 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation\nOther"
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

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/client.py` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/client.pyi` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/literals.py` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/literals.pyi` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/paginator.py` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -54,40 +54,36 @@
     "ListDataflowEndpointGroupsPaginator",
     "ListEphemeridesPaginator",
     "ListGroundStationsPaginator",
     "ListMissionProfilesPaginator",
     "ListSatellitesPaginator",
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
 class ListConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listconfigspaginator)
         """
 
-
 class ListContactsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListContacts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listcontactspaginator)
     """
 
     def paginate(
@@ -95,94 +91,89 @@
         *,
         endTime: Union[datetime, str],
         startTime: Union[datetime, str],
         statusList: Sequence[ContactStatusType],
         groundStation: str = ...,
         missionProfileArn: str = ...,
         satelliteArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContactsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListContacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listcontactspaginator)
         """
 
-
 class ListDataflowEndpointGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListDataflowEndpointGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listdataflowendpointgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataflowEndpointGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListDataflowEndpointGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listdataflowendpointgroupspaginator)
         """
 
-
 class ListEphemeridesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListEphemerides)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listephemeridespaginator)
     """
 
     def paginate(
         self,
         *,
         endTime: Union[datetime, str],
         satelliteId: str,
         startTime: Union[datetime, str],
         statusList: Sequence[EphemerisStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEphemeridesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListEphemerides.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listephemeridespaginator)
         """
 
-
 class ListGroundStationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListGroundStations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listgroundstationspaginator)
     """
 
     def paginate(
-        self, *, satelliteId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, satelliteId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroundStationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListGroundStations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listgroundstationspaginator)
         """
 
-
 class ListMissionProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListMissionProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listmissionprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMissionProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListMissionProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listmissionprofilespaginator)
         """
 
-
 class ListSatellitesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListSatellites)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listsatellitespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSatellitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListSatellites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listsatellitespaginator)
         """
```

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/paginator.pyi` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/paginator.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,36 +54,40 @@
     "ListDataflowEndpointGroupsPaginator",
     "ListEphemeridesPaginator",
     "ListGroundStationsPaginator",
     "ListMissionProfilesPaginator",
     "ListSatellitesPaginator",
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
 class ListConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listconfigspaginator)
         """
 
+
 class ListContactsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListContacts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listcontactspaginator)
     """
 
     def paginate(
@@ -91,89 +95,94 @@
         *,
         endTime: Union[datetime, str],
         startTime: Union[datetime, str],
         statusList: Sequence[ContactStatusType],
         groundStation: str = ...,
         missionProfileArn: str = ...,
         satelliteArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContactsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListContacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listcontactspaginator)
         """
 
+
 class ListDataflowEndpointGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListDataflowEndpointGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listdataflowendpointgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataflowEndpointGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListDataflowEndpointGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listdataflowendpointgroupspaginator)
         """
 
+
 class ListEphemeridesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListEphemerides)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listephemeridespaginator)
     """
 
     def paginate(
         self,
         *,
         endTime: Union[datetime, str],
         satelliteId: str,
         startTime: Union[datetime, str],
         statusList: Sequence[EphemerisStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEphemeridesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListEphemerides.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listephemeridespaginator)
         """
 
+
 class ListGroundStationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListGroundStations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listgroundstationspaginator)
     """
 
     def paginate(
-        self, *, satelliteId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, satelliteId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroundStationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListGroundStations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listgroundstationspaginator)
         """
 
+
 class ListMissionProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListMissionProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listmissionprofilespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMissionProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListMissionProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listmissionprofilespaginator)
         """
 
+
 class ListSatellitesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListSatellites)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listsatellitespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSatellitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Paginator.ListSatellites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/paginators/#listsatellitespaginator)
         """
```

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/type_defs.py` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -38,151 +38,126 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ComponentVersionTypeDef",
     "AggregateStatusTypeDef",
     "AntennaDemodDecodeDetailsTypeDef",
-    "DecodeConfigOutputTypeDef",
-    "DemodulationConfigOutputTypeDef",
     "DecodeConfigTypeDef",
     "DemodulationConfigTypeDef",
-    "EirpOutputTypeDef",
     "EirpTypeDef",
     "CancelContactRequestRequestTypeDef",
     "ComponentStatusDataTypeDef",
     "S3RecordingDetailsTypeDef",
-    "ConfigIdResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ConfigListItemTypeDef",
-    "DataflowEndpointConfigOutputTypeDef",
-    "S3RecordingConfigOutputTypeDef",
-    "TrackingConfigOutputTypeDef",
-    "UplinkEchoConfigOutputTypeDef",
     "DataflowEndpointConfigTypeDef",
     "S3RecordingConfigTypeDef",
     "TrackingConfigTypeDef",
     "UplinkEchoConfigTypeDef",
-    "SocketAddressOutputTypeDef",
     "SocketAddressTypeDef",
     "ElevationTypeDef",
-    "ContactIdResponseTypeDef",
     "KmsKeyTypeDef",
-    "DataflowEndpointGroupIdResponseTypeDef",
     "DataflowEndpointListItemTypeDef",
     "DeleteConfigRequestRequestTypeDef",
     "DeleteDataflowEndpointGroupRequestRequestTypeDef",
     "DeleteEphemerisRequestRequestTypeDef",
     "DeleteMissionProfileRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeContactRequestRequestTypeDef",
     "DescribeEphemerisRequestRequestTypeDef",
     "DiscoveryDataTypeDef",
     "SecurityDetailsOutputTypeDef",
     "SecurityDetailsTypeDef",
-    "S3ObjectOutputTypeDef",
-    "EphemerisIdResponseTypeDef",
+    "S3ObjectTypeDef",
     "EphemerisMetaDataTypeDef",
-    "FrequencyBandwidthOutputTypeDef",
     "FrequencyBandwidthTypeDef",
-    "FrequencyOutputTypeDef",
     "FrequencyTypeDef",
     "GetAgentConfigurationRequestRequestTypeDef",
-    "GetAgentConfigurationResponseTypeDef",
     "GetConfigRequestRequestTypeDef",
     "GetDataflowEndpointGroupRequestRequestTypeDef",
     "GetMinuteUsageRequestRequestTypeDef",
-    "GetMinuteUsageResponseTypeDef",
     "GetMissionProfileRequestRequestTypeDef",
-    "KmsKeyOutputTypeDef",
     "GetSatelliteRequestRequestTypeDef",
     "GroundStationDataTypeDef",
-    "IntegerRangeOutputTypeDef",
     "IntegerRangeTypeDef",
-    "ListConfigsRequestListConfigsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListConfigsRequestRequestTypeDef",
-    "ListContactsRequestListContactsPaginateTypeDef",
     "ListContactsRequestRequestTypeDef",
-    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
-    "ListEphemeridesRequestListEphemeridesPaginateTypeDef",
     "ListEphemeridesRequestRequestTypeDef",
-    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
     "ListGroundStationsRequestRequestTypeDef",
-    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
     "ListMissionProfilesRequestRequestTypeDef",
     "MissionProfileListItemTypeDef",
-    "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListSatellitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "MissionProfileIdResponseTypeDef",
-    "S3ObjectTypeDef",
-    "PaginatorConfigTypeDef",
-    "RegisterAgentResponseTypeDef",
     "ReserveContactRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TimeRangeTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAgentStatusResponseTypeDef",
     "UpdateEphemerisRequestRequestTypeDef",
     "AgentDetailsTypeDef",
     "UpdateAgentStatusRequestRequestTypeDef",
+    "ConfigIdResponseTypeDef",
+    "ContactIdResponseTypeDef",
+    "DataflowEndpointGroupIdResponseTypeDef",
+    "EphemerisIdResponseTypeDef",
+    "GetAgentConfigurationResponseTypeDef",
+    "GetMinuteUsageResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "MissionProfileIdResponseTypeDef",
+    "RegisterAgentResponseTypeDef",
+    "UpdateAgentStatusResponseTypeDef",
     "ListConfigsResponseTypeDef",
-    "ConnectionDetailsOutputTypeDef",
-    "DataflowEndpointOutputTypeDef",
     "ConnectionDetailsTypeDef",
     "DataflowEndpointTypeDef",
     "ContactDataTypeDef",
     "CreateMissionProfileRequestRequestTypeDef",
+    "GetMissionProfileResponseTypeDef",
     "UpdateMissionProfileRequestRequestTypeDef",
     "ListDataflowEndpointGroupsResponseTypeDef",
     "DescribeContactRequestContactScheduledWaitTypeDef",
     "EphemerisDescriptionTypeDef",
     "EphemerisItemTypeDef",
+    "OEMEphemerisTypeDef",
     "GetSatelliteResponseTypeDef",
     "SatelliteListItemTypeDef",
-    "SpectrumConfigOutputTypeDef",
-    "UplinkSpectrumConfigOutputTypeDef",
     "SpectrumConfigTypeDef",
     "UplinkSpectrumConfigTypeDef",
-    "GetMissionProfileResponseTypeDef",
     "ListGroundStationsResponseTypeDef",
-    "RangedSocketAddressOutputTypeDef",
     "RangedSocketAddressTypeDef",
+    "ListConfigsRequestListConfigsPaginateTypeDef",
+    "ListContactsRequestListContactsPaginateTypeDef",
+    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
+    "ListEphemeridesRequestListEphemeridesPaginateTypeDef",
+    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
+    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
+    "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListMissionProfilesResponseTypeDef",
-    "OEMEphemerisTypeDef",
     "TLEDataTypeDef",
     "RegisterAgentRequestRequestTypeDef",
     "ListContactsResponseTypeDef",
     "EphemerisTypeDescriptionTypeDef",
     "ListEphemeridesResponseTypeDef",
     "ListSatellitesResponseTypeDef",
-    "AntennaDownlinkConfigOutputTypeDef",
-    "AntennaDownlinkDemodDecodeConfigOutputTypeDef",
-    "AntennaUplinkConfigOutputTypeDef",
     "AntennaDownlinkConfigTypeDef",
     "AntennaDownlinkDemodDecodeConfigTypeDef",
     "AntennaUplinkConfigTypeDef",
-    "RangedConnectionDetailsOutputTypeDef",
     "RangedConnectionDetailsTypeDef",
     "TLEEphemerisTypeDef",
     "DescribeEphemerisResponseTypeDef",
-    "ConfigTypeDataOutputTypeDef",
     "ConfigTypeDataTypeDef",
-    "AwsGroundStationAgentEndpointOutputTypeDef",
     "AwsGroundStationAgentEndpointTypeDef",
     "EphemerisDataTypeDef",
-    "GetConfigResponseTypeDef",
     "CreateConfigRequestRequestTypeDef",
+    "GetConfigResponseTypeDef",
     "UpdateConfigRequestRequestTypeDef",
     "EndpointDetailsOutputTypeDef",
     "EndpointDetailsTypeDef",
     "CreateEphemerisRequestRequestTypeDef",
     "ConfigDetailsTypeDef",
     "GetDataflowEndpointGroupResponseTypeDef",
     "CreateDataflowEndpointGroupRequestRequestTypeDef",
@@ -210,63 +185,39 @@
     "_OptionalAggregateStatusTypeDef",
     {
         "signatureMap": Mapping[str, bool],
     },
     total=False,
 )
 
-
 class AggregateStatusTypeDef(_RequiredAggregateStatusTypeDef, _OptionalAggregateStatusTypeDef):
     pass
 
-
 AntennaDemodDecodeDetailsTypeDef = TypedDict(
     "AntennaDemodDecodeDetailsTypeDef",
     {
         "outputNode": str,
     },
     total=False,
 )
 
-DecodeConfigOutputTypeDef = TypedDict(
-    "DecodeConfigOutputTypeDef",
-    {
-        "unvalidatedJSON": str,
-    },
-)
-
-DemodulationConfigOutputTypeDef = TypedDict(
-    "DemodulationConfigOutputTypeDef",
-    {
-        "unvalidatedJSON": str,
-    },
-)
-
 DecodeConfigTypeDef = TypedDict(
     "DecodeConfigTypeDef",
     {
         "unvalidatedJSON": str,
     },
 )
 
 DemodulationConfigTypeDef = TypedDict(
     "DemodulationConfigTypeDef",
     {
         "unvalidatedJSON": str,
     },
 )
 
-EirpOutputTypeDef = TypedDict(
-    "EirpOutputTypeDef",
-    {
-        "units": Literal["dBW"],
-        "value": float,
-    },
-)
-
 EirpTypeDef = TypedDict(
     "EirpTypeDef",
     {
         "units": Literal["dBW"],
         "value": float,
     },
 )
@@ -293,130 +244,69 @@
         "bytesReceived": int,
         "bytesSent": int,
         "packetsDropped": int,
     },
     total=False,
 )
 
-
 class ComponentStatusDataTypeDef(
     _RequiredComponentStatusDataTypeDef, _OptionalComponentStatusDataTypeDef
 ):
     pass
 
-
 S3RecordingDetailsTypeDef = TypedDict(
     "S3RecordingDetailsTypeDef",
     {
         "bucketArn": str,
         "keyTemplate": str,
     },
     total=False,
 )
 
-ConfigIdResponseTypeDef = TypedDict(
-    "ConfigIdResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "configArn": str,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ConfigListItemTypeDef = TypedDict(
     "ConfigListItemTypeDef",
     {
         "configArn": str,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
     },
     total=False,
 )
 
-_RequiredDataflowEndpointConfigOutputTypeDef = TypedDict(
-    "_RequiredDataflowEndpointConfigOutputTypeDef",
-    {
-        "dataflowEndpointName": str,
-    },
-)
-_OptionalDataflowEndpointConfigOutputTypeDef = TypedDict(
-    "_OptionalDataflowEndpointConfigOutputTypeDef",
-    {
-        "dataflowEndpointRegion": str,
-    },
-    total=False,
-)
-
-
-class DataflowEndpointConfigOutputTypeDef(
-    _RequiredDataflowEndpointConfigOutputTypeDef, _OptionalDataflowEndpointConfigOutputTypeDef
-):
-    pass
-
-
-_RequiredS3RecordingConfigOutputTypeDef = TypedDict(
-    "_RequiredS3RecordingConfigOutputTypeDef",
-    {
-        "bucketArn": str,
-        "roleArn": str,
-    },
-)
-_OptionalS3RecordingConfigOutputTypeDef = TypedDict(
-    "_OptionalS3RecordingConfigOutputTypeDef",
-    {
-        "prefix": str,
-    },
-    total=False,
-)
-
-
-class S3RecordingConfigOutputTypeDef(
-    _RequiredS3RecordingConfigOutputTypeDef, _OptionalS3RecordingConfigOutputTypeDef
-):
-    pass
-
-
-TrackingConfigOutputTypeDef = TypedDict(
-    "TrackingConfigOutputTypeDef",
-    {
-        "autotrack": CriticalityType,
-    },
-)
-
-UplinkEchoConfigOutputTypeDef = TypedDict(
-    "UplinkEchoConfigOutputTypeDef",
-    {
-        "antennaUplinkConfigArn": str,
-        "enabled": bool,
-    },
-)
-
 _RequiredDataflowEndpointConfigTypeDef = TypedDict(
     "_RequiredDataflowEndpointConfigTypeDef",
     {
         "dataflowEndpointName": str,
     },
 )
 _OptionalDataflowEndpointConfigTypeDef = TypedDict(
     "_OptionalDataflowEndpointConfigTypeDef",
     {
         "dataflowEndpointRegion": str,
     },
     total=False,
 )
 
-
 class DataflowEndpointConfigTypeDef(
     _RequiredDataflowEndpointConfigTypeDef, _OptionalDataflowEndpointConfigTypeDef
 ):
     pass
 
-
 _RequiredS3RecordingConfigTypeDef = TypedDict(
     "_RequiredS3RecordingConfigTypeDef",
     {
         "bucketArn": str,
         "roleArn": str,
     },
 )
@@ -424,21 +314,19 @@
     "_OptionalS3RecordingConfigTypeDef",
     {
         "prefix": str,
     },
     total=False,
 )
 
-
 class S3RecordingConfigTypeDef(
     _RequiredS3RecordingConfigTypeDef, _OptionalS3RecordingConfigTypeDef
 ):
     pass
 
-
 TrackingConfigTypeDef = TypedDict(
     "TrackingConfigTypeDef",
     {
         "autotrack": CriticalityType,
     },
 )
 
@@ -446,22 +334,14 @@
     "UplinkEchoConfigTypeDef",
     {
         "antennaUplinkConfigArn": str,
         "enabled": bool,
     },
 )
 
-SocketAddressOutputTypeDef = TypedDict(
-    "SocketAddressOutputTypeDef",
-    {
-        "name": str,
-        "port": int,
-    },
-)
-
 SocketAddressTypeDef = TypedDict(
     "SocketAddressTypeDef",
     {
         "name": str,
         "port": int,
     },
 )
@@ -470,39 +350,23 @@
     "ElevationTypeDef",
     {
         "unit": AngleUnitsType,
         "value": float,
     },
 )
 
-ContactIdResponseTypeDef = TypedDict(
-    "ContactIdResponseTypeDef",
-    {
-        "contactId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 KmsKeyTypeDef = TypedDict(
     "KmsKeyTypeDef",
     {
         "kmsAliasArn": str,
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-DataflowEndpointGroupIdResponseTypeDef = TypedDict(
-    "DataflowEndpointGroupIdResponseTypeDef",
-    {
-        "dataflowEndpointGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataflowEndpointListItemTypeDef = TypedDict(
     "DataflowEndpointListItemTypeDef",
     {
         "dataflowEndpointGroupArn": str,
         "dataflowEndpointGroupId": str,
     },
     total=False,
@@ -583,32 +447,24 @@
     {
         "roleArn": str,
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
     },
 )
 
-S3ObjectOutputTypeDef = TypedDict(
-    "S3ObjectOutputTypeDef",
+S3ObjectTypeDef = TypedDict(
+    "S3ObjectTypeDef",
     {
         "bucket": str,
         "key": str,
         "version": str,
     },
     total=False,
 )
 
-EphemerisIdResponseTypeDef = TypedDict(
-    "EphemerisIdResponseTypeDef",
-    {
-        "ephemerisId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEphemerisMetaDataTypeDef = TypedDict(
     "_RequiredEphemerisMetaDataTypeDef",
     {
         "source": EphemerisSourceType,
     },
 )
 _OptionalEphemerisMetaDataTypeDef = TypedDict(
@@ -617,45 +473,27 @@
         "ephemerisId": str,
         "epoch": datetime,
         "name": str,
     },
     total=False,
 )
 
-
 class EphemerisMetaDataTypeDef(
     _RequiredEphemerisMetaDataTypeDef, _OptionalEphemerisMetaDataTypeDef
 ):
     pass
 
-
-FrequencyBandwidthOutputTypeDef = TypedDict(
-    "FrequencyBandwidthOutputTypeDef",
-    {
-        "units": BandwidthUnitsType,
-        "value": float,
-    },
-)
-
 FrequencyBandwidthTypeDef = TypedDict(
     "FrequencyBandwidthTypeDef",
     {
         "units": BandwidthUnitsType,
         "value": float,
     },
 )
 
-FrequencyOutputTypeDef = TypedDict(
-    "FrequencyOutputTypeDef",
-    {
-        "units": FrequencyUnitsType,
-        "value": float,
-    },
-)
-
 FrequencyTypeDef = TypedDict(
     "FrequencyTypeDef",
     {
         "units": FrequencyUnitsType,
         "value": float,
     },
 )
@@ -663,23 +501,14 @@
 GetAgentConfigurationRequestRequestTypeDef = TypedDict(
     "GetAgentConfigurationRequestRequestTypeDef",
     {
         "agentId": str,
     },
 )
 
-GetAgentConfigurationResponseTypeDef = TypedDict(
-    "GetAgentConfigurationResponseTypeDef",
-    {
-        "agentId": str,
-        "taskingDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetConfigRequestRequestTypeDef = TypedDict(
     "GetConfigRequestRequestTypeDef",
     {
         "configId": str,
         "configType": ConfigCapabilityTypeType,
     },
 )
@@ -695,42 +524,21 @@
     "GetMinuteUsageRequestRequestTypeDef",
     {
         "month": int,
         "year": int,
     },
 )
 
-GetMinuteUsageResponseTypeDef = TypedDict(
-    "GetMinuteUsageResponseTypeDef",
-    {
-        "estimatedMinutesRemaining": int,
-        "isReservedMinutesCustomer": bool,
-        "totalReservedMinuteAllocation": int,
-        "totalScheduledMinutes": int,
-        "upcomingMinutesScheduled": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMissionProfileRequestRequestTypeDef = TypedDict(
     "GetMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
     },
 )
 
-KmsKeyOutputTypeDef = TypedDict(
-    "KmsKeyOutputTypeDef",
-    {
-        "kmsAliasArn": str,
-        "kmsKeyArn": str,
-    },
-    total=False,
-)
-
 GetSatelliteRequestRequestTypeDef = TypedDict(
     "GetSatelliteRequestRequestTypeDef",
     {
         "satelliteId": str,
     },
 )
 
@@ -740,74 +548,41 @@
         "groundStationId": str,
         "groundStationName": str,
         "region": str,
     },
     total=False,
 )
 
-IntegerRangeOutputTypeDef = TypedDict(
-    "IntegerRangeOutputTypeDef",
-    {
-        "maximum": int,
-        "minimum": int,
-    },
-)
-
 IntegerRangeTypeDef = TypedDict(
     "IntegerRangeTypeDef",
     {
         "maximum": int,
         "minimum": int,
     },
 )
 
-ListConfigsRequestListConfigsPaginateTypeDef = TypedDict(
-    "ListConfigsRequestListConfigsPaginateTypeDef",
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
 
 ListConfigsRequestRequestTypeDef = TypedDict(
     "ListConfigsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "_RequiredListContactsRequestListContactsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "startTime": Union[datetime, str],
-        "statusList": Sequence[ContactStatusType],
-    },
-)
-_OptionalListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "_OptionalListContactsRequestListContactsPaginateTypeDef",
-    {
-        "groundStation": str,
-        "missionProfileArn": str,
-        "satelliteArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListContactsRequestListContactsPaginateTypeDef(
-    _RequiredListContactsRequestListContactsPaginateTypeDef,
-    _OptionalListContactsRequestListContactsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListContactsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "startTime": Union[datetime, str],
         "statusList": Sequence[ContactStatusType],
     },
@@ -820,63 +595,28 @@
         "missionProfileArn": str,
         "nextToken": str,
         "satelliteArn": str,
     },
     total=False,
 )
 
-
 class ListContactsRequestRequestTypeDef(
     _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
 ):
     pass
 
-
-ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef = TypedDict(
-    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDataflowEndpointGroupsRequestRequestTypeDef = TypedDict(
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
-    "_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "satelliteId": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
-    "_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef",
-    {
-        "statusList": Sequence[EphemerisStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListEphemeridesRequestListEphemeridesPaginateTypeDef(
-    _RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef,
-    _OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEphemeridesRequestRequestTypeDef = TypedDict(
     "_RequiredListEphemeridesRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "satelliteId": str,
         "startTime": Union[datetime, str],
     },
@@ -887,48 +627,29 @@
         "maxResults": int,
         "nextToken": str,
         "statusList": Sequence[EphemerisStatusType],
     },
     total=False,
 )
 
-
 class ListEphemeridesRequestRequestTypeDef(
     _RequiredListEphemeridesRequestRequestTypeDef, _OptionalListEphemeridesRequestRequestTypeDef
 ):
     pass
 
-
-ListGroundStationsRequestListGroundStationsPaginateTypeDef = TypedDict(
-    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
-    {
-        "satelliteId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGroundStationsRequestRequestTypeDef = TypedDict(
     "ListGroundStationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "satelliteId": str,
     },
     total=False,
 )
 
-ListMissionProfilesRequestListMissionProfilesPaginateTypeDef = TypedDict(
-    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMissionProfilesRequestRequestTypeDef = TypedDict(
     "ListMissionProfilesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -941,22 +662,14 @@
         "missionProfileId": str,
         "name": str,
         "region": str,
     },
     total=False,
 )
 
-ListSatellitesRequestListSatellitesPaginateTypeDef = TypedDict(
-    "ListSatellitesRequestListSatellitesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSatellitesRequestRequestTypeDef = TypedDict(
     "ListSatellitesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -965,58 +678,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MissionProfileIdResponseTypeDef = TypedDict(
-    "MissionProfileIdResponseTypeDef",
-    {
-        "missionProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-S3ObjectTypeDef = TypedDict(
-    "S3ObjectTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-        "version": str,
-    },
-    total=False,
-)
-
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
-RegisterAgentResponseTypeDef = TypedDict(
-    "RegisterAgentResponseTypeDef",
-    {
-        "agentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredReserveContactRequestRequestTypeDef = TypedDict(
     "_RequiredReserveContactRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "groundStation": str,
         "missionProfileArn": str,
         "satelliteArn": str,
@@ -1027,32 +696,19 @@
     "_OptionalReserveContactRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ReserveContactRequestRequestTypeDef(
     _RequiredReserveContactRequestRequestTypeDef, _OptionalReserveContactRequestRequestTypeDef
 ):
     pass
 
-
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
 TimeRangeTypeDef = TypedDict(
     "TimeRangeTypeDef",
     {
         "endTime": Union[datetime, str],
         "startTime": Union[datetime, str],
     },
 )
@@ -1069,22 +725,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateAgentStatusResponseTypeDef = TypedDict(
-    "UpdateAgentStatusResponseTypeDef",
-    {
-        "agentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateEphemerisRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEphemerisRequestRequestTypeDef",
     {
         "enabled": bool,
         "ephemerisId": str,
     },
 )
@@ -1093,21 +741,19 @@
     {
         "name": str,
         "priority": int,
     },
     total=False,
 )
 
-
 class UpdateEphemerisRequestRequestTypeDef(
     _RequiredUpdateEphemerisRequestRequestTypeDef, _OptionalUpdateEphemerisRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredAgentDetailsTypeDef = TypedDict(
     "_RequiredAgentDetailsTypeDef",
     {
         "agentVersion": str,
         "componentVersions": Sequence[ComponentVersionTypeDef],
         "instanceId": str,
         "instanceType": str,
@@ -1118,68 +764,121 @@
     {
         "agentCpuCores": Sequence[int],
         "reservedCpuCores": Sequence[int],
     },
     total=False,
 )
 
-
 class AgentDetailsTypeDef(_RequiredAgentDetailsTypeDef, _OptionalAgentDetailsTypeDef):
     pass
 
-
 UpdateAgentStatusRequestRequestTypeDef = TypedDict(
     "UpdateAgentStatusRequestRequestTypeDef",
     {
         "agentId": str,
         "aggregateStatus": AggregateStatusTypeDef,
         "componentStatuses": Sequence[ComponentStatusDataTypeDef],
         "taskId": str,
     },
 )
 
-ListConfigsResponseTypeDef = TypedDict(
-    "ListConfigsResponseTypeDef",
+ConfigIdResponseTypeDef = TypedDict(
+    "ConfigIdResponseTypeDef",
     {
-        "configList": List[ConfigListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "configArn": str,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredConnectionDetailsOutputTypeDef = TypedDict(
-    "_RequiredConnectionDetailsOutputTypeDef",
+ContactIdResponseTypeDef = TypedDict(
+    "ContactIdResponseTypeDef",
     {
-        "socketAddress": SocketAddressOutputTypeDef,
+        "contactId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalConnectionDetailsOutputTypeDef = TypedDict(
-    "_OptionalConnectionDetailsOutputTypeDef",
+
+DataflowEndpointGroupIdResponseTypeDef = TypedDict(
+    "DataflowEndpointGroupIdResponseTypeDef",
     {
-        "mtu": int,
+        "dataflowEndpointGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+EphemerisIdResponseTypeDef = TypedDict(
+    "EphemerisIdResponseTypeDef",
+    {
+        "ephemerisId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ConnectionDetailsOutputTypeDef(
-    _RequiredConnectionDetailsOutputTypeDef, _OptionalConnectionDetailsOutputTypeDef
-):
-    pass
+GetAgentConfigurationResponseTypeDef = TypedDict(
+    "GetAgentConfigurationResponseTypeDef",
+    {
+        "agentId": str,
+        "taskingDocument": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetMinuteUsageResponseTypeDef = TypedDict(
+    "GetMinuteUsageResponseTypeDef",
+    {
+        "estimatedMinutesRemaining": int,
+        "isReservedMinutesCustomer": bool,
+        "totalReservedMinuteAllocation": int,
+        "totalScheduledMinutes": int,
+        "upcomingMinutesScheduled": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-DataflowEndpointOutputTypeDef = TypedDict(
-    "DataflowEndpointOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "address": SocketAddressOutputTypeDef,
-        "mtu": int,
-        "name": str,
-        "status": EndpointStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MissionProfileIdResponseTypeDef = TypedDict(
+    "MissionProfileIdResponseTypeDef",
+    {
+        "missionProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterAgentResponseTypeDef = TypedDict(
+    "RegisterAgentResponseTypeDef",
+    {
+        "agentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAgentStatusResponseTypeDef = TypedDict(
+    "UpdateAgentStatusResponseTypeDef",
+    {
+        "agentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigsResponseTypeDef = TypedDict(
+    "ListConfigsResponseTypeDef",
+    {
+        "configList": List[ConfigListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredConnectionDetailsTypeDef = TypedDict(
     "_RequiredConnectionDetailsTypeDef",
     {
         "socketAddress": SocketAddressTypeDef,
     },
@@ -1188,21 +887,19 @@
     "_OptionalConnectionDetailsTypeDef",
     {
         "mtu": int,
     },
     total=False,
 )
 
-
 class ConnectionDetailsTypeDef(
     _RequiredConnectionDetailsTypeDef, _OptionalConnectionDetailsTypeDef
 ):
     pass
 
-
 DataflowEndpointTypeDef = TypedDict(
     "DataflowEndpointTypeDef",
     {
         "address": SocketAddressTypeDef,
         "mtu": int,
         "name": str,
         "status": EndpointStatusType,
@@ -1247,21 +944,38 @@
         "streamsKmsKey": KmsKeyTypeDef,
         "streamsKmsRole": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateMissionProfileRequestRequestTypeDef(
     _RequiredCreateMissionProfileRequestRequestTypeDef,
     _OptionalCreateMissionProfileRequestRequestTypeDef,
 ):
     pass
 
+GetMissionProfileResponseTypeDef = TypedDict(
+    "GetMissionProfileResponseTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "dataflowEdges": List[List[str]],
+        "minimumViableContactDurationSeconds": int,
+        "missionProfileArn": str,
+        "missionProfileId": str,
+        "name": str,
+        "region": str,
+        "streamsKmsKey": KmsKeyTypeDef,
+        "streamsKmsRole": str,
+        "tags": Dict[str, str],
+        "trackingConfigArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredUpdateMissionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
     },
 )
@@ -1276,28 +990,26 @@
         "streamsKmsKey": KmsKeyTypeDef,
         "streamsKmsRole": str,
         "trackingConfigArn": str,
     },
     total=False,
 )
 
-
 class UpdateMissionProfileRequestRequestTypeDef(
     _RequiredUpdateMissionProfileRequestRequestTypeDef,
     _OptionalUpdateMissionProfileRequestRequestTypeDef,
 ):
     pass
 
-
 ListDataflowEndpointGroupsResponseTypeDef = TypedDict(
     "ListDataflowEndpointGroupsResponseTypeDef",
     {
         "dataflowEndpointGroupList": List[DataflowEndpointListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeContactRequestContactScheduledWaitTypeDef = TypedDict(
     "_RequiredDescribeContactRequestContactScheduledWaitTypeDef",
     {
         "contactId": str,
@@ -1307,54 +1019,61 @@
     "_OptionalDescribeContactRequestContactScheduledWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeContactRequestContactScheduledWaitTypeDef(
     _RequiredDescribeContactRequestContactScheduledWaitTypeDef,
     _OptionalDescribeContactRequestContactScheduledWaitTypeDef,
 ):
     pass
 
-
 EphemerisDescriptionTypeDef = TypedDict(
     "EphemerisDescriptionTypeDef",
     {
         "ephemerisData": str,
-        "sourceS3Object": S3ObjectOutputTypeDef,
+        "sourceS3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
 EphemerisItemTypeDef = TypedDict(
     "EphemerisItemTypeDef",
     {
         "creationTime": datetime,
         "enabled": bool,
         "ephemerisId": str,
         "name": str,
         "priority": int,
-        "sourceS3Object": S3ObjectOutputTypeDef,
+        "sourceS3Object": S3ObjectTypeDef,
         "status": EphemerisStatusType,
     },
     total=False,
 )
 
+OEMEphemerisTypeDef = TypedDict(
+    "OEMEphemerisTypeDef",
+    {
+        "oemData": str,
+        "s3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
 GetSatelliteResponseTypeDef = TypedDict(
     "GetSatelliteResponseTypeDef",
     {
         "currentEphemeris": EphemerisMetaDataTypeDef,
         "groundStations": List[str],
         "noradSatelliteID": int,
         "satelliteArn": str,
         "satelliteId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SatelliteListItemTypeDef = TypedDict(
     "SatelliteListItemTypeDef",
     {
         "currentEphemeris": EphemerisMetaDataTypeDef,
@@ -1362,160 +1081,166 @@
         "noradSatelliteID": int,
         "satelliteArn": str,
         "satelliteId": str,
     },
     total=False,
 )
 
-_RequiredSpectrumConfigOutputTypeDef = TypedDict(
-    "_RequiredSpectrumConfigOutputTypeDef",
+_RequiredSpectrumConfigTypeDef = TypedDict(
+    "_RequiredSpectrumConfigTypeDef",
     {
-        "bandwidth": FrequencyBandwidthOutputTypeDef,
-        "centerFrequency": FrequencyOutputTypeDef,
+        "bandwidth": FrequencyBandwidthTypeDef,
+        "centerFrequency": FrequencyTypeDef,
     },
 )
-_OptionalSpectrumConfigOutputTypeDef = TypedDict(
-    "_OptionalSpectrumConfigOutputTypeDef",
+_OptionalSpectrumConfigTypeDef = TypedDict(
+    "_OptionalSpectrumConfigTypeDef",
     {
         "polarization": PolarizationType,
     },
     total=False,
 )
 
-
-class SpectrumConfigOutputTypeDef(
-    _RequiredSpectrumConfigOutputTypeDef, _OptionalSpectrumConfigOutputTypeDef
-):
+class SpectrumConfigTypeDef(_RequiredSpectrumConfigTypeDef, _OptionalSpectrumConfigTypeDef):
     pass
 
-
-_RequiredUplinkSpectrumConfigOutputTypeDef = TypedDict(
-    "_RequiredUplinkSpectrumConfigOutputTypeDef",
+_RequiredUplinkSpectrumConfigTypeDef = TypedDict(
+    "_RequiredUplinkSpectrumConfigTypeDef",
     {
-        "centerFrequency": FrequencyOutputTypeDef,
+        "centerFrequency": FrequencyTypeDef,
     },
 )
-_OptionalUplinkSpectrumConfigOutputTypeDef = TypedDict(
-    "_OptionalUplinkSpectrumConfigOutputTypeDef",
+_OptionalUplinkSpectrumConfigTypeDef = TypedDict(
+    "_OptionalUplinkSpectrumConfigTypeDef",
     {
         "polarization": PolarizationType,
     },
     total=False,
 )
 
-
-class UplinkSpectrumConfigOutputTypeDef(
-    _RequiredUplinkSpectrumConfigOutputTypeDef, _OptionalUplinkSpectrumConfigOutputTypeDef
+class UplinkSpectrumConfigTypeDef(
+    _RequiredUplinkSpectrumConfigTypeDef, _OptionalUplinkSpectrumConfigTypeDef
 ):
     pass
 
+ListGroundStationsResponseTypeDef = TypedDict(
+    "ListGroundStationsResponseTypeDef",
+    {
+        "groundStationList": List[GroundStationDataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredSpectrumConfigTypeDef = TypedDict(
-    "_RequiredSpectrumConfigTypeDef",
+RangedSocketAddressTypeDef = TypedDict(
+    "RangedSocketAddressTypeDef",
     {
-        "bandwidth": FrequencyBandwidthTypeDef,
-        "centerFrequency": FrequencyTypeDef,
+        "name": str,
+        "portRange": IntegerRangeTypeDef,
     },
 )
-_OptionalSpectrumConfigTypeDef = TypedDict(
-    "_OptionalSpectrumConfigTypeDef",
+
+ListConfigsRequestListConfigsPaginateTypeDef = TypedDict(
+    "ListConfigsRequestListConfigsPaginateTypeDef",
     {
-        "polarization": PolarizationType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class SpectrumConfigTypeDef(_RequiredSpectrumConfigTypeDef, _OptionalSpectrumConfigTypeDef):
-    pass
-
-
-_RequiredUplinkSpectrumConfigTypeDef = TypedDict(
-    "_RequiredUplinkSpectrumConfigTypeDef",
+_RequiredListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "_RequiredListContactsRequestListContactsPaginateTypeDef",
     {
-        "centerFrequency": FrequencyTypeDef,
+        "endTime": Union[datetime, str],
+        "startTime": Union[datetime, str],
+        "statusList": Sequence[ContactStatusType],
     },
 )
-_OptionalUplinkSpectrumConfigTypeDef = TypedDict(
-    "_OptionalUplinkSpectrumConfigTypeDef",
+_OptionalListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "_OptionalListContactsRequestListContactsPaginateTypeDef",
     {
-        "polarization": PolarizationType,
+        "groundStation": str,
+        "missionProfileArn": str,
+        "satelliteArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class UplinkSpectrumConfigTypeDef(
-    _RequiredUplinkSpectrumConfigTypeDef, _OptionalUplinkSpectrumConfigTypeDef
+class ListContactsRequestListContactsPaginateTypeDef(
+    _RequiredListContactsRequestListContactsPaginateTypeDef,
+    _OptionalListContactsRequestListContactsPaginateTypeDef,
 ):
     pass
 
+ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef = TypedDict(
+    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-GetMissionProfileResponseTypeDef = TypedDict(
-    "GetMissionProfileResponseTypeDef",
+_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
+    "_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef",
     {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "dataflowEdges": List[List[str]],
-        "minimumViableContactDurationSeconds": int,
-        "missionProfileArn": str,
-        "missionProfileId": str,
-        "name": str,
-        "region": str,
-        "streamsKmsKey": KmsKeyOutputTypeDef,
-        "streamsKmsRole": str,
-        "tags": Dict[str, str],
-        "trackingConfigArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "endTime": Union[datetime, str],
+        "satelliteId": str,
+        "startTime": Union[datetime, str],
+    },
+)
+_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
+    "_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef",
+    {
+        "statusList": Sequence[EphemerisStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListGroundStationsResponseTypeDef = TypedDict(
-    "ListGroundStationsResponseTypeDef",
+class ListEphemeridesRequestListEphemeridesPaginateTypeDef(
+    _RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef,
+    _OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef,
+):
+    pass
+
+ListGroundStationsRequestListGroundStationsPaginateTypeDef = TypedDict(
+    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
     {
-        "groundStationList": List[GroundStationDataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "satelliteId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-RangedSocketAddressOutputTypeDef = TypedDict(
-    "RangedSocketAddressOutputTypeDef",
+ListMissionProfilesRequestListMissionProfilesPaginateTypeDef = TypedDict(
+    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
     {
-        "name": str,
-        "portRange": IntegerRangeOutputTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-RangedSocketAddressTypeDef = TypedDict(
-    "RangedSocketAddressTypeDef",
+ListSatellitesRequestListSatellitesPaginateTypeDef = TypedDict(
+    "ListSatellitesRequestListSatellitesPaginateTypeDef",
     {
-        "name": str,
-        "portRange": IntegerRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListMissionProfilesResponseTypeDef = TypedDict(
     "ListMissionProfilesResponseTypeDef",
     {
         "missionProfileList": List[MissionProfileListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OEMEphemerisTypeDef = TypedDict(
-    "OEMEphemerisTypeDef",
-    {
-        "oemData": str,
-        "s3Object": S3ObjectTypeDef,
-    },
-    total=False,
-)
-
 TLEDataTypeDef = TypedDict(
     "TLEDataTypeDef",
     {
         "tleLine1": str,
         "tleLine2": str,
         "validTimeRange": TimeRangeTypeDef,
     },
@@ -1530,15 +1255,15 @@
 )
 
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "contactList": List[ContactDataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EphemerisTypeDescriptionTypeDef = TypedDict(
     "EphemerisTypeDescriptionTypeDef",
     {
         "oem": EphemerisDescriptionTypeDef,
@@ -1548,64 +1273,26 @@
 )
 
 ListEphemeridesResponseTypeDef = TypedDict(
     "ListEphemeridesResponseTypeDef",
     {
         "ephemerides": List[EphemerisItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSatellitesResponseTypeDef = TypedDict(
     "ListSatellitesResponseTypeDef",
     {
         "nextToken": str,
         "satellites": List[SatelliteListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AntennaDownlinkConfigOutputTypeDef = TypedDict(
-    "AntennaDownlinkConfigOutputTypeDef",
-    {
-        "spectrumConfig": SpectrumConfigOutputTypeDef,
-    },
-)
-
-AntennaDownlinkDemodDecodeConfigOutputTypeDef = TypedDict(
-    "AntennaDownlinkDemodDecodeConfigOutputTypeDef",
-    {
-        "decodeConfig": DecodeConfigOutputTypeDef,
-        "demodulationConfig": DemodulationConfigOutputTypeDef,
-        "spectrumConfig": SpectrumConfigOutputTypeDef,
-    },
-)
-
-_RequiredAntennaUplinkConfigOutputTypeDef = TypedDict(
-    "_RequiredAntennaUplinkConfigOutputTypeDef",
-    {
-        "spectrumConfig": UplinkSpectrumConfigOutputTypeDef,
-        "targetEirp": EirpOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAntennaUplinkConfigOutputTypeDef = TypedDict(
-    "_OptionalAntennaUplinkConfigOutputTypeDef",
-    {
-        "transmitDisabled": bool,
-    },
-    total=False,
-)
-
-
-class AntennaUplinkConfigOutputTypeDef(
-    _RequiredAntennaUplinkConfigOutputTypeDef, _OptionalAntennaUplinkConfigOutputTypeDef
-):
-    pass
-
 
 AntennaDownlinkConfigTypeDef = TypedDict(
     "AntennaDownlinkConfigTypeDef",
     {
         "spectrumConfig": SpectrumConfigTypeDef,
     },
 )
@@ -1630,63 +1317,38 @@
     "_OptionalAntennaUplinkConfigTypeDef",
     {
         "transmitDisabled": bool,
     },
     total=False,
 )
 
-
 class AntennaUplinkConfigTypeDef(
     _RequiredAntennaUplinkConfigTypeDef, _OptionalAntennaUplinkConfigTypeDef
 ):
     pass
 
-
-_RequiredRangedConnectionDetailsOutputTypeDef = TypedDict(
-    "_RequiredRangedConnectionDetailsOutputTypeDef",
-    {
-        "socketAddress": RangedSocketAddressOutputTypeDef,
-    },
-)
-_OptionalRangedConnectionDetailsOutputTypeDef = TypedDict(
-    "_OptionalRangedConnectionDetailsOutputTypeDef",
-    {
-        "mtu": int,
-    },
-    total=False,
-)
-
-
-class RangedConnectionDetailsOutputTypeDef(
-    _RequiredRangedConnectionDetailsOutputTypeDef, _OptionalRangedConnectionDetailsOutputTypeDef
-):
-    pass
-
-
 _RequiredRangedConnectionDetailsTypeDef = TypedDict(
     "_RequiredRangedConnectionDetailsTypeDef",
     {
         "socketAddress": RangedSocketAddressTypeDef,
     },
 )
 _OptionalRangedConnectionDetailsTypeDef = TypedDict(
     "_OptionalRangedConnectionDetailsTypeDef",
     {
         "mtu": int,
     },
     total=False,
 )
 
-
 class RangedConnectionDetailsTypeDef(
     _RequiredRangedConnectionDetailsTypeDef, _OptionalRangedConnectionDetailsTypeDef
 ):
     pass
 
-
 TLEEphemerisTypeDef = TypedDict(
     "TLEEphemerisTypeDef",
     {
         "s3Object": S3ObjectTypeDef,
         "tleData": Sequence[TLEDataTypeDef],
     },
     total=False,
@@ -1701,30 +1363,16 @@
         "invalidReason": EphemerisInvalidReasonType,
         "name": str,
         "priority": int,
         "satelliteId": str,
         "status": EphemerisStatusType,
         "suppliedData": EphemerisTypeDescriptionTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ConfigTypeDataOutputTypeDef = TypedDict(
-    "ConfigTypeDataOutputTypeDef",
-    {
-        "antennaDownlinkConfig": AntennaDownlinkConfigOutputTypeDef,
-        "antennaDownlinkDemodDecodeConfig": AntennaDownlinkDemodDecodeConfigOutputTypeDef,
-        "antennaUplinkConfig": AntennaUplinkConfigOutputTypeDef,
-        "dataflowEndpointConfig": DataflowEndpointConfigOutputTypeDef,
-        "s3RecordingConfig": S3RecordingConfigOutputTypeDef,
-        "trackingConfig": TrackingConfigOutputTypeDef,
-        "uplinkEchoConfig": UplinkEchoConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ConfigTypeDataTypeDef = TypedDict(
     "ConfigTypeDataTypeDef",
     {
         "antennaDownlinkConfig": AntennaDownlinkConfigTypeDef,
         "antennaDownlinkDemodDecodeConfig": AntennaDownlinkDemodDecodeConfigTypeDef,
@@ -1733,39 +1381,14 @@
         "s3RecordingConfig": S3RecordingConfigTypeDef,
         "trackingConfig": TrackingConfigTypeDef,
         "uplinkEchoConfig": UplinkEchoConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredAwsGroundStationAgentEndpointOutputTypeDef = TypedDict(
-    "_RequiredAwsGroundStationAgentEndpointOutputTypeDef",
-    {
-        "egressAddress": ConnectionDetailsOutputTypeDef,
-        "ingressAddress": RangedConnectionDetailsOutputTypeDef,
-        "name": str,
-    },
-)
-_OptionalAwsGroundStationAgentEndpointOutputTypeDef = TypedDict(
-    "_OptionalAwsGroundStationAgentEndpointOutputTypeDef",
-    {
-        "agentStatus": AgentStatusType,
-        "auditResults": AuditResultsType,
-    },
-    total=False,
-)
-
-
-class AwsGroundStationAgentEndpointOutputTypeDef(
-    _RequiredAwsGroundStationAgentEndpointOutputTypeDef,
-    _OptionalAwsGroundStationAgentEndpointOutputTypeDef,
-):
-    pass
-
-
 _RequiredAwsGroundStationAgentEndpointTypeDef = TypedDict(
     "_RequiredAwsGroundStationAgentEndpointTypeDef",
     {
         "egressAddress": ConnectionDetailsTypeDef,
         "ingressAddress": RangedConnectionDetailsTypeDef,
         "name": str,
     },
@@ -1775,43 +1398,28 @@
     {
         "agentStatus": AgentStatusType,
         "auditResults": AuditResultsType,
     },
     total=False,
 )
 
-
 class AwsGroundStationAgentEndpointTypeDef(
     _RequiredAwsGroundStationAgentEndpointTypeDef, _OptionalAwsGroundStationAgentEndpointTypeDef
 ):
     pass
 
-
 EphemerisDataTypeDef = TypedDict(
     "EphemerisDataTypeDef",
     {
         "oem": OEMEphemerisTypeDef,
         "tle": TLEEphemerisTypeDef,
     },
     total=False,
 )
 
-GetConfigResponseTypeDef = TypedDict(
-    "GetConfigResponseTypeDef",
-    {
-        "configArn": str,
-        "configData": ConfigTypeDataOutputTypeDef,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigRequestRequestTypeDef",
     {
         "configData": ConfigTypeDataTypeDef,
         "name": str,
     },
 )
@@ -1819,36 +1427,47 @@
     "_OptionalCreateConfigRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateConfigRequestRequestTypeDef(
     _RequiredCreateConfigRequestRequestTypeDef, _OptionalCreateConfigRequestRequestTypeDef
 ):
     pass
 
+GetConfigResponseTypeDef = TypedDict(
+    "GetConfigResponseTypeDef",
+    {
+        "configArn": str,
+        "configData": ConfigTypeDataTypeDef,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 UpdateConfigRequestRequestTypeDef = TypedDict(
     "UpdateConfigRequestRequestTypeDef",
     {
         "configData": ConfigTypeDataTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
     },
 )
 
 EndpointDetailsOutputTypeDef = TypedDict(
     "EndpointDetailsOutputTypeDef",
     {
-        "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointOutputTypeDef,
-        "endpoint": DataflowEndpointOutputTypeDef,
+        "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointTypeDef,
+        "endpoint": DataflowEndpointTypeDef,
         "healthReasons": List[CapabilityHealthReasonType],
         "healthStatus": CapabilityHealthType,
         "securityDetails": SecurityDetailsOutputTypeDef,
     },
     total=False,
 )
 
@@ -1880,21 +1499,19 @@
         "kmsKeyArn": str,
         "priority": int,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateEphemerisRequestRequestTypeDef(
     _RequiredCreateEphemerisRequestRequestTypeDef, _OptionalCreateEphemerisRequestRequestTypeDef
 ):
     pass
 
-
 ConfigDetailsTypeDef = TypedDict(
     "ConfigDetailsTypeDef",
     {
         "antennaDemodDecodeDetails": AntennaDemodDecodeDetailsTypeDef,
         "endpointDetails": EndpointDetailsOutputTypeDef,
         "s3RecordingDetails": S3RecordingDetailsTypeDef,
     },
@@ -1906,15 +1523,15 @@
     {
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
         "dataflowEndpointGroupArn": str,
         "dataflowEndpointGroupId": str,
         "endpointsDetails": List[EndpointDetailsOutputTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
     {
         "endpointDetails": Sequence[EndpointDetailsTypeDef],
@@ -1926,22 +1543,20 @@
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateDataflowEndpointGroupRequestRequestTypeDef(
     _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
     _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
 ):
     pass
 
-
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "configDetails": ConfigDetailsTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "dataflowDestinationRegion": str,
@@ -1983,10 +1598,10 @@
         "missionProfileArn": str,
         "postPassEndTime": datetime,
         "prePassStartTime": datetime,
         "region": str,
         "satelliteArn": str,
         "startTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/type_defs.pyi` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,150 +38,127 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ComponentVersionTypeDef",
     "AggregateStatusTypeDef",
     "AntennaDemodDecodeDetailsTypeDef",
-    "DecodeConfigOutputTypeDef",
-    "DemodulationConfigOutputTypeDef",
     "DecodeConfigTypeDef",
     "DemodulationConfigTypeDef",
-    "EirpOutputTypeDef",
     "EirpTypeDef",
     "CancelContactRequestRequestTypeDef",
     "ComponentStatusDataTypeDef",
     "S3RecordingDetailsTypeDef",
-    "ConfigIdResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ConfigListItemTypeDef",
-    "DataflowEndpointConfigOutputTypeDef",
-    "S3RecordingConfigOutputTypeDef",
-    "TrackingConfigOutputTypeDef",
-    "UplinkEchoConfigOutputTypeDef",
     "DataflowEndpointConfigTypeDef",
     "S3RecordingConfigTypeDef",
     "TrackingConfigTypeDef",
     "UplinkEchoConfigTypeDef",
-    "SocketAddressOutputTypeDef",
     "SocketAddressTypeDef",
     "ElevationTypeDef",
-    "ContactIdResponseTypeDef",
     "KmsKeyTypeDef",
-    "DataflowEndpointGroupIdResponseTypeDef",
     "DataflowEndpointListItemTypeDef",
     "DeleteConfigRequestRequestTypeDef",
     "DeleteDataflowEndpointGroupRequestRequestTypeDef",
     "DeleteEphemerisRequestRequestTypeDef",
     "DeleteMissionProfileRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeContactRequestRequestTypeDef",
     "DescribeEphemerisRequestRequestTypeDef",
     "DiscoveryDataTypeDef",
     "SecurityDetailsOutputTypeDef",
     "SecurityDetailsTypeDef",
-    "S3ObjectOutputTypeDef",
-    "EphemerisIdResponseTypeDef",
+    "S3ObjectTypeDef",
     "EphemerisMetaDataTypeDef",
-    "FrequencyBandwidthOutputTypeDef",
     "FrequencyBandwidthTypeDef",
-    "FrequencyOutputTypeDef",
     "FrequencyTypeDef",
     "GetAgentConfigurationRequestRequestTypeDef",
-    "GetAgentConfigurationResponseTypeDef",
     "GetConfigRequestRequestTypeDef",
     "GetDataflowEndpointGroupRequestRequestTypeDef",
     "GetMinuteUsageRequestRequestTypeDef",
-    "GetMinuteUsageResponseTypeDef",
     "GetMissionProfileRequestRequestTypeDef",
-    "KmsKeyOutputTypeDef",
     "GetSatelliteRequestRequestTypeDef",
     "GroundStationDataTypeDef",
-    "IntegerRangeOutputTypeDef",
     "IntegerRangeTypeDef",
-    "ListConfigsRequestListConfigsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListConfigsRequestRequestTypeDef",
-    "ListContactsRequestListContactsPaginateTypeDef",
     "ListContactsRequestRequestTypeDef",
-    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
-    "ListEphemeridesRequestListEphemeridesPaginateTypeDef",
     "ListEphemeridesRequestRequestTypeDef",
-    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
     "ListGroundStationsRequestRequestTypeDef",
-    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
     "ListMissionProfilesRequestRequestTypeDef",
     "MissionProfileListItemTypeDef",
-    "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListSatellitesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "MissionProfileIdResponseTypeDef",
-    "S3ObjectTypeDef",
-    "PaginatorConfigTypeDef",
-    "RegisterAgentResponseTypeDef",
     "ReserveContactRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TimeRangeTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAgentStatusResponseTypeDef",
     "UpdateEphemerisRequestRequestTypeDef",
     "AgentDetailsTypeDef",
     "UpdateAgentStatusRequestRequestTypeDef",
+    "ConfigIdResponseTypeDef",
+    "ContactIdResponseTypeDef",
+    "DataflowEndpointGroupIdResponseTypeDef",
+    "EphemerisIdResponseTypeDef",
+    "GetAgentConfigurationResponseTypeDef",
+    "GetMinuteUsageResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "MissionProfileIdResponseTypeDef",
+    "RegisterAgentResponseTypeDef",
+    "UpdateAgentStatusResponseTypeDef",
     "ListConfigsResponseTypeDef",
-    "ConnectionDetailsOutputTypeDef",
-    "DataflowEndpointOutputTypeDef",
     "ConnectionDetailsTypeDef",
     "DataflowEndpointTypeDef",
     "ContactDataTypeDef",
     "CreateMissionProfileRequestRequestTypeDef",
+    "GetMissionProfileResponseTypeDef",
     "UpdateMissionProfileRequestRequestTypeDef",
     "ListDataflowEndpointGroupsResponseTypeDef",
     "DescribeContactRequestContactScheduledWaitTypeDef",
     "EphemerisDescriptionTypeDef",
     "EphemerisItemTypeDef",
+    "OEMEphemerisTypeDef",
     "GetSatelliteResponseTypeDef",
     "SatelliteListItemTypeDef",
-    "SpectrumConfigOutputTypeDef",
-    "UplinkSpectrumConfigOutputTypeDef",
     "SpectrumConfigTypeDef",
     "UplinkSpectrumConfigTypeDef",
-    "GetMissionProfileResponseTypeDef",
     "ListGroundStationsResponseTypeDef",
-    "RangedSocketAddressOutputTypeDef",
     "RangedSocketAddressTypeDef",
+    "ListConfigsRequestListConfigsPaginateTypeDef",
+    "ListContactsRequestListContactsPaginateTypeDef",
+    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
+    "ListEphemeridesRequestListEphemeridesPaginateTypeDef",
+    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
+    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
+    "ListSatellitesRequestListSatellitesPaginateTypeDef",
     "ListMissionProfilesResponseTypeDef",
-    "OEMEphemerisTypeDef",
     "TLEDataTypeDef",
     "RegisterAgentRequestRequestTypeDef",
     "ListContactsResponseTypeDef",
     "EphemerisTypeDescriptionTypeDef",
     "ListEphemeridesResponseTypeDef",
     "ListSatellitesResponseTypeDef",
-    "AntennaDownlinkConfigOutputTypeDef",
-    "AntennaDownlinkDemodDecodeConfigOutputTypeDef",
-    "AntennaUplinkConfigOutputTypeDef",
     "AntennaDownlinkConfigTypeDef",
     "AntennaDownlinkDemodDecodeConfigTypeDef",
     "AntennaUplinkConfigTypeDef",
-    "RangedConnectionDetailsOutputTypeDef",
     "RangedConnectionDetailsTypeDef",
     "TLEEphemerisTypeDef",
     "DescribeEphemerisResponseTypeDef",
-    "ConfigTypeDataOutputTypeDef",
     "ConfigTypeDataTypeDef",
-    "AwsGroundStationAgentEndpointOutputTypeDef",
     "AwsGroundStationAgentEndpointTypeDef",
     "EphemerisDataTypeDef",
-    "GetConfigResponseTypeDef",
     "CreateConfigRequestRequestTypeDef",
+    "GetConfigResponseTypeDef",
     "UpdateConfigRequestRequestTypeDef",
     "EndpointDetailsOutputTypeDef",
     "EndpointDetailsTypeDef",
     "CreateEphemerisRequestRequestTypeDef",
     "ConfigDetailsTypeDef",
     "GetDataflowEndpointGroupResponseTypeDef",
     "CreateDataflowEndpointGroupRequestRequestTypeDef",
@@ -209,61 +186,41 @@
     "_OptionalAggregateStatusTypeDef",
     {
         "signatureMap": Mapping[str, bool],
     },
     total=False,
 )
 
+
 class AggregateStatusTypeDef(_RequiredAggregateStatusTypeDef, _OptionalAggregateStatusTypeDef):
     pass
 
+
 AntennaDemodDecodeDetailsTypeDef = TypedDict(
     "AntennaDemodDecodeDetailsTypeDef",
     {
         "outputNode": str,
     },
     total=False,
 )
 
-DecodeConfigOutputTypeDef = TypedDict(
-    "DecodeConfigOutputTypeDef",
-    {
-        "unvalidatedJSON": str,
-    },
-)
-
-DemodulationConfigOutputTypeDef = TypedDict(
-    "DemodulationConfigOutputTypeDef",
-    {
-        "unvalidatedJSON": str,
-    },
-)
-
 DecodeConfigTypeDef = TypedDict(
     "DecodeConfigTypeDef",
     {
         "unvalidatedJSON": str,
     },
 )
 
 DemodulationConfigTypeDef = TypedDict(
     "DemodulationConfigTypeDef",
     {
         "unvalidatedJSON": str,
     },
 )
 
-EirpOutputTypeDef = TypedDict(
-    "EirpOutputTypeDef",
-    {
-        "units": Literal["dBW"],
-        "value": float,
-    },
-)
-
 EirpTypeDef = TypedDict(
     "EirpTypeDef",
     {
         "units": Literal["dBW"],
         "value": float,
     },
 )
@@ -290,122 +247,73 @@
         "bytesReceived": int,
         "bytesSent": int,
         "packetsDropped": int,
     },
     total=False,
 )
 
+
 class ComponentStatusDataTypeDef(
     _RequiredComponentStatusDataTypeDef, _OptionalComponentStatusDataTypeDef
 ):
     pass
 
+
 S3RecordingDetailsTypeDef = TypedDict(
     "S3RecordingDetailsTypeDef",
     {
         "bucketArn": str,
         "keyTemplate": str,
     },
     total=False,
 )
 
-ConfigIdResponseTypeDef = TypedDict(
-    "ConfigIdResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "configArn": str,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ConfigListItemTypeDef = TypedDict(
     "ConfigListItemTypeDef",
     {
         "configArn": str,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
     },
     total=False,
 )
 
-_RequiredDataflowEndpointConfigOutputTypeDef = TypedDict(
-    "_RequiredDataflowEndpointConfigOutputTypeDef",
-    {
-        "dataflowEndpointName": str,
-    },
-)
-_OptionalDataflowEndpointConfigOutputTypeDef = TypedDict(
-    "_OptionalDataflowEndpointConfigOutputTypeDef",
-    {
-        "dataflowEndpointRegion": str,
-    },
-    total=False,
-)
-
-class DataflowEndpointConfigOutputTypeDef(
-    _RequiredDataflowEndpointConfigOutputTypeDef, _OptionalDataflowEndpointConfigOutputTypeDef
-):
-    pass
-
-_RequiredS3RecordingConfigOutputTypeDef = TypedDict(
-    "_RequiredS3RecordingConfigOutputTypeDef",
-    {
-        "bucketArn": str,
-        "roleArn": str,
-    },
-)
-_OptionalS3RecordingConfigOutputTypeDef = TypedDict(
-    "_OptionalS3RecordingConfigOutputTypeDef",
-    {
-        "prefix": str,
-    },
-    total=False,
-)
-
-class S3RecordingConfigOutputTypeDef(
-    _RequiredS3RecordingConfigOutputTypeDef, _OptionalS3RecordingConfigOutputTypeDef
-):
-    pass
-
-TrackingConfigOutputTypeDef = TypedDict(
-    "TrackingConfigOutputTypeDef",
-    {
-        "autotrack": CriticalityType,
-    },
-)
-
-UplinkEchoConfigOutputTypeDef = TypedDict(
-    "UplinkEchoConfigOutputTypeDef",
-    {
-        "antennaUplinkConfigArn": str,
-        "enabled": bool,
-    },
-)
-
 _RequiredDataflowEndpointConfigTypeDef = TypedDict(
     "_RequiredDataflowEndpointConfigTypeDef",
     {
         "dataflowEndpointName": str,
     },
 )
 _OptionalDataflowEndpointConfigTypeDef = TypedDict(
     "_OptionalDataflowEndpointConfigTypeDef",
     {
         "dataflowEndpointRegion": str,
     },
     total=False,
 )
 
+
 class DataflowEndpointConfigTypeDef(
     _RequiredDataflowEndpointConfigTypeDef, _OptionalDataflowEndpointConfigTypeDef
 ):
     pass
 
+
 _RequiredS3RecordingConfigTypeDef = TypedDict(
     "_RequiredS3RecordingConfigTypeDef",
     {
         "bucketArn": str,
         "roleArn": str,
     },
 )
@@ -413,19 +321,21 @@
     "_OptionalS3RecordingConfigTypeDef",
     {
         "prefix": str,
     },
     total=False,
 )
 
+
 class S3RecordingConfigTypeDef(
     _RequiredS3RecordingConfigTypeDef, _OptionalS3RecordingConfigTypeDef
 ):
     pass
 
+
 TrackingConfigTypeDef = TypedDict(
     "TrackingConfigTypeDef",
     {
         "autotrack": CriticalityType,
     },
 )
 
@@ -433,22 +343,14 @@
     "UplinkEchoConfigTypeDef",
     {
         "antennaUplinkConfigArn": str,
         "enabled": bool,
     },
 )
 
-SocketAddressOutputTypeDef = TypedDict(
-    "SocketAddressOutputTypeDef",
-    {
-        "name": str,
-        "port": int,
-    },
-)
-
 SocketAddressTypeDef = TypedDict(
     "SocketAddressTypeDef",
     {
         "name": str,
         "port": int,
     },
 )
@@ -457,39 +359,23 @@
     "ElevationTypeDef",
     {
         "unit": AngleUnitsType,
         "value": float,
     },
 )
 
-ContactIdResponseTypeDef = TypedDict(
-    "ContactIdResponseTypeDef",
-    {
-        "contactId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 KmsKeyTypeDef = TypedDict(
     "KmsKeyTypeDef",
     {
         "kmsAliasArn": str,
         "kmsKeyArn": str,
     },
     total=False,
 )
 
-DataflowEndpointGroupIdResponseTypeDef = TypedDict(
-    "DataflowEndpointGroupIdResponseTypeDef",
-    {
-        "dataflowEndpointGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataflowEndpointListItemTypeDef = TypedDict(
     "DataflowEndpointListItemTypeDef",
     {
         "dataflowEndpointGroupArn": str,
         "dataflowEndpointGroupId": str,
     },
     total=False,
@@ -570,32 +456,24 @@
     {
         "roleArn": str,
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
     },
 )
 
-S3ObjectOutputTypeDef = TypedDict(
-    "S3ObjectOutputTypeDef",
+S3ObjectTypeDef = TypedDict(
+    "S3ObjectTypeDef",
     {
         "bucket": str,
         "key": str,
         "version": str,
     },
     total=False,
 )
 
-EphemerisIdResponseTypeDef = TypedDict(
-    "EphemerisIdResponseTypeDef",
-    {
-        "ephemerisId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEphemerisMetaDataTypeDef = TypedDict(
     "_RequiredEphemerisMetaDataTypeDef",
     {
         "source": EphemerisSourceType,
     },
 )
 _OptionalEphemerisMetaDataTypeDef = TypedDict(
@@ -604,43 +482,29 @@
         "ephemerisId": str,
         "epoch": datetime,
         "name": str,
     },
     total=False,
 )
 
+
 class EphemerisMetaDataTypeDef(
     _RequiredEphemerisMetaDataTypeDef, _OptionalEphemerisMetaDataTypeDef
 ):
     pass
 
-FrequencyBandwidthOutputTypeDef = TypedDict(
-    "FrequencyBandwidthOutputTypeDef",
-    {
-        "units": BandwidthUnitsType,
-        "value": float,
-    },
-)
 
 FrequencyBandwidthTypeDef = TypedDict(
     "FrequencyBandwidthTypeDef",
     {
         "units": BandwidthUnitsType,
         "value": float,
     },
 )
 
-FrequencyOutputTypeDef = TypedDict(
-    "FrequencyOutputTypeDef",
-    {
-        "units": FrequencyUnitsType,
-        "value": float,
-    },
-)
-
 FrequencyTypeDef = TypedDict(
     "FrequencyTypeDef",
     {
         "units": FrequencyUnitsType,
         "value": float,
     },
 )
@@ -648,23 +512,14 @@
 GetAgentConfigurationRequestRequestTypeDef = TypedDict(
     "GetAgentConfigurationRequestRequestTypeDef",
     {
         "agentId": str,
     },
 )
 
-GetAgentConfigurationResponseTypeDef = TypedDict(
-    "GetAgentConfigurationResponseTypeDef",
-    {
-        "agentId": str,
-        "taskingDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetConfigRequestRequestTypeDef = TypedDict(
     "GetConfigRequestRequestTypeDef",
     {
         "configId": str,
         "configType": ConfigCapabilityTypeType,
     },
 )
@@ -680,42 +535,21 @@
     "GetMinuteUsageRequestRequestTypeDef",
     {
         "month": int,
         "year": int,
     },
 )
 
-GetMinuteUsageResponseTypeDef = TypedDict(
-    "GetMinuteUsageResponseTypeDef",
-    {
-        "estimatedMinutesRemaining": int,
-        "isReservedMinutesCustomer": bool,
-        "totalReservedMinuteAllocation": int,
-        "totalScheduledMinutes": int,
-        "upcomingMinutesScheduled": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMissionProfileRequestRequestTypeDef = TypedDict(
     "GetMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
     },
 )
 
-KmsKeyOutputTypeDef = TypedDict(
-    "KmsKeyOutputTypeDef",
-    {
-        "kmsAliasArn": str,
-        "kmsKeyArn": str,
-    },
-    total=False,
-)
-
 GetSatelliteRequestRequestTypeDef = TypedDict(
     "GetSatelliteRequestRequestTypeDef",
     {
         "satelliteId": str,
     },
 )
 
@@ -725,72 +559,41 @@
         "groundStationId": str,
         "groundStationName": str,
         "region": str,
     },
     total=False,
 )
 
-IntegerRangeOutputTypeDef = TypedDict(
-    "IntegerRangeOutputTypeDef",
-    {
-        "maximum": int,
-        "minimum": int,
-    },
-)
-
 IntegerRangeTypeDef = TypedDict(
     "IntegerRangeTypeDef",
     {
         "maximum": int,
         "minimum": int,
     },
 )
 
-ListConfigsRequestListConfigsPaginateTypeDef = TypedDict(
-    "ListConfigsRequestListConfigsPaginateTypeDef",
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
 
 ListConfigsRequestRequestTypeDef = TypedDict(
     "ListConfigsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "_RequiredListContactsRequestListContactsPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "startTime": Union[datetime, str],
-        "statusList": Sequence[ContactStatusType],
-    },
-)
-_OptionalListContactsRequestListContactsPaginateTypeDef = TypedDict(
-    "_OptionalListContactsRequestListContactsPaginateTypeDef",
-    {
-        "groundStation": str,
-        "missionProfileArn": str,
-        "satelliteArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListContactsRequestListContactsPaginateTypeDef(
-    _RequiredListContactsRequestListContactsPaginateTypeDef,
-    _OptionalListContactsRequestListContactsPaginateTypeDef,
-):
-    pass
-
 _RequiredListContactsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactsRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "startTime": Union[datetime, str],
         "statusList": Sequence[ContactStatusType],
     },
@@ -803,59 +606,30 @@
         "missionProfileArn": str,
         "nextToken": str,
         "satelliteArn": str,
     },
     total=False,
 )
 
+
 class ListContactsRequestRequestTypeDef(
     _RequiredListContactsRequestRequestTypeDef, _OptionalListContactsRequestRequestTypeDef
 ):
     pass
 
-ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef = TypedDict(
-    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListDataflowEndpointGroupsRequestRequestTypeDef = TypedDict(
     "ListDataflowEndpointGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
-    "_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "satelliteId": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
-    "_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef",
-    {
-        "statusList": Sequence[EphemerisStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListEphemeridesRequestListEphemeridesPaginateTypeDef(
-    _RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef,
-    _OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef,
-):
-    pass
-
 _RequiredListEphemeridesRequestRequestTypeDef = TypedDict(
     "_RequiredListEphemeridesRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "satelliteId": str,
         "startTime": Union[datetime, str],
     },
@@ -866,46 +640,31 @@
         "maxResults": int,
         "nextToken": str,
         "statusList": Sequence[EphemerisStatusType],
     },
     total=False,
 )
 
+
 class ListEphemeridesRequestRequestTypeDef(
     _RequiredListEphemeridesRequestRequestTypeDef, _OptionalListEphemeridesRequestRequestTypeDef
 ):
     pass
 
-ListGroundStationsRequestListGroundStationsPaginateTypeDef = TypedDict(
-    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
-    {
-        "satelliteId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListGroundStationsRequestRequestTypeDef = TypedDict(
     "ListGroundStationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "satelliteId": str,
     },
     total=False,
 )
 
-ListMissionProfilesRequestListMissionProfilesPaginateTypeDef = TypedDict(
-    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMissionProfilesRequestRequestTypeDef = TypedDict(
     "ListMissionProfilesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -918,22 +677,14 @@
         "missionProfileId": str,
         "name": str,
         "region": str,
     },
     total=False,
 )
 
-ListSatellitesRequestListSatellitesPaginateTypeDef = TypedDict(
-    "ListSatellitesRequestListSatellitesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSatellitesRequestRequestTypeDef = TypedDict(
     "ListSatellitesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -942,58 +693,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MissionProfileIdResponseTypeDef = TypedDict(
-    "MissionProfileIdResponseTypeDef",
-    {
-        "missionProfileId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-S3ObjectTypeDef = TypedDict(
-    "S3ObjectTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-        "version": str,
-    },
-    total=False,
-)
-
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
-RegisterAgentResponseTypeDef = TypedDict(
-    "RegisterAgentResponseTypeDef",
-    {
-        "agentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredReserveContactRequestRequestTypeDef = TypedDict(
     "_RequiredReserveContactRequestRequestTypeDef",
     {
         "endTime": Union[datetime, str],
         "groundStation": str,
         "missionProfileArn": str,
         "satelliteArn": str,
@@ -1004,29 +711,20 @@
     "_OptionalReserveContactRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ReserveContactRequestRequestTypeDef(
     _RequiredReserveContactRequestRequestTypeDef, _OptionalReserveContactRequestRequestTypeDef
 ):
     pass
 
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
 
 TimeRangeTypeDef = TypedDict(
     "TimeRangeTypeDef",
     {
         "endTime": Union[datetime, str],
         "startTime": Union[datetime, str],
     },
@@ -1044,22 +742,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateAgentStatusResponseTypeDef = TypedDict(
-    "UpdateAgentStatusResponseTypeDef",
-    {
-        "agentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateEphemerisRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEphemerisRequestRequestTypeDef",
     {
         "enabled": bool,
         "ephemerisId": str,
     },
 )
@@ -1068,19 +758,21 @@
     {
         "name": str,
         "priority": int,
     },
     total=False,
 )
 
+
 class UpdateEphemerisRequestRequestTypeDef(
     _RequiredUpdateEphemerisRequestRequestTypeDef, _OptionalUpdateEphemerisRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredAgentDetailsTypeDef = TypedDict(
     "_RequiredAgentDetailsTypeDef",
     {
         "agentVersion": str,
         "componentVersions": Sequence[ComponentVersionTypeDef],
         "instanceId": str,
         "instanceType": str,
@@ -1091,64 +783,123 @@
     {
         "agentCpuCores": Sequence[int],
         "reservedCpuCores": Sequence[int],
     },
     total=False,
 )
 
+
 class AgentDetailsTypeDef(_RequiredAgentDetailsTypeDef, _OptionalAgentDetailsTypeDef):
     pass
 
+
 UpdateAgentStatusRequestRequestTypeDef = TypedDict(
     "UpdateAgentStatusRequestRequestTypeDef",
     {
         "agentId": str,
         "aggregateStatus": AggregateStatusTypeDef,
         "componentStatuses": Sequence[ComponentStatusDataTypeDef],
         "taskId": str,
     },
 )
 
-ListConfigsResponseTypeDef = TypedDict(
-    "ListConfigsResponseTypeDef",
+ConfigIdResponseTypeDef = TypedDict(
+    "ConfigIdResponseTypeDef",
     {
-        "configList": List[ConfigListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "configArn": str,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredConnectionDetailsOutputTypeDef = TypedDict(
-    "_RequiredConnectionDetailsOutputTypeDef",
+ContactIdResponseTypeDef = TypedDict(
+    "ContactIdResponseTypeDef",
     {
-        "socketAddress": SocketAddressOutputTypeDef,
+        "contactId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalConnectionDetailsOutputTypeDef = TypedDict(
-    "_OptionalConnectionDetailsOutputTypeDef",
+
+DataflowEndpointGroupIdResponseTypeDef = TypedDict(
+    "DataflowEndpointGroupIdResponseTypeDef",
     {
-        "mtu": int,
+        "dataflowEndpointGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ConnectionDetailsOutputTypeDef(
-    _RequiredConnectionDetailsOutputTypeDef, _OptionalConnectionDetailsOutputTypeDef
-):
-    pass
+EphemerisIdResponseTypeDef = TypedDict(
+    "EphemerisIdResponseTypeDef",
+    {
+        "ephemerisId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-DataflowEndpointOutputTypeDef = TypedDict(
-    "DataflowEndpointOutputTypeDef",
+GetAgentConfigurationResponseTypeDef = TypedDict(
+    "GetAgentConfigurationResponseTypeDef",
     {
-        "address": SocketAddressOutputTypeDef,
-        "mtu": int,
-        "name": str,
-        "status": EndpointStatusType,
+        "agentId": str,
+        "taskingDocument": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMinuteUsageResponseTypeDef = TypedDict(
+    "GetMinuteUsageResponseTypeDef",
+    {
+        "estimatedMinutesRemaining": int,
+        "isReservedMinutesCustomer": bool,
+        "totalReservedMinuteAllocation": int,
+        "totalScheduledMinutes": int,
+        "upcomingMinutesScheduled": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MissionProfileIdResponseTypeDef = TypedDict(
+    "MissionProfileIdResponseTypeDef",
+    {
+        "missionProfileId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterAgentResponseTypeDef = TypedDict(
+    "RegisterAgentResponseTypeDef",
+    {
+        "agentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAgentStatusResponseTypeDef = TypedDict(
+    "UpdateAgentStatusResponseTypeDef",
+    {
+        "agentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigsResponseTypeDef = TypedDict(
+    "ListConfigsResponseTypeDef",
+    {
+        "configList": List[ConfigListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredConnectionDetailsTypeDef = TypedDict(
     "_RequiredConnectionDetailsTypeDef",
     {
         "socketAddress": SocketAddressTypeDef,
     },
@@ -1157,19 +908,21 @@
     "_OptionalConnectionDetailsTypeDef",
     {
         "mtu": int,
     },
     total=False,
 )
 
+
 class ConnectionDetailsTypeDef(
     _RequiredConnectionDetailsTypeDef, _OptionalConnectionDetailsTypeDef
 ):
     pass
 
+
 DataflowEndpointTypeDef = TypedDict(
     "DataflowEndpointTypeDef",
     {
         "address": SocketAddressTypeDef,
         "mtu": int,
         "name": str,
         "status": EndpointStatusType,
@@ -1214,20 +967,41 @@
         "streamsKmsKey": KmsKeyTypeDef,
         "streamsKmsRole": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateMissionProfileRequestRequestTypeDef(
     _RequiredCreateMissionProfileRequestRequestTypeDef,
     _OptionalCreateMissionProfileRequestRequestTypeDef,
 ):
     pass
 
+
+GetMissionProfileResponseTypeDef = TypedDict(
+    "GetMissionProfileResponseTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "dataflowEdges": List[List[str]],
+        "minimumViableContactDurationSeconds": int,
+        "missionProfileArn": str,
+        "missionProfileId": str,
+        "name": str,
+        "region": str,
+        "streamsKmsKey": KmsKeyTypeDef,
+        "streamsKmsRole": str,
+        "tags": Dict[str, str],
+        "trackingConfigArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateMissionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMissionProfileRequestRequestTypeDef",
     {
         "missionProfileId": str,
     },
 )
 _OptionalUpdateMissionProfileRequestRequestTypeDef = TypedDict(
@@ -1241,26 +1015,28 @@
         "streamsKmsKey": KmsKeyTypeDef,
         "streamsKmsRole": str,
         "trackingConfigArn": str,
     },
     total=False,
 )
 
+
 class UpdateMissionProfileRequestRequestTypeDef(
     _RequiredUpdateMissionProfileRequestRequestTypeDef,
     _OptionalUpdateMissionProfileRequestRequestTypeDef,
 ):
     pass
 
+
 ListDataflowEndpointGroupsResponseTypeDef = TypedDict(
     "ListDataflowEndpointGroupsResponseTypeDef",
     {
         "dataflowEndpointGroupList": List[DataflowEndpointListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeContactRequestContactScheduledWaitTypeDef = TypedDict(
     "_RequiredDescribeContactRequestContactScheduledWaitTypeDef",
     {
         "contactId": str,
@@ -1270,52 +1046,63 @@
     "_OptionalDescribeContactRequestContactScheduledWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeContactRequestContactScheduledWaitTypeDef(
     _RequiredDescribeContactRequestContactScheduledWaitTypeDef,
     _OptionalDescribeContactRequestContactScheduledWaitTypeDef,
 ):
     pass
 
+
 EphemerisDescriptionTypeDef = TypedDict(
     "EphemerisDescriptionTypeDef",
     {
         "ephemerisData": str,
-        "sourceS3Object": S3ObjectOutputTypeDef,
+        "sourceS3Object": S3ObjectTypeDef,
     },
     total=False,
 )
 
 EphemerisItemTypeDef = TypedDict(
     "EphemerisItemTypeDef",
     {
         "creationTime": datetime,
         "enabled": bool,
         "ephemerisId": str,
         "name": str,
         "priority": int,
-        "sourceS3Object": S3ObjectOutputTypeDef,
+        "sourceS3Object": S3ObjectTypeDef,
         "status": EphemerisStatusType,
     },
     total=False,
 )
 
+OEMEphemerisTypeDef = TypedDict(
+    "OEMEphemerisTypeDef",
+    {
+        "oemData": str,
+        "s3Object": S3ObjectTypeDef,
+    },
+    total=False,
+)
+
 GetSatelliteResponseTypeDef = TypedDict(
     "GetSatelliteResponseTypeDef",
     {
         "currentEphemeris": EphemerisMetaDataTypeDef,
         "groundStations": List[str],
         "noradSatelliteID": int,
         "satelliteArn": str,
         "satelliteId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SatelliteListItemTypeDef = TypedDict(
     "SatelliteListItemTypeDef",
     {
         "currentEphemeris": EphemerisMetaDataTypeDef,
@@ -1323,152 +1110,174 @@
         "noradSatelliteID": int,
         "satelliteArn": str,
         "satelliteId": str,
     },
     total=False,
 )
 
-_RequiredSpectrumConfigOutputTypeDef = TypedDict(
-    "_RequiredSpectrumConfigOutputTypeDef",
+_RequiredSpectrumConfigTypeDef = TypedDict(
+    "_RequiredSpectrumConfigTypeDef",
     {
-        "bandwidth": FrequencyBandwidthOutputTypeDef,
-        "centerFrequency": FrequencyOutputTypeDef,
+        "bandwidth": FrequencyBandwidthTypeDef,
+        "centerFrequency": FrequencyTypeDef,
     },
 )
-_OptionalSpectrumConfigOutputTypeDef = TypedDict(
-    "_OptionalSpectrumConfigOutputTypeDef",
+_OptionalSpectrumConfigTypeDef = TypedDict(
+    "_OptionalSpectrumConfigTypeDef",
     {
         "polarization": PolarizationType,
     },
     total=False,
 )
 
-class SpectrumConfigOutputTypeDef(
-    _RequiredSpectrumConfigOutputTypeDef, _OptionalSpectrumConfigOutputTypeDef
-):
+
+class SpectrumConfigTypeDef(_RequiredSpectrumConfigTypeDef, _OptionalSpectrumConfigTypeDef):
     pass
 
-_RequiredUplinkSpectrumConfigOutputTypeDef = TypedDict(
-    "_RequiredUplinkSpectrumConfigOutputTypeDef",
+
+_RequiredUplinkSpectrumConfigTypeDef = TypedDict(
+    "_RequiredUplinkSpectrumConfigTypeDef",
     {
-        "centerFrequency": FrequencyOutputTypeDef,
+        "centerFrequency": FrequencyTypeDef,
     },
 )
-_OptionalUplinkSpectrumConfigOutputTypeDef = TypedDict(
-    "_OptionalUplinkSpectrumConfigOutputTypeDef",
+_OptionalUplinkSpectrumConfigTypeDef = TypedDict(
+    "_OptionalUplinkSpectrumConfigTypeDef",
     {
         "polarization": PolarizationType,
     },
     total=False,
 )
 
-class UplinkSpectrumConfigOutputTypeDef(
-    _RequiredUplinkSpectrumConfigOutputTypeDef, _OptionalUplinkSpectrumConfigOutputTypeDef
+
+class UplinkSpectrumConfigTypeDef(
+    _RequiredUplinkSpectrumConfigTypeDef, _OptionalUplinkSpectrumConfigTypeDef
 ):
     pass
 
-_RequiredSpectrumConfigTypeDef = TypedDict(
-    "_RequiredSpectrumConfigTypeDef",
+
+ListGroundStationsResponseTypeDef = TypedDict(
+    "ListGroundStationsResponseTypeDef",
     {
-        "bandwidth": FrequencyBandwidthTypeDef,
-        "centerFrequency": FrequencyTypeDef,
+        "groundStationList": List[GroundStationDataTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalSpectrumConfigTypeDef = TypedDict(
-    "_OptionalSpectrumConfigTypeDef",
+
+RangedSocketAddressTypeDef = TypedDict(
+    "RangedSocketAddressTypeDef",
     {
-        "polarization": PolarizationType,
+        "name": str,
+        "portRange": IntegerRangeTypeDef,
     },
-    total=False,
 )
 
-class SpectrumConfigTypeDef(_RequiredSpectrumConfigTypeDef, _OptionalSpectrumConfigTypeDef):
-    pass
+ListConfigsRequestListConfigsPaginateTypeDef = TypedDict(
+    "ListConfigsRequestListConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-_RequiredUplinkSpectrumConfigTypeDef = TypedDict(
-    "_RequiredUplinkSpectrumConfigTypeDef",
+_RequiredListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "_RequiredListContactsRequestListContactsPaginateTypeDef",
     {
-        "centerFrequency": FrequencyTypeDef,
+        "endTime": Union[datetime, str],
+        "startTime": Union[datetime, str],
+        "statusList": Sequence[ContactStatusType],
     },
 )
-_OptionalUplinkSpectrumConfigTypeDef = TypedDict(
-    "_OptionalUplinkSpectrumConfigTypeDef",
+_OptionalListContactsRequestListContactsPaginateTypeDef = TypedDict(
+    "_OptionalListContactsRequestListContactsPaginateTypeDef",
     {
-        "polarization": PolarizationType,
+        "groundStation": str,
+        "missionProfileArn": str,
+        "satelliteArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class UplinkSpectrumConfigTypeDef(
-    _RequiredUplinkSpectrumConfigTypeDef, _OptionalUplinkSpectrumConfigTypeDef
+
+class ListContactsRequestListContactsPaginateTypeDef(
+    _RequiredListContactsRequestListContactsPaginateTypeDef,
+    _OptionalListContactsRequestListContactsPaginateTypeDef,
 ):
     pass
 
-GetMissionProfileResponseTypeDef = TypedDict(
-    "GetMissionProfileResponseTypeDef",
+
+ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef = TypedDict(
+    "ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef",
     {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "dataflowEdges": List[List[str]],
-        "minimumViableContactDurationSeconds": int,
-        "missionProfileArn": str,
-        "missionProfileId": str,
-        "name": str,
-        "region": str,
-        "streamsKmsKey": KmsKeyOutputTypeDef,
-        "streamsKmsRole": str,
-        "tags": Dict[str, str],
-        "trackingConfigArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListGroundStationsResponseTypeDef = TypedDict(
-    "ListGroundStationsResponseTypeDef",
+_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
+    "_RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef",
     {
-        "groundStationList": List[GroundStationDataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "endTime": Union[datetime, str],
+        "satelliteId": str,
+        "startTime": Union[datetime, str],
     },
 )
-
-RangedSocketAddressOutputTypeDef = TypedDict(
-    "RangedSocketAddressOutputTypeDef",
+_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef = TypedDict(
+    "_OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef",
     {
-        "name": str,
-        "portRange": IntegerRangeOutputTypeDef,
+        "statusList": Sequence[EphemerisStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-RangedSocketAddressTypeDef = TypedDict(
-    "RangedSocketAddressTypeDef",
+
+class ListEphemeridesRequestListEphemeridesPaginateTypeDef(
+    _RequiredListEphemeridesRequestListEphemeridesPaginateTypeDef,
+    _OptionalListEphemeridesRequestListEphemeridesPaginateTypeDef,
+):
+    pass
+
+
+ListGroundStationsRequestListGroundStationsPaginateTypeDef = TypedDict(
+    "ListGroundStationsRequestListGroundStationsPaginateTypeDef",
     {
-        "name": str,
-        "portRange": IntegerRangeTypeDef,
+        "satelliteId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListMissionProfilesResponseTypeDef = TypedDict(
-    "ListMissionProfilesResponseTypeDef",
+ListMissionProfilesRequestListMissionProfilesPaginateTypeDef = TypedDict(
+    "ListMissionProfilesRequestListMissionProfilesPaginateTypeDef",
     {
-        "missionProfileList": List[MissionProfileListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-OEMEphemerisTypeDef = TypedDict(
-    "OEMEphemerisTypeDef",
+ListSatellitesRequestListSatellitesPaginateTypeDef = TypedDict(
+    "ListSatellitesRequestListSatellitesPaginateTypeDef",
     {
-        "oemData": str,
-        "s3Object": S3ObjectTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListMissionProfilesResponseTypeDef = TypedDict(
+    "ListMissionProfilesResponseTypeDef",
+    {
+        "missionProfileList": List[MissionProfileListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TLEDataTypeDef = TypedDict(
     "TLEDataTypeDef",
     {
         "tleLine1": str,
         "tleLine2": str,
         "validTimeRange": TimeRangeTypeDef,
     },
@@ -1483,15 +1292,15 @@
 )
 
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "contactList": List[ContactDataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EphemerisTypeDescriptionTypeDef = TypedDict(
     "EphemerisTypeDescriptionTypeDef",
     {
         "oem": EphemerisDescriptionTypeDef,
@@ -1501,63 +1310,27 @@
 )
 
 ListEphemeridesResponseTypeDef = TypedDict(
     "ListEphemeridesResponseTypeDef",
     {
         "ephemerides": List[EphemerisItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSatellitesResponseTypeDef = TypedDict(
     "ListSatellitesResponseTypeDef",
     {
         "nextToken": str,
         "satellites": List[SatelliteListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AntennaDownlinkConfigOutputTypeDef = TypedDict(
-    "AntennaDownlinkConfigOutputTypeDef",
-    {
-        "spectrumConfig": SpectrumConfigOutputTypeDef,
-    },
-)
-
-AntennaDownlinkDemodDecodeConfigOutputTypeDef = TypedDict(
-    "AntennaDownlinkDemodDecodeConfigOutputTypeDef",
-    {
-        "decodeConfig": DecodeConfigOutputTypeDef,
-        "demodulationConfig": DemodulationConfigOutputTypeDef,
-        "spectrumConfig": SpectrumConfigOutputTypeDef,
-    },
-)
-
-_RequiredAntennaUplinkConfigOutputTypeDef = TypedDict(
-    "_RequiredAntennaUplinkConfigOutputTypeDef",
-    {
-        "spectrumConfig": UplinkSpectrumConfigOutputTypeDef,
-        "targetEirp": EirpOutputTypeDef,
-    },
-)
-_OptionalAntennaUplinkConfigOutputTypeDef = TypedDict(
-    "_OptionalAntennaUplinkConfigOutputTypeDef",
-    {
-        "transmitDisabled": bool,
-    },
-    total=False,
-)
-
-class AntennaUplinkConfigOutputTypeDef(
-    _RequiredAntennaUplinkConfigOutputTypeDef, _OptionalAntennaUplinkConfigOutputTypeDef
-):
-    pass
-
 AntennaDownlinkConfigTypeDef = TypedDict(
     "AntennaDownlinkConfigTypeDef",
     {
         "spectrumConfig": SpectrumConfigTypeDef,
     },
 )
 
@@ -1581,37 +1354,20 @@
     "_OptionalAntennaUplinkConfigTypeDef",
     {
         "transmitDisabled": bool,
     },
     total=False,
 )
 
+
 class AntennaUplinkConfigTypeDef(
     _RequiredAntennaUplinkConfigTypeDef, _OptionalAntennaUplinkConfigTypeDef
 ):
     pass
 
-_RequiredRangedConnectionDetailsOutputTypeDef = TypedDict(
-    "_RequiredRangedConnectionDetailsOutputTypeDef",
-    {
-        "socketAddress": RangedSocketAddressOutputTypeDef,
-    },
-)
-_OptionalRangedConnectionDetailsOutputTypeDef = TypedDict(
-    "_OptionalRangedConnectionDetailsOutputTypeDef",
-    {
-        "mtu": int,
-    },
-    total=False,
-)
-
-class RangedConnectionDetailsOutputTypeDef(
-    _RequiredRangedConnectionDetailsOutputTypeDef, _OptionalRangedConnectionDetailsOutputTypeDef
-):
-    pass
 
 _RequiredRangedConnectionDetailsTypeDef = TypedDict(
     "_RequiredRangedConnectionDetailsTypeDef",
     {
         "socketAddress": RangedSocketAddressTypeDef,
     },
 )
@@ -1619,19 +1375,21 @@
     "_OptionalRangedConnectionDetailsTypeDef",
     {
         "mtu": int,
     },
     total=False,
 )
 
+
 class RangedConnectionDetailsTypeDef(
     _RequiredRangedConnectionDetailsTypeDef, _OptionalRangedConnectionDetailsTypeDef
 ):
     pass
 
+
 TLEEphemerisTypeDef = TypedDict(
     "TLEEphemerisTypeDef",
     {
         "s3Object": S3ObjectTypeDef,
         "tleData": Sequence[TLEDataTypeDef],
     },
     total=False,
@@ -1646,69 +1404,32 @@
         "invalidReason": EphemerisInvalidReasonType,
         "name": str,
         "priority": int,
         "satelliteId": str,
         "status": EphemerisStatusType,
         "suppliedData": EphemerisTypeDescriptionTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigTypeDataOutputTypeDef = TypedDict(
-    "ConfigTypeDataOutputTypeDef",
-    {
-        "antennaDownlinkConfig": AntennaDownlinkConfigOutputTypeDef,
-        "antennaDownlinkDemodDecodeConfig": AntennaDownlinkDemodDecodeConfigOutputTypeDef,
-        "antennaUplinkConfig": AntennaUplinkConfigOutputTypeDef,
-        "dataflowEndpointConfig": DataflowEndpointConfigOutputTypeDef,
-        "s3RecordingConfig": S3RecordingConfigOutputTypeDef,
-        "trackingConfig": TrackingConfigOutputTypeDef,
-        "uplinkEchoConfig": UplinkEchoConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 ConfigTypeDataTypeDef = TypedDict(
     "ConfigTypeDataTypeDef",
     {
         "antennaDownlinkConfig": AntennaDownlinkConfigTypeDef,
         "antennaDownlinkDemodDecodeConfig": AntennaDownlinkDemodDecodeConfigTypeDef,
         "antennaUplinkConfig": AntennaUplinkConfigTypeDef,
         "dataflowEndpointConfig": DataflowEndpointConfigTypeDef,
         "s3RecordingConfig": S3RecordingConfigTypeDef,
         "trackingConfig": TrackingConfigTypeDef,
         "uplinkEchoConfig": UplinkEchoConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredAwsGroundStationAgentEndpointOutputTypeDef = TypedDict(
-    "_RequiredAwsGroundStationAgentEndpointOutputTypeDef",
-    {
-        "egressAddress": ConnectionDetailsOutputTypeDef,
-        "ingressAddress": RangedConnectionDetailsOutputTypeDef,
-        "name": str,
-    },
-)
-_OptionalAwsGroundStationAgentEndpointOutputTypeDef = TypedDict(
-    "_OptionalAwsGroundStationAgentEndpointOutputTypeDef",
-    {
-        "agentStatus": AgentStatusType,
-        "auditResults": AuditResultsType,
-    },
-    total=False,
-)
-
-class AwsGroundStationAgentEndpointOutputTypeDef(
-    _RequiredAwsGroundStationAgentEndpointOutputTypeDef,
-    _OptionalAwsGroundStationAgentEndpointOutputTypeDef,
-):
-    pass
-
 _RequiredAwsGroundStationAgentEndpointTypeDef = TypedDict(
     "_RequiredAwsGroundStationAgentEndpointTypeDef",
     {
         "egressAddress": ConnectionDetailsTypeDef,
         "ingressAddress": RangedConnectionDetailsTypeDef,
         "name": str,
     },
@@ -1718,41 +1439,30 @@
     {
         "agentStatus": AgentStatusType,
         "auditResults": AuditResultsType,
     },
     total=False,
 )
 
+
 class AwsGroundStationAgentEndpointTypeDef(
     _RequiredAwsGroundStationAgentEndpointTypeDef, _OptionalAwsGroundStationAgentEndpointTypeDef
 ):
     pass
 
+
 EphemerisDataTypeDef = TypedDict(
     "EphemerisDataTypeDef",
     {
         "oem": OEMEphemerisTypeDef,
         "tle": TLEEphemerisTypeDef,
     },
     total=False,
 )
 
-GetConfigResponseTypeDef = TypedDict(
-    "GetConfigResponseTypeDef",
-    {
-        "configArn": str,
-        "configData": ConfigTypeDataOutputTypeDef,
-        "configId": str,
-        "configType": ConfigCapabilityTypeType,
-        "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigRequestRequestTypeDef",
     {
         "configData": ConfigTypeDataTypeDef,
         "name": str,
     },
 )
@@ -1760,34 +1470,49 @@
     "_OptionalCreateConfigRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateConfigRequestRequestTypeDef(
     _RequiredCreateConfigRequestRequestTypeDef, _OptionalCreateConfigRequestRequestTypeDef
 ):
     pass
 
+
+GetConfigResponseTypeDef = TypedDict(
+    "GetConfigResponseTypeDef",
+    {
+        "configArn": str,
+        "configData": ConfigTypeDataTypeDef,
+        "configId": str,
+        "configType": ConfigCapabilityTypeType,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateConfigRequestRequestTypeDef = TypedDict(
     "UpdateConfigRequestRequestTypeDef",
     {
         "configData": ConfigTypeDataTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
     },
 )
 
 EndpointDetailsOutputTypeDef = TypedDict(
     "EndpointDetailsOutputTypeDef",
     {
-        "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointOutputTypeDef,
-        "endpoint": DataflowEndpointOutputTypeDef,
+        "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointTypeDef,
+        "endpoint": DataflowEndpointTypeDef,
         "healthReasons": List[CapabilityHealthReasonType],
         "healthStatus": CapabilityHealthType,
         "securityDetails": SecurityDetailsOutputTypeDef,
     },
     total=False,
 )
 
@@ -1819,19 +1544,21 @@
         "kmsKeyArn": str,
         "priority": int,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateEphemerisRequestRequestTypeDef(
     _RequiredCreateEphemerisRequestRequestTypeDef, _OptionalCreateEphemerisRequestRequestTypeDef
 ):
     pass
 
+
 ConfigDetailsTypeDef = TypedDict(
     "ConfigDetailsTypeDef",
     {
         "antennaDemodDecodeDetails": AntennaDemodDecodeDetailsTypeDef,
         "endpointDetails": EndpointDetailsOutputTypeDef,
         "s3RecordingDetails": S3RecordingDetailsTypeDef,
     },
@@ -1843,15 +1570,15 @@
     {
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
         "dataflowEndpointGroupArn": str,
         "dataflowEndpointGroupId": str,
         "endpointsDetails": List[EndpointDetailsOutputTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
     {
         "endpointDetails": Sequence[EndpointDetailsTypeDef],
@@ -1863,20 +1590,22 @@
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateDataflowEndpointGroupRequestRequestTypeDef(
     _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
     _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
 ):
     pass
 
+
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "configDetails": ConfigDetailsTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "dataflowDestinationRegion": str,
@@ -1918,10 +1647,10 @@
         "missionProfileArn": str,
         "postPassEndTime": datetime,
         "prePassStartTime": datetime,
         "region": str,
         "satelliteArn": str,
         "startTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/waiter.py` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation/waiter.pyi` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/PKG-INFO` & `mypy-boto3-groundstation-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-groundstation
-Version: 1.28.12
-Summary: Type annotations for boto3.GroundStation 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 groundstation type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-groundstation"></a>
 
 # mypy-boto3-groundstation
 
 [![PyPI - mypy-boto3-groundstation](https://img.shields.io/pypi/v/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-groundstation)](https://pepy.tech/project/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
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
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -387,146 +355,122 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_groundstation.type_defs import (
     ComponentVersionTypeDef,
     AggregateStatusTypeDef,
     AntennaDemodDecodeDetailsTypeDef,
-    DecodeConfigOutputTypeDef,
-    DemodulationConfigOutputTypeDef,
     DecodeConfigTypeDef,
     DemodulationConfigTypeDef,
-    EirpOutputTypeDef,
     EirpTypeDef,
     CancelContactRequestRequestTypeDef,
     ComponentStatusDataTypeDef,
     S3RecordingDetailsTypeDef,
-    ConfigIdResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConfigListItemTypeDef,
-    DataflowEndpointConfigOutputTypeDef,
-    S3RecordingConfigOutputTypeDef,
-    TrackingConfigOutputTypeDef,
-    UplinkEchoConfigOutputTypeDef,
     DataflowEndpointConfigTypeDef,
     S3RecordingConfigTypeDef,
     TrackingConfigTypeDef,
     UplinkEchoConfigTypeDef,
-    SocketAddressOutputTypeDef,
     SocketAddressTypeDef,
     ElevationTypeDef,
-    ContactIdResponseTypeDef,
     KmsKeyTypeDef,
-    DataflowEndpointGroupIdResponseTypeDef,
     DataflowEndpointListItemTypeDef,
     DeleteConfigRequestRequestTypeDef,
     DeleteDataflowEndpointGroupRequestRequestTypeDef,
     DeleteEphemerisRequestRequestTypeDef,
     DeleteMissionProfileRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeContactRequestRequestTypeDef,
     DescribeEphemerisRequestRequestTypeDef,
     DiscoveryDataTypeDef,
     SecurityDetailsOutputTypeDef,
     SecurityDetailsTypeDef,
-    S3ObjectOutputTypeDef,
-    EphemerisIdResponseTypeDef,
+    S3ObjectTypeDef,
     EphemerisMetaDataTypeDef,
-    FrequencyBandwidthOutputTypeDef,
     FrequencyBandwidthTypeDef,
-    FrequencyOutputTypeDef,
     FrequencyTypeDef,
     GetAgentConfigurationRequestRequestTypeDef,
-    GetAgentConfigurationResponseTypeDef,
     GetConfigRequestRequestTypeDef,
     GetDataflowEndpointGroupRequestRequestTypeDef,
     GetMinuteUsageRequestRequestTypeDef,
-    GetMinuteUsageResponseTypeDef,
     GetMissionProfileRequestRequestTypeDef,
-    KmsKeyOutputTypeDef,
     GetSatelliteRequestRequestTypeDef,
     GroundStationDataTypeDef,
-    IntegerRangeOutputTypeDef,
     IntegerRangeTypeDef,
-    ListConfigsRequestListConfigsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListConfigsRequestRequestTypeDef,
-    ListContactsRequestListContactsPaginateTypeDef,
     ListContactsRequestRequestTypeDef,
-    ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
     ListDataflowEndpointGroupsRequestRequestTypeDef,
-    ListEphemeridesRequestListEphemeridesPaginateTypeDef,
     ListEphemeridesRequestRequestTypeDef,
-    ListGroundStationsRequestListGroundStationsPaginateTypeDef,
     ListGroundStationsRequestRequestTypeDef,
-    ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
     ListMissionProfilesRequestRequestTypeDef,
     MissionProfileListItemTypeDef,
-    ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListSatellitesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MissionProfileIdResponseTypeDef,
-    S3ObjectTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterAgentResponseTypeDef,
     ReserveContactRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TimeRangeTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAgentStatusResponseTypeDef,
     UpdateEphemerisRequestRequestTypeDef,
     AgentDetailsTypeDef,
     UpdateAgentStatusRequestRequestTypeDef,
+    ConfigIdResponseTypeDef,
+    ContactIdResponseTypeDef,
+    DataflowEndpointGroupIdResponseTypeDef,
+    EphemerisIdResponseTypeDef,
+    GetAgentConfigurationResponseTypeDef,
+    GetMinuteUsageResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    MissionProfileIdResponseTypeDef,
+    RegisterAgentResponseTypeDef,
+    UpdateAgentStatusResponseTypeDef,
     ListConfigsResponseTypeDef,
-    ConnectionDetailsOutputTypeDef,
-    DataflowEndpointOutputTypeDef,
     ConnectionDetailsTypeDef,
     DataflowEndpointTypeDef,
     ContactDataTypeDef,
     CreateMissionProfileRequestRequestTypeDef,
+    GetMissionProfileResponseTypeDef,
     UpdateMissionProfileRequestRequestTypeDef,
     ListDataflowEndpointGroupsResponseTypeDef,
     DescribeContactRequestContactScheduledWaitTypeDef,
     EphemerisDescriptionTypeDef,
     EphemerisItemTypeDef,
+    OEMEphemerisTypeDef,
     GetSatelliteResponseTypeDef,
     SatelliteListItemTypeDef,
-    SpectrumConfigOutputTypeDef,
-    UplinkSpectrumConfigOutputTypeDef,
     SpectrumConfigTypeDef,
     UplinkSpectrumConfigTypeDef,
-    GetMissionProfileResponseTypeDef,
     ListGroundStationsResponseTypeDef,
-    RangedSocketAddressOutputTypeDef,
     RangedSocketAddressTypeDef,
+    ListConfigsRequestListConfigsPaginateTypeDef,
+    ListContactsRequestListContactsPaginateTypeDef,
+    ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef,
+    ListEphemeridesRequestListEphemeridesPaginateTypeDef,
+    ListGroundStationsRequestListGroundStationsPaginateTypeDef,
+    ListMissionProfilesRequestListMissionProfilesPaginateTypeDef,
+    ListSatellitesRequestListSatellitesPaginateTypeDef,
     ListMissionProfilesResponseTypeDef,
-    OEMEphemerisTypeDef,
     TLEDataTypeDef,
     RegisterAgentRequestRequestTypeDef,
     ListContactsResponseTypeDef,
     EphemerisTypeDescriptionTypeDef,
     ListEphemeridesResponseTypeDef,
     ListSatellitesResponseTypeDef,
-    AntennaDownlinkConfigOutputTypeDef,
-    AntennaDownlinkDemodDecodeConfigOutputTypeDef,
-    AntennaUplinkConfigOutputTypeDef,
     AntennaDownlinkConfigTypeDef,
     AntennaDownlinkDemodDecodeConfigTypeDef,
     AntennaUplinkConfigTypeDef,
-    RangedConnectionDetailsOutputTypeDef,
     RangedConnectionDetailsTypeDef,
     TLEEphemerisTypeDef,
     DescribeEphemerisResponseTypeDef,
-    ConfigTypeDataOutputTypeDef,
     ConfigTypeDataTypeDef,
-    AwsGroundStationAgentEndpointOutputTypeDef,
     AwsGroundStationAgentEndpointTypeDef,
     EphemerisDataTypeDef,
-    GetConfigResponseTypeDef,
     CreateConfigRequestRequestTypeDef,
+    GetConfigResponseTypeDef,
     UpdateConfigRequestRequestTypeDef,
     EndpointDetailsOutputTypeDef,
     EndpointDetailsTypeDef,
     CreateEphemerisRequestRequestTypeDef,
     ConfigDetailsTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
     CreateDataflowEndpointGroupRequestRequestTypeDef,
```

### Comparing `mypy-boto3-groundstation-1.28.12/mypy_boto3_groundstation.egg-info/SOURCES.txt` & `mypy-boto3-groundstation-1.28.15/mypy_boto3_groundstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.28.12/setup.py` & `mypy-boto3-groundstation-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-groundstation",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_groundstation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GroundStation 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.GroundStation 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

