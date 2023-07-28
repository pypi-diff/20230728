# Comparing `tmp/mypy-boto3-shield-1.28.12.tar.gz` & `tmp/mypy-boto3-shield-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-shield-1.28.12.tar", last modified: Thu Jul 27 11:49:39 2023, max compression
+gzip compressed data, was "mypy-boto3-shield-1.28.15.tar", last modified: Fri Jul 28 20:43:45 2023, max compression
```

## Comparing `mypy-boto3-shield-1.28.12.tar` & `mypy-boto3-shield-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:39.525300 mypy-boto3-shield-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-07-27 11:49:39.525300 mypy-boto3-shield-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:39.521300 mypy-boto3-shield-1.28.12/mypy_boto3_shield/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25575 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-27 11:46:59.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-27 11:46:59.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23299 2023-07-27 11:46:59.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23278 2023-07-27 11:46:59.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:57.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:39.525300 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-07-27 11:49:39.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 11:49:39.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:39.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:39.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:39.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 11:49:39.000000 mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:39.525300 mypy-boto3-shield-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 11:46:56.000000 mypy-boto3-shield-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.777892 mypy-boto3-shield-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-07-28 20:43:45.773892 mypy-boto3-shield-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.773892 mypy-boto3-shield-1.28.15/mypy_boto3_shield/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25575 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-28 20:39:31.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-28 20:39:31.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-07-28 20:39:31.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22613 2023-07-28 20:39:31.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.773892 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15815 2023-07-28 20:43:45.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:43:45.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:45.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:45.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:45.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:43:45.000000 mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:45.777892 mypy-boto3-shield-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:39:30.000000 mypy-boto3-shield-1.28.15/setup.py
```

### Comparing `mypy-boto3-shield-1.28.12/LICENSE` & `mypy-boto3-shield-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.12/PKG-INFO` & `mypy-boto3-shield-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-shield
-Version: 1.28.12
-Summary: Type annotations for boto3.Shield 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Shield 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-shield)](https://pepy.tech/project/mypy-boto3-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Shield 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[boto3.Shield 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,30 +346,28 @@
     AttackVolumeStatisticsTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DeleteProtectionGroupRequestRequestTypeDef,
     DeleteProtectionRequestRequestTypeDef,
     DescribeAttackRequestRequestTypeDef,
     TimeRangeOutputTypeDef,
-    EmergencyContactOutputTypeDef,
     DescribeProtectionGroupRequestRequestTypeDef,
     ProtectionGroupTypeDef,
     DescribeProtectionRequestRequestTypeDef,
     DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
     ResponseActionTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
     PaginatorConfigTypeDef,
     TimeRangeTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
@@ -378,28 +376,28 @@
     AttackSummaryTypeDef,
     AttackVolumeTypeDef,
     CreateProtectionGroupRequestRequestTypeDef,
     CreateProtectionRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateProtectionResponseTypeDef,
     DescribeDRTAccessResponseTypeDef,
+    DescribeEmergencyContactSettingsResponseTypeDef,
     GetSubscriptionStateResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
     ListProtectionsRequestListProtectionsPaginateTypeDef,
     ListAttacksRequestListAttacksPaginateTypeDef,
     ListAttacksRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
     DescribeProtectionResponseTypeDef,
```

### Comparing `mypy-boto3-shield-1.28.12/README.md` & `mypy-boto3-shield-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-shield)](https://pepy.tech/project/mypy-boto3-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Shield 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[boto3.Shield 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
 See how it helps to find and fix potential bugs:
 
@@ -314,30 +314,28 @@
     AttackVolumeStatisticsTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DeleteProtectionGroupRequestRequestTypeDef,
     DeleteProtectionRequestRequestTypeDef,
     DescribeAttackRequestRequestTypeDef,
     TimeRangeOutputTypeDef,
-    EmergencyContactOutputTypeDef,
     DescribeProtectionGroupRequestRequestTypeDef,
     ProtectionGroupTypeDef,
     DescribeProtectionRequestRequestTypeDef,
     DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
     ResponseActionTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
     PaginatorConfigTypeDef,
     TimeRangeTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
@@ -346,28 +344,28 @@
     AttackSummaryTypeDef,
     AttackVolumeTypeDef,
     CreateProtectionGroupRequestRequestTypeDef,
     CreateProtectionRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateProtectionResponseTypeDef,
     DescribeDRTAccessResponseTypeDef,
+    DescribeEmergencyContactSettingsResponseTypeDef,
     GetSubscriptionStateResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
     ListProtectionsRequestListProtectionsPaginateTypeDef,
     ListAttacksRequestListAttacksPaginateTypeDef,
     ListAttacksRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
     DescribeProtectionResponseTypeDef,
```

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield/__init__.py` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield/__init__.pyi` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield/__main__.py` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Shield 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Shield 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield\nOther"
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

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield/client.py` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield/client.pyi` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield/literals.py` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield/literals.pyi` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield/paginator.py` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield/paginator.pyi` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield/type_defs.py` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,30 +48,28 @@
     "AttackVolumeStatisticsTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteProtectionGroupRequestRequestTypeDef",
     "DeleteProtectionRequestRequestTypeDef",
     "DescribeAttackRequestRequestTypeDef",
     "TimeRangeOutputTypeDef",
-    "EmergencyContactOutputTypeDef",
     "DescribeProtectionGroupRequestRequestTypeDef",
     "ProtectionGroupTypeDef",
     "DescribeProtectionRequestRequestTypeDef",
     "DisableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "DisassociateDRTLogBucketRequestRequestTypeDef",
     "DisassociateHealthCheckRequestRequestTypeDef",
     "ResponseActionTypeDef",
     "InclusionProtectionFiltersTypeDef",
     "InclusionProtectionGroupFiltersTypeDef",
     "LimitTypeDef",
     "PaginatorConfigTypeDef",
     "TimeRangeTypeDef",
     "ListResourcesInProtectionGroupRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProtectionGroupRequestRequestTypeDef",
     "UpdateSubscriptionRequestRequestTypeDef",
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
@@ -80,28 +78,28 @@
     "AttackSummaryTypeDef",
     "AttackVolumeTypeDef",
     "CreateProtectionGroupRequestRequestTypeDef",
     "CreateProtectionRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateProtectionResponseTypeDef",
     "DescribeDRTAccessResponseTypeDef",
+    "DescribeEmergencyContactSettingsResponseTypeDef",
     "GetSubscriptionStateResponseTypeDef",
     "ListResourcesInProtectionGroupResponseTypeDef",
-    "DescribeEmergencyContactSettingsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DescribeProtectionGroupResponseTypeDef",
     "ListProtectionGroupsResponseTypeDef",
     "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "ListProtectionsRequestRequestTypeDef",
     "ListProtectionGroupsRequestRequestTypeDef",
     "ProtectionLimitsTypeDef",
     "ListProtectionsRequestListProtectionsPaginateTypeDef",
     "ListAttacksRequestListAttacksPaginateTypeDef",
     "ListAttacksRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ProtectionGroupPatternTypeLimitsTypeDef",
     "ProtectionTypeDef",
     "SubResourceSummaryTypeDef",
     "ListAttacksResponseTypeDef",
     "AttackStatisticsDataItemTypeDef",
     "ProtectionGroupLimitsTypeDef",
     "DescribeProtectionResponseTypeDef",
@@ -255,36 +253,14 @@
     {
         "FromInclusive": datetime,
         "ToExclusive": datetime,
     },
     total=False,
 )
 
-_RequiredEmergencyContactOutputTypeDef = TypedDict(
-    "_RequiredEmergencyContactOutputTypeDef",
-    {
-        "EmailAddress": str,
-    },
-)
-_OptionalEmergencyContactOutputTypeDef = TypedDict(
-    "_OptionalEmergencyContactOutputTypeDef",
-    {
-        "PhoneNumber": str,
-        "ContactNotes": str,
-    },
-    total=False,
-)
-
-
-class EmergencyContactOutputTypeDef(
-    _RequiredEmergencyContactOutputTypeDef, _OptionalEmergencyContactOutputTypeDef
-):
-    pass
-
-
 DescribeProtectionGroupRequestRequestTypeDef = TypedDict(
     "DescribeProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 
@@ -426,23 +402,14 @@
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
 ProtectionGroupArbitraryPatternLimitsTypeDef = TypedDict(
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     {
         "MaxMembers": int,
     },
 )
 
@@ -634,14 +601,22 @@
     {
         "RoleArn": str,
         "LogBucketList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
+    "DescribeEmergencyContactSettingsResponseTypeDef",
+    {
+        "EmergencyContactList": List[EmergencyContactTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetSubscriptionStateResponseTypeDef = TypedDict(
     "GetSubscriptionStateResponseTypeDef",
     {
         "SubscriptionState": SubscriptionStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -651,18 +626,18 @@
     {
         "ResourceArns": List[str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
-    "DescribeEmergencyContactSettingsResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "EmergencyContactList": List[EmergencyContactOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProtectionGroupResponseTypeDef = TypedDict(
     "DescribeProtectionGroupResponseTypeDef",
     {
@@ -751,22 +726,14 @@
         "EndTime": TimeRangeTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
     "ProtectionGroupPatternTypeLimitsTypeDef",
     {
         "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
     },
 )
```

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield/type_defs.pyi` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,30 +47,28 @@
     "AttackVolumeStatisticsTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteProtectionGroupRequestRequestTypeDef",
     "DeleteProtectionRequestRequestTypeDef",
     "DescribeAttackRequestRequestTypeDef",
     "TimeRangeOutputTypeDef",
-    "EmergencyContactOutputTypeDef",
     "DescribeProtectionGroupRequestRequestTypeDef",
     "ProtectionGroupTypeDef",
     "DescribeProtectionRequestRequestTypeDef",
     "DisableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "DisassociateDRTLogBucketRequestRequestTypeDef",
     "DisassociateHealthCheckRequestRequestTypeDef",
     "ResponseActionTypeDef",
     "InclusionProtectionFiltersTypeDef",
     "InclusionProtectionGroupFiltersTypeDef",
     "LimitTypeDef",
     "PaginatorConfigTypeDef",
     "TimeRangeTypeDef",
     "ListResourcesInProtectionGroupRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProtectionGroupRequestRequestTypeDef",
     "UpdateSubscriptionRequestRequestTypeDef",
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
@@ -79,28 +77,28 @@
     "AttackSummaryTypeDef",
     "AttackVolumeTypeDef",
     "CreateProtectionGroupRequestRequestTypeDef",
     "CreateProtectionRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateProtectionResponseTypeDef",
     "DescribeDRTAccessResponseTypeDef",
+    "DescribeEmergencyContactSettingsResponseTypeDef",
     "GetSubscriptionStateResponseTypeDef",
     "ListResourcesInProtectionGroupResponseTypeDef",
-    "DescribeEmergencyContactSettingsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DescribeProtectionGroupResponseTypeDef",
     "ListProtectionGroupsResponseTypeDef",
     "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "ListProtectionsRequestRequestTypeDef",
     "ListProtectionGroupsRequestRequestTypeDef",
     "ProtectionLimitsTypeDef",
     "ListProtectionsRequestListProtectionsPaginateTypeDef",
     "ListAttacksRequestListAttacksPaginateTypeDef",
     "ListAttacksRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ProtectionGroupPatternTypeLimitsTypeDef",
     "ProtectionTypeDef",
     "SubResourceSummaryTypeDef",
     "ListAttacksResponseTypeDef",
     "AttackStatisticsDataItemTypeDef",
     "ProtectionGroupLimitsTypeDef",
     "DescribeProtectionResponseTypeDef",
@@ -252,34 +250,14 @@
     {
         "FromInclusive": datetime,
         "ToExclusive": datetime,
     },
     total=False,
 )
 
-_RequiredEmergencyContactOutputTypeDef = TypedDict(
-    "_RequiredEmergencyContactOutputTypeDef",
-    {
-        "EmailAddress": str,
-    },
-)
-_OptionalEmergencyContactOutputTypeDef = TypedDict(
-    "_OptionalEmergencyContactOutputTypeDef",
-    {
-        "PhoneNumber": str,
-        "ContactNotes": str,
-    },
-    total=False,
-)
-
-class EmergencyContactOutputTypeDef(
-    _RequiredEmergencyContactOutputTypeDef, _OptionalEmergencyContactOutputTypeDef
-):
-    pass
-
 DescribeProtectionGroupRequestRequestTypeDef = TypedDict(
     "DescribeProtectionGroupRequestRequestTypeDef",
     {
         "ProtectionGroupId": str,
     },
 )
 
@@ -417,23 +395,14 @@
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
 ProtectionGroupArbitraryPatternLimitsTypeDef = TypedDict(
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     {
         "MaxMembers": int,
     },
 )
 
@@ -617,14 +586,22 @@
     {
         "RoleArn": str,
         "LogBucketList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
+    "DescribeEmergencyContactSettingsResponseTypeDef",
+    {
+        "EmergencyContactList": List[EmergencyContactTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetSubscriptionStateResponseTypeDef = TypedDict(
     "GetSubscriptionStateResponseTypeDef",
     {
         "SubscriptionState": SubscriptionStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -634,18 +611,18 @@
     {
         "ResourceArns": List[str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeEmergencyContactSettingsResponseTypeDef = TypedDict(
-    "DescribeEmergencyContactSettingsResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "EmergencyContactList": List[EmergencyContactOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProtectionGroupResponseTypeDef = TypedDict(
     "DescribeProtectionGroupResponseTypeDef",
     {
@@ -734,22 +711,14 @@
         "EndTime": TimeRangeTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
     "ProtectionGroupPatternTypeLimitsTypeDef",
     {
         "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
     },
 )
```

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/PKG-INFO` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-shield
-Version: 1.28.12
-Summary: Type annotations for boto3.Shield 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Shield 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-shield.svg?color=blue)](https://pypi.org/project/mypy-boto3-shield)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-shield)](https://pepy.tech/project/mypy-boto3-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Shield 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[boto3.Shield 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [mypy-boto3-shield docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_shield/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,30 +346,28 @@
     AttackVolumeStatisticsTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     DeleteProtectionGroupRequestRequestTypeDef,
     DeleteProtectionRequestRequestTypeDef,
     DescribeAttackRequestRequestTypeDef,
     TimeRangeOutputTypeDef,
-    EmergencyContactOutputTypeDef,
     DescribeProtectionGroupRequestRequestTypeDef,
     ProtectionGroupTypeDef,
     DescribeProtectionRequestRequestTypeDef,
     DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     DisassociateDRTLogBucketRequestRequestTypeDef,
     DisassociateHealthCheckRequestRequestTypeDef,
     ResponseActionTypeDef,
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     LimitTypeDef,
     PaginatorConfigTypeDef,
     TimeRangeTypeDef,
     ListResourcesInProtectionGroupRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ProtectionGroupArbitraryPatternLimitsTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateProtectionGroupRequestRequestTypeDef,
     UpdateSubscriptionRequestRequestTypeDef,
     ApplicationLayerAutomaticResponseConfigurationTypeDef,
     AssociateProactiveEngagementDetailsRequestRequestTypeDef,
     UpdateEmergencyContactSettingsRequestRequestTypeDef,
@@ -378,28 +376,28 @@
     AttackSummaryTypeDef,
     AttackVolumeTypeDef,
     CreateProtectionGroupRequestRequestTypeDef,
     CreateProtectionRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateProtectionResponseTypeDef,
     DescribeDRTAccessResponseTypeDef,
+    DescribeEmergencyContactSettingsResponseTypeDef,
     GetSubscriptionStateResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeProtectionGroupResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
     UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
     ListProtectionsRequestRequestTypeDef,
     ListProtectionGroupsRequestRequestTypeDef,
     ProtectionLimitsTypeDef,
     ListProtectionsRequestListProtectionsPaginateTypeDef,
     ListAttacksRequestListAttacksPaginateTypeDef,
     ListAttacksRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ProtectionGroupPatternTypeLimitsTypeDef,
     ProtectionTypeDef,
     SubResourceSummaryTypeDef,
     ListAttacksResponseTypeDef,
     AttackStatisticsDataItemTypeDef,
     ProtectionGroupLimitsTypeDef,
     DescribeProtectionResponseTypeDef,
```

### Comparing `mypy-boto3-shield-1.28.12/mypy_boto3_shield.egg-info/SOURCES.txt` & `mypy-boto3-shield-1.28.15/mypy_boto3_shield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-shield-1.28.12/setup.py` & `mypy-boto3-shield-1.28.15/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-shield",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_shield"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Shield 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Shield 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

