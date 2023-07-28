# Comparing `tmp/mypy-boto3-route53-recovery-readiness-1.28.12.tar.gz` & `tmp/mypy-boto3-route53-recovery-readiness-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-recovery-readiness-1.28.12.tar", last modified: Thu Jul 27 11:49:32 2023, max compression
+gzip compressed data, was "mypy-boto3-route53-recovery-readiness-1.28.15.tar", last modified: Fri Jul 28 20:43:36 2023, max compression
```

## Comparing `mypy-boto3-route53-recovery-readiness-1.28.12.tar` & `mypy-boto3-route53-recovery-readiness-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:32.973238 mypy-boto3-route53-recovery-readiness-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-07-27 11:49:32.973238 mypy-boto3-route53-recovery-readiness-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:32.973238 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28483 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30991 2023-07-27 11:44:53.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-07-27 11:44:52.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:32.973238 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-07-27 11:49:32.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-27 11:49:32.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:32.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:32.000000 mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:32.973238 mypy-boto3-route53-recovery-readiness-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-27 11:44:51.000000 mypy-boto3-route53-recovery-readiness-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.929771 mypy-boto3-route53-recovery-readiness-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19048 2023-07-28 20:43:36.929771 mypy-boto3-route53-recovery-readiness-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17487 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.909771 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28483 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-07-28 20:37:17.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-28 20:37:17.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-07-28 20:37:17.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-28 20:37:17.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30054 2023-07-28 20:37:18.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30017 2023-07-28 20:37:17.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.929771 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19048 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:36.000000 mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:36.929771 mypy-boto3-route53-recovery-readiness-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-28 20:37:16.000000 mypy-boto3-route53-recovery-readiness-1.28.15/setup.py
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/LICENSE` & `mypy-boto3-route53-recovery-readiness-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/PKG-INFO` & `mypy-boto3-route53-recovery-readiness-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-readiness
-Version: 1.28.12
-Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-readiness)](https://pepy.tech/project/mypy-boto3-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryReadiness 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[boto3.Route53RecoveryReadiness 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -398,17 +398,15 @@
     ReadinessCheckOutputTypeDef,
     ListRecoveryGroupsRequestRequestTypeDef,
     RecoveryGroupOutputTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ListRulesOutputTypeDef,
     ListRulesRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
-    NLBResourceOutputTypeDef,
     NLBResourceTypeDef,
-    R53ResourceRecordOutputTypeDef,
     R53ResourceRecordTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCellRequestRequestTypeDef,
     UpdateReadinessCheckRequestRequestTypeDef,
     UpdateRecoveryGroupRequestRequestTypeDef,
     CreateCellResponseTypeDef,
@@ -439,18 +437,16 @@
     GetCellReadinessSummaryResponseTypeDef,
     GetRecoveryGroupReadinessSummaryResponseTypeDef,
     RuleResultTypeDef,
     GetReadinessCheckStatusResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListRulesResponseTypeDef,
-    TargetResourceOutputTypeDef,
     TargetResourceTypeDef,
     GetReadinessCheckResourceStatusResponseTypeDef,
-    DNSTargetResourceOutputTypeDef,
     DNSTargetResourceTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     CreateResourceSetResponseTypeDef,
     GetResourceSetResponseTypeDef,
     ResourceSetOutputTypeDef,
     UpdateResourceSetResponseTypeDef,
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/README.md` & `mypy-boto3-route53-recovery-readiness-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-readiness)](https://pepy.tech/project/mypy-boto3-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryReadiness 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[boto3.Route53RecoveryReadiness 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,17 +366,15 @@
     ReadinessCheckOutputTypeDef,
     ListRecoveryGroupsRequestRequestTypeDef,
     RecoveryGroupOutputTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ListRulesOutputTypeDef,
     ListRulesRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
-    NLBResourceOutputTypeDef,
     NLBResourceTypeDef,
-    R53ResourceRecordOutputTypeDef,
     R53ResourceRecordTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCellRequestRequestTypeDef,
     UpdateReadinessCheckRequestRequestTypeDef,
     UpdateRecoveryGroupRequestRequestTypeDef,
     CreateCellResponseTypeDef,
@@ -407,18 +405,16 @@
     GetCellReadinessSummaryResponseTypeDef,
     GetRecoveryGroupReadinessSummaryResponseTypeDef,
     RuleResultTypeDef,
     GetReadinessCheckStatusResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListRulesResponseTypeDef,
-    TargetResourceOutputTypeDef,
     TargetResourceTypeDef,
     GetReadinessCheckResourceStatusResponseTypeDef,
-    DNSTargetResourceOutputTypeDef,
     DNSTargetResourceTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     CreateResourceSetResponseTypeDef,
     GetResourceSetResponseTypeDef,
     ResourceSetOutputTypeDef,
     UpdateResourceSetResponseTypeDef,
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/__init__.py` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/__init__.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/__main__.py` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53RecoveryReadiness 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.Route53RecoveryReadiness 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness\nOther"
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

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/client.py` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/client.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/literals.py` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/literals.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/paginator.py` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/paginator.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/type_defs.py` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,17 +55,15 @@
     "ReadinessCheckOutputTypeDef",
     "ListRecoveryGroupsRequestRequestTypeDef",
     "RecoveryGroupOutputTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ListRulesOutputTypeDef",
     "ListRulesRequestRequestTypeDef",
     "ListTagsForResourcesRequestRequestTypeDef",
-    "NLBResourceOutputTypeDef",
     "NLBResourceTypeDef",
-    "R53ResourceRecordOutputTypeDef",
     "R53ResourceRecordTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCellRequestRequestTypeDef",
     "UpdateReadinessCheckRequestRequestTypeDef",
     "UpdateRecoveryGroupRequestRequestTypeDef",
     "CreateCellResponseTypeDef",
@@ -96,18 +94,16 @@
     "GetCellReadinessSummaryResponseTypeDef",
     "GetRecoveryGroupReadinessSummaryResponseTypeDef",
     "RuleResultTypeDef",
     "GetReadinessCheckStatusResponseTypeDef",
     "ListReadinessChecksResponseTypeDef",
     "ListRecoveryGroupsResponseTypeDef",
     "ListRulesResponseTypeDef",
-    "TargetResourceOutputTypeDef",
     "TargetResourceTypeDef",
     "GetReadinessCheckResourceStatusResponseTypeDef",
-    "DNSTargetResourceOutputTypeDef",
     "DNSTargetResourceTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "CreateResourceSetResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "ResourceSetOutputTypeDef",
     "UpdateResourceSetResponseTypeDef",
@@ -571,39 +567,22 @@
 ListTagsForResourcesRequestRequestTypeDef = TypedDict(
     "ListTagsForResourcesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-NLBResourceOutputTypeDef = TypedDict(
-    "NLBResourceOutputTypeDef",
-    {
-        "Arn": str,
-    },
-    total=False,
-)
-
 NLBResourceTypeDef = TypedDict(
     "NLBResourceTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-R53ResourceRecordOutputTypeDef = TypedDict(
-    "R53ResourceRecordOutputTypeDef",
-    {
-        "DomainName": str,
-        "RecordSetId": str,
-    },
-    total=False,
-)
-
 R53ResourceRecordTypeDef = TypedDict(
     "R53ResourceRecordTypeDef",
     {
         "DomainName": str,
         "RecordSetId": str,
     },
     total=False,
@@ -1004,23 +983,14 @@
     {
         "NextToken": str,
         "Rules": List[ListRulesOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TargetResourceOutputTypeDef = TypedDict(
-    "TargetResourceOutputTypeDef",
-    {
-        "NLBResource": NLBResourceOutputTypeDef,
-        "R53Resource": R53ResourceRecordOutputTypeDef,
-    },
-    total=False,
-)
-
 TargetResourceTypeDef = TypedDict(
     "TargetResourceTypeDef",
     {
         "NLBResource": NLBResourceTypeDef,
         "R53Resource": R53ResourceRecordTypeDef,
     },
     total=False,
@@ -1032,26 +1002,14 @@
         "NextToken": str,
         "Readiness": ReadinessType,
         "Rules": List[RuleResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DNSTargetResourceOutputTypeDef = TypedDict(
-    "DNSTargetResourceOutputTypeDef",
-    {
-        "DomainName": str,
-        "HostedZoneArn": str,
-        "RecordSetId": str,
-        "RecordType": str,
-        "TargetResource": TargetResourceOutputTypeDef,
-    },
-    total=False,
-)
-
 DNSTargetResourceTypeDef = TypedDict(
     "DNSTargetResourceTypeDef",
     {
         "DomainName": str,
         "HostedZoneArn": str,
         "RecordSetId": str,
         "RecordType": str,
@@ -1060,15 +1018,15 @@
     total=False,
 )
 
 ResourceOutputTypeDef = TypedDict(
     "ResourceOutputTypeDef",
     {
         "ComponentId": str,
-        "DnsTargetResource": DNSTargetResourceOutputTypeDef,
+        "DnsTargetResource": DNSTargetResourceTypeDef,
         "ReadinessScopes": List[str],
         "ResourceArn": str,
     },
     total=False,
 )
 
 ResourceTypeDef = TypedDict(
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness/type_defs.pyi` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -54,17 +54,15 @@
     "ReadinessCheckOutputTypeDef",
     "ListRecoveryGroupsRequestRequestTypeDef",
     "RecoveryGroupOutputTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ListRulesOutputTypeDef",
     "ListRulesRequestRequestTypeDef",
     "ListTagsForResourcesRequestRequestTypeDef",
-    "NLBResourceOutputTypeDef",
     "NLBResourceTypeDef",
-    "R53ResourceRecordOutputTypeDef",
     "R53ResourceRecordTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCellRequestRequestTypeDef",
     "UpdateReadinessCheckRequestRequestTypeDef",
     "UpdateRecoveryGroupRequestRequestTypeDef",
     "CreateCellResponseTypeDef",
@@ -95,18 +93,16 @@
     "GetCellReadinessSummaryResponseTypeDef",
     "GetRecoveryGroupReadinessSummaryResponseTypeDef",
     "RuleResultTypeDef",
     "GetReadinessCheckStatusResponseTypeDef",
     "ListReadinessChecksResponseTypeDef",
     "ListRecoveryGroupsResponseTypeDef",
     "ListRulesResponseTypeDef",
-    "TargetResourceOutputTypeDef",
     "TargetResourceTypeDef",
     "GetReadinessCheckResourceStatusResponseTypeDef",
-    "DNSTargetResourceOutputTypeDef",
     "DNSTargetResourceTypeDef",
     "ResourceOutputTypeDef",
     "ResourceTypeDef",
     "CreateResourceSetResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "ResourceSetOutputTypeDef",
     "UpdateResourceSetResponseTypeDef",
@@ -546,39 +542,22 @@
 ListTagsForResourcesRequestRequestTypeDef = TypedDict(
     "ListTagsForResourcesRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-NLBResourceOutputTypeDef = TypedDict(
-    "NLBResourceOutputTypeDef",
-    {
-        "Arn": str,
-    },
-    total=False,
-)
-
 NLBResourceTypeDef = TypedDict(
     "NLBResourceTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-R53ResourceRecordOutputTypeDef = TypedDict(
-    "R53ResourceRecordOutputTypeDef",
-    {
-        "DomainName": str,
-        "RecordSetId": str,
-    },
-    total=False,
-)
-
 R53ResourceRecordTypeDef = TypedDict(
     "R53ResourceRecordTypeDef",
     {
         "DomainName": str,
         "RecordSetId": str,
     },
     total=False,
@@ -971,23 +950,14 @@
     {
         "NextToken": str,
         "Rules": List[ListRulesOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TargetResourceOutputTypeDef = TypedDict(
-    "TargetResourceOutputTypeDef",
-    {
-        "NLBResource": NLBResourceOutputTypeDef,
-        "R53Resource": R53ResourceRecordOutputTypeDef,
-    },
-    total=False,
-)
-
 TargetResourceTypeDef = TypedDict(
     "TargetResourceTypeDef",
     {
         "NLBResource": NLBResourceTypeDef,
         "R53Resource": R53ResourceRecordTypeDef,
     },
     total=False,
@@ -999,26 +969,14 @@
         "NextToken": str,
         "Readiness": ReadinessType,
         "Rules": List[RuleResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DNSTargetResourceOutputTypeDef = TypedDict(
-    "DNSTargetResourceOutputTypeDef",
-    {
-        "DomainName": str,
-        "HostedZoneArn": str,
-        "RecordSetId": str,
-        "RecordType": str,
-        "TargetResource": TargetResourceOutputTypeDef,
-    },
-    total=False,
-)
-
 DNSTargetResourceTypeDef = TypedDict(
     "DNSTargetResourceTypeDef",
     {
         "DomainName": str,
         "HostedZoneArn": str,
         "RecordSetId": str,
         "RecordType": str,
@@ -1027,15 +985,15 @@
     total=False,
 )
 
 ResourceOutputTypeDef = TypedDict(
     "ResourceOutputTypeDef",
     {
         "ComponentId": str,
-        "DnsTargetResource": DNSTargetResourceOutputTypeDef,
+        "DnsTargetResource": DNSTargetResourceTypeDef,
         "ReadinessScopes": List[str],
         "ResourceArn": str,
     },
     total=False,
 )
 
 ResourceTypeDef = TypedDict(
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53-recovery-readiness
-Version: 1.28.12
-Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Route53RecoveryReadiness 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53-recovery-readiness.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53-recovery-readiness)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53-recovery-readiness)](https://pepy.tech/project/mypy-boto3-route53-recovery-readiness)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53RecoveryReadiness 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
+[boto3.Route53RecoveryReadiness 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
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
 [mypy-boto3-route53-recovery-readiness docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53_recovery_readiness/).
 
 See how it helps to find and fix potential bugs:
 
@@ -398,17 +398,15 @@
     ReadinessCheckOutputTypeDef,
     ListRecoveryGroupsRequestRequestTypeDef,
     RecoveryGroupOutputTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ListRulesOutputTypeDef,
     ListRulesRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
-    NLBResourceOutputTypeDef,
     NLBResourceTypeDef,
-    R53ResourceRecordOutputTypeDef,
     R53ResourceRecordTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCellRequestRequestTypeDef,
     UpdateReadinessCheckRequestRequestTypeDef,
     UpdateRecoveryGroupRequestRequestTypeDef,
     CreateCellResponseTypeDef,
@@ -439,18 +437,16 @@
     GetCellReadinessSummaryResponseTypeDef,
     GetRecoveryGroupReadinessSummaryResponseTypeDef,
     RuleResultTypeDef,
     GetReadinessCheckStatusResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListRulesResponseTypeDef,
-    TargetResourceOutputTypeDef,
     TargetResourceTypeDef,
     GetReadinessCheckResourceStatusResponseTypeDef,
-    DNSTargetResourceOutputTypeDef,
     DNSTargetResourceTypeDef,
     ResourceOutputTypeDef,
     ResourceTypeDef,
     CreateResourceSetResponseTypeDef,
     GetResourceSetResponseTypeDef,
     ResourceSetOutputTypeDef,
     UpdateResourceSetResponseTypeDef,
```

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt` & `mypy-boto3-route53-recovery-readiness-1.28.15/mypy_boto3_route53_recovery_readiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-recovery-readiness-1.28.12/setup.py` & `mypy-boto3-route53-recovery-readiness-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53-recovery-readiness",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_route53_recovery_readiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53RecoveryReadiness 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Route53RecoveryReadiness 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

